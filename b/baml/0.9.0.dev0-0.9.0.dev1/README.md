# Comparing `tmp/baml-0.9.0.dev0.tar.gz` & `tmp/baml-0.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baml-0.9.0.dev0.tar", max compression
+gzip compressed data, was "baml-0.9.0.dev1.tar", max compression
```

## Comparing `baml-0.9.0.dev0.tar` & `baml-0.9.0.dev1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      511 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/__init__.py
--rw-r--r--   0        0        0      299 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/cache_manager/__init__.py
--rw-r--r--   0        0        0      556 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/cache_manager/abstract_cache_provider.py
--rw-r--r--   0        0        0     1378 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/cache_manager/cache_factory.py
--rw-r--r--   0        0        0     1859 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/cache_manager/cache_manager.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/configs/__init__.py
--rw-r--r--   0        0        0     1700 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/configs/retry_policy.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/errors/__init__.py
--rw-r--r--   0        0        0     1566 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/errors/llm_exc.py
--rw-r--r--   0        0        0      618 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/logger.py
--rw-r--r--   0        0        0      376 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/__init__.py
--rw-r--r--   0        0        0     2348 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/env.py
--rw-r--r--   0        0        0    15773 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/helper.py
--rw-r--r--   0        0        0      710 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/main.py
--rw-r--r--   0        0        0     9568 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/provider.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/py.typed
--rw-r--r--   0        0        0     3337 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/tracer.py
--rw-r--r--   0        0        0      284 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/otel/tracer.pyi
--rw-r--r--   0        0        0      362 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/provider_manager/__init__.py
--rw-r--r--   0        0        0     1311 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/provider_manager/llm_manager.py
--rw-r--r--   0        0        0    13865 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/provider_manager/llm_provider.py
--rw-r--r--   0        0        0     1320 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/provider_manager/llm_provider_factory.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/py.typed
--rw-r--r--   0        0        0      147 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/registrations/__init__.py
--rw-r--r--   0        0        0       66 2023-12-27 23:06:30.936024 baml-0.9.0.dev0/baml_core/registrations/caches/__init__.py
--rw-r--r--   0        0        0      752 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/caches/gloo_cache.py
--rw-r--r--   0        0        0      339 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/__init__.py
--rw-r--r--   0        0        0     3975 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/anthropic_provider.py
--rw-r--r--   0        0        0     5321 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/fallback_provider.py
--rw-r--r--   0        0        0     2057 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/openai_chat_provider.py
--rw-r--r--   0        0        0     1606 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/openai_completion_provider.py
--rw-r--r--   0        0        0     1027 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/registrations/providers/openai_helper.py
--rw-r--r--   0        0        0       58 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/services/__init__.py
--rw-r--r--   0        0        0     7490 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/services/api.py
--rw-r--r--   0        0        0    12727 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_core/services/api_types.py
--rw-r--r--   0        0        0      289 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/__init__.py
--rw-r--r--   0        0        0      292 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/__init__.py
--rw-r--r--   0        0        0     1913 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/base_deserialzier.py
--rw-r--r--   0        0        0     2997 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/complex_deserializer.py
--rw-r--r--   0        0        0     2939 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/deserialzier.py
--rw-r--r--   0        0        0     4507 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/diagnostics.py
--rw-r--r--   0        0        0     2202 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/enum_deserializer.py
--rw-r--r--   0        0        0     2224 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/exports.py
--rw-r--r--   0        0        0     3419 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/object_deserializer.py
--rw-r--r--   0        0        0     1371 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/primitive_deserialzier.py
--rw-r--r--   0        0        0      110 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/__init__.py
--rw-r--r--   0        0        0     1877 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/dict_wrapper.py
--rw-r--r--   0        0        0     1696 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/list_wrapper.py
--rw-r--r--   0        0        0     4245 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/loader.py
--rw-r--r--   0        0        0     4872 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/primitive_wrapper.py
--rw-r--r--   0        0        0     1205 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/raw_wrapper.py
--rw-r--r--   0        0        0     2955 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/test_raw_wrapper.py
--rw-r--r--   0        0        0      251 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/wrappers.py
--rw-r--r--   0        0        0     8160 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/test_deserializer.py
--rw-r--r--   0        0        0     2657 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/deserializer/type_definition.py
--rw-r--r--   0        0        0     8990 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/_impl/functions.py
--rw-r--r--   0        0        0     6003 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/helpers.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_lib/py.typed
--rw-r--r--   0        0        0       27 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_version/__init__.py
--rw-r--r--   0        0        0       78 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/baml_version/__main__.py
--rw-r--r--   0        0        0     1369 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pytest_baml/__init__.py
--rw-r--r--   0        0        0     1657 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pytest_baml/conftest.py
--rw-r--r--   0        0        0      102 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pytest_baml/exports.py
--rw-r--r--   0        0        0     1490 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pytest_baml/ipc_channel.py
--rw-r--r--   0        0        0        0 2023-12-27 23:06:30.940024 baml-0.9.0.dev0/pytest_baml/py.typed
--rw-r--r--   0        0        0    13994 2023-12-27 23:06:30.944024 baml-0.9.0.dev0/pytest_baml/pytest_baml.py
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 baml-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/__init__.py
+-rw-r--r--   0        0        0      299 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/cache_manager/__init__.py
+-rw-r--r--   0        0        0      556 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/cache_manager/abstract_cache_provider.py
+-rw-r--r--   0        0        0     1378 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/cache_manager/cache_factory.py
+-rw-r--r--   0        0        0     1859 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/cache_manager/cache_manager.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/configs/__init__.py
+-rw-r--r--   0        0        0     1700 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/configs/retry_policy.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/errors/__init__.py
+-rw-r--r--   0        0        0     1566 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/errors/llm_exc.py
+-rw-r--r--   0        0        0      618 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/logger.py
+-rw-r--r--   0        0        0      376 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/__init__.py
+-rw-r--r--   0        0        0     2348 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/env.py
+-rw-r--r--   0        0        0    15773 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/helper.py
+-rw-r--r--   0        0        0      710 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/main.py
+-rw-r--r--   0        0        0     9568 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/provider.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/py.typed
+-rw-r--r--   0        0        0     3337 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/tracer.py
+-rw-r--r--   0        0        0      284 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/otel/tracer.pyi
+-rw-r--r--   0        0        0      362 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/provider_manager/__init__.py
+-rw-r--r--   0        0        0     1528 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/provider_manager/llm_manager.py
+-rw-r--r--   0        0        0    15286 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/provider_manager/llm_provider.py
+-rw-r--r--   0        0        0     1320 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/provider_manager/llm_provider_factory.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/py.typed
+-rw-r--r--   0        0        0      147 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/__init__.py
+-rw-r--r--   0        0        0       66 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/caches/__init__.py
+-rw-r--r--   0        0        0      752 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/caches/gloo_cache.py
+-rw-r--r--   0        0        0      339 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/__init__.py
+-rw-r--r--   0        0        0     3975 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/anthropic_provider.py
+-rw-r--r--   0        0        0     5361 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/fallback_provider.py
+-rw-r--r--   0        0        0     2057 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/openai_chat_provider.py
+-rw-r--r--   0        0        0     1606 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/openai_completion_provider.py
+-rw-r--r--   0        0        0     1027 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/registrations/providers/openai_helper.py
+-rw-r--r--   0        0        0       58 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/services/__init__.py
+-rw-r--r--   0        0        0     7490 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/services/api.py
+-rw-r--r--   0        0        0    12727 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_core/services/api_types.py
+-rw-r--r--   0        0        0      289 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/__init__.py
+-rw-r--r--   0        0        0      292 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/__init__.py
+-rw-r--r--   0        0        0     1913 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/base_deserialzier.py
+-rw-r--r--   0        0        0     2997 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/complex_deserializer.py
+-rw-r--r--   0        0        0     2939 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/deserialzier.py
+-rw-r--r--   0        0        0     4507 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/diagnostics.py
+-rw-r--r--   0        0        0     2202 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/enum_deserializer.py
+-rw-r--r--   0        0        0     2224 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/exports.py
+-rw-r--r--   0        0        0     3419 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/object_deserializer.py
+-rw-r--r--   0        0        0     1371 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/primitive_deserialzier.py
+-rw-r--r--   0        0        0      110 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/__init__.py
+-rw-r--r--   0        0        0     1877 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/dict_wrapper.py
+-rw-r--r--   0        0        0     1696 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/list_wrapper.py
+-rw-r--r--   0        0        0     4245 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/loader.py
+-rw-r--r--   0        0        0     4872 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/primitive_wrapper.py
+-rw-r--r--   0        0        0     1205 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/raw_wrapper.py
+-rw-r--r--   0        0        0     2955 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/test_raw_wrapper.py
+-rw-r--r--   0        0        0      251 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/wrappers.py
+-rw-r--r--   0        0        0     8160 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/test_deserializer.py
+-rw-r--r--   0        0        0     2657 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/deserializer/type_definition.py
+-rw-r--r--   0        0        0     8990 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/_impl/functions.py
+-rw-r--r--   0        0        0     5927 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/helpers.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_lib/py.typed
+-rw-r--r--   0        0        0       27 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_version/__init__.py
+-rw-r--r--   0        0        0       78 2024-01-04 07:44:16.196487 baml-0.9.0.dev1/baml_version/__main__.py
+-rw-r--r--   0        0        0     1369 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/__init__.py
+-rw-r--r--   0        0        0     1657 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/conftest.py
+-rw-r--r--   0        0        0      102 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/exports.py
+-rw-r--r--   0        0        0     1490 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/ipc_channel.py
+-rw-r--r--   0        0        0        0 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/py.typed
+-rw-r--r--   0        0        0    13994 2024-01-04 07:44:16.200487 baml-0.9.0.dev1/pytest_baml/pytest_baml.py
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 baml-0.9.0.dev1/PKG-INFO
```

### Comparing `baml-0.9.0.dev0/baml_core/cache_manager/abstract_cache_provider.py` & `baml-0.9.0.dev1/baml_core/cache_manager/abstract_cache_provider.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/cache_manager/cache_factory.py` & `baml-0.9.0.dev1/baml_core/cache_manager/cache_factory.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/cache_manager/cache_manager.py` & `baml-0.9.0.dev1/baml_core/cache_manager/cache_manager.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/configs/retry_policy.py` & `baml-0.9.0.dev1/baml_core/configs/retry_policy.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/errors/llm_exc.py` & `baml-0.9.0.dev1/baml_core/errors/llm_exc.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/logger.py` & `baml-0.9.0.dev1/baml_core/logger.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/otel/env.py` & `baml-0.9.0.dev1/baml_core/otel/env.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/otel/helper.py` & `baml-0.9.0.dev1/baml_core/otel/helper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/otel/main.py` & `baml-0.9.0.dev1/baml_core/otel/main.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/otel/provider.py` & `baml-0.9.0.dev1/baml_core/otel/provider.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/otel/tracer.py` & `baml-0.9.0.dev1/baml_core/otel/tracer.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/provider_manager/llm_manager.py` & `baml-0.9.0.dev1/baml_core/provider_manager/llm_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from .llm_provider_factory import llm_provider_factory
 from .llm_provider import AbstractLLMProvider
 from ..logger import logger
 
 
 class _LLMManager:
     __llms: typing.Dict[str, AbstractLLMProvider]
+    __validated: bool
 
     def __init__(self) -> None:
         self.__llms = {}
+        self.__validated = False
 
     def add_llm(
         self, *, name: str, provider: str, **kwargs: typing.Any
     ) -> AbstractLLMProvider:
         if name in self.__llms:
             raise ValueError(f"LLM with {name} already exists")
         self.__llms[name] = llm_provider_factory(provider=provider, **kwargs)
@@ -23,21 +25,25 @@
         if name not in self.__llms:
             raise ValueError(
                 f"LLM {name} not found. You can use one of {self.__llms.keys()}"
             )
         return self.__llms[name]
 
     def validate(self) -> None:
-        errors = []
+        if self.__validated:
+            assert False, "LLMManager already validated"
+
+        errors: typing.List[typing.Tuple[str, Exception]] = []
         for name, llm in self.__llms.items():
             try:
                 llm.validate()
             except Exception as e:
                 errors.append((name, e))
         if len(errors) > 0:
             # Print all errors
             for name, err in errors:
                 logger.error(f"Validating {name} Failed: {err}")
             raise ValueError("LLM validation failed")
+        self.__validated = True
 
 
 LLMManager = _LLMManager()
```

### Comparing `baml-0.9.0.dev0/baml_core/provider_manager/llm_provider.py` & `baml-0.9.0.dev1/baml_core/provider_manager/llm_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,36 +118,83 @@
         self.__retry_policy = retry_policy
         assert not kwargs, f"Unhandled provider settings: {', '.join(kwargs.keys())}"
 
     @property
     def provider(self) -> str:
         return self.__provider
 
-    @abc.abstractmethod
+    #
+    # Public API
+    #
+    @typing.final
+    @typechecked
+    async def run_prompt_template(
+        self,
+        *,
+        template: str,
+        replacers: typing.Iterable[str],
+        params: typing.Dict[str, typing.Any],
+    ) -> LLMResponse:
+        return await self._run_prompt_template_internal(
+            template=template,
+            replacers=replacers,
+            params=params,
+        )
+
+    @typing.final
+    @typechecked
+    async def run_chat_template(
+        self,
+        *message_templates: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]],
+        replacers: typing.Iterable[str],
+        params: typing.Dict[str, typing.Any],
+    ) -> LLMResponse:
+        return await self._run_chat_template_internal(
+            *message_templates,
+            replacers=replacers,
+            params=params,
+        )
+
+    @typing.final
+    @typechecked
     async def run_prompt(self, prompt: str) -> LLMResponse:
+        return await self._run_prompt_internal(prompt=prompt)
+
+    @typing.final
+    @typechecked
+    async def run_chat(
+        self, *messages: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]]
+    ) -> LLMResponse:
+        return await self._run_chat_internal(*messages)
+
+    #
+    # Internal API
+    #
+    @abc.abstractmethod
+    async def _run_prompt_internal(self, prompt: str) -> LLMResponse:
         pass
 
     @abc.abstractmethod
-    async def run_prompt_template(
+    async def _run_prompt_template_internal(
         self,
         *,
         template: str,
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         pass
 
     @abc.abstractmethod
-    async def run_chat(
+    async def _run_chat_internal(
         self, *messages: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]]
     ) -> LLMResponse:
         pass
 
     @abc.abstractmethod
-    async def run_chat_template(
+    async def _run_chat_template_internal(
         self,
         *message_templates: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]],
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         pass
 
@@ -267,15 +314,15 @@
         **kwargs: typing.Any,
     ) -> None:
         super().__init__(**kwargs)
         self.__chat_to_prompt = chat_to_prompt
 
     @typing.final
     @typechecked
-    async def run_prompt_template(
+    async def _run_prompt_template_internal(
         self,
         *,
         template: str,
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         updates = {k: k.format(**params) for k in replacers}
@@ -293,51 +340,51 @@
         try:
             return await self.__run(prompt)
         except Exception as e:
             self._raise_error(e)
 
     @typing.final
     @typechecked
-    async def run_chat_template(
+    async def _run_chat_template_internal(
         self,
         *message_templates: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]],
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         if len(message_templates) == 1 and isinstance(message_templates[0], list):
             chats = message_templates[0]
         else:
             chats = typing.cast(typing.List[LLMChatMessage], message_templates)
-        return await self.run_prompt_template(
+        return await self._run_prompt_template_internal(
             template=self.__chat_to_prompt(chats),
             replacers=replacers,
             params=params,
         )
 
     @typing.final
     @typechecked
-    async def run_prompt(self, prompt: str) -> LLMResponse:
+    async def _run_prompt_internal(self, prompt: str) -> LLMResponse:
         if cached := self._check_cache(prompt=prompt, prompt_vars={}):
             return cached
 
         try:
             return await self.__run(prompt)
         except Exception as e:
             self._raise_error(e)
 
     @typing.final
     @typechecked
-    async def run_chat(
+    async def _run_chat_internal(
         self, *messages: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]]
     ) -> LLMResponse:
         if len(messages) == 1 and isinstance(messages[0], list):
             chats = messages[0]
         else:
             chats = typing.cast(typing.List[LLMChatMessage], messages)
-        return await self.run_prompt(self.__chat_to_prompt(chats))
+        return await self._run_prompt_internal(self.__chat_to_prompt(chats))
 
     @typing.final
     async def __run(self, prompt: str) -> LLMResponse:
         self._start_run(prompt)
         response = await self._run(prompt)
         self._end_run(response)
         return response
@@ -356,28 +403,28 @@
         **kwargs: typing.Any,
     ) -> None:
         super().__init__(**kwargs)
         self.__prompt_to_chat = prompt_to_chat
 
     @typing.final
     @typechecked
-    async def run_prompt_template(
+    async def _run_prompt_template_internal(
         self,
         *,
         template: str,
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
-        return await self.run_chat_template(
+        return await self._run_chat_template_internal(
             [self.__prompt_to_chat(template)], replacers=replacers, params=params
         )
 
     @typing.final
     @typechecked
-    async def run_chat_template(
+    async def _run_chat_template_internal(
         self,
         *message_templates: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]],
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         updates = {k: k.format(**params) for k in replacers}
         if len(message_templates) == 1 and isinstance(message_templates[0], list):
@@ -412,19 +459,19 @@
 
         try:
             return await self.__run_chat(messages)
         except Exception as e:
             self._raise_error(e)
 
     @typechecked
-    async def run_prompt(self, prompt: str) -> LLMResponse:
-        return await self.run_chat([self.__prompt_to_chat(prompt)])
+    async def _run_prompt_internal(self, prompt: str) -> LLMResponse:
+        return await self._run_chat_internal([self.__prompt_to_chat(prompt)])
 
     @typechecked
-    async def run_chat(
+    async def _run_chat_internal(
         self, *messages: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]]
     ) -> LLMResponse:
         if len(messages) == 1 and isinstance(messages[0], list):
             chat_message = messages[0]
         else:
             chat_message = typing.cast(typing.List[LLMChatMessage], messages)
```

### Comparing `baml-0.9.0.dev0/baml_core/provider_manager/llm_provider_factory.py` & `baml-0.9.0.dev1/baml_core/provider_manager/llm_provider_factory.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/registrations/caches/gloo_cache.py` & `baml-0.9.0.dev1/baml_core/registrations/caches/gloo_cache.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/registrations/providers/anthropic_provider.py` & `baml-0.9.0.dev1/baml_core/registrations/providers/anthropic_provider.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/registrations/providers/fallback_provider.py` & `baml-0.9.0.dev1/baml_core/registrations/providers/fallback_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,34 +125,34 @@
                 )
             except Exception as e:
                 error_code = self._to_error_code(e)
                 last_exception = e
         assert last_exception is not None, "Should have caught an exception"
         raise last_exception
 
-    async def run_prompt(self, prompt: str) -> LLMResponse:
+    async def _run_prompt_internal(self, prompt: str) -> LLMResponse:
         return await self._run_strategy("run_prompt", prompt)
 
-    async def run_prompt_template(
+    async def _run_prompt_template_internal(
         self,
         *,
         template: str,
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         return await self._run_strategy(
             "run_prompt_template", template=template, replacers=replacers, params=params
         )
 
-    async def run_chat(
+    async def _run_chat_internal(
         self, *messages: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]]
     ) -> LLMResponse:
         return await self._run_strategy("run_chat", *messages)
 
-    async def run_chat_template(
+    async def _run_chat_template_internal(
         self,
         *message_templates: typing.Union[LLMChatMessage, typing.List[LLMChatMessage]],
         replacers: typing.Iterable[str],
         params: typing.Dict[str, typing.Any],
     ) -> LLMResponse:
         return await self._run_strategy(
             "run_chat_template",
```

### Comparing `baml-0.9.0.dev0/baml_core/registrations/providers/openai_chat_provider.py` & `baml-0.9.0.dev1/baml_core/registrations/providers/openai_chat_provider.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/registrations/providers/openai_completion_provider.py` & `baml-0.9.0.dev1/baml_core/registrations/providers/openai_completion_provider.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/registrations/providers/openai_helper.py` & `baml-0.9.0.dev1/baml_core/registrations/providers/openai_helper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/services/api.py` & `baml-0.9.0.dev1/baml_core/services/api.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_core/services/api_types.py` & `baml-0.9.0.dev1/baml_core/services/api_types.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/base_deserialzier.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/base_deserialzier.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/complex_deserializer.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/complex_deserializer.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/deserialzier.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/deserialzier.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/diagnostics.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/diagnostics.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/enum_deserializer.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/enum_deserializer.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/exports.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/exports.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/object_deserializer.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/object_deserializer.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/primitive_deserialzier.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/primitive_deserialzier.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/dict_wrapper.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/list_wrapper.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/list_wrapper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/loader.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/loader.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/primitive_wrapper.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/primitive_wrapper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/raw_wrapper.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/raw_wrapper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/raw_wrapper/test_raw_wrapper.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/raw_wrapper/test_raw_wrapper.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/test_deserializer.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/deserializer/type_definition.py` & `baml-0.9.0.dev1/baml_lib/_impl/deserializer/type_definition.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/_impl/functions.py` & `baml-0.9.0.dev1/baml_lib/_impl/functions.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/baml_lib/helpers.py` & `baml-0.9.0.dev1/baml_lib/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import typing
 import uuid
 
-from baml_core.provider_manager import LLMManager
 from baml_core.cache_manager import CacheManager
 from baml_core import otel
 from baml_core.services.api import APIWrapper
 from baml_core.logger import logger
 from baml_core.otel.provider import set_print_log_level
 import logging
 
@@ -167,9 +166,8 @@
             logger.info("Using GlooCache")
             CacheManager.add_cache("gloo", api=__CachedParams.api)
         else:
             logger.warning(
                 "Wanted to use GlooCache but no API key was provided. Did you set BOUNDARY_PROJECT_ID and BOUNDARY_SECRET?"
             )
 
-    LLMManager.validate()
     return __InternalBAMLConfig(api=__CachedParams.api)
```

### Comparing `baml-0.9.0.dev0/pyproject.toml` & `baml-0.9.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "baml"
-version = "0.9.0.dev0"
+version = "0.9.0.dev1"
 description = ""
 authors = [ "Gloo <contact@trygloo.com>",]
 
 [[tool.poetry.packages]]
 include = "baml_core"
 from = "."
```

### Comparing `baml-0.9.0.dev0/pytest_baml/conftest.py` & `baml-0.9.0.dev1/pytest_baml/conftest.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/pytest_baml/ipc_channel.py` & `baml-0.9.0.dev1/pytest_baml/ipc_channel.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/pytest_baml/pytest_baml.py` & `baml-0.9.0.dev1/pytest_baml/pytest_baml.py`

 * *Files identical despite different names*

### Comparing `baml-0.9.0.dev0/PKG-INFO` & `baml-0.9.0.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baml
-Version: 0.9.0.dev0
+Version: 0.9.0.dev1
 Summary: 
 Author: Gloo
 Author-email: contact@trygloo.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

