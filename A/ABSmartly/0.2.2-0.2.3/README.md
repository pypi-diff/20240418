# Comparing `tmp/ABSmartly-0.2.2.tar.gz` & `tmp/absmartly-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSmartly-0.2.2.tar", last modified: Wed Dec 13 09:54:11 2023, max compression
+gzip compressed data, was "absmartly-0.2.3.tar", last modified: Thu Apr 18 10:33:53 2024, max compression
```

## Comparing `ABSmartly-0.2.2.tar` & `absmartly-0.2.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/ABSmartly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2023-12-13 09:54:11.000000 ABSmartly-0.2.2/ABSmartly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-13 09:54:11.000000 ABSmartly-0.2.2/ABSmartly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 09:54:11.000000 ABSmartly-0.2.2/ABSmartly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-13 09:54:11.000000 ABSmartly-0.2.2/ABSmartly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-13 09:54:11.000000 ABSmartly-0.2.2/ABSmartly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.247745 ABSmartly-0.2.2/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/absmartly.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/absmartly_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/audience_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/audience_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32088 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_data_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_event_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/context_event_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_audience_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_context_data_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_context_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_context_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_context_event_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_http_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/default_variable_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.247745 ABSmartly-0.2.2/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/buffers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.247745 ABSmartly-0.2.2/sdk/internal/lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/lock/atomic_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/lock/atomic_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/lock/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/lock/read_write_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/murmur32.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/internal/variant_assigner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.251745 ABSmartly-0.2.2/sdk/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/context_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/experiement_application.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/experiment_variant.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/goal_achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/publish_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/json/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.251745 ABSmartly-0.2.2/sdk/jsonexpr/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/expr_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/json_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.251745 ABSmartly-0.2.2/sdk/jsonexpr/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/and_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/binary_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/boolean_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/equals_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/greater_than_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/greater_than_or_equal_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/in_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/less_than_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/less_than_or_equal_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/match_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/not_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/null_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/or_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/unary_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/value_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/jsonexpr/operators/var_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/sdk/time/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/time/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/time/fixed_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/time/system_clock_utc.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/sdk/variable_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:54:11.255745 ABSmartly-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42607 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_default_audience_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_default_context_data_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_default_context_event_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_murmur32.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2023-12-13 09:53:12.000000 ABSmartly-0.2.2/test/test_variant_assigner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.081833 absmartly-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.081833 absmartly-0.2.3/ABSmartly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-18 10:33:53.000000 absmartly-0.2.3/ABSmartly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-18 10:33:53.000000 absmartly-0.2.3/ABSmartly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:33:53.000000 absmartly-0.2.3/ABSmartly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 10:33:53.000000 absmartly-0.2.3/ABSmartly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 10:33:53.000000 absmartly-0.2.3/ABSmartly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-18 10:32:55.000000 absmartly-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 10:32:55.000000 absmartly-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-18 10:33:53.081833 absmartly-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-18 10:32:55.000000 absmartly-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-18 10:32:55.000000 absmartly-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.073833 absmartly-0.2.3/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/absmartly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/absmartly_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/audience_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/audience_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32397 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_data_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/context_event_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_audience_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_context_data_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_context_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_context_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_context_event_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_http_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/default_variable_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.073833 absmartly-0.2.3/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/buffers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.073833 absmartly-0.2.3/sdk/internal/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/lock/atomic_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/lock/atomic_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/lock/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/lock/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/murmur32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/internal/variant_assigner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.077833 absmartly-0.2.3/sdk/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/context_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/experiement_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/experiment_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/goal_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/json/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.077833 absmartly-0.2.3/sdk/jsonexpr/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/expr_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/json_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.081833 absmartly-0.2.3/sdk/jsonexpr/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/and_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/binary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/boolean_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/equals_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/greater_than_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/greater_than_or_equal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/in_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/less_than_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/less_than_or_equal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/match_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/not_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/null_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/or_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/unary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/value_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/jsonexpr/operators/var_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.081833 absmartly-0.2.3/sdk/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/time/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/time/fixed_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/time/system_clock_utc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-18 10:32:55.000000 absmartly-0.2.3/sdk/variable_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:33:53.085833 absmartly-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:33:53.081833 absmartly-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_default_audience_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_default_context_data_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_default_context_event_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_murmur32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-18 10:32:55.000000 absmartly-0.2.3/test/test_variant_assigner.py
```

### Comparing `ABSmartly-0.2.2/ABSmartly.egg-info/PKG-INFO` & `absmartly-0.2.3/ABSmartly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSmartly
-Version: 0.2.2
+Version: 0.2.3
 Summary: ABSmartly Python SDK lib
 Author-email: ABSmartly <info@ABSmartly.com>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -38,15 +38,15 @@
 The A/B Smartly Python SDK is compatible with Python 3.
 It provides both a blocking and an asynchronous interfaces.
 
 ## Getting Started
 
 ### Install the SDK
  ```bash
- pip install absmartly==0.1.4
+ pip install absmartly==0.2.3
  ```
 
 ### Dependencies
 ```
 setuptools~=60.2.0  
 requests~=2.28.1  
 urllib3~=1.26.12
```

### Comparing `ABSmartly-0.2.2/ABSmartly.egg-info/SOURCES.txt` & `absmartly-0.2.3/ABSmartly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/LICENSE` & `absmartly-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/PKG-INFO` & `absmartly-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSmartly
-Version: 0.2.2
+Version: 0.2.3
 Summary: ABSmartly Python SDK lib
 Author-email: ABSmartly <info@ABSmartly.com>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -38,15 +38,15 @@
 The A/B Smartly Python SDK is compatible with Python 3.
 It provides both a blocking and an asynchronous interfaces.
 
 ## Getting Started
 
 ### Install the SDK
  ```bash
- pip install absmartly==0.1.4
+ pip install absmartly==0.2.3
  ```
 
 ### Dependencies
 ```
 setuptools~=60.2.0  
 requests~=2.28.1  
 urllib3~=1.26.12
```

### Comparing `ABSmartly-0.2.2/README.md` & `absmartly-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 The A/B Smartly Python SDK is compatible with Python 3.
 It provides both a blocking and an asynchronous interfaces.
 
 ## Getting Started
 
 ### Install the SDK
  ```bash
- pip install absmartly==0.1.4
+ pip install absmartly==0.2.3
  ```
 
 ### Dependencies
 ```
 setuptools~=60.2.0  
 requests~=2.28.1  
 urllib3~=1.26.12
```

### Comparing `ABSmartly-0.2.2/pyproject.toml` & `absmartly-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ABSmartly"
-version = "0.2.2"
+version = "0.2.3"
 description = "ABSmartly Python SDK lib"
 readme = "README.md"
 authors = [{ name = "ABSmartly", email = "info@ABSmartly.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `ABSmartly-0.2.2/sdk/absmartly.py` & `absmartly-0.2.3/sdk/absmartly.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/absmartly_config.py` & `absmartly-0.2.3/sdk/absmartly_config.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/audience_matcher.py` & `absmartly-0.2.3/sdk/audience_matcher.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/client.py` & `absmartly-0.2.3/sdk/client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/client_config.py` & `absmartly-0.2.3/sdk/client_config.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/context.py` & `absmartly-0.2.3/sdk/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.overridden: Optional[bool] = False
         self.eligible: Optional[bool] = False
         self.full_on: Optional[bool] = False
         self.custom: Optional[bool] = False
         self.audience_mismatch: Optional[bool] = False
         self.variables: dict = {}
         self.exposed = AtomicBool()
+        self.exposedAt: Optional[int] = None
 
 
 class ExperimentVariables:
     data: Optional[Experiment]
     variables: Optional[list[dict]]
 
 class ContextCustomFieldValue:
@@ -74,14 +75,15 @@
         self.publish_delay = config.publish_delay
         self.refresh_interval = config.refresh_interval
         self.event_handler = event_handler
         self.event_logger = event_logger
         self.data_provider = data_provider
         self.variable_parser = variable_parser
         self.audience_matcher = audience_matcher
+        self.historic = config.historic
 
         self.units = {}
         self.index = {}
         self.index_variables = {}
         self.context_custom_fields = {}
         self.assignment_cache = {}
         self.cassignments = {}
@@ -401,14 +403,15 @@
                         event.units.append(unit)
                     if len(self.attributes) > 0:
                         event.attributes = list(self.attributes)
                     else:
                         event.attributes = None
                     event.exposures = exposures
                     event.goals = achievements
+                    event.historic = self.historic
 
                     result = Future()
 
                     def run(data):
                         if data.done() and \
                                 data.cancelled() is False and \
                                 data.exception() is None:
@@ -539,17 +542,17 @@
 
         return Concurrency.compute_if_absent_rw(
             self.context_lock,
             self.hashed_units,
             unit_type,
             computer)
 
-    def get_treatment(self, experiment_name: str):
+    def get_treatment(self, experiment_name: str, exposed_at: int = None):
         self.check_ready(True)
-        assignment = self.get_assignment(experiment_name)
+        assignment = self.get_assignment(experiment_name, exposed_at=exposed_at)
         if not assignment.exposed.value:
             self.queue_exposure(assignment)
         return assignment.variant
 
     def get_variable_keys(self):
         self.check_ready(True)
 
@@ -615,15 +618,15 @@
                     type = customFieldValue[key].type
 
         finally:
             self.data_lock.release_read()
 
         return type
 
-    def get_assignment(self, experiment_name: str):
+    def get_assignment(self, experiment_name: str, exposed_at: int = None):
         try:
             self.context_lock.acquire_read()
 
             if experiment_name in self.assignment_cache:
                 assignment: Assignment = self.assignment_cache[experiment_name]
 
                 experiment: ExperimentVariables = \
@@ -649,14 +652,17 @@
             self.context_lock.acquire_write()
             experiment: ExperimentVariables = \
                 self.get_experiment(experiment_name)
             assignment = Assignment()
             assignment.name = experiment_name
             assignment.eligible = True
 
+            if exposed_at:
+                assignment.exposedAt = exposed_at
+
             if experiment_name in self.overrides:
                 if experiment is not None:
                     assignment.id = experiment.data.id
                     assignment.unit_type = experiment.data.unitType
 
                 assignment.overridden = True
                 assignment.variant = self.overrides[experiment_name]
@@ -848,15 +854,15 @@
     def queue_exposure(self, assignment: Assignment):
         if assignment.exposed.compare_and_set(False, True):
             exposure = Exposure()
             exposure.id = assignment.id
             exposure.name = assignment.name
             exposure.unit = assignment.unit_type
             exposure.variant = assignment.variant
-            exposure.exposedAt = self.clock.millis()
+            exposure.exposedAt = assignment.exposedAt or self.clock.millis()
             exposure.assigned = assignment.assigned
             exposure.eligible = assignment.eligible
             exposure.overridden = assignment.overridden
             exposure.fullOn = assignment.full_on
             exposure.custom = assignment.custom
             exposure.audienceMismatch = assignment.audience_mismatch
```

### Comparing `ABSmartly-0.2.2/sdk/default_context_data_deserializer.py` & `absmartly-0.2.3/sdk/default_context_data_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/default_context_event_handler.py` & `absmartly-0.2.3/sdk/default_context_event_handler.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/default_http_client.py` & `absmartly-0.2.3/sdk/default_http_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/http_client.py` & `absmartly-0.2.3/sdk/http_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/internal/buffers.py` & `absmartly-0.2.3/sdk/internal/buffers.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/internal/lock/concurrency.py` & `absmartly-0.2.3/sdk/internal/lock/concurrency.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/internal/lock/read_write_lock.py` & `absmartly-0.2.3/sdk/internal/lock/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/internal/murmur32.py` & `absmartly-0.2.3/sdk/internal/murmur32.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/internal/variant_assigner.py` & `absmartly-0.2.3/sdk/internal/variant_assigner.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/json/experiment.py` & `absmartly-0.2.3/sdk/json/experiment.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/jsonexpr/evaluator.py` & `absmartly-0.2.3/sdk/jsonexpr/evaluator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/jsonexpr/expr_evaluator.py` & `absmartly-0.2.3/sdk/jsonexpr/expr_evaluator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/jsonexpr/json_expr.py` & `absmartly-0.2.3/sdk/jsonexpr/json_expr.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/jsonexpr/operators/binary_operator.py` & `absmartly-0.2.3/sdk/jsonexpr/operators/binary_operator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/sdk/jsonexpr/operators/in_operator.py` & `absmartly-0.2.3/sdk/jsonexpr/operators/in_operator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_buffers.py` & `absmartly-0.2.3/test/test_buffers.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_client.py` & `absmartly-0.2.3/test/test_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_context.py` & `absmartly-0.2.3/test/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1115,7 +1115,23 @@
         self.assertEqual(2, context.get_pending_count())
         self.assertEqual(self.event_logger.logger_type, EventType.EXPOSURE)
         self.assertEqual(type(self.event_logger.logger_data),
                          type(Exposure()))
         context.close()
         self.assertEqual(self.event_logger.logger_type, EventType.CLOSE)
         self.assertIsNone(self.event_logger.logger_data)
+
+    def test_assignment_with_historical_exposed_at_timestamp(self):
+        self.set_up()
+        config = ContextConfig()
+        config.units = self.units
+        context = self.create_test_context(config, self.data_future_ready)
+        self.assertEqual(True, context.is_ready())
+        self.assertEqual(False, context.is_failed())
+
+        res = context.get_treatment(
+            "exp_test_historical_timestamp",
+            exposed_at = 1713218400000
+        )
+        exposure = context.exposures[0]
+        self.assertEqual(1713218400000, exposure.exposedAt)
+        context.close()
```

### Comparing `ABSmartly-0.2.2/test/test_default_audience_deserializer.py` & `absmartly-0.2.3/test/test_default_audience_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_default_context_data_deserializer.py` & `absmartly-0.2.3/test/test_default_context_data_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_default_context_event_serializer.py` & `absmartly-0.2.3/test/test_default_context_event_serializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_murmur32.py` & `absmartly-0.2.3/test/test_murmur32.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.2.2/test/test_variant_assigner.py` & `absmartly-0.2.3/test/test_variant_assigner.py`

 * *Files identical despite different names*

