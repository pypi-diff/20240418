# Comparing `tmp/forloop_modules-1.0.1.tar.gz` & `tmp/forloop_modules-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.0.1.tar", last modified: Mon Apr  8 16:57:58 2024, max compression
+gzip compressed data, was "forloop_modules-1.0.2.tar", last modified: Thu Apr 18 13:46:39 2024, max compression
```

## Comparing `forloop_modules-1.0.1.tar` & `forloop_modules-1.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.521124 forloop_modules-1.0.1/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      658 2024-04-08 16:57:58.518114 forloop_modules-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.875992 forloop_modules-1.0.1/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.904942 forloop_modules-1.0.1/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.0.1/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.234545 forloop_modules-1.0.1/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.288063 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7504 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    22132 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.318163 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103324 2024-03-12 11:46:28.000000 forloop_modules-1.0.1/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.373702 forloop_modules-1.0.1/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5145 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     5482 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    17317 2024-03-14 09:29:03.000000 forloop_modules-1.0.1/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    32308 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.389742 forloop_modules-1.0.1/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.403095 forloop_modules-1.0.1/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    22387 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    41165 2024-03-21 12:02:54.000000 forloop_modules-1.0.1/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.405659 forloop_modules-1.0.1/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.406665 forloop_modules-1.0.1/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.511628 forloop_modules-1.0.1/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/synchronization_flags.py
--rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/forloop_modules/utils/url_template_builder.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.0.1/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:57.898908 forloop_modules-1.0.1/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3493 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-08 16:57:57.000000 forloop_modules-1.0.1/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 16:57:58.522114 forloop_modules-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-04-08 16:57:42.000000 forloop_modules-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:57:58.517113 forloop_modules-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.0.1/tests/test_url_template_builder.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.095402 forloop_modules-1.0.2/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.128244 forloop_modules-1.0.2/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.0.2/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.237142 forloop_modules-1.0.2/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.286309 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7504 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    22515 2024-04-18 13:45:44.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.322744 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103324 2024-03-12 11:46:28.000000 forloop_modules-1.0.2/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.369957 forloop_modules-1.0.2/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5145 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     5482 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    17317 2024-03-14 09:29:03.000000 forloop_modules-1.0.2/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    32107 2024-04-18 13:45:44.000000 forloop_modules-1.0.2/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.385548 forloop_modules-1.0.2/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.408708 forloop_modules-1.0.2/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    22387 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    41165 2024-03-21 12:02:54.000000 forloop_modules-1.0.2/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.414719 forloop_modules-1.0.2/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.421414 forloop_modules-1.0.2/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.480239 forloop_modules-1.0.2/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.0.2/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.119575 forloop_modules-1.0.2/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3493 2024-04-18 13:46:39.000000 forloop_modules-1.0.2/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-18 13:46:38.000000 forloop_modules-1.0.2/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:46:39.487948 forloop_modules-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-04-18 13:46:17.000000 forloop_modules-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:46:39.486697 forloop_modules-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.0.2/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.0.1/LICENSE` & `forloop_modules-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/PKG-INFO` & `forloop_modules-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.1/forloop_modules/errors/errors.py` & `forloop_modules-1.0.2/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/flog.py` & `forloop_modules-1.0.2/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/browser_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -290,14 +290,24 @@
         )
         kv_redis.set(redis_action_key, suh.webpage_elements)
 
     def direct_execute(
         self, url: str, incl_tables, incl_bullets, incl_texts, incl_headlines, incl_links,
         incl_images, incl_buttons, xpath
     ):
+        scraping_options = {
+            'incl_tables': incl_tables,
+            'incl_bullets': incl_bullets,
+            'incl_texts': incl_texts,
+            'incl_headlines': incl_headlines,
+            'incl_links': incl_links,
+            'incl_images': incl_images,
+            'incl_buttons': incl_buttons,
+            'by_xpath': xpath
+        }
         # start_time = time.perf_counter()
         # a_time = time.perf_counter() - start_time
 
         output_folder = Path.cwd() / 'tmp' / 'screenshots'
 
         # random_number = 50000000 + random.randint(1, 10000000)  # initialization
 
@@ -351,15 +361,15 @@
         # request_thread=slack_notif.UnblockingFunctionThread(slack_notif.send_slack_notification, api_scan_webpage.url, user_email=api_scan_webpage.email)
         # request_thread.start()
 
         #slack_notif.send_slack_notification(api_scan_webpage.url,user_email=api_scan_webpage.email)  #2 seconds
         # e_time = time.perf_counter() - start_time #12.5s
 
         suh.webscraping_client.load_website(url, timeout=30)
-        elements = suh.scan_web_page_API(output_folder)  #9 seconds
+        elements = suh.scan_web_page_API(output_folder, scraping_options)  #9 seconds
         # with open(output_folder / "website.png", "rb") as file:
         #     screenshot = file.read()
         #     screenshot = base64.b64encode(screenshot).decode("utf-8")
 
         # Convert to WEBP
         img = Image.open(output_folder / "website.png")
         webp_filename = url
```

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/database_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.0.2/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.0.2/forloop_modules/globals/active_entity_tracker.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.0.2/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/db_connection.py` & `forloop_modules-1.0.2/forloop_modules/globals/db_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.0.2/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.0.2/forloop_modules/globals/local_variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.0.2/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
 
         self.webscraping_client.set_browser_scanned_elements(webpage_elements)
         self.webpage_elements = webpage_elements
         self.are_elements_updated = True
     
         return generalised_xpaths, optimal_xpath_index
 
-    def scan_web_page_API(self, output_folder):
+    def scan_web_page_API(self, output_folder, scraping_options: dict):
         """
         Function only to use in "Getting Started" tutorial on web app !!!
         Combines ScanWebPage (all elements) with Cookies Detection
         """
         def generate_folder_structure(folder_name):
             try:
                 os.mkdir(folder_name)
@@ -624,17 +624,15 @@
         generate_folder_structure("tmp")
         generate_folder_structure("tmp/screenshots")
         generate_folder_structure("tmp/scraped_data")
 
         xpath = self.detect_cookies_xpath_preparation()
     
         self.webscraping_client.take_png_screenshot(str(Path(output_folder, 'website.png'))) #needs to run before the scanner so there is enough time for the parallel thread
-        self.webscraping_client.scan_web_page(incl_tables=True, incl_bullets=True, incl_texts=True,
-                                       incl_headlines=True, incl_links=True, incl_images=True,
-                                       incl_buttons=True, by_xpath=None, cookies_xpath=xpath, timeout = 60) #Duration: ~3s
+        self.webscraping_client.scan_web_page(**scraping_options, timeout = 60) #Duration: ~3s
         
     
         webpage_elements = self.update_webpage_elements(refresh_browser_view_elements=False) #Duration: ~ 0s
 
         cookies_elements, rest_elements = [], []
 
         # Split elements
```

### Comparing `forloop_modules-1.0.1/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.0.2/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.0.2/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.0.2/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/node_detail_form.py` & `forloop_modules-1.0.2/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.0.2/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.0.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.0.2/forloop_modules/queries/db_model_templates.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.0.2/forloop_modules/queries/node_context_requests_backend.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/redis/config/config.py` & `forloop_modules-1.0.2/forloop_modules/redis/config/config.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.0.2/forloop_modules/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/definitions.py` & `forloop_modules-1.0.2/forloop_modules/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/encryption.py` & `forloop_modules-1.0.2/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.0.2/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.0.2/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/script_utils.py` & `forloop_modules-1.0.2/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.0.2/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/synchronization_flags.py` & `forloop_modules-1.0.2/forloop_modules/utils/synchronization_flags.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/url_template_builder.py` & `forloop_modules-1.0.2/forloop_modules/utils/url_template_builder.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules/utils/various.py` & `forloop_modules-1.0.2/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.0.2/forloop_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.0.1/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.0.2/forloop_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.0.1/setup.py` & `forloop_modules-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.0.1',
+    version='1.0.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

### Comparing `forloop_modules-1.0.1/tests/test_url_template_builder.py` & `forloop_modules-1.0.2/tests/test_url_template_builder.py`

 * *Files identical despite different names*

