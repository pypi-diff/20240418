# Comparing `tmp/manticoresearch-devel-4.2.24041700.tar.gz` & `tmp/manticoresearch-devel-4.3.24041813.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manticoresearch-devel-4.2.24041700.tar", last modified: Tue Apr 16 17:11:35 2024, max compression
+gzip compressed data, was "manticoresearch-devel-4.3.24041813.tar", last modified: Thu Apr 18 06:09:25 2024, max compression
```

## Comparing `manticoresearch-devel-4.2.24041700.tar` & `manticoresearch-devel-4.3.24041813.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1095 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.618816 manticoresearch-devel-4.2.24041700/manticoresearch/
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.618816 manticoresearch-devel-4.2.24041700/manticoresearch/api/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45843 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/api/index_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/api/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.618816 manticoresearch-devel-4.2.24041700/manticoresearch/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/manticoresearch/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite_sources_inner_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite_sources_inner_value_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_sort_inner_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/attr_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/bool_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/bulk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/delete_document_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/equals_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/facet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/fulltext_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/geo_distance_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/geo_distance_filter_location_anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/highlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/highlight_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/in_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/insert_document_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/knn_query_by_doc_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/knn_query_by_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/match_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/match_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/match_op_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/match_phrase_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/percolate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/percolate_request_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/query_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/replace_document_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18428 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/search_request_knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/search_response_hits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_mva.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/source_by_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/source_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/sql_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/success_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/update_document_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model/update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/manticoresearch/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/manticoresearch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-16 17:11:35.000000 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-16 17:11:35.000000 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:11:35.000000 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 17:11:35.000000 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 17:11:35.000000 manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:11:35.630816 manticoresearch-devel-4.2.24041700/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/test/test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6204 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/test/test_index_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18278 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/test/test_manual.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3485 2024-04-16 17:11:28.000000 manticoresearch-devel-4.2.24041700/test/test_search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1095 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.640315 manticoresearch-devel-4.3.24041813/manticoresearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.644315 manticoresearch-devel-4.3.24041813/manticoresearch/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45843 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/api/index_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.644315 manticoresearch-devel-4.3.24041813/manticoresearch/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/manticoresearch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite_sources_inner_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite_sources_inner_value_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_sort_inner_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/attr_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/bool_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/bulk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/delete_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/equals_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/fulltext_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/geo_distance_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/geo_distance_filter_location_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/highlight_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/insert_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/knn_query_by_doc_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/knn_query_by_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/match_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/match_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/match_op_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/match_phrase_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/percolate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/percolate_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/query_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/range_filter_lte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/replace_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18428 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/search_request_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/search_response_hits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_mva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/source_by_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/source_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/success_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/update_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model/update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/manticoresearch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/manticoresearch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-18 06:09:25.000000 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-18 06:09:25.000000 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:09:25.000000 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 06:09:25.000000 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 06:09:25.000000 manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-18 06:09:15.000000 manticoresearch-devel-4.3.24041813/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:09:25.652315 manticoresearch-devel-4.3.24041813/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/test/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6204 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/test/test_index_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18547 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/test/test_manual.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3485 2024-04-18 06:09:14.000000 manticoresearch-devel-4.3.24041813/test/test_search_api.py
```

### Comparing `manticoresearch-devel-4.2.24041700/LICENSE.txt` & `manticoresearch-devel-4.3.24041813/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/PKG-INFO` & `manticoresearch-devel-4.3.24041813/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manticoresearch-devel
-Version: 4.2.24041700
+Version: 4.3.24041813
 Summary: Python client for Manticore Search
 Home-page: 
 Author: Manticore Software Ltd.
 Author-email: info@manticoresearch.com
 License: MIT
 Project-URL: Documentation, https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs
 Project-URL: Source Code, https://github.com/manticoresoftware/manticoresearch-python
@@ -36,26 +36,26 @@
 
 ## Requirements.
 
 Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
-| dev               | manticoresearch-dev      | >= 3.4        |
+| dev               | manticoresearch-devel    | >= 3.4        |
 | >= 6.2.0          | >= 3.3.1                 | >= 3.4        |
 | >= 4.2.1          | >= 2.0.x                 | >= 3.4        |
 | >= 4.0.2  < 4.2.1 | >= 1.0.6                 | >= 3.4        |
 | >= 2.5.1  < 4.0.2 | >= 1.0.5                 | >= 2.7        |
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
-pip install manticoresearch-dev
+pip install manticoresearch-devel
 ```
 
 Then import the package:
 ```python
 import manticoresearch
 ```
```

### Comparing `manticoresearch-devel-4.2.24041700/README.md` & `manticoresearch-devel-4.3.24041813/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 ## Requirements.
 
 Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
-| dev               | manticoresearch-dev      | >= 3.4        |
+| dev               | manticoresearch-devel    | >= 3.4        |
 | >= 6.2.0          | >= 3.3.1                 | >= 3.4        |
 | >= 4.2.1          | >= 2.0.x                 | >= 3.4        |
 | >= 4.0.2  < 4.2.1 | >= 1.0.6                 | >= 3.4        |
 | >= 2.5.1  < 4.0.2 | >= 1.0.5                 | >= 2.7        |
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
-pip install manticoresearch-dev
+pip install manticoresearch-devel
 ```
 
 Then import the package:
 ```python
 import manticoresearch
 ```
 
@@ -151,14 +151,15 @@
  - [NotFilterNumber](docs/NotFilterNumber.md)
  - [NotFilterString](docs/NotFilterString.md)
  - [Option](docs/Option.md)
  - [PercolateRequest](docs/PercolateRequest.md)
  - [PercolateRequestQuery](docs/PercolateRequestQuery.md)
  - [QueryFilter](docs/QueryFilter.md)
  - [RangeFilter](docs/RangeFilter.md)
+ - [RangeFilterLte](docs/RangeFilterLte.md)
  - [SearchRequest](docs/SearchRequest.md)
  - [SearchRequestKnn](docs/SearchRequestKnn.md)
  - [SearchResponse](docs/SearchResponse.md)
  - [SearchResponseHits](docs/SearchResponseHits.md)
  - [SortMVA](docs/SortMVA.md)
  - [SortMultiple](docs/SortMultiple.md)
  - [SortOrder](docs/SortOrder.md)
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/__init__.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 from manticoresearch.model.not_filter_number import NotFilterNumber
 from manticoresearch.model.not_filter_string import NotFilterString
 from manticoresearch.model.option import Option
 from manticoresearch.model.percolate_request import PercolateRequest
 from manticoresearch.model.percolate_request_query import PercolateRequestQuery
 from manticoresearch.model.query_filter import QueryFilter
 from manticoresearch.model.range_filter import RangeFilter
+from manticoresearch.model.range_filter_lte import RangeFilterLte
 from manticoresearch.model.replace_document_request import ReplaceDocumentRequest
 from manticoresearch.model.search_request import SearchRequest
 from manticoresearch.model.search_request_knn import SearchRequestKnn
 from manticoresearch.model.search_response import SearchResponse
 from manticoresearch.model.search_response_hits import SearchResponseHits
 from manticoresearch.model.sort_mva import SortMVA
 from manticoresearch.model.sort_multiple import SortMultiple
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/api/index_api.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/api/index_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/api/search_api.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/api/search_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/api/utils_api.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/api_client.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/api_client.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/apis/__init__.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/configuration.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/configuration.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/exceptions.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/exceptions.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/__init__.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from manticoresearch.model.not_filter_number import NotFilterNumber
 from manticoresearch.model.not_filter_string import NotFilterString
 from manticoresearch.model.option import Option
 from manticoresearch.model.percolate_request import PercolateRequest
 from manticoresearch.model.percolate_request_query import PercolateRequestQuery
 from manticoresearch.model.query_filter import QueryFilter
 from manticoresearch.model.range_filter import RangeFilter
+from manticoresearch.model.range_filter_lte import RangeFilterLte
 from manticoresearch.model.replace_document_request import ReplaceDocumentRequest
 from manticoresearch.model.search_request import SearchRequest
 from manticoresearch.model.search_request_knn import SearchRequestKnn
 from manticoresearch.model.search_response import SearchResponse
 from manticoresearch.model.search_response_hits import SearchResponseHits
 from manticoresearch.model.sort_mva import SortMVA
 from manticoresearch.model.sort_multiple import SortMultiple
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite_sources_inner_value.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite_sources_inner_value.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_composite_sources_inner_value_terms.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_composite_sources_inner_value_terms.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_sort_inner_value.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_sort_inner_value.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/aggregation_terms.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/aggregation_terms.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/attr_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/attr_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/bool_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/bool_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/bulk_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/bulk_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/delete_document_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/delete_document_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/delete_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/delete_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/equals_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/equals_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/error_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/error_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/facet.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/facet.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_boolean.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_boolean.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_number.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_number.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/filter_string.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/filter_string.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/fulltext_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/fulltext_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/geo_distance_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/geo_distance_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/geo_distance_filter_location_anchor.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/geo_distance_filter_location_anchor.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/highlight.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/highlight.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/highlight_field.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/highlight_field.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/in_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/in_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/insert_document_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/insert_document_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/knn_query_by_doc_id.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/knn_query_by_doc_id.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/knn_query_by_vector.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/knn_query_by_vector.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/match_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/match_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/match_op.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/match_op.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/match_op_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/match_op_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/match_phrase_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/match_phrase_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_boolean.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_boolean.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_number.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_number.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/not_filter_string.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/not_filter_string.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/option.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/option.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/percolate_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/percolate_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/percolate_request_query.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/percolate_request_query.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/query_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/query_filter.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/range_filter.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/range_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'field': 'str',
-        'lte': 'float, none_type',
-        'gte': 'float, none_type',
-        'lt': 'float, none_type',
-        'gt': 'float, none_type'
+        'lte': 'RangeFilterLte',
+        'gte': 'RangeFilterLte',
+        'lt': 'RangeFilterLte',
+        'gt': 'RangeFilterLte'
     }
 
     attribute_map = {
         'field': 'field',
         'lte': 'lte',
         'gte': 'gte',
         'lt': 'lt',
@@ -89,87 +89,87 @@
 
     @property
     def lte(self):
         """Gets the lte of this RangeFilter.  # noqa: E501
 
 
         :return: The lte of this RangeFilter.  # noqa: E501
-        :rtype: float, none_type
+        :rtype: RangeFilterLte
         """
         return self._lte
     @lte.setter
     def lte(self, lte):
         """Sets the lte of this RangeFilter.
 
 
         :param lte: The lte of this RangeFilter.  # noqa: E501
-        :type lte: float, none_type
+        :type lte: RangeFilterLte
         """
 
         self._lte = lte
         
 
     @property
     def gte(self):
         """Gets the gte of this RangeFilter.  # noqa: E501
 
 
         :return: The gte of this RangeFilter.  # noqa: E501
-        :rtype: float, none_type
+        :rtype: RangeFilterLte
         """
         return self._gte
     @gte.setter
     def gte(self, gte):
         """Sets the gte of this RangeFilter.
 
 
         :param gte: The gte of this RangeFilter.  # noqa: E501
-        :type gte: float, none_type
+        :type gte: RangeFilterLte
         """
 
         self._gte = gte
         
 
     @property
     def lt(self):
         """Gets the lt of this RangeFilter.  # noqa: E501
 
 
         :return: The lt of this RangeFilter.  # noqa: E501
-        :rtype: float, none_type
+        :rtype: RangeFilterLte
         """
         return self._lt
     @lt.setter
     def lt(self, lt):
         """Sets the lt of this RangeFilter.
 
 
         :param lt: The lt of this RangeFilter.  # noqa: E501
-        :type lt: float, none_type
+        :type lt: RangeFilterLte
         """
 
         self._lt = lt
         
 
     @property
     def gt(self):
         """Gets the gt of this RangeFilter.  # noqa: E501
 
 
         :return: The gt of this RangeFilter.  # noqa: E501
-        :rtype: float, none_type
+        :rtype: RangeFilterLte
         """
         return self._gt
     @gt.setter
     def gt(self, gt):
         """Sets the gt of this RangeFilter.
 
 
         :param gt: The gt of this RangeFilter.  # noqa: E501
-        :type gt: float, none_type
+        :type gt: RangeFilterLte
         """
 
         self._gt = gt
         
 
 
     def to_dict(self):
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/replace_document_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/replace_document_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/search_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/search_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/search_request_knn.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/search_request_knn.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/search_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/search_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/search_response_hits.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/search_response_hits.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_multiple.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_multiple.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_mva.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_mva.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/sort_order.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/source_by_rules.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/source_by_rules.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/source_multiple.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/source_multiple.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/sql_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/sql_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/success_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/success_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/update_document_request.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/update_document_request.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model/update_response.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model/update_response.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/model_utils.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/model_utils.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/models/__init__.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from manticoresearch.model.not_filter_number import NotFilterNumber
 from manticoresearch.model.not_filter_string import NotFilterString
 from manticoresearch.model.option import Option
 from manticoresearch.model.percolate_request import PercolateRequest
 from manticoresearch.model.percolate_request_query import PercolateRequestQuery
 from manticoresearch.model.query_filter import QueryFilter
 from manticoresearch.model.range_filter import RangeFilter
+from manticoresearch.model.range_filter_lte import RangeFilterLte
 from manticoresearch.model.replace_document_request import ReplaceDocumentRequest
 from manticoresearch.model.search_request import SearchRequest
 from manticoresearch.model.search_request_knn import SearchRequestKnn
 from manticoresearch.model.search_response import SearchResponse
 from manticoresearch.model.search_response_hits import SearchResponseHits
 from manticoresearch.model.sort_mva import SortMVA
 from manticoresearch.model.sort_multiple import SortMultiple
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch/rest.py` & `manticoresearch-devel-4.3.24041813/manticoresearch/rest.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/PKG-INFO` & `manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manticoresearch-devel
-Version: 4.2.24041700
+Version: 4.3.24041813
 Summary: Python client for Manticore Search
 Home-page: 
 Author: Manticore Software Ltd.
 Author-email: info@manticoresearch.com
 License: MIT
 Project-URL: Documentation, https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs
 Project-URL: Source Code, https://github.com/manticoresoftware/manticoresearch-python
@@ -36,26 +36,26 @@
 
 ## Requirements.
 
 Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
-| dev               | manticoresearch-dev      | >= 3.4        |
+| dev               | manticoresearch-devel    | >= 3.4        |
 | >= 6.2.0          | >= 3.3.1                 | >= 3.4        |
 | >= 4.2.1          | >= 2.0.x                 | >= 3.4        |
 | >= 4.0.2  < 4.2.1 | >= 1.0.6                 | >= 3.4        |
 | >= 2.5.1  < 4.0.2 | >= 1.0.5                 | >= 2.7        |
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
-pip install manticoresearch-dev
+pip install manticoresearch-devel
 ```
 
 Then import the package:
 ```python
 import manticoresearch
 ```
```

### Comparing `manticoresearch-devel-4.2.24041700/manticoresearch_devel.egg-info/SOURCES.txt` & `manticoresearch-devel-4.3.24041813/manticoresearch_devel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 manticoresearch/model/not_filter_number.py
 manticoresearch/model/not_filter_string.py
 manticoresearch/model/option.py
 manticoresearch/model/percolate_request.py
 manticoresearch/model/percolate_request_query.py
 manticoresearch/model/query_filter.py
 manticoresearch/model/range_filter.py
+manticoresearch/model/range_filter_lte.py
 manticoresearch/model/replace_document_request.py
 manticoresearch/model/search_request.py
 manticoresearch/model/search_request_knn.py
 manticoresearch/model/search_response.py
 manticoresearch/model/search_response_hits.py
 manticoresearch/model/sort_multiple.py
 manticoresearch/model/sort_mva.py
```

### Comparing `manticoresearch-devel-4.2.24041700/setup.py` & `manticoresearch-devel-4.3.24041813/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 from setuptools import setup, find_packages
 from os import path
 
 NAME = "manticoresearch-devel"
-VERSION = "4.2.24041700"
+VERSION = "4.3.24041813"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `manticoresearch-devel-4.2.24041700/test/test.py` & `manticoresearch-devel-4.3.24041813/test/test.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/test/test_index_api.py` & `manticoresearch-devel-4.3.24041813/test/test_index_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-devel-4.2.24041700/test/test_manual.py` & `manticoresearch-devel-4.3.24041813/test/test_manual.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     def test_manual(self):
         client = self.client
         indexApi = manticoresearch.IndexApi(client)
         utilsApi = manticoresearch.UtilsApi(client)
         searchApi = manticoresearch.SearchApi(client)
         
         utilsApi.sql('DROP TABLE IF EXISTS movies')
-        res = utilsApi.sql("CREATE TABLE IF NOT EXISTS movies (title text, plot text, _year integer, rating float, code multi, type_vector float_vector knn_type='hnsw' knn_dims='3' hnsw_similarity='l2' )")
+        res = utilsApi.sql("CREATE TABLE IF NOT EXISTS movies (title text, plot text, _year integer, rating float, cat string, code multi, type_vector float_vector knn_type='hnsw' knn_dims='3' hnsw_similarity='l2' )")
         
         docs = [
-            {"insert": {"index" : "movies", "id" : 1, "doc" : {"title" : "Star Trek 2: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2002, "rating": 6.4, "code": [1,2,3], "type_vector": [0.2, 1.4, -2.3]}}},
-            {"insert": {"index" : "movies", "id" : 2, "doc" : {"title" : "Star Trek 1: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2001, "rating": 6.5, "code": [1,12,3], "type_vector": [0.8, 0.4, 1.3]}}},
-            {"insert": {"index" : "movies", "id" : 3, "doc" : {"title" : "Star Trek 3: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2003, "rating": 6.6, "code": [11,2,3], "type_vector": [1.5, -1.0, 1.6]}}},
-            {"insert": {"index" : "movies", "id" : 4, "doc" : {"title" : "Star Trek 4: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2003, "rating": 6.5, "code": [1,2,4], "type_vector": [0.4, 2.4, 0.9]}}},
+            {"insert": {"index" : "movies", "id" : 1, "doc" : {"title" : "Star Trek 2: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2002, "rating": 6.4, "cat": "R", "code": [1,2,3], "type_vector": [0.2, 1.4, -2.3]}}},
+            {"insert": {"index" : "movies", "id" : 2, "doc" : {"title" : "Star Trek 1: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2001, "rating": 6.5, "cat": "PG-13", "code": [1,12,3], "type_vector": [0.8, 0.4, 1.3]}}},
+            {"insert": {"index" : "movies", "id" : 3, "doc" : {"title" : "Star Trek 3: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2003, "rating": 6.6, "cat": "R", "code": [11,2,3], "type_vector": [1.5, -1.0, 1.6]}}},
+            {"insert": {"index" : "movies", "id" : 4, "doc" : {"title" : "Star Trek 4: Nemesis", "plot": "The Enterprise is diverted to the Romulan homeworld Romulus, supposedly because they want to negotiate a peace treaty. Captain Picard and his crew discover a serious threat to the Federation once Praetor Shinzon plans to attack Earth.", "_year": 2003, "rating": 6.5, "cat": "R", "code": [1,2,4], "type_vector": [0.4, 2.4, 0.9]}}},
         ]
         indexApi.bulk("\n".join(map(json.dumps,docs)))
         
         
         search_request = SearchRequest(
             index="movies",
             query={"match_all": {}}
@@ -152,14 +152,21 @@
         rangeFilter = RangeFilter('rating')
         rangeFilter.gt = 2000.5
         rangeFilter.lt = 2002
         search_request.attr_filter = rangeFilter
 
         res = searchApi.search(search_request)
 
+        rangeFilter = RangeFilter('cat')
+        rangeFilter.gt = "N"
+        rangeFilter.lt = "R"
+        search_request.attr_filter = rangeFilter
+
+        res = searchApi.search(search_request)
+        
         geoFilter = GeoDistanceFilter(location_anchor={'lat':10,'lon':20.5}, location_source='_year,rating')
         geoFilter.location_source='_year,rating'
         geoFilter.distance_type='adaptive'
         geoFilter.distance='100 km'
         search_request.attr_filter = geoFilter
         
         res = searchApi.search(search_request)
```

### Comparing `manticoresearch-devel-4.2.24041700/test/test_search_api.py` & `manticoresearch-devel-4.3.24041813/test/test_search_api.py`

 * *Files identical despite different names*

