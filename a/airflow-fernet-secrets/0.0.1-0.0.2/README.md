# Comparing `tmp/airflow_fernet_secrets-0.0.1.tar.gz` & `tmp/airflow_fernet_secrets-0.0.2.tar.gz`

## Comparing `airflow_fernet_secrets-0.0.1.tar` & `airflow_fernet_secrets-0.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/ruff.toml
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/.github/workflows/check.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/get_provider_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/operators/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/operators/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/secrets/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow/providers/fernet_secrets/secrets/secret_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/_typeshed.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/const.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/dynamic.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/exceptions.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/info.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/info.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/__init__.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/client.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/common.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/server.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/client.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/common.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/server.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/main.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/odbc.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/postgresql.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/json/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/json/class_to_tuple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/__init__.py
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/connect.py
--rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/revision/__init__.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/revision/init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/client.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/common.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/server.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/__init__.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/base.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/dump.py
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/client.py
--rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/common.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/utils/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/utils/cast.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/utils/re.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/base.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/test_dump.py
--rw-r--r--   0        0        0    23820 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/test_operator.py
--rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/tests/test_secrets_manager.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/LICENSE
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/README.md
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    15088 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/ruff.toml
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/get_provider_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/operators/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/operators/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/secrets/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow/providers/fernet_secrets/secrets/secret_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/_typeshed.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/const.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/dynamic.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/exceptions.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/info.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/info.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/__init__.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/client.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/common.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/server.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/client.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/common.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/server.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/main.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/odbc.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/postgresql.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/json/__init__.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/json/class_to_tuple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/__init__.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/connect.py
+-rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/revision/__init__.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/revision/init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/client.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/common.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/server.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/__init__.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/base.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/dump.py
+-rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/client.py
+-rw-r--r--   0        0        0    20916 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/common.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/utils/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/utils/cast.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/utils/re.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/base.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/test_dump.py
+-rw-r--r--   0        0        0    23820 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/test_operator.py
+-rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/tests/test_secrets_manager.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/README.md
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15088 2020-02-02 00:00:00.000000 airflow_fernet_secrets-0.0.2/PKG-INFO
```

### Comparing `airflow_fernet_secrets-0.0.1/ruff.toml` & `airflow_fernet_secrets-0.0.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/.github/workflows/check.yaml` & `airflow_fernet_secrets-0.0.2/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/.github/workflows/publish.yaml` & `airflow_fernet_secrets-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/const.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 LOGGER_NAME = "airflow.fernet_secrets"
 
 SQL_CONN_TYPE = "sql"
 SA_DATACLASS_METADATA_KEY = "sa"
 
 JSONABLE_CLASS_TYPE_FLAG = "_jsonable_class_type_flag_"
+CONNECTION_BEGIN_INFO_KEY = "is_begin_immediate"
 
 # connection type
 SQLITE_CONN_TYPE = "sqlite"
 SQLITE_CONN_TYPES = frozenset({SQLITE_CONN_TYPE, "sqlite"})
 POSTGRESQL_CONN_TYPE = "postgresql"
 POSTGRESQL_CONN_TYPES = frozenset({POSTGRESQL_CONN_TYPE, "postgres", "postgresql"})
 ODBC_CONN_TYPE = "odbc"
```

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/dynamic.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/dynamic.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/exceptions.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/exceptions.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/info.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/info.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/info.yaml` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/info.yaml`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/client.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/client.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/common.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/common.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/config/server.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/config/server.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/client.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/client.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/common.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/common.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/server.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 
 def convert_connection_to_dict(connection: Connection) -> ConnectionDict:
     """airflow connection to connection dict"""
     from airflow_fernet_secrets.connection.dump import connection_to_args
 
-    as_dict = connection.to_dict()
+    as_dict = _connection_to_dict(connection)
 
     conn_type = _get_conn_type(connection)
     args = connection_to_args(connection) if is_sql_connection(connection) else None
     result: ConnectionDict = {
         "conn_type": conn_type,
         "extra": as_dict["extra"],
         "args": args,
@@ -72,7 +72,28 @@
         return False
     hook_class = import_string(hook_info.hook_class_name)
     return callable(getattr(hook_class, "get_sqlalchemy_engine", None))
 
 
 def _get_conn_type(connection: Connection) -> str:
     return cast(str, connection.conn_type)
+
+
+def _connection_to_dict(connection: Connection) -> dict[str, Any]:
+    """obtained from airflow.models.Connection.to_dict"""
+    if callable(getattr(connection, "to_dict", None)):
+        return connection.to_dict()
+
+    as_dict = {
+        "conn_id": connection.conn_id,
+        "conn_type": connection.conn_type,
+        "description": connection.description,
+        "host": connection.host,
+        "login": connection.login,
+        "password": connection.password,
+        "schema": connection.schema,
+        "port": connection.port,
+    }
+    as_dict = {key: value for key, value in as_dict.items() if value is not None}
+    as_dict["extra"] = connection.extra_dejson
+    json.dumps(as_dict)
+    return as_dict
```

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/main.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/main.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/odbc.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/odbc.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/postgresql.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/postgresql.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/dump/sqlite.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/dump/sqlite.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/connection/json/class_to_tuple.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/connection/json/class_to_tuple.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/connect.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Callable,
     Generator,
     Protocol,
     overload,
     runtime_checkable,
 )
 
-import sqlalchemy as sa
 from sqlalchemy.dialects.sqlite import dialect as sqlite_dialect
 from sqlalchemy.engine import Connection, Engine, create_engine
 from sqlalchemy.engine.url import URL, make_url
 from sqlalchemy.event import listen
 from sqlalchemy.ext.asyncio import (
     AsyncConnection,
     AsyncEngine,
@@ -259,31 +258,25 @@
         await session.close()
 
 
 def _is_async_dialect(dialect: type[Dialect] | Dialect) -> bool:
     return getattr(dialect, "is_async", False) is True
 
 
-def _sqlite_isolation_read(
+def _sqlite_busy_timeout(
     dbapi_connection: _DBAPIConnection,
     connection_record: Any,  # noqa: ARG001
 ) -> None:
     cursor = dbapi_connection.cursor()
-    cursor.execute("PRAGMA read_uncommitted = true;", ())
-
-
-def _sqlite_isolation_non_read(conn: Connection) -> None:
-    stmt = sa.text("PRAGMA read_uncommitted = false;")
-    conn.execute(stmt)
+    cursor.execute("PRAGMA busy_timeout = 10000;", ())
 
 
 @overload
 def _set_listeners(engine: Engine) -> Engine: ...
 @overload
 def _set_listeners(engine: AsyncEngine) -> AsyncEngine: ...
 @overload
 def _set_listeners(engine: Engine | AsyncEngine) -> Engine | AsyncEngine: ...
 def _set_listeners(engine: Engine | AsyncEngine) -> Engine | AsyncEngine:
     sync_engine = engine.sync_engine if isinstance(engine, AsyncEngine) else engine
-    listen(sync_engine, "connect", _sqlite_isolation_read)
-    listen(sync_engine, "begin", _sqlite_isolation_non_read)
+    listen(sync_engine, "connect", _sqlite_busy_timeout)
     return engine
```

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/model.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/model.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/database/revision/init.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/database/revision/init.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/common.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/common.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/log/server.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/log/server.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/base.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/base.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/dump.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/dump.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/operators/load.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/operators/load.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/client.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/client.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/common.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import json
 from abc import ABC, abstractmethod
-from contextlib import asynccontextmanager, contextmanager
+from contextlib import asynccontextmanager, contextmanager, suppress
 from functools import cached_property
 from typing import TYPE_CHECKING, AsyncGenerator, Generator, Generic, Literal, cast
 
 import sqlalchemy as sa
+from sqlalchemy.exc import ResourceClosedError
 from typing_extensions import TypeVar, override
 
 from airflow_fernet_secrets.config.common import ensure_fernet
+from airflow_fernet_secrets.const import CONNECTION_BEGIN_INFO_KEY
 from airflow_fernet_secrets.database.connect import (
     create_sqlite_url,
     ensure_sqlite_async_engine,
     ensure_sqlite_sync_engine,
     enter_async_database,
     enter_sync_database,
 )
@@ -250,29 +252,29 @@
         value = self.serialize_connection(conn_id, connection)
         await self.aset_conn_value(conn_id=conn_id, conn_type=conn_type, value=value)
 
     def delete_connection(self, conn_id: str) -> None:
         """delete connection in backend"""
         secret_key = self._secret()
         with enter_sync_database(self._backend_sync_engine) as session:
-            value = FernetConnection.get(session, conn_id)
-            if value is None:
-                return
             with _sync_transact(session):
+                value = FernetConnection.get(session, conn_id)
+                if value is None:
+                    return
                 value.delete(session, secret_key=secret_key)
                 session.commit()
 
     async def adelete_connection(self, conn_id: str) -> None:
         """delete connection in backend"""
         secret_key = self._secret()
         async with enter_async_database(self._backend_async_engine) as session:
-            value = await FernetConnection.aget(session, conn_id)
-            if value is None:
-                return
             async with _async_transact(session):
+                value = await FernetConnection.aget(session, conn_id)
+                if value is None:
+                    return
                 await value.adelete(session, secret_key=secret_key)
                 await session.commit()
 
     @override
     def get_variable(self, key: str) -> str | None:
         with enter_sync_database(self._backend_sync_engine) as session:
             value = FernetVariable.get(session, key)
@@ -294,57 +296,57 @@
         fernet = self._secret()
         return FernetVariable.decrypt(value.encrypted, fernet)
 
     def set_variable(self, key: str, value: str) -> None:
         """set variable to backend"""
         secret_key = self._secret()
         with enter_sync_database(self._backend_sync_engine) as session:
-            as_bytes = FernetVariable.encrypt(value, secret_key)
-            variable = FernetVariable.get(session, key)
-            if variable is None:
-                variable = FernetVariable(encrypted=as_bytes, key=key)
-            else:
-                variable.encrypted = as_bytes
             with _sync_transact(session):
+                as_bytes = FernetVariable.encrypt(value, secret_key)
+                variable = FernetVariable.get(session, key)
+                if variable is None:
+                    variable = FernetVariable(encrypted=as_bytes, key=key)
+                else:
+                    variable.encrypted = as_bytes
                 variable.upsert(session, secret_key=secret_key)
                 session.commit()
 
     async def aset_variable(self, key: str, value: str) -> None:
         """set variable to backend"""
         secret_key = self._secret()
         async with enter_async_database(self._backend_async_engine) as session:
-            as_bytes = FernetVariable.encrypt(value, secret_key)
-            variable = await FernetVariable.aget(session, key)
-            if variable is None:
-                variable = FernetVariable(encrypted=as_bytes, key=key)
-            else:
-                variable.encrypted = as_bytes
             async with _async_transact(session):
+                as_bytes = FernetVariable.encrypt(value, secret_key)
+                variable = await FernetVariable.aget(session, key)
+                if variable is None:
+                    variable = FernetVariable(encrypted=as_bytes, key=key)
+                else:
+                    variable.encrypted = as_bytes
                 await variable.aupsert(session, secret_key=secret_key)
                 await session.commit()
 
     def delete_variable(self, key: str) -> None:
         """delete variable to backend"""
         secret_key = self._secret()
         with enter_sync_database(self._backend_sync_engine) as session:
-            variable = FernetVariable.get(session, key=key)
-            if variable is None:
-                return
             with _sync_transact(session):
+                variable = FernetVariable.get(session, key=key)
+                if variable is None:
+                    return
                 variable.delete(session, secret_key=secret_key)
                 session.commit()
 
     async def adelete_variable(self, key: str) -> None:
         """delete variable to backend"""
         secret_key = self._secret()
         async with enter_async_database(self._backend_async_engine) as session:
-            variable = await FernetVariable.aget(session, key=key)
-            if variable is None:
-                return
             async with _async_transact(session):
+                variable = await FernetVariable.aget(session, key=key)
+                if variable is None:
+                    return
                 await variable.adelete(session, secret_key=secret_key)
                 await session.commit()
 
     def has_variable(self, key: str) -> bool:
         """check has variable"""
         with enter_sync_database(self._backend_sync_engine) as session:
             count: int = session.scalar(
@@ -509,24 +511,32 @@
     @abstractmethod
     def _get_conn_type(self, connection: ConnectionT) -> str: ...
 
 
 @contextmanager
 def _sync_transact(session: Session) -> Generator[Session, None, None]:
     conn = session.connection()
-    if conn.in_transaction() or conn.in_nested_transaction():
-        func = conn.begin_nested
-    else:
-        func = conn.begin
-    with func():
+    is_begin = conn.info.get(CONNECTION_BEGIN_INFO_KEY, False)
+    if is_begin is False:
+        conn.execute(sa.text("BEGIN IMMEDIATE;"))
+        conn.info[CONNECTION_BEGIN_INFO_KEY] = True
+
+    try:
         yield session
+    finally:
+        with suppress(ResourceClosedError):
+            conn.info[CONNECTION_BEGIN_INFO_KEY] = False
 
 
 @asynccontextmanager
 async def _async_transact(session: AsyncSession) -> AsyncGenerator[AsyncSession, None]:
     conn = await session.connection()
-    if conn.in_transaction() or conn.in_nested_transaction():
-        func = conn.begin_nested
-    else:
-        func = conn.begin
-    async with func():
+    is_begin = conn.info.get(CONNECTION_BEGIN_INFO_KEY, False)
+    if is_begin is False:
+        await conn.execute(sa.text("BEGIN IMMEDIATE;"))
+        conn.info[CONNECTION_BEGIN_INFO_KEY] = True
+
+    try:
         yield session
+    finally:
+        with suppress(ResourceClosedError):
+            conn.info[CONNECTION_BEGIN_INFO_KEY] = False
```

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/secrets/server.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/secrets/server.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/utils/cast.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/utils/cast.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/src/airflow_fernet_secrets/utils/re.py` & `airflow_fernet_secrets-0.0.2/src/airflow_fernet_secrets/utils/re.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/tests/base.py` & `airflow_fernet_secrets-0.0.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/tests/conftest.py` & `airflow_fernet_secrets-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/tests/test_dump.py` & `airflow_fernet_secrets-0.0.2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/tests/test_operator.py` & `airflow_fernet_secrets-0.0.2/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/tests/test_secrets_manager.py` & `airflow_fernet_secrets-0.0.2/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/.gitignore` & `airflow_fernet_secrets-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/LICENSE` & `airflow_fernet_secrets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/README.md` & `airflow_fernet_secrets-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_fernet_secrets-0.0.1/pyproject.toml` & `airflow_fernet_secrets-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "airflow-fernet-secrets"
-version = "0.0.1"
+version = "0.0.2"
 description = "airflow filesystem secret backend using fernet"
 authors = [{ name = "phi", email = "phi.friday@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Apache Airflow",
```

### Comparing `airflow_fernet_secrets-0.0.1/PKG-INFO` & `airflow_fernet_secrets-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: airflow-fernet-secrets
-Version: 0.0.1
+Version: 0.0.2
 Summary: airflow filesystem secret backend using fernet
 Project-URL: Repository, https://github.com/phi-friday/airflow-fernet-secrets
 Author-email: phi <phi.friday@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

