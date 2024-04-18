# Comparing `tmp/singlestoredb-1.0.4.tar.gz` & `tmp/singlestoredb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.0.4.tar", last modified: Wed Apr  3 17:43:03 2024, max compression
+gzip compressed data, was "singlestoredb-1.1.0.tar", last modified: Thu Apr 18 15:00:25 2024, max compression
```

## Comparing `singlestoredb-1.0.4.tar` & `singlestoredb-1.1.0.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   151339 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36712 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21938 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/mmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.686379 singlestoredb-1.0.4/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    64746 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.690379 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/mysql/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    50741 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37347 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47693 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.694379 singlestoredb-1.0.4/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-03 17:42:41.000000 singlestoredb-1.0.4/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:43:03.682379 singlestoredb-1.0.4/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:43:03.000000 singlestoredb-1.0.4/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   154182 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39861 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21337 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19643 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38818 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67380 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16196 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   111071 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.0.4/LICENSE` & `singlestoredb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/PKG-INFO` & `singlestoredb-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.4
+Version: 1.1.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.4/README.md` & `singlestoredb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/accel.c` & `singlestoredb-1.1.0/accel.c`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 #define PyBUF_WRITE 0x200
 #endif
 
 #define ACCEL_OUT_TUPLES 0
 #define ACCEL_OUT_STRUCTSEQUENCES 1
 #define ACCEL_OUT_DICTS 2
 #define ACCEL_OUT_NAMEDTUPLES 3
+#define ACCEL_OUT_NUMPY 4
+#define ACCEL_OUT_PANDAS 5
+#define ACCEL_OUT_POLARS 6
+#define ACCEL_OUT_ARROW 7
 
 #define NUMPY_BOOL 1
 #define NUMPY_INT8 2
 #define NUMPY_INT16 3
 #define NUMPY_INT32 4
 #define NUMPY_INT64 5
 #define NUMPY_UINT8 6
@@ -385,14 +389,17 @@
     PyObject *_next_seq_id;
     PyObject *rows;
     PyObject *namedtuple;
     PyObject *Row;
     PyObject *Series;
     PyObject *array;
     PyObject *vectorize;
+    PyObject *DataFrame;
+    PyObject *Table;
+    PyObject *from_pylist;
 } PyStrings;
 
 static PyStrings PyStr = {0};
 
 //
 // Cached Python functions
 //
@@ -402,14 +409,18 @@
     PyObject *datetime_date;
     PyObject *datetime_time;
     PyObject *datetime_timedelta;
     PyObject *datetime_datetime;
     PyObject *collections_namedtuple;
     PyObject *numpy_array;
     PyObject *numpy_vectorize;
+    PyObject *pandas_DataFrame;
+    PyObject *polars_DataFrame;
+    PyObject *pyarrow_Table;
+    PyObject *pyarrow_Table_from_pylist;
 } PyFunctions;
 
 static PyFunctions PyFunc = {0};
 
 //
 // Cached Python objects
 //
@@ -462,18 +473,96 @@
     struct {
         PyObject *_next_seq_id;
         PyObject *rows;
     } py_str;
     char *encoding_errors;
 } StateObject;
 
-static void read_options(MySQLAccelOptions *options, PyObject *dict);
+static int read_options(MySQLAccelOptions *options, PyObject *dict);
 
 #define DESTROY(x) do { if (x) { free((void*)x); (x) = NULL; } } while (0)
 
+int ensure_numpy() {
+    if (PyFunc.numpy_array && PyFunc.numpy_vectorize) goto exit;
+
+    // Import numpy if it exists
+    PyObject *numpy_mod = PyImport_ImportModule("numpy");
+    if (!numpy_mod) goto error;
+
+    PyFunc.numpy_array = PyObject_GetAttr(numpy_mod, PyStr.array);
+    if (!PyFunc.numpy_array) goto error;
+
+    PyFunc.numpy_vectorize = PyObject_GetAttr(numpy_mod, PyStr.vectorize);
+    if (!PyFunc.numpy_vectorize) goto error;
+
+exit:
+    return 0;
+
+error:
+    return -1;
+}
+
+
+int ensure_pandas() {
+    if (PyFunc.pandas_DataFrame) goto exit;
+
+    // Import pandas if it exists
+    PyObject *pandas_mod = PyImport_ImportModule("pandas");
+    if (!pandas_mod) goto error;
+
+    PyFunc.pandas_DataFrame = PyObject_GetAttr(pandas_mod, PyStr.DataFrame);
+    if (!PyFunc.pandas_DataFrame) goto error;
+
+exit:
+    return 0;
+
+error:
+    return -1;
+}
+
+
+int ensure_polars() {
+    if (PyFunc.polars_DataFrame) goto exit;
+
+    // Import polars if it exists
+    PyObject *polars_mod = PyImport_ImportModule("polars");
+    if (!polars_mod) goto error;
+
+    PyFunc.polars_DataFrame = PyObject_GetAttr(polars_mod, PyStr.DataFrame);
+    if (!PyFunc.polars_DataFrame) goto error;
+
+exit:
+    return 0;
+
+error:
+    return -1;
+}
+
+
+int ensure_pyarrow() {
+    if (PyFunc.pyarrow_Table_from_pylist) goto exit;
+
+    // Import pyarrow if it exists
+    PyObject *pyarrow_mod = PyImport_ImportModule("pyarrow");
+    if (!pyarrow_mod) goto error;
+
+    PyFunc.pyarrow_Table = PyObject_GetAttr(pyarrow_mod, PyStr.Table);
+    if (!PyFunc.pyarrow_Table) goto error;
+
+    PyFunc.pyarrow_Table_from_pylist = PyObject_GetAttr(PyFunc.pyarrow_Table, PyStr.from_pylist);
+    if (!PyFunc.pyarrow_Table_from_pylist) goto error;
+
+exit:
+    return 0;
+
+error:
+    return -1;
+}
+
+
 static void State_clear_fields(StateObject *self) {
     if (!self) return;
     DESTROY(self->offsets);
     DESTROY(self->scales);
     DESTROY(self->flags);
     DESTROY(self->type_codes);
     DESTROY(self->encodings);
@@ -676,15 +765,15 @@
                               NULL : _PyUnicode_AsUTF8(py_encoding);
 
         self->py_invalid_values[i] = (!py_invalid_value || py_invalid_value == Py_None) ?
                                       NULL : py_converter;
         Py_XINCREF(self->py_invalid_values[i]);
 
         self->py_converters[i] = (!py_converter
-                                  || py_converter == Py_None
+                                  // || py_converter == Py_None
                                   || py_converter == py_default_converter) ?
                                  NULL : py_converter;
         Py_XINCREF(self->py_converters[i]);
     }
 
     // Loop over all data packets.
     self->py_conn = PyObject_GetAttr(py_res, PyStr.connection);
@@ -705,15 +794,16 @@
 
     PyObject *py_next_seq_id = PyObject_GetAttr(self->py_conn, PyStr._next_seq_id);
     if (!py_next_seq_id) goto error;
     self->next_seq_id = PyLong_AsUnsignedLongLong(py_next_seq_id);
     Py_XDECREF(py_next_seq_id);
 
     if (py_options && PyDict_Check(py_options)) {
-        read_options(&self->options, py_options);
+        rc = read_options(&self->options, py_options);
+        if (rc) goto error;
     }
 
     switch (self->options.results_type) {
     case ACCEL_OUT_NAMEDTUPLES:
     case ACCEL_OUT_STRUCTSEQUENCES:
         if (self->options.results_type == ACCEL_OUT_NAMEDTUPLES)
         {
@@ -821,20 +911,21 @@
     .slots = StateType_slots,
 };
 
 //
 // End State
 //
 
-static void read_options(MySQLAccelOptions *options, PyObject *dict) {
-    if (!options || !dict) return;
+static int read_options(MySQLAccelOptions *options, PyObject *dict) {
+    if (!options || !dict) return 0;
 
     PyObject *key = NULL;
     PyObject *value = NULL;
     Py_ssize_t pos = 0;
+    int rc = 0;
 
     while (PyDict_Next(dict, &pos, &key, &value)) {
         if (PyUnicode_CompareWithASCIIString(key, "results_type") == 0) {
             if (PyUnicode_CompareWithASCIIString(value, "dict") == 0 ||
                 PyUnicode_CompareWithASCIIString(value, "dicts") == 0 ) {
                 options->results_type = ACCEL_OUT_DICTS;
             }
@@ -842,25 +933,44 @@
                      PyUnicode_CompareWithASCIIString(value, "namedtuples") == 0) {
                 options->results_type = ACCEL_OUT_NAMEDTUPLES;
             }
             else if (PyUnicode_CompareWithASCIIString(value, "structsequence") == 0 ||
                      PyUnicode_CompareWithASCIIString(value, "structsequences") == 0) {
                 options->results_type = ACCEL_OUT_STRUCTSEQUENCES;
             }
+            else if (PyUnicode_CompareWithASCIIString(value, "numpy") == 0) {
+                options->results_type = ACCEL_OUT_NUMPY;
+                rc = ensure_numpy();
+            }
+            else if (PyUnicode_CompareWithASCIIString(value, "pandas") == 0) {
+                options->results_type = ACCEL_OUT_PANDAS;
+                rc = ensure_pandas();
+            }
+            else if (PyUnicode_CompareWithASCIIString(value, "polars") == 0) {
+                options->results_type = ACCEL_OUT_POLARS;
+                rc = ensure_polars();
+            }
+            else if (PyUnicode_CompareWithASCIIString(value, "arrow") == 0 ||
+                     PyUnicode_CompareWithASCIIString(value, "pyarrow") == 0) {
+                options->results_type = ACCEL_OUT_ARROW;
+                rc = ensure_pyarrow();
+            }
             else {
                 options->results_type = ACCEL_OUT_TUPLES;
             }
         } else if (PyUnicode_CompareWithASCIIString(key, "parse_json") == 0) {
             options->parse_json = PyObject_IsTrue(value);
         } else if (PyUnicode_CompareWithASCIIString(key, "invalid_values") == 0) {
             if (PyDict_Check(value)) {
                 options->invalid_values = value;
             }
         }
     }
+
+    return rc;
 }
 
 static void raise_exception(
     PyObject *self,
     char *err_type,
     unsigned long long err_code,
     char *err_str
@@ -1319,14 +1429,15 @@
     int hour = 0;
     int minute = 0;
     int second = 0;
     int microsecond = 0;
 
     switch (py_state->options.results_type) {
     case ACCEL_OUT_DICTS:
+    case ACCEL_OUT_ARROW:
         py_result = PyDict_New();
         break;
    case ACCEL_OUT_STRUCTSEQUENCES: {
         if (!py_state->structsequence) goto error;
         py_result = PyStructSequence_New(py_state->structsequence);
         break;
         }
@@ -1358,16 +1469,20 @@
                 if (py_state->encodings[i] == NULL) {
                     py_str = PyBytes_FromStringAndSize(out, out_l);
                     if (!py_str) goto error;
                 } else {
                     py_str = PyUnicode_Decode(out, out_l, py_state->encodings[i], py_state->encoding_errors);
                     if (!py_str) goto error;
                 }
-                py_item = PyObject_CallFunctionObjArgs(py_state->py_converters[i], py_str, NULL);
-                Py_CLEAR(py_str);
+                if (py_state->py_converters[i] == Py_None) {
+                    py_item = py_str;
+                } else {
+                    py_item = PyObject_CallFunctionObjArgs(py_state->py_converters[i], py_str, NULL);
+                    Py_CLEAR(py_str);
+                }
                 if (!py_item) goto error;
             }
 
             // If no converter was passed in, do the default processing.
             else {
                 switch (py_state->type_codes[i]) {
                 case MYSQL_TYPE_NEWDECIMAL:
@@ -1582,14 +1697,15 @@
         }
 
         switch (py_state->options.results_type) {
         case ACCEL_OUT_STRUCTSEQUENCES:
             PyStructSequence_SetItem(py_result, i, py_item);
             break;
         case ACCEL_OUT_DICTS:
+        case ACCEL_OUT_ARROW:
             PyDict_SetItem(py_result, py_state->py_names[i], py_item);
             Py_INCREF(py_state->py_names[i]);
             Py_DECREF(py_item);
             break;
         default:
             PyTuple_SetItem(py_result, i, py_item);
         }
@@ -1843,35 +1959,14 @@
     Py_XDECREF(py_out);
     py_out = NULL;
 
     goto exit;
 }
 
 
-int ensure_numpy() {
-    if (PyFunc.numpy_array && PyFunc.numpy_vectorize) goto exit;
-
-    // Import numpy if it exists
-    PyObject *numpy_mod = PyImport_ImportModule("numpy");
-    if (!numpy_mod) goto error;
-
-    PyFunc.numpy_array = PyObject_GetAttr(numpy_mod, PyStr.array);
-    if (!PyFunc.numpy_array) goto error;
-
-    PyFunc.numpy_vectorize = PyObject_GetAttr(numpy_mod, PyStr.vectorize);
-    if (!PyFunc.numpy_vectorize) goto error;
-
-exit:
-    return 0;
-
-error:
-    return -1;
-}
-
-
 static PyObject *load_rowdat_1_numpy(PyObject *self, PyObject *args, PyObject *kwargs) {
     PyObject *py_data = NULL;
     PyObject *py_out = NULL;
     PyObject *py_colspec = NULL;
     PyObject *py_str = NULL;
     PyObject *py_blob = NULL;
     PyObject *py_memview = NULL;
@@ -4368,14 +4463,17 @@
     PyStr._next_seq_id = PyUnicode_FromString("_next_seq_id");
     PyStr.rows = PyUnicode_FromString("rows");
     PyStr.namedtuple = PyUnicode_FromString("namedtuple");
     PyStr.Row = PyUnicode_FromString("Row");
     PyStr.Series = PyUnicode_FromString("Series");
     PyStr.array = PyUnicode_FromString("array");
     PyStr.vectorize = PyUnicode_FromString("vectorize");
+    PyStr.DataFrame = PyUnicode_FromString("DataFrame");
+    PyStr.Table = PyUnicode_FromString("Table");
+    PyStr.from_pylist = PyUnicode_FromString("from_pylist");
 
     PyObject *decimal_mod = PyImport_ImportModule("decimal");
     if (!decimal_mod) goto error;
     PyObject *datetime_mod = PyImport_ImportModule("datetime");
     if (!datetime_mod) goto error;
     PyObject *json_mod = PyImport_ImportModule("json");
     if (!json_mod) goto error;
```

### Comparing `singlestoredb-1.0.4/setup.cfg` & `singlestoredb-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.0.4
+version = 1.1.0
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
@@ -22,14 +22,15 @@
 	PyJWT
 	build
 	parsimonious
 	requests
 	setuptools
 	sqlparams
 	wheel
+	tomli>=1.1.0;python_version < '3.11'
 python_requires = >=3.8
 tests_require = 
 	coverage
 	pytest
 	pandas
 
 [options.packages.find]
@@ -73,15 +74,15 @@
 	management
 
 [flake8]
 exclude = 
 	docs/*
 	resources/*
 	licenses/*
-max-complexity = 30
+max-complexity = 35
 max-line-length = 90
 per-file-ignores = 
 	singlestoredb/__init__.py:F401
 	singlestoredb/fusion/__init__.py:F401
 	singlestoredb/fusion/grammar.py:E501
 	singlestoredb/http/__init__.py:F401
 	singlestoredb/management/__init__.py:F401
```

### Comparing `singlestoredb-1.0.4/setup.py` & `singlestoredb-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/__init__.py` & `singlestoredb-1.1.0/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.0.4'
+__version__ = '1.1.0'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.0.4/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.1.0/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/auth.py` & `singlestoredb-1.1.0/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/config.py` & `singlestoredb-1.1.0/singlestoredb/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 """SingleStoreDB package options."""
 import functools
+import os
 
 from . import auth
 from .utils.config import check_bool  # noqa: F401
 from .utils.config import check_dict_str_str  # noqa: F401
 from .utils.config import check_float  # noqa: F401
 from .utils.config import check_int  # noqa: F401
 from .utils.config import check_optional_bool  # noqa: F401
@@ -226,14 +227,15 @@
 register_option(
     'results.type', 'string',
     functools.partial(
         check_str,
         valid_values=[
             'tuple', 'tuples', 'namedtuple', 'namedtuples',
             'dict', 'dicts', 'structsequence', 'structsequences',
+            'numpy', 'pandas', 'polars', 'arrow', 'pyarrow',
         ],
     ),
     'tuples',
     'What form should the query results take?',
     environ='SINGLESTOREDB_RESULTS_TYPE',
 )
 
@@ -263,14 +265,137 @@
     'management.version', 'string', check_str, 'v1',
     'Specifies the version for the management API.',
     environ=['SINGLESTOREDB_MANAGEMENT_VERSION'],
 )
 
 
 #
+# External function options
+#
+register_option(
+    'external_function.url', 'string', check_str, 'http://localhost:8000/invoke',
+    'Specifies the URL of the external function application.',
+    environ=['SINGLESTOREDB_EXT_FUNC_URL'],
+)
+
+register_option(
+    'external_function.app_mode', 'string',
+    functools.partial(
+        check_str,
+        valid_values=['remote', 'collocated'],
+    ),
+    'remote',
+    'Specifies the mode of operation of the external function application.',
+    environ=['SINGLESTOREDB_EXT_FUNC_APP_MODE'],
+)
+
+register_option(
+    'external_function.data_format', 'string',
+    functools.partial(
+        check_str,
+        valid_values=['rowdat_1', 'json'],
+    ),
+    'rowdat_1',
+    'Specifies the format for the data rows.',
+    environ=['SINGLESTOREDB_EXT_FUNC_DATA_FORMAT'],
+)
+
+register_option(
+    'external_function.data_version', 'string', check_str, '1.0',
+    'Specifies the version of the data format.',
+    environ=['SINGLESTOREDB_EXT_FUNC_DATA_VERSION'],
+)
+
+register_option(
+    'external_function.link_name', 'string', check_str, None,
+    'Specifies the link name to use for remote external functions.',
+    environ=['SINGLESTOREDB_EXT_FUNC_LINK_NAME'],
+)
+
+register_option(
+    'external_function.link_config', 'string', check_str, None,
+    'Specifies the link config in JSON format.',
+    environ=['SINGLESTOREDB_EXT_FUNC_LINK_CONFIG'],
+)
+
+register_option(
+    'external_function.link_credentials', 'string', check_str, None,
+    'Specifies the link credentials in JSON format.',
+    environ=['SINGLESTOREDB_EXT_FUNC_LINK_CREDENTIALS'],
+)
+
+register_option(
+    'external_function.replace_existing', 'bool', check_bool, False,
+    'Should existing functions be replaced when registering external functions?',
+    environ=['SINGLESTOREDB_EXT_FUNC_REPLACE_EXISTING'],
+)
+
+register_option(
+    'external_function.socket_path', 'string', check_str, None,
+    'Specifies the socket path for collocated external functions.',
+    environ=['SINGLESTOREDB_EXT_FUNC_SOCKET_PATH'],
+)
+
+register_option(
+    'external_function.max_connections', 'int', check_int, 32,
+    'Specifies the maximum connections in a collocated external function ' +
+    'before reusing them.',
+    environ=['SINGLESTOREDB_EXT_FUNC_MAX_CONNECTIONS'],
+)
+
+register_option(
+    'external_function.process_mode', 'string',
+    functools.partial(
+        check_str,
+        valid_values=['thread', 'subprocess'],
+    ),
+    'subprocess',
+    'Specifies the method to use for concurrent handlers in ' +
+    'collocated external functions',
+    environ=['SINGLESTOREDB_EXT_FUNC_PROCESS_MODE'],
+)
+
+register_option(
+    'external_function.single_thread', 'bool', check_bool, False,
+    'Should the collocated server run in single-thread mode?',
+    environ=['SINGLESTOREDB_EXT_FUNC_SINGLE_THREAD'],
+)
+
+register_option(
+    'external_function.log_level', 'string',
+    functools.partial(
+        check_str,
+        valid_values=['info', 'debug', 'warning', 'error'],
+    ),
+    'info',
+    'Logging level of external function server.',
+    environ=['SINGLESTOREDB_EXT_FUNC_LOG_LEVEL'],
+)
+
+register_option(
+    'external_function.connection', 'string', check_str,
+    os.environ.get('SINGLESTOREDB_URL') or None,
+    'Specifies the connection string for the database to register functions with.',
+    environ=['SINGLESTOREDB_EXT_FUNC_CONNECTION'],
+)
+
+register_option(
+    'external_function.host', 'string', check_str, '127.0.0.1',
+    'Specifies the host to bind the server to.',
+    environ=['SINGLESTOREDB_EXT_FUNC_HOST'],
+)
+
+register_option(
+    'external_function.port', 'int', check_int, 8000,
+    'Specifies the port to bind the server to.',
+    environ=['SINGLESTOREDB_EXT_FUNC_PORT'],
+)
+
+
+#
 # Debugging options
 #
 register_option(
     'debug.queries', 'bool', check_bool, False,
     'Print queries and parameters to stderr.',
     environ='SINGLESTOREDB_DEBUG_QUERIES',
 )
```

### Comparing `singlestoredb-1.0.4/singlestoredb/connection.py` & `singlestoredb-1.1.0/singlestoredb/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/converters.py` & `singlestoredb-1.1.0/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/exceptions.py` & `singlestoredb-1.1.0/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/decorator.py` & `singlestoredb-1.1.0/singlestoredb/functions/decorator.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.1.0/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.1.0/singlestoredb/fusion/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,661 +1,721 @@
 #!/usr/bin/env python3
-'''
-Web application for SingleStoreDB external functions.
-
-This module supplies a function that can create web apps intended for use
-with the external function feature of SingleStoreDB. The application
-function is a standard ASGI <https://asgi.readthedocs.io/en/latest/index.html>
-request handler for use with servers such as Uvicorn <https://www.uvicorn.org>.
-
-An external function web application can be created using the `create_app`
-function. By default, the exported Python functions are specified by
-environment variables starting with SINGLESTOREDB_EXT_FUNCTIONS. See the
-documentation in `create_app` for the full syntax. If the application is
-created in Python code rather than from the command-line, exported
-functions can be specified in the parameters.
-
-An example of starting a server is shown below.
-
-Example
--------
-$ SINGLESTOREDB_EXT_FUNCTIONS='myfuncs.[percentage_90,percentage_95]' \
-    uvicorn --factory singlestoredb.functions.ext:create_app
-
-'''
-import importlib.util
-import io
-import itertools
-import json
-import os
+import abc
+import functools
 import re
-import secrets
-from types import ModuleType
+import textwrap
 from typing import Any
-from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
-from typing import Sequence
-from typing import Set
 from typing import Tuple
-from typing import Union
 
-from . import arrow
-from . import json as jdata
-from . import rowdat_1
-from ... import connection
-from ...mysql.constants import FIELD_TYPE as ft
-from ..signature import get_signature
-from ..signature import signature_to_sql
-
-# If a number of processes is specified, create a pool of workers
-num_processes = max(0, int(os.environ.get('SINGLESTOREDB_EXT_NUM_PROCESSES', 0)))
-if num_processes > 1:
-    try:
-        from ray.util.multiprocessing import Pool
-    except ImportError:
-        from multiprocessing import Pool
-    func_map = Pool(num_processes).starmap
-else:
-    func_map = itertools.starmap
-
-
-# Use negative values to indicate unsigned ints / binary data / usec time precision
-rowdat_1_type_map = {
-    'bool': ft.LONGLONG,
-    'int8': ft.LONGLONG,
-    'int16': ft.LONGLONG,
-    'int32': ft.LONGLONG,
-    'int64': ft.LONGLONG,
-    'uint8': -ft.LONGLONG,
-    'uint16': -ft.LONGLONG,
-    'uint32': -ft.LONGLONG,
-    'uint64': -ft.LONGLONG,
-    'float32': ft.DOUBLE,
-    'float64': ft.DOUBLE,
-    'str': ft.STRING,
-    'bytes': -ft.STRING,
+from parsimonious import Grammar
+from parsimonious import ParseError
+from parsimonious.nodes import Node
+from parsimonious.nodes import NodeVisitor
+
+from . import result
+from ..connection import Connection
+
+CORE_GRAMMAR = r'''
+    ws = ~r"(\s+|(\s*/\*.*\*/\s*)+)"
+    qs = ~r"\"([^\"]*)\"|'([^\']*)'|`([^\`]*)`|([A-Za-z0-9_\-\.]+)"
+    number = ~r"[-+]?(\d*\.)?\d+(e[-+]?\d+)?"i
+    integer = ~r"-?\d+"
+    comma = ws* "," ws*
+    eq = ws* "=" ws*
+    open_paren = ws* "(" ws*
+    close_paren = ws* ")" ws*
+    select = ~r"SELECT"i ws+ ~r".+" ws*
+'''
+
+BUILTINS = {
+    '<order-by>': r'''
+    order_by = ORDER BY order_by_key_,...
+    order_by_key_ = '<key>' [ ASC | DESC ]
+    ''',
+    '<like>': r'''
+    like = LIKE '<pattern>'
+    ''',
+    '<extended>': r'''
+    extended = EXTENDED
+    ''',
+    '<limit>': r'''
+    limit = LIMIT <integer>
+    ''',
+    '<integer>': '',
+    '<number>': '',
+}
+
+BUILTIN_DEFAULTS = {  # type: ignore
+    'order_by': {'by': []},
+    'like': None,
+    'extended': False,
+    'limit': None,
 }
 
 
-def get_func_names(funcs: str) -> List[Tuple[str, str]]:
-    '''
-    Parse all function names from string.
+def get_keywords(grammar: str) -> Tuple[str, ...]:
+    """Return all all-caps words from the beginning of the line."""
+    m = re.match(r'^\s*((?:[A-Z0-9_]+)(\s+|$|;))+', grammar)
+    if not m:
+        return tuple()
+    return tuple(re.split(r'\s+', m.group(0).replace(';', '').strip()))
+
+
+def is_bool(grammar: str) -> bool:
+    """Determine if the rule is a boolean."""
+    return bool(re.match(r'^[A-Z0-9_\s*]+$', grammar))
+
+
+def process_optional(m: Any) -> str:
+    """Create options or groups of options."""
+    sql = m.group(1).strip()
+    if '|' in sql:
+        return f'( {sql} )*'
+    return f'( {sql} )?'
+
+
+def process_alternates(m: Any) -> str:
+    """Make alternates mandatory groups."""
+    sql = m.group(1).strip()
+    if '|' in sql:
+        return f'( {sql} )'
+    raise ValueError(f'alternates must contain "|": {sql}')
+
+
+def process_repeats(m: Any) -> str:
+    """Add repeated patterns."""
+    sql = m.group(1).strip()
+    return f'open_paren? {sql} ws* ( comma {sql} ws* )* close_paren?'
+
+
+def lower_and_regex(m: Any) -> str:
+    """Lowercase and convert literal to regex."""
+    sql = m.group(1)
+    return f'~"{sql.lower()}"i'
+
+
+def split_unions(grammar: str) -> str:
+    """
+    Convert grammar in the form '[ x ] [ y ]' to '[ x | y ]'.
 
     Parameters
     ----------
-    func_names : str
-        String containing one or more function names. The syntax is
-        as follows: [func-name-1@func-alias-1,func-name-2@func-alias-2,...].
-        The optional '@name' portion is an alias if you want the function
-        to be renamed.
+    grammar : str
+        SQL grammar
 
     Returns
     -------
-    List[Tuple[str]] : a list of tuples containing the names and aliases
-        of each function.
-
-    '''
-    if funcs.startswith('['):
-        func_names = funcs.replace('[', '').replace(']', '').split(',')
-        func_names = [x.strip() for x in func_names]
-    else:
-        func_names = [funcs]
+    str
 
+    """
+    in_alternate = False
     out = []
-    for name in func_names:
-        alias = name
-        if '@' in name:
-            name, alias = name.split('@', 1)
-        out.append((name, alias))
-
-    return out
+    for c in grammar:
+        if c == '{':
+            in_alternate = True
+            out.append(c)
+        elif c == '}':
+            in_alternate = False
+            out.append(c)
+        elif not in_alternate and c == '|':
+            out.append(']')
+            out.append(' ')
+            out.append('[')
+        else:
+            out.append(c)
+    return ''.join(out)
 
 
-def make_func(name: str, func: Callable[..., Any]) -> Callable[..., Any]:
-    '''
-    Make a function endpoint.
+def expand_rules(rules: Dict[str, str], m: Any) -> str:
+    """
+    Return expanded grammar syntax for given rule.
 
     Parameters
     ----------
-    name : str
-        Name of the function to create
-    func : Callable
-        The function to call as the endpoint
+    ops : Dict[str, str]
+        Dictionary of rules in grammar
 
     Returns
     -------
-    Callable
+    str
+
+    """
+    txt = m.group(1)
+    if txt in rules:
+        return f' {rules[txt]} '
+    return f' <{txt}> '
+
+
+def build_cmd(grammar: str) -> str:
+    """Pre-process grammar to construct top-level command."""
+    if ';' not in grammar:
+        raise ValueError('a semi-colon exist at the end of the primary rule')
+
+    # Pre-space
+    m = re.match(r'^\s*', grammar)
+    space = m.group(0) if m else ''
+
+    # Split on ';' on a line by itself
+    begin, end = grammar.split(';', 1)
+
+    # Get statement keywords
+    keywords = get_keywords(begin)
+    cmd = '_'.join(x.lower() for x in keywords) + '_cmd'
+
+    # Collapse multi-line to one
+    begin = re.sub(r'\s+', r' ', begin)
+
+    return f'{space}{cmd} ={begin}\n{end}'
+
+
+def build_syntax(grammar: str) -> str:
+    """Construct full syntax."""
+    if ';' not in grammar:
+        raise ValueError('a semi-colon exist at the end of the primary rule')
+
+    # Split on ';' on a line by itself
+    cmd, end = grammar.split(';', 1)
+
+    rules = {}
+    for line in end.split('\n'):
+        line = line.strip()
+        if not line:
+            continue
+        name, value = line.split('=', 1)
+        name = name.strip()
+        value = value.strip()
+        rules[name] = value
+
+    while re.search(r' [a-z0-9_]+\b', cmd):
+        cmd = re.sub(r' ([a-z0-9_]+)\b', functools.partial(expand_rules, rules), cmd)
+
+    cmd = textwrap.dedent(cmd).rstrip() + ';'
+    cmd = re.sub(r'  +', ' ', cmd)
+    cmd = re.sub(r'^ ', '    ', cmd, flags=re.M)
+    cmd = re.sub(r'\s+,\.\.\.', ',...', cmd)
+
+    return cmd
+
+
+def _format_examples(ex: str) -> str:
+    """Convert examples into sections."""
+    return re.sub(r'(^Example\s+\d+.*$)', r'### \1', ex, flags=re.M)
+
+
+def _format_arguments(arg: str) -> str:
+    """Format arguments as subsections."""
+    out = []
+    for line in arg.split('\n'):
+        if line.startswith('<'):
+            out.append(f'### {line.replace("<", "&lt;").replace(">", "&gt;")}')
+            out.append('')
+        else:
+            out.append(line.strip())
+    return '\n'.join(out)
+
+
+def _to_markdown(txt: str) -> str:
+    """Convert formatting to markdown."""
+    txt = txt.replace('``', '`')
+
+    # Format code blocks
+    lines = re.split(r'\n', txt)
+    out = []
+    while lines:
+        line = lines.pop(0)
+        if line.endswith('::'):
+            out.append(line[:-2])
+            code = []
+            while lines and (not lines[0].strip() or lines[0].startswith(' ')):
+                code.append(lines.pop(0).rstrip())
+            out.extend(['```sql', '\n'.join(code).rstrip(), '```\n'])
+        else:
+            out.append(line)
+
+    return '\n'.join(out)
+
+
+def build_help(syntax: str, grammar: str) -> str:
+    """Build full help text."""
+    syntax = re.sub(r'\s*\n+\s*', r' ', syntax.strip())
+
+    cmd = re.match(r'([A-Z0-9_ ]+)', syntax)
+    if not cmd:
+        raise ValueError(f'no command found: {syntax}')
+
+    out = [f'# {cmd.group(1)}\n\n']
+
+    sections: Dict[str, str] = {}
+    grammar = textwrap.dedent(grammar.rstrip())
+    desc_re = re.compile(r'^([A-Z][\S ]+)\s*^\-\-\-\-+\s*$', flags=re.M)
+    if desc_re.search(grammar):
+        _, *txt = desc_re.split(grammar)
+        txt = [x.strip() for x in txt]
+        sections = {}
+        while txt:
+            key = txt.pop(0)
+            value = txt.pop(0)
+            sections[key.lower()] = _to_markdown(value).strip()
+
+    if 'description' in sections:
+        out.extend([sections['description'], '\n\n'])
+
+    out.extend(['## Syntax\n```sql\n', syntax, '\n```\n\n'])
+
+    if 'arguments' in sections:
+        out.extend([
+            '## Arguments\n\n',
+            _format_arguments(sections['arguments']),
+            '\n\n',
+        ])
+
+    if 'remarks' in sections:
+        out.extend(['## Remarks\n', sections['remarks'], '\n\n'])
+
+    if 'examples' in sections:
+        out.extend(['## Examples\n\n', _format_examples(sections['examples']), '\n\n'])
+    elif 'example' in sections:
+        out.extend(['## Example\n\n', _format_examples(sections['example']), '\n\n'])
+
+    if 'see also' in sections:
+        out.extend(['## See Also\n', sections['see also'], '\n\n'])
+
+    return ''.join(out).rstrip() + '\n'
 
-    '''
-    attrs = getattr(func, '_singlestoredb_attrs', {})
-    data_format = attrs.get('data_format') or 'python'
-    include_masks = attrs.get('include_masks', False)
-
-    if data_format == 'python':
-        async def do_func(
-            row_ids: Sequence[int],
-            rows: Sequence[Sequence[Any]],
-        ) -> Tuple[
-            Sequence[int],
-            List[Tuple[Any]],
-        ]:
-            '''Call function on given rows of data.'''
-            return row_ids, list(zip(func_map(func, rows)))
-
-    else:
-        # Vector formats use the same function wrapper
-        async def do_func(  # type: ignore
-            row_ids: Sequence[int],
-            cols: Sequence[Tuple[Sequence[Any], Optional[Sequence[bool]]]],
-        ) -> Tuple[Sequence[int], List[Tuple[Any, ...]]]:
-            '''Call function on given cols of data.'''
-            # TODO: only supports a single return value
-            if include_masks:
-                out = func(*cols)
-                assert isinstance(out, tuple)
-                return row_ids, [out]
-            return row_ids, [(func(*[x[0] for x in cols]), None)]
-
-    do_func.__name__ = name
-    do_func.__doc__ = func.__doc__
-
-    sig = get_signature(func, name=name)
-
-    # Store signature for generating CREATE FUNCTION calls
-    do_func._ext_func_signature = sig  # type: ignore
-
-    # Set data format
-    do_func._ext_func_data_format = data_format  # type: ignore
-
-    # Setup argument types for rowdat_1 parser
-    colspec = []
-    for x in sig['args']:
-        dtype = x['dtype'].replace('?', '')
-        if dtype not in rowdat_1_type_map:
-            raise TypeError(f'no data type mapping for {dtype}')
-        colspec.append((x['name'], rowdat_1_type_map[dtype]))
-    do_func._ext_func_colspec = colspec  # type: ignore
-
-    # Setup return type
-    dtype = sig['returns']['dtype'].replace('?', '')
-    if dtype not in rowdat_1_type_map:
-        raise TypeError(f'no data type mapping for {dtype}')
-    do_func._ext_func_returns = [rowdat_1_type_map[dtype]]  # type: ignore
-
-    return do_func
-
-
-def create_app(  # noqa: C901
-    functions: Optional[
-        Union[
-            str,
-            Iterable[str],
-            Callable[..., Any],
-            Iterable[Callable[..., Any]],
-            ModuleType,
-            Iterable[ModuleType],
-        ]
-    ] = None,
-    app_mode: str = 'remote',
-    url: str = 'http://localhost:8000/invoke',
-    data_format: str = 'rowdat_1',
-    data_version: str = '1.0',
-    link_config: Optional[Dict[str, Any]] = None,
-    link_credentials: Optional[Dict[str, Any]] = None,
-) -> Callable[..., Any]:
-    '''
-    Create an external function application.
-
-    If `functions` is None, the environment is searched for function
-    specifications in variables starting with `SINGLESTOREDB_EXT_FUNCTIONS`.
-    Any number of environment variables can be specified as long as they
-    have this prefix. The format of the environment variable value is the
-    same as for the `functions` parameter.
+
+def strip_comments(grammar: str) -> str:
+    """Strip comments from grammar."""
+    desc_re = re.compile(r'(^\s*Description\s*^\s*-----------\s*$)', flags=re.M)
+    grammar = desc_re.split(grammar, maxsplit=1)[0]
+    return re.sub(r'^\s*#.*$', r'', grammar, flags=re.M)
+
+
+def get_rule_info(grammar: str) -> Dict[str, Any]:
+    """Compute metadata about rule used in coallescing parsed output."""
+    return dict(
+        n_keywords=len(get_keywords(grammar)),
+        repeats=',...' in grammar,
+        default=False if is_bool(grammar) else [] if ',...' in grammar else None,
+    )
+
+
+def inject_builtins(grammar: str) -> str:
+    """Inject complex builtin rules."""
+    for k, v in BUILTINS.items():
+        if re.search(k, grammar):
+            grammar = re.sub(
+                k,
+                k.replace('<', '').replace('>', '').replace('-', '_'),
+                grammar,
+            )
+            grammar += v
+    return grammar
+
+
+def process_grammar(
+    grammar: str,
+) -> Tuple[Grammar, Tuple[str, ...], Dict[str, Any], str, str]:
+    """
+    Convert SQL grammar to a Parsimonious grammar.
 
     Parameters
     ----------
-    functions : str or Iterable[str], optional
-        Python functions are specified using a string format as follows:
-            * Single function : <pkg1>.<func1>
-            * Multiple functions : <pkg1>.[<func1-name,func2-name,...]
-            * Function aliases : <pkg1>.[<func1@alias1,func2@alias2,...]
-            * Multiple packages : <pkg1>.<func1>:<pkg2>.<func2>
-    app_mode : str, optional
-        The mode of operation for the application: remote or collocated
-    url : str, optional
-        The URL of the function API
-    data_format : str, optional
-        The format of the data rows: 'rowdat_1' or 'json'
-    data_version : str, optional
-        The version of the call format to expect: '1.0'
-    link_config : Dict[str, Any], optional
-        The CONFIG section of a LINK definition. This dictionary gets
-        converted to JSON for the CREATE LINK call.
-    link_credentials : Dict[str, Any], optional
-        The CREDENTIALS section of a LINK definition. This dictionary gets
-        converted to JSON for the CREATE LINK call.
+    grammar : str
+        The SQL grammar
 
     Returns
     -------
-    Callable : the application request handler
+    (Grammar, Tuple[str, ...], Dict[str, Any], str) - Grammar is the parsimonious
+    grammar object. The tuple is a series of the keywords that start the command.
+    The dictionary is a set of metadata about each rule. The final string is
+    a human-readable version of the grammar for documentation and errors.
 
-    '''
+    """
+    out = []
+    rules = {}
+    rule_info = {}
 
-    # List of functions specs
-    specs: List[Union[str, Callable[..., Any], ModuleType]] = []
+    full_grammar = grammar
+    grammar = strip_comments(grammar)
+    grammar = inject_builtins(grammar)
+    command_key = get_keywords(grammar)
+    syntax_txt = build_syntax(grammar)
+    help_txt = build_help(syntax_txt, full_grammar)
+    grammar = build_cmd(grammar)
 
-    # Look up Python function specifications
-    if functions is None:
-        env_vars = [
-            x for x in os.environ.keys()
-            if x.startswith('SINGLESTOREDB_EXT_FUNCTIONS')
-        ]
-        if env_vars:
-            specs = [os.environ[x] for x in env_vars]
-        else:
-            import __main__
-            specs = [__main__]
+    # Make sure grouping characters all have whitespace around them
+    grammar = re.sub(r' *(\[|\{|\||\}|\]) *', r' \1 ', grammar)
 
-    elif isinstance(functions, ModuleType):
-        specs = [functions]
+    for line in grammar.split('\n'):
+        if not line.strip():
+            continue
 
-    elif isinstance(functions, str):
-        specs = [functions]
+        op, sql = line.split('=', 1)
+        op = op.strip()
+        sql = sql.strip()
+        sql = split_unions(sql)
 
-    elif callable(functions):
-        specs = [functions]
-
-    else:
-        specs = list(functions)
-
-    # Add functions to application
-    endpoints = dict()
-    for funcs in itertools.chain(specs):
-
-        if isinstance(funcs, str):
-            # Module name
-            if importlib.util.find_spec(funcs) is not None:
-                items = importlib.import_module(funcs)
-                for x in vars(items).values():
-                    if not hasattr(x, '_singlestoredb_attrs'):
-                        continue
-                    name = x._singlestoredb_attrs.get('name', x.__name__)
-                    func = make_func(name, x)
-                    endpoints[name.encode('utf-8')] = func
-
-            # Fully qualified function name
-            else:
-                pkg_path, func_names = funcs.rsplit('.', 1)
-                pkg = importlib.import_module(pkg_path)
-
-                # Add endpoint for each exported function
-                for name, alias in get_func_names(func_names):
-                    item = getattr(pkg, name)
-                    func = make_func(alias, item)
-                    endpoints[alias.encode('utf-8')] = func
-
-        elif isinstance(funcs, ModuleType):
-            for x in vars(funcs).values():
-                if not hasattr(x, '_singlestoredb_attrs'):
-                    continue
-                name = x._singlestoredb_attrs.get('name', x.__name__)
-                func = make_func(name, x)
-                endpoints[name.encode('utf-8')] = func
+        rules[op] = sql
+        rule_info[op] = get_rule_info(sql)
 
-        else:
-            alias = funcs.__name__
-            func = make_func(alias, funcs)
-            endpoints[alias.encode('utf-8')] = func
-
-    # Plain text response start
-    text_response_dict: Dict[str, Any] = dict(
-        type='http.response.start',
-        status=200,
-        headers=[(b'content-type', b'text/plain')],
-    )
+        # Convert consecutive optionals to a union
+        sql = re.sub(r'\]\s+\[', r' | ', sql)
 
-    # JSON response start
-    json_response_dict: Dict[str, Any] = dict(
-        type='http.response.start',
-        status=200,
-        headers=[(b'content-type', b'application/json')],
-    )
+        # Lower-case keywords and make them case-insensitive
+        sql = re.sub(r'\b([A-Z0-9]+)\b', lower_and_regex, sql)
 
-    # ROWDAT_1 response start
-    rowdat_1_response_dict: Dict[str, Any] = dict(
-        type='http.response.start',
-        status=200,
-        headers=[(b'content-type', b'x-application/rowdat_1')],
-    )
+        # Convert literal strings to 'qs'
+        sql = re.sub(r"'[^']+'", r'qs', sql)
 
-    # Apache Arrow response start
-    arrow_response_dict: Dict[str, Any] = dict(
-        type='http.response.start',
-        status=200,
-        headers=[(b'content-type', b'application/vnd.apache.arrow.file')],
-    )
+        # Convert special characters to literal tokens
+        sql = re.sub(r'([=]) ', r' eq ', sql)
 
-    # Path not found response start
-    path_not_found_response_dict: Dict[str, Any] = dict(
-        type='http.response.start',
-        status=404,
-    )
+        # Convert [...] groups to (...)*
+        sql = re.sub(r'\[([^\]]+)\]', process_optional, sql)
+
+        # Convert {...} groups to (...)
+        sql = re.sub(r'\{([^\}]+)\}', process_alternates, sql)
+
+        # Convert <...> to ... (<...> is the form for core types)
+        sql = re.sub(r'<([a-z0-9_]+)>', r'\1', sql)
+
+        # Insert ws between every token to allow for whitespace and comments
+        sql = ' ws '.join(re.split(r'\s+', sql)) + ' ws'
+
+        # Remove ws in optional groupings
+        sql = sql.replace('( ws', '(')
+        sql = sql.replace('| ws', '|')
+
+        # Convert | to /
+        sql = sql.replace('|', '/')
+
+        # Remove ws after operation names, all operations contain ws at the end
+        sql = re.sub(r'(\s+[a-z0-9_]+)\s+ws\b', r'\1', sql)
+
+        # Convert foo,... to foo ("," foo)*
+        sql = re.sub(r'(\S+),...', process_repeats, sql)
+
+        # Remove ws before / and )
+        sql = re.sub(r'(\s*\S+\s+)ws\s+/', r'\1/', sql)
+        sql = re.sub(r'(\s*\S+\s+)ws\s+\)', r'\1)', sql)
+
+        # Make sure every operation ends with ws
+        sql = re.sub(r'\s+ws\s+ws$', r' ws', sql + ' ws')
+        sql = re.sub(r'(\s+ws)*\s+ws\*$', r' ws*', sql)
+        sql = re.sub(r'\s+ws$', r' ws*', sql)
+        sql = re.sub(r'\s+ws\s+\(', r' ws* (', sql)
+        sql = re.sub(r'\)\s+ws\s+', r') ws* ', sql)
+        sql = re.sub(r'\s+ws\s+', r' ws+ ', sql)
+        sql = re.sub(r'\?\s+ws\+', r'? ws*', sql)
+
+        # Remove extra ws around eq
+        sql = re.sub(r'ws\+\s*eq\b', r'eq', sql)
+
+        out.append(f'{op} = {sql}')
+
+    for k, v in list(rules.items()):
+        while re.search(r' ([a-z0-9_]+) ', v):
+            v = re.sub(r' ([a-z0-9_]+) ', functools.partial(expand_rules, rules), v)
+        rules[k] = v
+
+    for k, v in list(rules.items()):
+        while re.search(r' <([a-z0-9_]+)> ', v):
+            v = re.sub(r' <([a-z0-9_]+)> ', r' \1 ', v)
+        rules[k] = v
 
-    # Response body template
-    body_response_dict: Dict[str, Any] = dict(
-        type='http.response.body',
+    cmds = ' / '.join(x for x in rules if x.endswith('_cmd'))
+    cmds = f'init = ws* ( {cmds} ) ws* ";"? ws*\n'
+
+    return (
+        Grammar(cmds + CORE_GRAMMAR + '\n'.join(out)), command_key,
+        rule_info, syntax_txt, help_txt,
     )
 
-    # Data format + version handlers
-    handlers = {
-        (b'application/octet-stream', b'1.0', 'python'): dict(
-            load=rowdat_1.load,
-            dump=rowdat_1.dump,
-            response=rowdat_1_response_dict,
-        ),
-        (b'application/octet-stream', b'1.0', 'pandas'): dict(
-            load=rowdat_1.load_pandas,
-            dump=rowdat_1.dump_pandas,
-            response=rowdat_1_response_dict,
-        ),
-        (b'application/octet-stream', b'1.0', 'numpy'): dict(
-            load=rowdat_1.load_numpy,
-            dump=rowdat_1.dump_numpy,
-            response=rowdat_1_response_dict,
-        ),
-        (b'application/octet-stream', b'1.0', 'polars'): dict(
-            load=rowdat_1.load_polars,
-            dump=rowdat_1.dump_polars,
-            response=rowdat_1_response_dict,
-        ),
-        (b'application/octet-stream', b'1.0', 'arrow'): dict(
-            load=rowdat_1.load_arrow,
-            dump=rowdat_1.dump_arrow,
-            response=rowdat_1_response_dict,
-        ),
-        (b'application/json', b'1.0', 'python'): dict(
-            load=jdata.load,
-            dump=jdata.dump,
-            response=json_response_dict,
-        ),
-        (b'application/json', b'1.0', 'pandas'): dict(
-            load=jdata.load_pandas,
-            dump=jdata.dump_pandas,
-            response=json_response_dict,
-        ),
-        (b'application/json', b'1.0', 'numpy'): dict(
-            load=jdata.load_numpy,
-            dump=jdata.dump_numpy,
-            response=json_response_dict,
-        ),
-        (b'application/json', b'1.0', 'polars'): dict(
-            load=jdata.load_polars,
-            dump=jdata.dump_polars,
-            response=json_response_dict,
-        ),
-        (b'application/json', b'1.0', 'arrow'): dict(
-            load=jdata.load_arrow,
-            dump=jdata.dump_arrow,
-            response=json_response_dict,
-        ),
-        (b'application/vnd.apache.arrow.file', b'1.0', 'python'): dict(
-            load=arrow.load,
-            dump=arrow.dump,
-            response=arrow_response_dict,
-        ),
-        (b'application/vnd.apache.arrow.file', b'1.0', 'pandas'): dict(
-            load=arrow.load_pandas,
-            dump=arrow.dump_pandas,
-            response=arrow_response_dict,
-        ),
-        (b'application/vnd.apache.arrow.file', b'1.0', 'numpy'): dict(
-            load=arrow.load_numpy,
-            dump=arrow.dump_numpy,
-            response=arrow_response_dict,
-        ),
-        (b'application/vnd.apache.arrow.file', b'1.0', 'polars'): dict(
-            load=arrow.load_polars,
-            dump=arrow.dump_polars,
-            response=arrow_response_dict,
-        ),
-        (b'application/vnd.apache.arrow.file', b'1.0', 'arrow'): dict(
-            load=arrow.load_arrow,
-            dump=arrow.dump_arrow,
-            response=arrow_response_dict,
-        ),
-    }
-
-    # Valid URL paths
-    invoke_path = ('invoke',)
-    show_create_function_path = ('show', 'create_function')
-
-    async def app(
-        scope: Dict[str, Any],
-        receive: Callable[..., Awaitable[Any]],
-        send: Callable[..., Awaitable[Any]],
-    ) -> None:
-        '''
-        Application request handler.
 
-        Parameters
-        ----------
-        scope : dict
-            ASGI request scope
-        receive : Callable
-            Function to receieve request information
-        send : Callable
-            Function to send response information
-
-        '''
-        assert scope['type'] == 'http'
-
-        method = scope['method']
-        path = tuple(x for x in scope['path'].split('/') if x)
-        headers = dict(scope['headers'])
-
-        content_type = headers.get(
-            b'content-type',
-            b'application/octet-stream',
-        )
-        accepts = headers.get(b'accepts', content_type)
-        func_name = headers.get(b's2-ef-name', b'')
-        func = endpoints.get(func_name)
-
-        # Call the endpoint
-        if method == 'POST' and func is not None and path == invoke_path:
-            data_format = func._ext_func_data_format  # type: ignore
-            data = []
-            more_body = True
-            while more_body:
-                request = await receive()
-                data.append(request['body'])
-                more_body = request.get('more_body', False)
-
-            data_version = headers.get(b's2-ef-version', b'')
-            input_handler = handlers[(content_type, data_version, data_format)]
-            output_handler = handlers[(accepts, data_version, data_format)]
-
-            out = await func(
-                *input_handler['load'](
-                    func._ext_func_colspec, b''.join(data),  # type: ignore
-                ),
-            )
-            body = output_handler['dump'](func._ext_func_returns, *out)  # type: ignore
+def flatten(items: Iterable[Any]) -> List[Any]:
+    """Flatten a list of iterables."""
+    out = []
+    for x in items:
+        if isinstance(x, (str, bytes, dict)):
+            out.append(x)
+        elif isinstance(x, Iterable):
+            for sub_x in flatten(x):
+                if sub_x is not None:
+                    out.append(sub_x)
+        elif x is not None:
+            out.append(x)
+    return out
+
 
-            await send(output_handler['response'])
+def merge_dicts(items: List[Dict[str, Any]]) -> Dict[str, Any]:
+    """Merge list of dictionaries together."""
+    out: Dict[str, Any] = {}
+    for x in items:
+        if isinstance(x, dict):
+            same = list(set(x.keys()).intersection(set(out.keys())))
+            if same:
+                raise ValueError(f"found duplicate rules for '{same[0]}'")
+            out.update(x)
+    return out
 
-        # Handle api reflection
-        elif method == 'GET' and path == show_create_function_path:
-            host = headers.get(b'host', b'localhost:80')
-            reflected_url = f'{scope["scheme"]}://{host.decode("utf-8")}/invoke'
-            data_format = 'json' if b'json' in content_type else 'rowdat_1'
-
-            syntax = []
-            for key, endpoint in endpoints.items():
-                if not func_name or key == func_name:
-                    syntax.append(
-                        signature_to_sql(
-                            endpoint._ext_func_signature,  # type: ignore
-                            url=url or reflected_url,
-                            data_format=data_format,
-                        ),
-                    )
-            body = '\n'.join(syntax).encode('utf-8')
 
-            await send(text_response_dict)
+class SQLHandler(NodeVisitor):
+    """Base class for all SQL handler classes."""
 
-        # Path not found
-        else:
-            body = b''
-            await send(path_not_found_response_dict)
+    #: Parsimonious grammar object
+    grammar: Grammar = Grammar(CORE_GRAMMAR)
 
-        # Send body
-        out = body_response_dict.copy()
-        out['body'] = body
-        await send(out)
-
-    def _create_link(
-        config: Optional[Dict[str, Any]],
-        credentials: Optional[Dict[str, Any]],
-    ) -> Tuple[str, str]:
-        """Generate CREATE LINK command."""
-        if not config and not credentials:
-            return '', ''
-
-        link_name = f'link_{secrets.token_hex(16)}'
-        out = [f'CREATE LINK {link_name} AS HTTP']
-
-        if config:
-            out.append(f"CONFIG '{json.dumps(config)}'")
-
-        if credentials:
-            out.append(f"CREDENTIALS '{json.dumps(credentials)}'")
-
-        return link_name, ' '.join(out) + ';'
-
-    def _locate_app_functions(cur: Any) -> Tuple[Set[str], Set[str]]:
-        """Locate all current functions and links belonging to this app."""
-        funcs, links = set(), set()
-        cur.execute('SHOW FUNCTIONS')
-        for name, ftype, _, _, _, link in list(cur):
-            # Only look at external functions
-            if 'external' not in ftype.lower():
-                continue
-            # See if function URL matches url
-            cur.execute(f'SHOW CREATE FUNCTION `{name}`')
-            for fname, _, code, *_ in list(cur):
-                m = re.search(r" (?:\w+) SERVICE '([^']+)'", code)
-                if m and m.group(1) == url:
-                    funcs.add(fname)
-                    if link:
-                        links.add(link)
-        return funcs, links
-
-    def show_create_functions(
-        replace: bool = False,
-    ) -> List[str]:
-        """Generate CREATE FUNCTION calls."""
-        if not endpoints:
-            return []
-
-        out = []
-        link = ''
-        if app_mode.lower() == 'remote':
-            link, link_str = _create_link(link_config, link_credentials)
-            if link and link_str:
-                out.append(link_str)
-
-        for key, endpoint in endpoints.items():
-            out.append(
-                signature_to_sql(
-                    endpoint._ext_func_signature,  # type: ignore
-                    url=url,
-                    data_format=data_format,
-                    app_mode=app_mode,
-                    replace=replace,
-                    link=link or None,
-                ),
-            )
+    #: SQL keywords that start the command
+    command_key: Tuple[str, ...] = ()
 
-        return out
+    #: Metadata about the parse rules
+    rule_info: Dict[str, Any] = {}
 
-    app.show_create_functions = show_create_functions  # type: ignore
+    #: Syntax string for use in error messages
+    syntax: str = ''
 
-    def register_functions(
-        *connection_args: Any,
-        replace: bool = False,
-        **connection_kwargs: Any,
-    ) -> None:
-        """Register functions with the database."""
-        with connection.connect(*connection_args, **connection_kwargs) as conn:
-            with conn.cursor() as cur:
-                if replace:
-                    funcs, links = _locate_app_functions(cur)
-                    for fname in funcs:
-                        cur.execute(f'DROP FUNCTION IF EXISTS `{fname}`')
-                    for link in links:
-                        cur.execute(f'DROP LINK {link}')
-                for func in app.show_create_functions(replace=replace):  # type: ignore
-                    cur.execute(func)
-
-    app.register_functions = register_functions  # type: ignore
-
-    def drop_functions(
-        *connection_args: Any,
-        **connection_kwargs: Any,
-    ) -> None:
-        """Drop registered functions from database."""
-        with connection.connect(*connection_args, **connection_kwargs) as conn:
-            with conn.cursor() as cur:
-                funcs, links = _locate_app_functions(cur)
-                for fname in funcs:
-                    cur.execute(f'DROP FUNCTION IF EXISTS `{fname}`')
-                for link in links:
-                    cur.execute(f'DROP LINK {link}')
-
-    app.drop_functions = drop_functions  # type: ignore
-
-    async def call(
-        name: str,
-        data_in: io.BytesIO,
-        data_out: io.BytesIO,
-        data_format: str = data_format,
-        data_version: str = data_version,
-    ) -> None:
-
-        async def receive() -> Dict[str, Any]:
-            return dict(body=data_in.read())
-
-        async def send(content: Dict[str, Any]) -> None:
-            status = content.get('status', 200)
-            if status != 200:
-                raise KeyError(f'error occurred when calling `{name}`: {status}')
-            data_out.write(content.get('body', b''))
-
-        accepts = dict(
-            json=b'application/json',
-            rowdat_1=b'application/octet-stream',
-            arrow=b'application/vnd.apache.arrow.file',
-        )
+    #: Full help for the command
+    help: str = ''
+
+    #: Rule validation functions
+    validators: Dict[str, Callable[..., Any]] = {}
+
+    _grammar: str = CORE_GRAMMAR
+    _is_compiled: bool = False
+
+    def __init__(self, connection: Connection):
+        self.connection = connection
 
-        # Mock an ASGI scope
-        scope = dict(
-            type='http',
-            path='invoke',
-            method='POST',
-            headers={
-                b'content-type': accepts[data_format.lower()],
-                b'accepts': accepts[data_format.lower()],
-                b's2-ef-name': name.encode('utf-8'),
-                b's2-ef-version': data_version.encode('utf-8'),
-            },
+    @classmethod
+    def compile(cls, grammar: str = '') -> None:
+        """
+        Compile the grammar held in the docstring.
+
+        This method modifies attributes on the class: ``grammar``,
+        ``command_key``, ``rule_info``, ``syntax``, and ``help``.
+
+        Parameters
+        ----------
+        grammar : str, optional
+            Grammar to use instead of docstring
+
+        """
+        if cls._is_compiled:
+            return
+
+        cls.grammar, cls.command_key, cls.rule_info, cls.syntax, cls.help = \
+            process_grammar(grammar or cls.__doc__ or '')
+
+        cls._grammar = grammar or cls.__doc__ or ''
+        cls._is_compiled = True
+
+    @classmethod
+    def register(cls, overwrite: bool = False) -> None:
+        """
+        Register the handler class.
+
+        Paraemeters
+        -----------
+        overwrite : bool, optional
+            Overwrite an existing command with the same name?
+
+        """
+        from . import registry
+        cls.compile()
+        registry.register_handler(cls, overwrite=overwrite)
+
+    def execute(self, sql: str) -> result.FusionSQLResult:
+        """
+        Parse the SQL and invoke the handler method.
+
+        Parameters
+        ----------
+        sql : str
+            SQL statement to execute
+
+        Returns
+        -------
+        DummySQLResult
+
+        """
+        import warnings
+        warnings.warn(
+            'Fusion SQL is currently a preview feature. '
+            'Run `SHOW FUSION COMMANDS` to see all commands.',
+            RuntimeWarning,
         )
 
-        await app(scope, receive, send)
+        type(self).compile()
+        try:
+            params = self.visit(type(self).grammar.parse(sql))
+            for k, v in params.items():
+                params[k] = self.validate_rule(k, v)
+
+            res = self.run(params)
+            if res is not None:
+                res.format_results(self.connection)
+                return res
+
+            res = result.FusionSQLResult()
+            res.set_rows([])
+            res.format_results(self.connection)
+            return res
+
+        except ParseError as exc:
+            s = str(exc)
+            msg = ''
+            m = re.search(r'(The non-matching portion.*$)', s)
+            if m:
+                msg = ' ' + m.group(1)
+            m = re.search(r"(Rule) '.+?'( didn't match at.*$)", s)
+            if m:
+                msg = ' ' + m.group(1) + m.group(2)
+            raise ValueError(
+                f'Could not parse statement.{msg} '
+                'Expecting:\n' + textwrap.indent(type(self).syntax, '  '),
+            )
 
-    app.call = call  # type: ignore
+    @abc.abstractmethod
+    def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
+        """
+        Run the handler command.
 
-    return app
+        Parameters
+        ----------
+        params : Dict[str, Any]
+            Values parsed from the SQL query. Each rule in the grammar
+            results in a key/value pair in the ``params` dictionary.
+
+        Returns
+        -------
+        SQLResult - tuple containing the column definitions and
+            rows of data in the result
+
+        """
+        raise NotImplementedError
+
+    def visit_qs(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Quoted strings."""
+        if node is None:
+            return None
+        return node.match.group(1) or node.match.group(2) or \
+            node.match.group(3) or node.match.group(4)
+
+    def visit_number(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Numeric value."""
+        return float(node.match.group(0))
+
+    def visit_integer(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Integer value."""
+        return int(node.match.group(0))
+
+    def visit_ws(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Whitespace and comments."""
+        return
+
+    def visit_eq(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Equals sign."""
+        return
+
+    def visit_comma(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Single comma."""
+        return
+
+    def visit_open_paren(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Open parenthesis."""
+        return
+
+    def visit_close_paren(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Close parenthesis."""
+        return
+
+    def visit_init(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Entry point of the grammar."""
+        _, out, *_ = visited_children
+        return out
+
+    def visit_select(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        out = ' '.join(flatten(visited_children))
+        return {'select': out}
+
+    def visit_order_by(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """Handle ORDER BY."""
+        by = []
+        ascending = []
+        data = [x for x in flatten(visited_children)[2:] if x]
+        for item in data:
+            value = item.popitem()[-1]
+            if not isinstance(value, list):
+                value = [value]
+            value.append('A')
+            by.append(value[0])
+            ascending.append(value[1].upper().startswith('A'))
+        return {'order_by': {'by': by, 'ascending': ascending}}
+
+    def generic_visit(self, node: Node, visited_children: Iterable[Any]) -> Any:
+        """
+        Handle all undefined rules.
+
+        This method processes all user-defined rules. Each rule results in
+        a dictionary with a single key corresponding to the rule name, with
+        a value corresponding to the data value following the rule keywords.
+
+        If no value exists, the value True is used. If the rule is not a
+        rule with possible repeated values, a single value is used. If the
+        rule can have repeated values, a list of values is returned.
+
+        """
+        # Call a grammar rule
+        if node.expr_name in type(self).rule_info:
+            n_keywords = type(self).rule_info[node.expr_name]['n_keywords']
+            repeats = type(self).rule_info[node.expr_name]['repeats']
+
+            # If this is the top-level command, create the final result
+            if node.expr_name.endswith('_cmd'):
+                final = merge_dicts(flatten(visited_children)[n_keywords:])
+                for k, v in type(self).rule_info.items():
+                    if k.endswith('_cmd') or k.endswith('_'):
+                        continue
+                    if k not in final:
+                        final[k] = BUILTIN_DEFAULTS.get(k, v['default'])
+                return final
+
+            # Filter out stray empty strings
+            out = [x for x in flatten(visited_children)[n_keywords:] if x]
+
+            if repeats or len(out) > 1:
+                return {node.expr_name: out}
+
+            return {node.expr_name: out[0] if out else True}
+
+        if hasattr(node, 'match'):
+            if not visited_children and not node.match.groups():
+                return node.text
+            return visited_children or list(node.match.groups())
+
+        return visited_children or node.text
+
+    def validate_rule(self, rule: str, value: Any) -> Any:
+        """
+        Validate the value of the given rule.
+
+        Paraemeters
+        -----------
+        rule : str
+            Name of the grammar rule the value belongs to
+        value : Any
+            Value parsed from the query
+
+        Returns
+        -------
+        Any - result of the validator function
+
+        """
+        validator = type(self).validators.get(rule)
+        if validator is not None:
+            return validator(value)
+        return value
```

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/ext/json.py` & `singlestoredb-1.1.0/singlestoredb/functions/ext/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,16 +208,16 @@
     if not has_numpy:
         raise RuntimeError('This operation requires numpy to be installed')
 
     row_ids, cols = _load_vectors(colspec, data)
     return np.asarray(row_ids, dtype=np.longlong), \
         [
             (
-                np.asarray(data, dtype=NUMPY_TYPE_MAP[spec[1]]),
-                np.asarray(mask, dtype=np.bool_),
+                np.asarray(data, dtype=NUMPY_TYPE_MAP[spec[1]]),  # type: ignore
+                np.asarray(mask, dtype=np.bool_),  # type: ignore
             )
             for (data, mask), spec in zip(cols, colspec)
         ]
 
 
 def load_arrow(
     colspec: List[Tuple[str, int]],
```

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.1.0/singlestoredb/functions/ext/rowdat_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,16 +283,16 @@
     if not has_numpy:
         raise RuntimeError('numpy must be installed for this operation')
 
     row_ids, cols = _load_vectors(colspec, data)
     return np.asarray(row_ids, dtype=np.int64), \
         [
             (
-                np.asarray(data, dtype=NUMPY_TYPE_MAP[dtype]),
-                np.asarray(mask, dtype=np.bool_),
+                np.asarray(data, dtype=NUMPY_TYPE_MAP[dtype]),  # type: ignore
+                np.asarray(mask, dtype=np.bool_),  # type: ignore
             )
             for (data, mask), (name, dtype) in zip(cols, colspec)
         ]
 
 
 def _load_arrow(
     colspec: List[Tuple[str, int]],
```

### Comparing `singlestoredb-1.0.4/singlestoredb/functions/signature.py` & `singlestoredb-1.1.0/singlestoredb/functions/signature.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/fusion/graphql.py` & `singlestoredb-1.1.0/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.1.0/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/fusion/registry.py` & `singlestoredb-1.1.0/singlestoredb/fusion/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import re
+import sys
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
@@ -116,23 +117,37 @@
 class ShowFusionCommandsHandler(SQLHandler):
     """
     SHOW FUSION COMMANDS [ like ];
 
     # LIKE pattern
     like = LIKE '<pattern>'
 
+    Description
+    -----------
+    Display all Fusion SQL commands.
+
+    Remarks
+    -------
+    * ``LIKE`` indicates a pattern of commands to display. ``%`` is a wildcard.
+
+    Example
+    -------
+    Display all commands starting with 'SHOW'::
+
+        SHOW FUSION COMMANDS LIKE 'SHOW%';
+
     """
 
     def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
         res = result.FusionSQLResult()
         res.add_field('Command', result.STRING)
 
         data: List[Tuple[Any, ...]] = []
         for _, v in sorted(_handlers.items()):
-            data.append((v.help.lstrip(),))
+            data.append((v.syntax.lstrip(),))
 
         res.set_rows(data)
 
         if params['like']:
             res = res.like(Command=params['like'])
 
         return res
@@ -144,21 +159,74 @@
 class ShowFusionGrammarHandler(SQLHandler):
     """
     SHOW FUSION GRAMMAR for_query;
 
     # Query to show grammar for
     for_query = FOR '<query>'
 
+    Description
+    -----------
+    Show the full grammar of a Fusion SQL command for a given query.
+
+    Remarks
+    -------
+    * ``<query>`` is a string containing a Fusion SQL command.
+
+    Example
+    -------
+    Display the full grammar of the ``CREATE WORKSPACE`` command::
+
+        SHOW FUSION GRAMMAR FOR 'CREATE WORKSPACE';
+
     """
 
     def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
         res = result.FusionSQLResult()
         res.add_field('Grammar', result.STRING)
         handler = get_handler(params['for_query'])
         data: List[Tuple[Any, ...]] = []
         if handler is not None:
             data.append((handler._grammar,))
         res.set_rows(data)
         return res
 
 
 ShowFusionGrammarHandler.register()
+
+
+class ShowFusionHelpHandler(SQLHandler):
+    """
+    SHOW FUSION HELP for_command;
+
+    # Command to show help for
+    for_command = FOR '<command>'
+
+    Description
+    -----------
+    Show the documentation for a Fusion SQL command.
+
+    Example
+    -------
+    Display the help for the ``CREATE WORKSPACE`` command::
+
+        SHOW FUSION HELP FOR 'CREATE WORKSPACE';
+
+    """
+
+    def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
+        handler = get_handler(params['for_command'])
+        if handler is not None:
+            try:
+                from IPython.display import display
+                from IPython.display import Markdown
+                display(Markdown(handler.help))
+            except Exception:
+                print(handler.help)
+        else:
+            print(
+                f'No handler found for command \'{params["for_command"]}\'',
+                file=sys.stderr,
+            )
+        return None
+
+
+ShowFusionHelpHandler.register()
```

### Comparing `singlestoredb-1.0.4/singlestoredb/fusion/result.py` & `singlestoredb-1.1.0/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/http/__init__.py` & `singlestoredb-1.1.0/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/http/connection.py` & `singlestoredb-1.1.0/singlestoredb/http/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 from ..exceptions import ProgrammingError
 from ..exceptions import Warning  # noqa: F401
 from ..utils.convert_rows import convert_rows
 from ..utils.debug import log_query
 from ..utils.mogrify import mogrify
 from ..utils.results import Description
 from ..utils.results import format_results
+from ..utils.results import get_schema
 from ..utils.results import Result
 
 
 # DB-API settings
 apilevel = '2.0'
 paramstyle = 'named'
 threadsafety = 1
@@ -329,14 +330,15 @@
         self._connection: Optional[Connection] = conn
         self._results: List[List[Tuple[Any, ...]]] = [[]]
         self._results_type: str = self._connection._results_type \
             if self._connection is not None else 'tuples'
         self._row_idx: int = -1
         self._result_idx: int = -1
         self._descriptions: List[List[Description]] = []
+        self._schemas: List[Dict[str, Any]] = []
         self.arraysize: int = get_option('results.arraysize')
         self.rowcount: int = 0
         self.lastrowid: Optional[int] = None
         self._pymy_results: List[PyMyResult] = []
         self._expect_results: bool = False
 
     @property
@@ -351,14 +353,22 @@
         """Return description for current result set."""
         if not self._descriptions:
             return None
         if self._result_idx >= 0 and self._result_idx < len(self._descriptions):
             return self._descriptions[self._result_idx]
         return None
 
+    @property
+    def _schema(self) -> Optional[Any]:
+        if not self._schemas:
+            return None
+        if self._result_idx >= 0 and self._result_idx < len(self._schemas):
+            return self._schemas[self._result_idx]
+        return None
+
     def _post(self, path: str, *args: Any, **kwargs: Any) -> requests.Response:
         """
         Invoke a POST request on the HTTP connection.
 
         Parameters
         ----------
         path : str
@@ -456,14 +466,15 @@
                 oper,
                 handler=handler,
             )
         finally:
             self._results_type = results_type
 
         self._descriptions.append(list(mgmt_res.description))
+        self._schemas.append(get_schema(self._results_type, list(mgmt_res.description)))
         self._results.append(list(mgmt_res.rows))
         self.rowcount = len(self._results[-1])
 
         pymy_res = PyMyResult()
         for field in mgmt_res.fields:
             pymy_res.append(
                 PyMyField(
@@ -483,14 +494,15 @@
 
     def _execute(
         self, oper: str,
         params: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
         is_callproc: bool = False,
     ) -> int:
         self._descriptions = []
+        self._schemas = []
         self._results = []
         self._pymy_results = []
         self._row_idx = -1
         self._result_idx = -1
         self.rowcount = 0
         self._expect_results = False
 
@@ -567,14 +579,28 @@
 
             # Merge passed in converters
             if self._connection._conv:
                 for k, v in self._connection._conv.items():
                     if isinstance(k, int):
                         http_converters[k] = v
 
+            # Make JSON a string for Arrow
+            if 'arrow' in self._results_type:
+                def json_to_str(x: Any) -> Optional[str]:
+                    if x is None:
+                        return None
+                    return json.dumps(x)
+                http_converters[245] = json_to_str
+
+            # Don't convert date/times in polars
+            elif 'polars' in self._results_type:
+                http_converters.pop(7, None)
+                http_converters.pop(10, None)
+                http_converters.pop(12, None)
+
             results = out['results']
 
             # Convert data to Python types
             if results and results[0]:
                 self._row_idx = 0
                 self._result_idx = 0
 
@@ -612,14 +638,15 @@
                                 None, None, prec, scale,
                                 col.get('nullable', False),
                                 flags, charset,
                             ),
                         )
                         pymy_res.append(PyMyField(col['name'], flags, charset))
                     self._descriptions.append(description)
+                    self._schemas.append(get_schema(self._results_type, description))
 
                     rows = convert_rows(result.get('rows', []), convs)
 
                     self._results.append(rows)
                     self._pymy_results.append(pymy_res)
 
             # For compatibility with PyMySQL/MySQLdb
@@ -655,28 +682,32 @@
         if self._connection is None:
             raise ProgrammingError(errno=2048, msg='Connection is closed.')
 
         results = []
         rowcount = 0
         if args is not None and len(args) > 0:
             description = []
+            schema = {}
             # Detect dataframes
             if hasattr(args, 'itertuples'):
                 argiter = args.itertuples(index=False)  # type: ignore
             else:
                 argiter = iter(args)
             for params in argiter:
                 self.execute(query, params)
                 if self._descriptions:
                     description = self._descriptions[-1]
+                if self._schemas:
+                    schema = self._schemas[-1]
                 if self._rows is not None:
                     results.append(self._rows)
                 rowcount += self.rowcount
             self._results = results
             self._descriptions = [description for _ in range(len(results))]
+            self._schemas = [schema for _ in range(len(results))]
         else:
             self.execute(query)
             rowcount += self.rowcount
 
         self.rowcount = rowcount
 
         return self.rowcount
@@ -717,14 +748,15 @@
             return None
         out = self._rows[self._row_idx]
         self._row_idx += 1
         return format_results(
             self._results_type,
             self.description or [],
             out, single=True,
+            schema=self._schema,
         )
 
     def fetchmany(
         self,
         size: Optional[int] = None,
     ) -> Result:
         """
@@ -748,15 +780,18 @@
             return tuple()
         if not size:
             size = max(int(self.arraysize), 1)
         else:
             size = max(int(size), 1)
         out = self._rows[self._row_idx:self._row_idx+size]
         self._row_idx += len(out)
-        return format_results(self._results_type, self.description or [], out)
+        return format_results(
+            self._results_type, self.description or [],
+            out, schema=self._schema,
+        )
 
     def fetchall(self) -> Result:
         """
         Fetch all rows in the result set.
 
         Returns
         -------
@@ -770,15 +805,18 @@
             raise self._connection.ProgrammingError(msg='No query has been submitted')
         if not self._has_row:
             if 'dict' in self._results_type:
                 return {}
             return tuple()
         out = list(self._rows[self._row_idx:])
         self._row_idx = len(out)
-        return format_results(self._results_type, self.description or [], out)
+        return format_results(
+            self._results_type, self.description or [],
+            out, schema=self._schema,
+        )
 
     def nextset(self) -> Optional[bool]:
         """Skip to the next available result set."""
         if self._connection is None:
             raise ProgrammingError(errno=2048, msg='Connection is closed')
 
         if self._result_idx < 0:
```

### Comparing `singlestoredb-1.0.4/singlestoredb/management/billing_usage.py` & `singlestoredb-1.1.0/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/cluster.py` & `singlestoredb-1.1.0/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/manager.py` & `singlestoredb-1.1.0/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/organization.py` & `singlestoredb-1.1.0/singlestoredb/management/organization.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/region.py` & `singlestoredb-1.1.0/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/utils.py` & `singlestoredb-1.1.0/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/management/workspace.py` & `singlestoredb-1.1.0/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/__init__.py` & `singlestoredb-1.1.0/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/_auth.py` & `singlestoredb-1.1.0/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/charset.py` & `singlestoredb-1.1.0/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/connection.py` & `singlestoredb-1.1.0/singlestoredb/mysql/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,36 @@
 from .cursors import (
     Cursor,
     CursorSV,
     DictCursor,
     DictCursorSV,
     NamedtupleCursor,
     NamedtupleCursorSV,
+    ArrowCursor,
+    ArrowCursorSV,
+    NumpyCursor,
+    NumpyCursorSV,
+    PandasCursor,
+    PandasCursorSV,
+    PolarsCursor,
+    PolarsCursorSV,
     SSCursor,
     SSCursorSV,
     SSDictCursor,
     SSDictCursorSV,
     SSNamedtupleCursor,
     SSNamedtupleCursorSV,
+    SSArrowCursor,
+    SSArrowCursorSV,
+    SSNumpyCursor,
+    SSNumpyCursorSV,
+    SSPandasCursor,
+    SSPandasCursorSV,
+    SSPolarsCursor,
+    SSPolarsCursorSV,
 )
 from .optionfile import Parser
 from .protocol import (
     dump_packet,
     MysqlPacket,
     FieldDescriptorPacket,
     OKPacketWrapper,
@@ -439,21 +455,37 @@
         if cursorclass is not None:
             self.cursorclass = cursorclass
         elif buffered:
             if 'dict' in self.results_type:
                 self.cursorclass = DictCursor
             elif 'namedtuple' in self.results_type:
                 self.cursorclass = NamedtupleCursor
+            elif 'numpy' in self.results_type:
+                self.cursorclass = NumpyCursor
+            elif 'arrow' in self.results_type:
+                self.cursorclass = ArrowCursor
+            elif 'pandas' in self.results_type:
+                self.cursorclass = PandasCursor
+            elif 'polars' in self.results_type:
+                self.cursorclass = PolarsCursor
             else:
                 self.cursorclass = Cursor
         else:
             if 'dict' in self.results_type:
                 self.cursorclass = SSDictCursor
             elif 'namedtuple' in self.results_type:
                 self.cursorclass = SSNamedtupleCursor
+            elif 'numpy' in self.results_type:
+                self.cursorclass = SSNumpyCursor
+            elif 'arrow' in self.results_type:
+                self.cursorclass = SSArrowCursor
+            elif 'pandas' in self.results_type:
+                self.cursorclass = SSPandasCursor
+            elif 'polars' in self.results_type:
+                self.cursorclass = SSPolarsCursor
             else:
                 self.cursorclass = SSCursor
 
         if self.pure_python is False and _singlestoredb_accel is None:
             try:
                 import _singlestortedb_accel  # noqa: F401
             except Exception:
@@ -483,28 +515,65 @@
                 self.results_type = 'dicts'
             elif self.cursorclass is NamedtupleCursor:
                 self.cursorclass = NamedtupleCursorSV
                 self.results_type = 'namedtuples'
             elif self.cursorclass is SSNamedtupleCursor:
                 self.cursorclass = SSNamedtupleCursorSV
                 self.results_type = 'namedtuples'
+            elif self.cursorclass is NumpyCursor:
+                self.cursorclass = NumpyCursorSV
+                self.results_type = 'numpy'
+            elif self.cursorclass is SSNumpyCursor:
+                self.cursorclass = SSNumpyCursorSV
+                self.results_type = 'numpy'
+            elif self.cursorclass is ArrowCursor:
+                self.cursorclass = ArrowCursorSV
+                self.results_type = 'arrow'
+            elif self.cursorclass is SSArrowCursor:
+                self.cursorclass = SSArrowCursorSV
+                self.results_type = 'arrow'
+            elif self.cursorclass is PandasCursor:
+                self.cursorclass = PandasCursorSV
+                self.results_type = 'pandas'
+            elif self.cursorclass is SSPandasCursor:
+                self.cursorclass = SSPandasCursorSV
+                self.results_type = 'pandas'
+            elif self.cursorclass is PolarsCursor:
+                self.cursorclass = PolarsCursorSV
+                self.results_type = 'polars'
+            elif self.cursorclass is SSPolarsCursor:
+                self.cursorclass = SSPolarsCursorSV
+                self.results_type = 'polars'
 
         self._result = None
         self._affected_rows = 0
         self.host_info = 'Not connected'
 
         # specified autocommit mode. None means use server default.
         self.autocommit_mode = autocommit
 
         if conv is None:
             conv = converters.conversions
 
+        conv = conv.copy()
+
         self.parse_json = parse_json
         self.invalid_values = (invalid_values or {}).copy()
 
+        # Disable JSON parsing for Arrow
+        if self.results_type in ['arrow']:
+            conv[245] = None
+            self.parse_json = False
+
+        # Disable date/time parsing for polars; let polars do the parsing
+        elif self.results_type in ['polars']:
+            conv[7] = None
+            conv[10] = None
+            conv[12] = None
+
         # Need for MySQLdb compatibility.
         self.encoders = {k: v for (k, v) in conv.items() if type(k) is not int}
         self.decoders = {k: v for (k, v) in conv.items() if type(k) is int}
         self.sql_mode = sql_mode
         self.init_command = init_command
         self.max_allowed_packet = max_allowed_packet
         self._auth_plugin_map = auth_plugin_map or {}
```

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.1.0/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.1.0/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.1.0/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.1.0/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/converters.py` & `singlestoredb-1.1.0/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/err.py` & `singlestoredb-1.1.0/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.1.0/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/protocol.py` & `singlestoredb-1.1.0/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/pytest.py` & `singlestoredb-1.1.0/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test.sql` & `singlestoredb-1.1.0/singlestoredb/tests/test.sql`

 * *Files 22% similar despite different names*

```diff
@@ -359,14 +359,224 @@
     `json`='{}',
     `enum`='one',
     `set`='two',
     `bit`=0
 ;
 
 
+CREATE TABLE IF NOT EXISTS alltypes_no_nulls (
+    `id` INT(11) NOT NULL,
+    `tinyint` TINYINT NOT NULL,
+    `unsigned_tinyint` TINYINT UNSIGNED NOT NULL,
+    `bool` BOOL NOT NULL,
+    `boolean` BOOLEAN NOT NULL,
+    `smallint` SMALLINT NOT NULL,
+    `unsigned_smallint` SMALLINT UNSIGNED NOT NULL,
+    `mediumint` MEDIUMINT NOT NULL,
+    `unsigned_mediumint` MEDIUMINT UNSIGNED NOT NULL,
+    `int24` MEDIUMINT NOT NULL,
+    `unsigned_int24` MEDIUMINT UNSIGNED NOT NULL,
+    `int` INT NOT NULL,
+    `unsigned_int` INT UNSIGNED NOT NULL,
+    `integer` INTEGER NOT NULL,
+    `unsigned_integer` INTEGER UNSIGNED NOT NULL,
+    `bigint` BIGINT NOT NULL,
+    `unsigned_bigint` BIGINT UNSIGNED NOT NULL,
+    `float` FLOAT NOT NULL,
+    `double` DOUBLE NOT NULL,
+    `real` REAL NOT NULL,
+    `decimal` DECIMAL(20,6) NOT NULL,
+    `dec` DEC(20,6) NOT NULL,
+    `fixed` FIXED(20,6) NOT NULL,
+    `numeric` NUMERIC(20,6) NOT NULL,
+    `date` DATE NOT NULL,
+    `time` TIME NOT NULL,
+    `time_6` TIME(6) NOT NULL,
+    `datetime` DATETIME NOT NULL,
+    `datetime_6` DATETIME(6) NOT NULL,
+    `timestamp` TIMESTAMP NOT NULL,
+    `timestamp_6` TIMESTAMP(6) NOT NULL,
+    `year` YEAR NOT NULL,
+    `char_100` CHAR(100) NOT NULL,
+    `binary_100` BINARY(100) NOT NULL,
+    `varchar_200` VARCHAR(200) NOT NULL,
+    `varbinary_200` VARBINARY(200) NOT NULL,
+    `longtext` LONGTEXT NOT NULL,
+    `mediumtext` MEDIUMTEXT NOT NULL,
+    `text` TEXT NOT NULL,
+    `tinytext` TINYTEXT NOT NULL,
+    `longblob` LONGBLOB NOT NULL,
+    `mediumblob` MEDIUMBLOB NOT NULL,
+    `blob` BLOB NOT NULL,
+    `tinyblob` TINYBLOB NOT NULL,
+    `json` JSON NOT NULL,
+--  `geographypoint` GEOGRAPHYPOINT NOT NULL,
+--  `geography` GEOGRAPHY NOT NULL,
+    `enum` ENUM('one', 'two', 'three') NOT NULL,
+    `set` SET('one', 'two', 'three') NOT NULL,
+    `bit` BIT NOT NULL
+)
+COLLATE='utf8_unicode_ci';
+
+INSERT INTO alltypes_no_nulls SET
+    `id`=0,
+    `tinyint`=80,
+    `unsigned_tinyint`=85,
+    `bool`=0,
+    `boolean`=1,
+    `smallint`=-27897,
+    `unsigned_smallint`=27897,
+    `mediumint`=104729,
+    `unsigned_mediumint`=120999,
+    `int24`=-200899,
+    `unsigned_int24`=407709,
+    `int`=-1295369311,
+    `unsigned_int`=3872362332,
+    `integer`=-1741727421,
+    `unsigned_integer`=3198387363,
+    `bigint`=-266883847,
+    `unsigned_bigint`=980007287362,
+    `float`=-146486683.754744,
+    `double`=-474646154.719356,
+    `real`=-901409776.279346,
+    `decimal`=28111097.610822,
+    `dec`=389451155.931428,
+    `fixed`=-143773416.044092,
+    `numeric`=866689461.300046,
+    `date`='8524-11-10',
+    `time`='00:07:00',
+    `time_6`='01:10:00.000002',
+    `datetime`='9948-03-11 15:29:22',
+    `datetime_6`='1756-10-29 02:02:42.000008',
+    `timestamp`='1980-12-31 01:10:23',
+    `timestamp_6`='1991-01-02 22:15:10.000006',
+    `year`=1923,
+    `char_100`='This is a test of a 100 character column.',
+    `binary_100`=x'000102030405060708090A0B0C0D0E0F',
+    `varchar_200`='This is a test of a variable character column.',
+    `varbinary_200`=x'000102030405060708090A0B0C0D0E0F000102030405060708090A0B0C0D0E0F',
+    `longtext`='This is a longtext column.',
+    `mediumtext`='This is a mediumtext column.',
+    `text`='This is a text column.',
+    `tinytext`='This is a tinytext column.',
+    `longblob`=x'000102030405060708090A0B0C0D0E0F000102030405060708090A0B0C0D0E0F000102030405060708090A0B0C0D0E0F',
+    `mediumblob`=x'000102030405060708090A0B0C0D0E0F000102030405060708090A0B0C0D0E0F',
+    `blob`=x'000102030405060708090A0B0C0D0E0F',
+    `tinyblob`=x'0A0B0C0D0E0F',
+    `json`='{"a": 10, "b": 2.75, "c": "hello world"}',
+    `enum`='one',
+    `set`='two',
+    `bit`=128
+;
+
+-- Minimum values
+INSERT INTO alltypes_no_nulls SET
+    `id`=2,
+    `tinyint`=-128,
+    `unsigned_tinyint`=0,
+    `bool`=-128,
+    `boolean`=-128,
+    `smallint`=-32768,
+    `unsigned_smallint`=0,
+    `mediumint`=-8388608,
+    `unsigned_mediumint`=0,
+    `int24`=-8388608,
+    `unsigned_int24`=0,
+    `int`=-2147483648,
+    `unsigned_int`=0,
+    `integer`=-2147483648,
+    `unsigned_integer`=0,
+    `bigint`=-9223372036854775808,
+    `unsigned_bigint`=0,
+    `float`=0,
+    `double`=-1.7976931348623158e308,
+    `real`=-1.7976931348623158e308,
+    `decimal`=-99999999999999.999999,
+    `dec`=-99999999999999.999999,
+    `fixed`=-99999999999999.999999,
+    `numeric`=-99999999999999.999999,
+    `date`='1000-01-01',
+    `time`='-838:59:59',
+    `time_6`='-838:59:59.000000',
+    `datetime`='1000-01-01 00:00:00',
+    `datetime_6`='1000-01-01 00:00:00.000000',
+    `timestamp`='1970-01-01 00:00:01',
+    `timestamp_6`='1970-01-01 00:00:01.000000',
+    `year`=1901,
+    `char_100`='',
+    `binary_100`=x'',
+    `varchar_200`='',
+    `varbinary_200`=x'',
+    `longtext`='',
+    `mediumtext`='',
+    `text`='',
+    `tinytext`='',
+    `longblob`=x'',
+    `mediumblob`=x'',
+    `blob`=x'',
+    `tinyblob`=x'',
+    `json`='{}',
+    `enum`='one',
+    `set`='two',
+    `bit`=0
+;
+
+-- Maximum values
+INSERT INTO alltypes_no_nulls SET
+    `id`=3,
+    `tinyint`=127,
+    `unsigned_tinyint`=255,
+    `bool`=127,
+    `boolean`=127,
+    `smallint`=32767,
+    `unsigned_smallint`=65535,
+    `mediumint`=8388607,
+    `unsigned_mediumint`=16777215,
+    `int24`=8388607,
+    `unsigned_int24`=16777215,
+    `int`=2147483647,
+    `unsigned_int`=4294967295,
+    `integer`=2147483647,
+    `unsigned_integer`=4294967295,
+    `bigint`=9223372036854775807,
+    `unsigned_bigint`=18446744073709551615,
+    `float`=0,
+    `double`=1.7976931348623158e308,
+    `real`=1.7976931348623158e308,
+    `decimal`=99999999999999.999999,
+    `dec`=99999999999999.999999,
+    `fixed`=99999999999999.999999,
+    `numeric`=99999999999999.999999,
+    `date`='9999-12-31',
+    `time`='838:59:59',
+    `time_6`='838:59:59.999999',
+    `datetime`='9999-12-31 23:59:59',
+    `datetime_6`='9999-12-31 23:59:59.999999',
+    `timestamp`='2038-01-18 21:14:07',
+    `timestamp_6`='2038-01-18 21:14:07.999999',
+    `year`=2155,
+    `char_100`='',
+    `binary_100`=x'',
+    `varchar_200`='',
+    `varbinary_200`=x'',
+    `longtext`='',
+    `mediumtext`='',
+    `text`='',
+    `tinytext`='',
+    `longblob`=x'',
+    `mediumblob`=x'',
+    `blob`=x'',
+    `tinyblob`=x'',
+    `json`='{}',
+    `enum`='one',
+    `set`='two',
+    `bit`=18446744073709551615
+;
+
+
 --
 -- Table of extended data types
 --
 CREATE ROWSTORE TABLE IF NOT EXISTS `extended_types` (
     `id` INT(11),
     `geography` GEOGRAPHY,
     `geographypoint` GEOGRAPHYPOINT,
```

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_basics.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_config.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_ext_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import requests
 
 import singlestoredb as s2
 import singlestoredb.mysql.constants.FIELD_TYPE as ft
 from . import ext_funcs
 from . import utils
-from singlestoredb.functions.ext import create_app
+from singlestoredb.functions.ext.asgi import create_app
 
 
 try:
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.connect(('8.8.8.8', 80))
     HTTP_HOST = s.getsockname()[0]
 except Exception:
@@ -37,15 +37,15 @@
 
 
 def start_http_server(database, data_format='rowdat_1'):
     """Start an external function server."""
     port = get_open_port()
     print(f'Start UDF HTTP server on http://{HTTP_HOST}:{port}')
     proc = subprocess.Popen(
-        ['uvicorn', 'singlestoredb.functions.ext:create_app'],
+        ['uvicorn', 'singlestoredb.functions.ext.asgi:create_app'],
         env=dict(
             PATH=os.environ['PATH'],
             PYTHONPATH=os.environ.get('PYTHONPATH', ''),
             UVICORN_HOST=str(HTTP_HOST),
             UVICORN_PORT=str(port),
             UVICORN_FACTORY='1',
             SINGLESTOREDB_EXT_FUNCTIONS='singlestoredb.tests.ext_funcs',
```

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_ext_func_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 polars_int24_arr = \
     pl.Series(None, numpy_int24_arr, dtype=pl.Int32)
 polars_unsigned_int24_arr = \
     pl.Series(None, numpy_unsigned_int24_arr, dtype=pl.UInt32)
 polars_string_arr = \
     pl.Series(None, numpy_string_arr.tolist(), dtype=pl.Utf8)
 polars_binary_arr = \
-    pl.Series(None, numpy_binary_arr.tolist(), dtype=pl.Utf8)
+    pl.Series(None, numpy_binary_arr.tolist(), dtype=pl.Binary)
 
 polars_data = [
     (polars_tiny_arr, polars_nulls),
     (polars_unsigned_tiny_arr, polars_nulls),
     (polars_short_arr, polars_nulls),
     (polars_unsigned_short_arr, polars_nulls),
     (polars_long_arr, polars_nulls),
```

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_http.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_management.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_results.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_types.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_udf.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.1.0/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/tests/utils.py` & `singlestoredb-1.1.0/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/types.py` & `singlestoredb-1.1.0/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/utils/config.py` & `singlestoredb-1.1.0/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.1.0/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/utils/mogrify.py` & `singlestoredb-1.1.0/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb/utils/xdict.py` & `singlestoredb-1.1.0/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.4/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.1.0/singlestoredb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.4
+Version: 1.1.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.4/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.1.0/singlestoredb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 singlestoredb/functions/signature.py
 singlestoredb/functions/ext/__init__.py
 singlestoredb/functions/ext/arrow.py
 singlestoredb/functions/ext/asgi.py
 singlestoredb/functions/ext/json.py
 singlestoredb/functions/ext/mmap.py
 singlestoredb/functions/ext/rowdat_1.py
+singlestoredb/functions/ext/utils.py
 singlestoredb/fusion/__init__.py
 singlestoredb/fusion/graphql.py
 singlestoredb/fusion/handler.py
 singlestoredb/fusion/registry.py
 singlestoredb/fusion/result.py
 singlestoredb/fusion/handlers/__init__.py
 singlestoredb/fusion/handlers/stage.py
@@ -108,10 +109,11 @@
 singlestoredb/tests/test_xdict.py
 singlestoredb/tests/utils.py
 singlestoredb/tests/ext_funcs/__init__.py
 singlestoredb/utils/__init__.py
 singlestoredb/utils/config.py
 singlestoredb/utils/convert_rows.py
 singlestoredb/utils/debug.py
+singlestoredb/utils/dtypes.py
 singlestoredb/utils/mogrify.py
 singlestoredb/utils/results.py
 singlestoredb/utils/xdict.py
```

