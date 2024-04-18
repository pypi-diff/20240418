# Comparing `tmp/snowflake-connector-python-3.8.1.tar.gz` & `tmp/snowflake_connector_python-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-3.8.1.tar", last modified: Mon Apr  8 23:44:56 2024, max compression
+gzip compressed data, was "snowflake_connector_python-3.9.0.tar", last modified: Thu Apr 18 18:18:21 2024, max compression
```

## Comparing `snowflake-connector-python-3.8.1.tar` & `snowflake_connector_python-3.9.0.tar`

### file list

```diff
@@ -1,257 +1,258 @@
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.107035 snowflake-connector-python-3.8.1/
--rw-r--r--   0 user      (1006) user      (1006)     1701 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/CONTRIBUTING.md
--rw-r--r--   0 user      (1006) user      (1006)    58487 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/DESCRIPTION.md
--rw-r--r--   0 user      (1006) user      (1006)    11365 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)      926 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/MANIFEST.in
--rw-r--r--   0 user      (1006) user      (1006)      457 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/NOTICE
--rw-r--r--   0 user      (1006) user      (1006)    61991 2024-04-08 23:44:56.107035 snowflake-connector-python-3.8.1/PKG-INFO
--rw-r--r--   0 user      (1006) user      (1006)     3045 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/README.md
--rw-r--r--   0 user      (1006) user      (1006)      308 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/SECURITY.md
--rw-r--r--   0 user      (1006) user      (1006)      593 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/pyproject.toml
--rw-r--r--   0 user      (1006) user      (1006)     3018 2024-04-08 23:44:56.107035 snowflake-connector-python-3.8.1/setup.cfg
--rw-r--r--   0 user      (1006) user      (1006)     6914 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/setup.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.059035 snowflake-connector-python-3.8.1/src/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.055035 snowflake-connector-python-3.8.1/src/snowflake/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.071035 snowflake-connector-python-3.8.1/src/snowflake/connector/
--rw-r--r--   0 user      (1006) user      (1006)     1759 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    11339 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 user      (1006) user      (1006)     1521 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 user      (1006) user      (1006)     5381 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/arrow_context.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.071035 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/
--rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    27978 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 user      (1006) user      (1006)     7050 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 user      (1006) user      (1006)     1034 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/default.py
--rw-r--r--   0 user      (1006) user      (1006)     2127 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 user      (1006) user      (1006)     6678 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 user      (1006) user      (1006)     1488 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 user      (1006) user      (1006)    11394 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 user      (1006) user      (1006)     1981 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 user      (1006) user      (1006)    17958 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 user      (1006) user      (1006)     9913 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     4346 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/backoff_policies.py
--rw-r--r--   0 user      (1006) user      (1006)     2355 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 user      (1006) user      (1006)    23454 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/cache.py
--rw-r--r--   0 user      (1006) user      (1006)     2894 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/compat.py
--rw-r--r--   0 user      (1006) user      (1006)    19252 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/config_manager.py
--rw-r--r--   0 user      (1006) user      (1006)    75785 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/connection.py
--rw-r--r--   0 user      (1006) user      (1006)    32728 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 user      (1006) user      (1006)    12971 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/constants.py
--rw-r--r--   0 user      (1006) user      (1006)    27710 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/converter.py
--rw-r--r--   0 user      (1006) user      (1006)     2864 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 user      (1006) user      (1006)      437 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/converter_null.py
--rw-r--r--   0 user      (1006) user      (1006)     7633 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/converter_snowsql.py
--rw-r--r--   0 user      (1006) user      (1006)    64707 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/cursor.py
--rw-r--r--   0 user      (1006) user      (1006)     1268 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/dbapi.py
--rw-r--r--   0 user      (1006) user      (1006)      615 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/description.py
--rw-r--r--   0 user      (1006) user      (1006)     8018 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 user      (1006) user      (1006)     2708 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/errorcode.py
--rw-r--r--   0 user      (1006) user      (1006)    20185 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/errors.py
--rw-r--r--   0 user      (1006) user      (1006)      184 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/feature.py
--rw-r--r--   0 user      (1006) user      (1006)     3246 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 user      (1006) user      (1006)    48252 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 user      (1006) user      (1006)     5011 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/file_util.py
--rw-r--r--   0 user      (1006) user      (1006)    16072 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     2802 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 user      (1006) user      (1006)     3162 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/local_storage_client.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.055035 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.079035 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
--rw-r--r--   0 user      (1006) user      (1006)     2039 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      765 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      633 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      547 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      499 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      503 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    19180 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2407 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)     4462 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4477 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)    42047 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4892 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1535 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      994 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     3655 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1788 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     2739 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      659 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      758 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      490 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)      750 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1011 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    11583 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)     2634 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      811 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1424 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      794 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.083035 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
--rw-r--r--   0 user      (1006) user      (1006)      216 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2522 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 user      (1006) user      (1006)      940 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1379 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 user      (1006) user      (1006)      933 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 user      (1006) user      (1006)      631 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      571 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1248 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)      708 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 user      (1006) user      (1006)    13329 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 user      (1006) user      (1006)     4114 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.083035 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
--rw-r--r--   0 user      (1006) user      (1006)      470 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 user      (1006) user      (1006)     1963 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 user      (1006) user      (1006)     2262 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.087036 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
--rw-r--r--   0 user      (1006) user      (1006)     6007 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
--rw-r--r--   0 user      (1006) user      (1006)     3515 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
--rw-r--r--   0 user      (1006) user      (1006)     1178 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
--rw-r--r--   0 user      (1006) user      (1006)    79675 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
--rw-r--r--   0 user      (1006) user      (1006)     7437 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
--rw-r--r--   0 user      (1006) user      (1006)     3998 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
--rw-r--r--   0 user      (1006) user      (1006)      119 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
--rw-r--r--   0 user      (1006) user      (1006)     1380 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
--rw-r--r--   0 user      (1006) user      (1006)     4778 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
--rw-r--r--   0 user      (1006) user      (1006)      575 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
--rw-r--r--   0 user      (1006) user      (1006)      165 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
--rw-r--r--   0 user      (1006) user      (1006)     4826 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
--rw-r--r--   0 user      (1006) user      (1006)     4917 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
--rw-r--r--   0 user      (1006) user      (1006)     3091 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
--rw-r--r--   0 user      (1006) user      (1006)    10913 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.087036 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
--rw-r--r--   0 user      (1006) user      (1006)      198 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
--rw-r--r--   0 user      (1006) user      (1006)     5852 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
--rw-r--r--   0 user      (1006) user      (1006)     2400 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
--rw-r--r--   0 user      (1006) user      (1006)     2613 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
--rw-r--r--   0 user      (1006) user      (1006)      600 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
--rw-r--r--   0 user      (1006) user      (1006)     1179 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
--rw-r--r--   0 user      (1006) user      (1006)     5284 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
--rw-r--r--   0 user      (1006) user      (1006)     3719 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
--rw-r--r--   0 user      (1006) user      (1006)      424 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
--rw-r--r--   0 user      (1006) user      (1006)     1064 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
--rw-r--r--   0 user      (1006) user      (1006)      104 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
--rw-r--r--   0 user      (1006) user      (1006)      677 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
--rw-r--r--   0 user      (1006) user      (1006)     1844 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
--rw-r--r--   0 user      (1006) user      (1006)     4295 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
--rw-r--r--   0 user      (1006) user      (1006)    31201 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
--rw-r--r--   0 user      (1006) user      (1006)     8882 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
--rw-r--r--   0 user      (1006) user      (1006)      190 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
--rw-r--r--   0 user      (1006) user      (1006)     1645 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
--rw-r--r--   0 user      (1006) user      (1006)   102952 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
--rw-r--r--   0 user      (1006) user      (1006)   107680 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
--rw-r--r--   0 user      (1006) user      (1006)   132283 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
--rw-r--r--   0 user      (1006) user      (1006)    12046 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
--rw-r--r--   0 user      (1006) user      (1006)     8404 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
--rw-r--r--   0 user      (1006) user      (1006)    18580 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
--rw-r--r--   0 user      (1006) user      (1006)    14382 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
--rw-r--r--   0 user      (1006) user      (1006)  1616169 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
--rw-r--r--   0 user      (1006) user      (1006)    17533 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.091035 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/Logging/
--rw-r--r--   0 user      (1006) user      (1006)     3113 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
--rw-r--r--   0 user      (1006) user      (1006)     1344 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
--rw-r--r--   0 user      (1006) user      (1006)    42377 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/network.py
--rw-r--r--   0 user      (1006) user      (1006)    16575 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 user      (1006) user      (1006)    69704 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 user      (1006) user      (1006)     4782 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/options.py
--rw-r--r--   0 user      (1006) user      (1006)    22495 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 user      (1006) user      (1006)     1582 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/proxy.py
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/py.typed
--rw-r--r--   0 user      (1006) user      (1006)    26617 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/result_batch.py
--rw-r--r--   0 user      (1006) user      (1006)     9380 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/result_set.py
--rw-r--r--   0 user      (1006) user      (1006)    21870 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 user      (1006) user      (1006)     1957 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 user      (1006) user      (1006)     1120 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 user      (1006) user      (1006)    12449 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 user      (1006) user      (1006)     4313 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 user      (1006) user      (1006)      432 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 user      (1006) user      (1006)      813 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 user      (1006) user      (1006)     4563 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 user      (1006) user      (1006)    17583 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/storage_client.py
--rw-r--r--   0 user      (1006) user      (1006)     8861 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/telemetry.py
--rw-r--r--   0 user      (1006) user      (1006)    19070 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 user      (1006) user      (1006)      982 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/test_util.py
--rw-r--r--   0 user      (1006) user      (1006)     5073 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.091035 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/
--rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 user      (1006) user      (1006)     4575 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 user      (1006) user      (1006)     6643 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 user      (1006) user      (1006)     2119 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 user      (1006) user      (1006)     1021 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/url_util.py
--rw-r--r--   0 user      (1006) user      (1006)    10405 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.091035 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/
--rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.095035 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 user      (1006) user      (1006)    10142 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 user      (1006) user      (1006)     4742 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)      435 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 user      (1006) user      (1006)     1495 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 user      (1006) user      (1006)    19577 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 user      (1006) user      (1006)     6449 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 user      (1006) user      (1006)    10187 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 user      (1006) user      (1006)      429 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 user      (1006) user      (1006)     1451 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 user      (1006) user      (1006)    18560 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 user      (1006) user      (1006)     3813 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 user      (1006) user      (1006)     3885 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 user      (1006) user      (1006)      733 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 user      (1006) user      (1006)    35231 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 user      (1006) user      (1006)    30373 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 user      (1006) user      (1006)     4235 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 user      (1006) user      (1006)     2912 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 user      (1006) user      (1006)    33450 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.095035 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 user      (1006) user      (1006)     1115 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 user      (1006) user      (1006)     2763 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    11372 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 user      (1006) user      (1006)       64 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 user      (1006) user      (1006)    20300 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 user      (1006) user      (1006)    40285 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.099036 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)      957 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.099036 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)    17632 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user      (1006) user      (1006)    13922 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user      (1006) user      (1006)    11012 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 user      (1006) user      (1006)     4528 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user      (1006) user      (1006)    16772 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user      (1006) user      (1006)    34431 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 user      (1006) user      (1006)     7097 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 user      (1006) user      (1006)     8217 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 user      (1006) user      (1006)     8579 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 user      (1006) user      (1006)     2440 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.099036 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.099036 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     1417 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0 user      (1006) user      (1006)    34665 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 user      (1006) user      (1006)    19990 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 user      (1006) user      (1006)     6691 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 user      (1006) user      (1006)    30760 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.103036 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 user      (1006) user      (1006)     1155 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 user      (1006) user      (1006)     5376 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 user      (1006) user      (1006)     1605 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 user      (1006) user      (1006)      498 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 user      (1006) user      (1006)     4225 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 user      (1006) user      (1006)     3510 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 user      (1006) user      (1006)    22013 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 user      (1006) user      (1006)    17165 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 user      (1006) user      (1006)     5758 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user      (1006) user      (1006)     6895 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 user      (1006) user      (1006)    10168 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 user      (1006) user      (1006)    14279 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 user      (1006) user      (1006)     5403 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 user      (1006) user      (1006)      107 2024-04-08 23:42:32.000000 snowflake-connector-python-3.8.1/src/snowflake/connector/version.py
-drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-08 23:44:56.103036 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/
--rw-r--r--   0 user      (1006) user      (1006)    61991 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1006) user      (1006)    13218 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1006) user      (1006)      322 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/entry_points.txt
--rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-08 23:43:15.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1006) user      (1006)      646 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/requires.txt
--rw-r--r--   0 user      (1006) user      (1006)       10 2024-04-08 23:44:56.000000 snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.100420 snowflake_connector_python-3.9.0/
+-rw-r--r--   0 user      (1006) user      (1006)     1701 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/CONTRIBUTING.md
+-rw-r--r--   0 user      (1006) user      (1006)    58717 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/DESCRIPTION.md
+-rw-r--r--   0 user      (1006) user      (1006)    11365 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)      926 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/MANIFEST.in
+-rw-r--r--   0 user      (1006) user      (1006)      457 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/NOTICE
+-rw-r--r--   0 user      (1006) user      (1006)    62221 2024-04-18 18:18:21.100420 snowflake_connector_python-3.9.0/PKG-INFO
+-rw-r--r--   0 user      (1006) user      (1006)     3045 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/README.md
+-rw-r--r--   0 user      (1006) user      (1006)      308 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/SECURITY.md
+-rw-r--r--   0 user      (1006) user      (1006)      593 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/pyproject.toml
+-rw-r--r--   0 user      (1006) user      (1006)     3018 2024-04-18 18:18:21.100420 snowflake_connector_python-3.9.0/setup.cfg
+-rw-r--r--   0 user      (1006) user      (1006)     6914 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/setup.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.052420 snowflake_connector_python-3.9.0/src/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.048420 snowflake_connector_python-3.9.0/src/snowflake/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.064420 snowflake_connector_python-3.9.0/src/snowflake/connector/
+-rw-r--r--   0 user      (1006) user      (1006)     1845 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    11339 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     1521 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     5381 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.064420 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/
+-rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    27978 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 user      (1006) user      (1006)     7050 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 user      (1006) user      (1006)     1034 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 user      (1006) user      (1006)     2127 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 user      (1006) user      (1006)     6678 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 user      (1006) user      (1006)     1488 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 user      (1006) user      (1006)    11394 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 user      (1006) user      (1006)     1981 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 user      (1006) user      (1006)    17958 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 user      (1006) user      (1006)     9913 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     4346 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/backoff_policies.py
+-rw-r--r--   0 user      (1006) user      (1006)     2355 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 user      (1006) user      (1006)    23454 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     2894 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/compat.py
+-rw-r--r--   0 user      (1006) user      (1006)    19252 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 user      (1006) user      (1006)    75979 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)    32728 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 user      (1006) user      (1006)    12971 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/constants.py
+-rw-r--r--   0 user      (1006) user      (1006)    27710 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/converter.py
+-rw-r--r--   0 user      (1006) user      (1006)     2864 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 user      (1006) user      (1006)      437 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 user      (1006) user      (1006)     7633 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/converter_snowsql.py
+-rw-r--r--   0 user      (1006) user      (1006)    64707 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/cursor.py
+-rw-r--r--   0 user      (1006) user      (1006)     1268 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 user      (1006) user      (1006)      615 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/description.py
+-rw-r--r--   0 user      (1006) user      (1006)     8018 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     2708 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 user      (1006) user      (1006)    20185 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/errors.py
+-rw-r--r--   0 user      (1006) user      (1006)      184 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/feature.py
+-rw-r--r--   0 user      (1006) user      (1006)     3246 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 user      (1006) user      (1006)    48252 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 user      (1006) user      (1006)     5011 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/file_util.py
+-rw-r--r--   0 user      (1006) user      (1006)    16072 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     2802 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 user      (1006) user      (1006)     3162 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     2505 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/log_configuration.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.048420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.076420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
+-rw-r--r--   0 user      (1006) user      (1006)     2039 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      765 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      633 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      547 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      499 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      503 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    19180 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2407 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     4462 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4477 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    42047 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4892 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1535 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      994 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     3655 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1788 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     2739 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      659 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      991 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      758 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      490 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      750 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1011 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    11583 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)     2634 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      811 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1424 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      794 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.076420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
+-rw-r--r--   0 user      (1006) user      (1006)      216 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2522 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      940 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1379 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      933 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 user      (1006) user      (1006)      631 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      571 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1248 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)      708 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    13329 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     4114 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.076420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
+-rw-r--r--   0 user      (1006) user      (1006)      470 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     1963 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     2262 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.080420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 user      (1006) user      (1006)     6007 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 user      (1006) user      (1006)     3515 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 user      (1006) user      (1006)     1178 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 user      (1006) user      (1006)    79675 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 user      (1006) user      (1006)     7437 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 user      (1006) user      (1006)     3998 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 user      (1006) user      (1006)      119 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 user      (1006) user      (1006)     1380 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 user      (1006) user      (1006)     4778 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 user      (1006) user      (1006)      575 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 user      (1006) user      (1006)      165 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 user      (1006) user      (1006)     4826 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 user      (1006) user      (1006)     4917 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 user      (1006) user      (1006)     3091 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 user      (1006) user      (1006)    10913 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.084420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 user      (1006) user      (1006)      198 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 user      (1006) user      (1006)     5852 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 user      (1006) user      (1006)     2400 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 user      (1006) user      (1006)     2613 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 user      (1006) user      (1006)      600 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 user      (1006) user      (1006)     1179 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 user      (1006) user      (1006)     5284 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 user      (1006) user      (1006)     3719 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 user      (1006) user      (1006)      424 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 user      (1006) user      (1006)     1064 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 user      (1006) user      (1006)      104 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 user      (1006) user      (1006)      677 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 user      (1006) user      (1006)     1844 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 user      (1006) user      (1006)     4295 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 user      (1006) user      (1006)    31201 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 user      (1006) user      (1006)     8882 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 user      (1006) user      (1006)      190 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 user      (1006) user      (1006)     1645 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 user      (1006) user      (1006)   102952 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 user      (1006) user      (1006)   107680 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 user      (1006) user      (1006)   132283 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 user      (1006) user      (1006)    12046 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 user      (1006) user      (1006)     8404 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
+-rw-r--r--   0 user      (1006) user      (1006)    18580 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 user      (1006) user      (1006)    14382 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 user      (1006) user      (1006)  1616169 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 user      (1006) user      (1006)    17533 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.084420 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/Logging/
+-rw-r--r--   0 user      (1006) user      (1006)     3113 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
+-rw-r--r--   0 user      (1006) user      (1006)     1344 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
+-rw-r--r--   0 user      (1006) user      (1006)    42377 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/network.py
+-rw-r--r--   0 user      (1006) user      (1006)    16575 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 user      (1006) user      (1006)    69704 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 user      (1006) user      (1006)     4782 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/options.py
+-rw-r--r--   0 user      (1006) user      (1006)    22495 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 user      (1006) user      (1006)     1582 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/proxy.py
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/py.typed
+-rw-r--r--   0 user      (1006) user      (1006)    26617 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 user      (1006) user      (1006)     9380 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/result_set.py
+-rw-r--r--   0 user      (1006) user      (1006)    22085 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 user      (1006) user      (1006)     1957 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 user      (1006) user      (1006)     1120 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 user      (1006) user      (1006)    12449 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 user      (1006) user      (1006)     4313 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 user      (1006) user      (1006)      432 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 user      (1006) user      (1006)      813 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 user      (1006) user      (1006)     4563 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 user      (1006) user      (1006)    17583 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 user      (1006) user      (1006)     8861 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 user      (1006) user      (1006)    19070 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 user      (1006) user      (1006)      982 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/test_util.py
+-rw-r--r--   0 user      (1006) user      (1006)     5073 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.084420 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/
+-rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1485 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 user      (1006) user      (1006)     4575 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 user      (1006) user      (1006)     6643 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 user      (1006) user      (1006)     2119 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 user      (1006) user      (1006)     1021 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/url_util.py
+-rw-r--r--   0 user      (1006) user      (1006)    10405 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.084420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/
+-rw-r--r--   0 user      (1006) user      (1006)       76 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.088420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 user      (1006) user      (1006)    10142 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 user      (1006) user      (1006)     4742 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)      435 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1495 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 user      (1006) user      (1006)    19577 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 user      (1006) user      (1006)     6449 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 user      (1006) user      (1006)    10187 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 user      (1006) user      (1006)      429 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 user      (1006) user      (1006)     1451 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 user      (1006) user      (1006)    18560 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 user      (1006) user      (1006)     3813 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 user      (1006) user      (1006)     3885 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 user      (1006) user      (1006)      733 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 user      (1006) user      (1006)    35231 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 user      (1006) user      (1006)    30373 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 user      (1006) user      (1006)     4235 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 user      (1006) user      (1006)     2912 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 user      (1006) user      (1006)    33450 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.092420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 user      (1006) user      (1006)     1115 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 user      (1006) user      (1006)     2763 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    11372 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 user      (1006) user      (1006)       64 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 user      (1006) user      (1006)    20300 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)    40285 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.092420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)      957 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.092420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)    17632 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user      (1006) user      (1006)    13922 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user      (1006) user      (1006)    11012 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 user      (1006) user      (1006)     4528 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user      (1006) user      (1006)    16772 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user      (1006) user      (1006)    34431 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user      (1006) user      (1006)     7097 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 user      (1006) user      (1006)     8217 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 user      (1006) user      (1006)     8579 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 user      (1006) user      (1006)     2440 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.092420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.092420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 user      (1006) user      (1006)        0 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     1417 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user      (1006) user      (1006)     5343 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 user      (1006) user      (1006)    34665 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 user      (1006) user      (1006)    19990 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 user      (1006) user      (1006)     6691 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 user      (1006) user      (1006)    30760 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.096420 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 user      (1006) user      (1006)     1155 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 user      (1006) user      (1006)     5376 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 user      (1006) user      (1006)     1605 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 user      (1006) user      (1006)      498 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 user      (1006) user      (1006)     4225 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 user      (1006) user      (1006)     3510 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 user      (1006) user      (1006)    22013 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 user      (1006) user      (1006)    17165 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 user      (1006) user      (1006)     5758 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user      (1006) user      (1006)     6895 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 user      (1006) user      (1006)    10168 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 user      (1006) user      (1006)    14279 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 user      (1006) user      (1006)     5403 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 user      (1006) user      (1006)      107 2024-04-18 18:15:46.000000 snowflake_connector_python-3.9.0/src/snowflake/connector/version.py
+drwxr-xr-x   0 user      (1006) user      (1006)        0 2024-04-18 18:18:21.096420 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/
+-rw-r--r--   0 user      (1006) user      (1006)    62221 2024-04-18 18:18:20.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1006) user      (1006)    13263 2024-04-18 18:18:21.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-18 18:18:20.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1006) user      (1006)      322 2024-04-18 18:18:20.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1006) user      (1006)        1 2024-04-18 18:16:32.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1006) user      (1006)      646 2024-04-18 18:18:20.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1006) user      (1006)       10 2024-04-18 18:18:20.000000 snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-3.8.1/CONTRIBUTING.md` & `snowflake_connector_python-3.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/DESCRIPTION.md` & `snowflake_connector_python-3.9.0/DESCRIPTION.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.9.0(April 20,2024)
+
+  - Added easy logging configuration so that users can easily generate log file by setup log config in `$SNOWFLAKE_HOME/config.toml`.
+  - Improved s3 acceleration logic when connecting to China endpoint.
+
 - v3.8.1(April 09, 2024)
 
   - Reverted the change "Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode." introduced in v3.8.0 (yanked) as it's a breaking change. `write_pandas` will be fixed in the future in a non-breaking way.
 
 - v3.8.0(April 04,2024)
 
   - Improved `externalbrowser` auth in containerized environments
```

### Comparing `snowflake-connector-python-3.8.1/LICENSE.txt` & `snowflake_connector_python-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/MANIFEST.in` & `snowflake_connector_python-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/PKG-INFO` & `snowflake_connector_python-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.8.1
+Version: 3.9.0
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -81,14 +81,19 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.9.0(April 20,2024)
+
+  - Added easy logging configuration so that users can easily generate log file by setup log config in `$SNOWFLAKE_HOME/config.toml`.
+  - Improved s3 acceleration logic when connecting to China endpoint.
+
 - v3.8.1(April 09, 2024)
 
   - Reverted the change "Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode." introduced in v3.8.0 (yanked) as it's a breaking change. `write_pandas` will be fixed in the future in a non-breaking way.
 
 - v3.8.0(April 04,2024)
 
   - Improved `externalbrowser` auth in containerized environments
```

### Comparing `snowflake-connector-python-3.8.1/README.md` & `snowflake_connector_python-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/pyproject.toml` & `snowflake_connector_python-3.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/setup.cfg` & `snowflake_connector_python-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/setup.py` & `snowflake_connector_python-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/__init__.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     InterfaceError,
     InternalError,
     NotSupportedError,
     OperationalError,
     ProgrammingError,
     _Warning,
 )
+from .log_configuration import EasyLoggingConfigPython
 from .version import VERSION
 
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
 @wraps(SnowflakeConnection.__init__)
 def Connect(**kwargs) -> SnowflakeConnection:
@@ -88,8 +89,9 @@
     "TimestampFromTicks",
     "STRING",
     "BINARY",
     "NUMBER",
     "DATETIME",
     "ROWID",
     # Extended data type (experimental)
+    "EasyLoggingConfigPython",
 ]
```

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/_query_context_cache.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/_sql_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/arrow_context.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/__init__.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/_auth.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/by_plugin.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/default.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/idtoken.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/keypair.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/oauth.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/okta.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/auth/webbrowser.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/azure_storage_client.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/backoff_policies.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/backoff_policies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/bind_upload_agent.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/cache.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/compat.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/config_manager.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/config_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/connection.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     ER_NO_ACCOUNT_NAME,
     ER_NO_NUMPY,
     ER_NO_PASSWORD,
     ER_NO_USER,
     ER_NOT_IMPLICITY_SNOWFLAKE_DATATYPE,
 )
 from .errors import DatabaseError, Error, OperationalError, ProgrammingError
+from .log_configuration import EasyLoggingConfigPython
 from .network import (
     DEFAULT_AUTHENTICATOR,
     EXTERNAL_BROWSER_AUTHENTICATOR,
     KEY_PAIR_AUTHENTICATOR,
     OAUTH_AUTHENTICATOR,
     REQUEST_ID,
     USR_PWD_MFA_AUTHENTICATOR,
@@ -379,14 +380,17 @@
         When no arguments are given (other than connection_file_path) the
         default connection will be loaded first. Note that no overwriting is
         supported in this case.
 
         If overwriting values from the default connection is desirable, supply
         the name explicitly.
         """
+        # initiate easy logging during every connection
+        easy_logging = EasyLoggingConfigPython()
+        easy_logging.create_log()
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
         self._errorhandler = Error.default_errorhandler
         self._lock_converter = Lock()
         self.messages = []
         self._async_sfqids: dict[str, None] = {}
         self._done_async_sfqids: dict[str, None] = {}
```

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/connection_diagnostic.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/constants.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/converter.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/converter_issue23517.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/converter_snowsql.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/cursor.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/dbapi.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/description.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/encryption_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/errorcode.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/errors.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/file_compression_type.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/file_transfer_agent.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/file_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/gcs_storage_client.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/gzip_decoder.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/local_storage_client.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp` & `snowflake_connector_python-3.9.0/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/network.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/ocsp_snowflake.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/options.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/pandas_tools.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/proxy.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/result_batch.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/result_set.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/s3_storage_client.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/s3_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,26 +76,30 @@
         self.etags: list[str] | None = None
         self.s3location: S3Location = (
             SnowflakeS3RestClient._extract_bucket_name_and_path(
                 self.stage_info["location"]
             )
         )
         self.use_s3_regional_url = use_s3_regional_url
+        self.location_type = stage_info.get("locationType")
 
         # if GS sends us an endpoint, it's likely for FIPS. Use it.
         self.endpoint: str | None = None
         if stage_info["endPoint"]:
             self.endpoint = (
                 f"https://{self.s3location.bucket_name}." + stage_info["endPoint"]
             )
         self.transfer_accelerate_config(use_accelerate_endpoint)
 
     def transfer_accelerate_config(
         self, use_accelerate_endpoint: bool | None = None
     ) -> bool:
+        # accelerate cannot be used in China and us government
+        if self.location_type and "S3China" in self.location_type:
+            return False
         # if self.endpoint has been set, e.g. by metadata, no more config is needed.
         if self.endpoint is not None:
             return self.endpoint.find("s3-accelerate.amazonaws.com") >= 0
         if self.use_s3_regional_url:
             self.endpoint = (
                 f"https://{self.s3location.bucket_name}."
                 f"s3.{self.region_name}.amazonaws.com"
```

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/secret_detector.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/sf_dirs.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/sfbinaryformat.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/sfdatetime.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/snow_logging.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/ssd_internal_keys.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/storage_client.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/telemetry.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/telemetry_oob.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/test_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/time_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_certs.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/tool/probe_connection.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/url_util.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/util_text.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/api.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/auth.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/compat.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/help.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/models.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/structures.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/requests/utils.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake_connector_python-3.9.0/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/PKG-INFO` & `snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.8.1
+Version: 3.9.0
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
@@ -81,14 +81,19 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.9.0(April 20,2024)
+
+  - Added easy logging configuration so that users can easily generate log file by setup log config in `$SNOWFLAKE_HOME/config.toml`.
+  - Improved s3 acceleration logic when connecting to China endpoint.
+
 - v3.8.1(April 09, 2024)
 
   - Reverted the change "Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode." introduced in v3.8.0 (yanked) as it's a breaking change. `write_pandas` will be fixed in the future in a non-breaking way.
 
 - v3.8.0(April 04,2024)
 
   - Improved `externalbrowser` auth in containerized environments
```

### Comparing `snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/SOURCES.txt` & `snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/snowflake/connector/feature.py
 src/snowflake/connector/file_compression_type.py
 src/snowflake/connector/file_transfer_agent.py
 src/snowflake/connector/file_util.py
 src/snowflake/connector/gcs_storage_client.py
 src/snowflake/connector/gzip_decoder.py
 src/snowflake/connector/local_storage_client.py
+src/snowflake/connector/log_configuration.py
 src/snowflake/connector/network.py
 src/snowflake/connector/ocsp_asn1crypto.py
 src/snowflake/connector/ocsp_snowflake.py
 src/snowflake/connector/options.py
 src/snowflake/connector/pandas_tools.py
 src/snowflake/connector/proxy.py
 src/snowflake/connector/py.typed
```

### Comparing `snowflake-connector-python-3.8.1/src/snowflake_connector_python.egg-info/requires.txt` & `snowflake_connector_python-3.9.0/src/snowflake_connector_python.egg-info/requires.txt`

 * *Files identical despite different names*
