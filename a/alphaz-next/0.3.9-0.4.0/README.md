# Comparing `tmp/alphaz-next-0.3.9.tar.gz` & `tmp/alphaz-next-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.3.9.tar", last modified: Wed Feb  7 10:25:40 2024, max compression
+gzip compressed data, was "alphaz-next-0.4.0.tar", last modified: Thu Apr 18 09:32:16 2024, max compression
```

## Comparing `alphaz-next-0.3.9.tar` & `alphaz-next-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/ujson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/uvicorn_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/logging_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-07 10:25:38.000000 alphaz-next-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.845673 alphaz-next-0.4.0/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.845673 alphaz-next-0.4.0/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/responses/ujson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/core/uvicorn_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.845673 alphaz-next-0.4.0/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.845673 alphaz-next-0.4.0/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.845673 alphaz-next-0.4.0/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-18 09:32:07.000000 alphaz-next-0.4.0/alphaz_next/utils/logging_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:32:16.841673 alphaz-next-0.4.0/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 09:32:16.000000 alphaz-next-0.4.0/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 09:32:16.000000 alphaz-next-0.4.0/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:32:16.000000 alphaz-next-0.4.0/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 09:32:16.000000 alphaz-next-0.4.0/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 09:32:16.000000 alphaz-next-0.4.0/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:32:16.849673 alphaz-next-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 09:32:14.000000 alphaz-next-0.4.0/setup.py
```

### Comparing `alphaz-next-0.3.9/alphaz_next/auth/auth.py` & `alphaz-next-0.4.0/alphaz_next/auth/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # MODULES
-from typing import Annotated as _Annotated, Any as _Any, Dict as _Dict, List as _List
+from typing import (
+    Annotated as _Annotated,
+    Any as _Any,
+    Dict as _Dict,
+    List as _List,
+    Type,
+    TypeVar,
+)
 
 # FASTAPI
 from fastapi import Depends as _Depends, status as _status
 from fastapi.security import (
     APIKeyHeader as _APIKeyHeader,
     OAuth2PasswordBearer as _OAuth2PasswordBearer,
     SecurityScopes as _SecurityScopes,
@@ -15,18 +22,15 @@
 # LIBS
 from alphaz_next.libs.httpx import (
     make_async_request_with_retry as _make_async_request_with_retry,
     post_process_http_response as _post_process_http_response,
 )
 
 # MODELS
-from alphaz_next.models.auth.user import (
-    UserSchema as _UserSchema,
-    UserShortSchema as _UserShortSchema,
-)
+from alphaz_next.models.auth.user import UserBaseSchema as _UserBaseSchema
 from alphaz_next.models.config._base.internal_config_settings import (
     create_internal_config as _create_internal_config,
 )
 
 # EXCEPTIONS
 from alphaz_next.core.exceptions import (
     InvalidCredentialsError as _InvalidCredentialsError,
@@ -35,14 +39,16 @@
 )
 
 INTERNAL_CONFIG = _create_internal_config()
 
 API_KEY_HEADER = _APIKeyHeader(name="api_key", auto_error=False)
 OAUTH2_SCHEME = _OAuth2PasswordBearer(tokenUrl=INTERNAL_CONFIG.token_url)
 
+_T = TypeVar("_T", bound=_UserBaseSchema)
+
 
 def decode_token(token: str) -> _Dict[str, _Any]:
     """
     Decode a JWT token and return the payload.
 
     Args:
         token (str): The JWT token to decode.
@@ -65,26 +71,27 @@
     username: str = payload.get("sub")
     if username is None:
         raise _InvalidCredentialsError()
 
     return payload
 
 
-async def get_user(token: str) -> _UserSchema:
+async def get_user(token: str, schema: Type[_T]) -> _T:
     """
     Retrieves user information using the provided token.
 
     Args:
         token (str): The authentication token.
+        schema (Type[_T]): The schema type to validate the response against.
 
     Returns:
-        UserSchema: The user information.
+        _T: The user information.
 
     Raises:
-        Exception: If there is an error retrieving the user information.
+        Any: Any exception raised during the request or response processing.
     """
     decode_token(token=token)
 
     headers = {
         "Authorization": f"Bearer {token}",
     }
 
@@ -94,28 +101,28 @@
         **{
             "headers": headers,
         },
     )
 
     return _post_process_http_response(
         response,
-        schema=_UserSchema,
+        schema=schema,
     )
 
 
-async def get_api_key(api_key: str) -> _UserShortSchema:
+async def get_api_key(api_key: str, schema: Type[_T]) -> _T:
     """
-    Retrieves user information using the provided API key.
+    Retrieves the API key using the provided `api_key` and returns the processed response.
 
     Args:
-        api_key (str): The API key for authentication.
+        api_key (str): The API key to be used for authentication.
+        schema (Type[_T]): The type of the response schema.
 
     Returns:
-        UserShortSchema: The user information.
-
+        _T: The processed response based on the provided schema.
     """
     headers = {
         "api_key": api_key,
     }
 
     response = await _make_async_request_with_retry(
         method="POST",
@@ -123,20 +130,21 @@
         **{
             "headers": headers,
         },
     )
 
     return _post_process_http_response(
         response,
-        schema=_UserShortSchema,
+        schema=schema,
     )
 
 
 def check_user_permissions(
-    permissions: _List[str], user_permissions: _List[str]
+    permissions: _List[str],
+    user_permissions: _List[str],
 ) -> None:
     """
     Check if the user has the required permissions.
 
     Args:
         permissions (List[str]): The list of required permissions.
         user_permissions (List[str]): The list of permissions the user has.
@@ -147,32 +155,35 @@
     if len(permissions) > 0 and not any(
         [user_permission in permissions for user_permission in user_permissions]
     ):
         raise _NotEnoughPermissionsError()
 
 
 async def get_user_from_jwt(
+    schema: Type[_T],
     security_scopes: _SecurityScopes,
     token: _Annotated[str, _Depends(OAUTH2_SCHEME)],
-) -> _UserSchema:
+) -> _T:
     """
-    Retrieves the user from the JWT token and performs permission checks.
+    Retrieves a user from a JWT token and performs permission checks.
 
     Args:
-        security_scopes (SecurityScopes): The security scopes required for the endpoint.
-        token (str): The JWT token.
+        schema (Type[_T]): The schema type used to deserialize the user data.
+        security_scopes (_SecurityScopes): The security scopes required for the user.
+        token (_Annotated[str, _Depends(OAUTH2_SCHEME)]): The JWT token.
 
     Returns:
-        UserSchema: The user object.
+        _T: The deserialized user object.
 
     Raises:
-        HTTPException: If the credentials are invalid or the user does not have enough permissions.
+        _HTTPException: If the credentials are invalid or the user does not have enough permissions.
     """
+
     try:
-        user = await get_user(token=token)
+        user = await get_user(token=token, schema=schema)
 
         check_user_permissions(
             permissions=security_scopes.scopes,
             user_permissions=user.permissions,
         )
 
         return user
@@ -196,38 +207,41 @@
             ext_headers={
                 "status_description": ex.args,
             },
         )
 
 
 async def get_user_from_api_key(
+    schema: Type[_T],
     security_scopes: _SecurityScopes,
     api_key: _Annotated[
         str,
         _Depends(API_KEY_HEADER),
     ],
-) -> _UserShortSchema:
+) -> _T:
     """
-    Retrieves a user from the API key and performs permission checks.
+    Retrieves a user from the API key.
 
     Args:
-        security_scopes (SecurityScopes): The security scopes required for the endpoint.
-        api_key (str): The API key provided in the request header.
+        schema (Type[_T]): The schema type.
+        security_scopes (_SecurityScopes): The security scopes.
+        api_key (_Annotated[str, _Depends(API_KEY_HEADER)]): The API key.
 
     Returns:
-        UserShortSchema: The user associated with the API key.
+        _T: The user retrieved from the API key.
 
     Raises:
-        HTTPException: If the API key is invalid or the user does not have sufficient permissions.
+        _HTTPException: If the credentials are invalid or the user doesn't have enough permissions.
     """
+
     try:
         if api_key is None:
             raise _InvalidCredentialsError()
 
-        user = await get_api_key(api_key=api_key)
+        user = await get_api_key(api_key=api_key, schema=schema)
 
         check_user_permissions(
             permissions=security_scopes.scopes,
             user_permissions=user.permissions,
         )
 
         return user
```

### Comparing `alphaz-next-0.3.9/alphaz_next/core/_base.py` & `alphaz-next-0.4.0/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/application.py` & `alphaz-next-0.4.0/alphaz_next/core/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # MODULES
+import logging as _logging
+from logging.handlers import TimedRotatingFileHandler as _TimedRotatingFileHandler
+from pathlib import Path as _Path
 import sys as _sys
 from typing import (
     Any as _Any,
+    AsyncContextManager as _AsyncContextManager,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Sequence as _Sequence,
     Union as _Union,
 )
 
@@ -23,46 +27,54 @@
     request_validation_exception_handler as _request_validation_exception_handler,
 )
 from fastapi.openapi.docs import (
     get_swagger_ui_html as _get_swagger_ui_html,
     get_redoc_html as _get_redoc_html,
 )
 from fastapi.openapi.utils import get_openapi as _get_openapi, BaseRoute as _BaseRoute
-from fastapi.middleware.cors import CORSMiddleware as _CORSMiddleware
 from fastapi.responses import (
     HTMLResponse as _HTMLResponse,
     JSONResponse as _JSONResponse,
     PlainTextResponse as _PlainTextResponse,
     RedirectResponse as _RedirectResponse,
 )
 
-# DEPENDENCY_INJECTOR
-from dependency_injector import containers as _containers
+if "dependency_injector" in _sys.modules:
+    from dependency_injector import containers as _containers
+
+    _ContainerType = _containers.DeclarativeContainer
+else:
+    _ContainerType = _Any
 
 # ELASTICAPM
 from elasticapm.contrib.starlette import (
     make_apm_client as _make_apm_client,
     ElasticAPM as _ElasticAPM,
 )
 
 # MODELS
 from alphaz_next.models.config.alpha_config import (
     AlphaConfigSchema as _AlphaConfigSchema,
 )
 
 # CORE
-from alphaz_next.core.middleware import (
+from alphaz_next.core._middleware import (
     log_request_middleware as _log_request_middleware,
+    CORSMiddleware as _CORSMiddleware,
 )
 from alphaz_next.core.uvicorn_logger import UVICORN_LOGGER as _UVICORN_LOGGER
 
 # UTILS
 from alphaz_next.utils.logging_filters import (
     ExcludeRoutersFilter as _ExcludeRoutersFilter,
 )
+from alphaz_next.utils.logger import (
+    DEFAULT_DATE_FORMAT as _DEFAULT_DATE_FORMAT,
+    DEFAULT_FORMAT as _DEFAULT_FORMAT,
+)
 
 
 # ELASTICAPM
 
 _DEFAULT_FAVICON_URL = "https://fastapi.tiangolo.com/img/favicon.png"
 
 
@@ -103,56 +115,89 @@
 
     return openapi_schema
 
 
 def create_app(
     config: _AlphaConfigSchema,
     routers: _List[_APIRouter],
-    container: _Optional[_containers.DeclarativeContainer] = None,
+    container: _Optional[_ContainerType] = None,
+    lifespan: _Optional[_AsyncContextManager] = None,
     allow_origins: _Sequence[str] = (),
     allow_methods: _Sequence[str] = ("GET",),
     allow_headers: _Sequence[str] = (),
     allow_credentials: bool = False,
+    allow_private_network: bool = False,
     status_response: _Dict = {"status": "OK"},
+    uvicorn_formatter: _Optional[_logging.Formatter] = None,
 ) -> _FastAPI:
     """
     Create a FastAPI application with the specified configuration.
 
     Args:
         config (AlphaConfigSchema): The configuration for the application.
         routers (List[APIRouter]): The list of API routers to include in the application.
-        container (Optional[containers.DeclarativeContainer], optional): The dependency injection container. Defaults to None.
-        allow_origins (Sequence[str], optional): The list of allowed origins for CORS. Defaults to ().
-        allow_methods (Sequence[str], optional): The list of allowed HTTP methods for CORS. Defaults to ("GET",).
-        allow_headers (Sequence[str], optional): The list of allowed headers for CORS. Defaults to ().
-        allow_credentials (bool, optional): Whether to allow credentials for CORS. Defaults to False.
-        status_response (Dict, optional): The response to return for the "/status" endpoint. Defaults to {"status": "OK"}.
+        container (Optional[containers.DeclarativeContainer]): The dependency injection container. Defaults to None.
+        allow_origins (Sequence[str]): The list of allowed origins for CORS. Defaults to ().
+        allow_methods (Sequence[str]): The list of allowed HTTP methods for CORS. Defaults to ("GET",).
+        allow_headers (Sequence[str]): The list of allowed headers for CORS. Defaults to ().
+        allow_credentials (bool): Whether to allow credentials for CORS. Defaults to False.
+        allow_private_network (bool): Whether to allow private network for CORS. Defaults to False.
+        status_response (Dict): The response to return for the "/status" endpoint. Defaults to {"status": "OK"}.
+        uvicorn_formatter (Optional[_logging.Formatter]): The formatter used in time rotating file handler if time rotating logging config exists. If None, use the default one.
 
     Returns:
         FastAPI: The created FastAPI application.
     """
-    _UVICORN_LOGGER.addFilter(
-        _ExcludeRoutersFilter(router_names=config.api_config.logging.excluded_routers)
-    )
+
+    if (
+        config.api_config.logging is not None
+        and config.api_config.logging.time_rotating is not None
+    ):
+        if uvicorn_formatter is None:
+            uvicorn_formatter = _logging.Formatter(
+                _DEFAULT_FORMAT,
+                datefmt=_DEFAULT_DATE_FORMAT,
+            )
+
+        directory_path = _Path(config.api_config.directories.logs)
+        directory_path.mkdir(parents=True, exist_ok=True)
+
+        handler = _TimedRotatingFileHandler(
+            filename=directory_path / "uvicorn.log",
+            when=config.api_config.logging.time_rotating.when,
+            interval=config.api_config.logging.time_rotating.interval,
+            backupCount=config.api_config.logging.time_rotating.backup_count,
+        )
+        handler.setFormatter(uvicorn_formatter)
+
+        _UVICORN_LOGGER.addHandler(handler)
+
+        _UVICORN_LOGGER.addFilter(
+            _ExcludeRoutersFilter(
+                router_names=config.api_config.logging.excluded_routers
+            )
+        )
 
     # APP
     app = _FastAPI(
         title=config.project_name.upper(),
         version=config.version,
         docs_url=None,
         redoc_url=None,
+        lifespan=lifespan,
     )
     app.container = container
 
     app.add_middleware(
         _CORSMiddleware,
         allow_origins=allow_origins,
         allow_credentials=allow_credentials,
         allow_methods=allow_methods,
         allow_headers=allow_headers,
+        allow_private_network=allow_private_network,
     )
 
     app.middleware("http")(_log_request_middleware)
 
     if config.api_config.apm is not None and config.api_config.apm.active:
         apm = _make_apm_client(
             {
```

### Comparing `alphaz-next-0.3.9/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.4.0/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/exceptions.py` & `alphaz-next-0.4.0/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.4.0/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/libs/httpx.py` & `alphaz-next-0.4.0/alphaz_next/libs/httpx.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # HTTPX
 import httpx
 from pydantic import BaseModel
 
 
 def make_request_with_retry(
     method: Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
-    url,
+    url: str,
     max_retries: int = 3,
     retry_on_status: Optional[List[int]] = None,
     timeout: Optional[float] = None,
     **kwargs,
 ) -> httpx.Response:
     """
     Makes an HTTP request with retries in case of a timeout error.
@@ -35,15 +35,15 @@
 
     Raises:
         RuntimeError: If the maximum number of retries is exceeded or unknown error occurs.
     """
     item_repr = {
         "method": method,
         "url": url,
-        "kwargs": kwargs,
+        "kwargs": {k: v for k, v in kwargs.items() if k in ["params", "headers"]},
     }
 
     retry_statuses = retry_on_status or []
 
     for retry_count in range(max_retries + 1):
         try:
             with httpx.Client(timeout=timeout) as client:
@@ -63,15 +63,15 @@
                 wait_time = 2**retry_count
                 time.sleep(wait_time)
             else:
                 raise ex
         except Exception as ex:
             raise RuntimeError(
                 f"An unknown error occurs while contacting external server {item_repr}"
-            )
+            ) from ex
         else:
             return response
 
     raise RuntimeError(f"Maximum number of retries exceeded {item_repr}")
 
 
 async def make_async_request_with_retry(
@@ -98,15 +98,15 @@
 
     Raises:
         RuntimeError: If the maximum number of retries is exceeded or unknown error occurs.
     """
     item_repr = {
         "method": method,
         "url": url,
-        "kwargs": kwargs,
+        "kwargs": {k: v for k, v in kwargs.items() if k in ["params", "headers"]},
     }
 
     retry_statuses = retry_on_status or []
 
     for retry_count in range(max_retries + 1):
         try:
             async with httpx.AsyncClient(timeout=timeout) as client:
@@ -126,15 +126,15 @@
                 wait_time = 2**retry_count
                 await asyncio.sleep(wait_time)
             else:
                 raise ex
         except Exception as ex:
             raise RuntimeError(
                 f"An unknown error occurs while contacting external server {item_repr}"
-            )
+            ) from ex
         else:
             return response
 
     raise RuntimeError(f"Maximum number of retries exceeded {item_repr}")
 
 
 T = TypeVar("T", bound=BaseModel)
```

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.4.0/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.4.0/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.4.0/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/api_config.py` & `alphaz-next-0.4.0/alphaz_next/models/config/api_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from typing import Optional as _Optional
 
 # PYDANTIC
 from pydantic import BaseModel as _BaseModel, ConfigDict as _ConfigDict, Field as _Field
 
 # MODELS
 from alphaz_next.models.config.apm_config import ApmConfig as _ApmConfig
+from alphaz_next.models.config.database_config import (
+    DatabasesConfigSchema as _DatabasesConfigSchema,
+)
+from alphaz_next.models.config.directories_config import (
+    DirectoriesSchema as _DirectoriesSchema,
+)
 from alphaz_next.models.config.logging_config import LoggingSchema as _LoggingSchema
 from alphaz_next.models.config.openapi_config_schema import (
     OpenApiSchema as _OpenApiSchema,
 )
 
 
 class AlphaApiConfigSchema(_BaseModel):
@@ -18,11 +24,12 @@
     """
 
     model_config = _ConfigDict(
         from_attributes=True,
         extra="allow",
     )
 
-    databases_config_path: str
-    logging: _LoggingSchema
+    databases_config: _DatabasesConfigSchema
+    directories: _DirectoriesSchema
+    logging: _Optional[_LoggingSchema] = _Field(default=None)
     apm: _Optional[_ApmConfig] = _Field(default=None)
     openapi: _Optional[_OpenApiSchema] = _Field(default=None)
```

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.4.0/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.4.0/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.4.0/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.4.0/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/mock_user.py` & `alphaz-next-0.4.0/alphaz_next/tests/utils/mocking/mock_user.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.4.0/alphaz_next/tests/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,14 @@
     @classmethod
     def setUpClass(cls) -> None:
         """
         Set up the test class by creating the app, initializing the client, and performing any necessary setup steps.
         """
         cls.app = cls.create_app()
 
-        cls.client = _TestClient(cls.app)
-
         cls.enable_reset_before_next_test()
 
     @classmethod
     def enable_reset_before_next_test(cls):
         """
         Enable the reset before the next test.
 
@@ -196,19 +194,20 @@
         """
         headers = self.add_fake_headers(
             headers=headers,
             with_fake_token=with_fake_token,
             with_fake_api_key=with_fake_api_key,
         )
 
-        response = self.client.get(
-            url,
-            params=params,
-            headers=headers,
-        )
+        with _TestClient(self.app) as client:
+            response = client.get(
+                url,
+                params=params,
+                headers=headers,
+            )
 
         status_code, data = self._post_process_response(
             response=response,
             response_format=response_format,
             saved_path=saved_path,
         )
 
@@ -254,21 +253,22 @@
         """
         headers = self.add_fake_headers(
             headers=headers,
             with_fake_token=with_fake_token,
             with_fake_api_key=with_fake_api_key,
         )
 
-        response = self.client.put(
-            url,
-            data=data,
-            json=json,
-            params=params,
-            headers=headers,
-        )
+        with _TestClient(self.app) as client:
+            response = client.put(
+                url,
+                data=data,
+                json=json,
+                params=params,
+                headers=headers,
+            )
 
         status_code, data = self._post_process_response(
             response=response,
             response_format=response_format,
             saved_path=saved_path,
         )
 
@@ -314,21 +314,22 @@
         """
         headers = self.add_fake_headers(
             headers=headers,
             with_fake_token=with_fake_token,
             with_fake_api_key=with_fake_api_key,
         )
 
-        response = self.client.patch(
-            url,
-            data=data,
-            json=json,
-            params=params,
-            headers=headers,
-        )
+        with _TestClient(self.app) as client:
+            response = client.patch(
+                url,
+                data=data,
+                json=json,
+                params=params,
+                headers=headers,
+            )
 
         status_code, data = self._post_process_response(
             response=response,
             response_format=response_format,
             saved_path=saved_path,
         )
 
@@ -376,21 +377,22 @@
         """
         headers = self.add_fake_headers(
             headers=headers,
             with_fake_token=with_fake_token,
             with_fake_api_key=with_fake_api_key,
         )
 
-        response = self.client.post(
-            url,
-            data=data,
-            json=json,
-            params=params,
-            headers=headers,
-        )
+        with _TestClient(self.app) as client:
+            response = client.post(
+                url,
+                data=data,
+                json=json,
+                params=params,
+                headers=headers,
+            )
 
         status_code, data = self._post_process_response(
             response=response,
             response_format=response_format,
             saved_path=saved_path,
         )
 
@@ -432,19 +434,20 @@
         """
         headers = self.add_fake_headers(
             headers=headers,
             with_fake_token=with_fake_token,
             with_fake_api_key=with_fake_api_key,
         )
 
-        response = self.client.delete(
-            url,
-            params=params,
-            headers=headers,
-        )
+        with _TestClient(self.app) as client:
+            response = client.delete(
+                url,
+                params=params,
+                headers=headers,
+            )
 
         status_code, data = self._post_process_response(
             response=response,
             response_format=response_format,
             saved_path=saved_path,
         )
```

### Comparing `alphaz-next-0.3.9/alphaz_next/utils/format.py` & `alphaz-next-0.4.0/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/utils/logger.py` & `alphaz-next-0.4.0/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.4.0/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.9/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.4.0/alphaz_next.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 alphaz_next.egg-info/SOURCES.txt
 alphaz_next.egg-info/dependency_links.txt
 alphaz_next.egg-info/requires.txt
 alphaz_next.egg-info/top_level.txt
 alphaz_next/asyncio/__init__.py
 alphaz_next/auth/auth.py
 alphaz_next/core/_base.py
+alphaz_next/core/_middleware.py
 alphaz_next/core/application.py
 alphaz_next/core/constants.py
 alphaz_next/core/exception_handlers.py
 alphaz_next/core/exceptions.py
-alphaz_next/core/middleware.py
 alphaz_next/core/uvicorn_logger.py
 alphaz_next/core/responses/__init__.py
 alphaz_next/core/responses/file_response.py
 alphaz_next/core/responses/html_response.py
 alphaz_next/core/responses/json_response.py
 alphaz_next/core/responses/orjson_response.py
 alphaz_next/core/responses/plaintext_response.py
@@ -29,14 +29,15 @@
 alphaz_next/libs/httpx.py
 alphaz_next/models/auth/user.py
 alphaz_next/models/config/alpha_config.py
 alphaz_next/models/config/api_config.py
 alphaz_next/models/config/apm_config.py
 alphaz_next/models/config/config_settings.py
 alphaz_next/models/config/database_config.py
+alphaz_next/models/config/directories_config.py
 alphaz_next/models/config/logging_config.py
 alphaz_next/models/config/openapi_config_schema.py
 alphaz_next/models/config/_base/internal_config_settings.py
 alphaz_next/models/config/_base/utils.py
 alphaz_next/tests/utils/utils.py
 alphaz_next/tests/utils/mocking/mock_user.py
 alphaz_next/utils/format.py
```

### Comparing `alphaz-next-0.3.9/setup.py` & `alphaz-next-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup
 
-version = "0.3.9"
+version = "0.4.0"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
+
+EXTRAS_REQUIRE = {
+    "dependency-injector": ["dependency-injector"],
+}
+
 setup(
     name="alphaz-next",
     version=version,
     packages=[
         "alphaz_next",
         "alphaz_next.asyncio",
         "alphaz_next.auth",
@@ -21,14 +26,15 @@
         "alphaz_next.models.config._base",
         "alphaz_next.tests",
         "alphaz_next.tests.utils",
         "alphaz_next.tests.utils.mocking",
         "alphaz_next.utils",
     ],
     install_requires=required_packages,
+    extras_require=EXTRAS_REQUIRE,
     license="MIT",
     author="Maxime MARTIN",
     author_email="maxime.martin02@hotmail.fr",
     description="A project to make a lib to start FASTAPI quickly",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/STDef200mm/alphaz-next",
```

