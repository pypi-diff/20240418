# Comparing `tmp/pytest_databases-0.2.5.tar.gz` & `tmp/pytest_databases-0.3.0.tar.gz`

## Comparing `pytest_databases-0.2.5.tar` & `pytest_databases-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,62 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/CODEOWNERS
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/Makefile
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/sonar-project.properties
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0     9412 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/docker-compose.yml
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/elastic_search.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/__init__.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_elasticsearch.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/LICENSE
--rw-r--r--   0        0        0    12199 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/README.md
--rw-r--r--   0        0        0    17239 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    14209 2020-02-02 00:00:00.000000 pytest_databases-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/CODEOWNERS
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/Makefile
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/sonar-project.properties
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/alloydb_omni.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.keydb.yml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.mariadb.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.mssql.yml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.oracle.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.postgres.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.redis.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/docker-compose.spanner.yml
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/elastic_search.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_alloydb_omni.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_elasticsearch.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/README.md
+-rw-r--r--   0        0        0    17357 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 pytest_databases-0.3.0/PKG-INFO
```

### Comparing `pytest_databases-0.2.5/.pre-commit-config.yaml` & `pytest_databases-0.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ["--fix=auto"] # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
   # Ruff replaces black, flake8, autoflake and isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.3.5" # make sure this is always consistent with hatch configs
+    rev: "v0.3.7" # make sure this is always consistent with hatch configs
     hooks:
       - id: ruff
         args: [--config, ./pyproject.toml]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
```

### Comparing `pytest_databases-0.2.5/.sourcery.yaml` & `pytest_databases-0.3.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/CONTRIBUTING.rst` & `pytest_databases-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/Makefile` & `pytest_databases-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/.vscode/settings.json` & `pytest_databases-0.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/requirements/requirements-dev.txt` & `pytest_databases-0.3.0/requirements/requirements-dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is autogenerated by hatch-pip-compile with Python 3.11
 #
-# [constraints] requirements/requirements-docs.txt (SHA256: 9f7a8dd3e4bc82266beb5962c0cb3e3f2c508a1a44d0bebc5413327ebc29c57c)
+# [constraints] requirements/requirements-docs.txt (SHA256: bc66ec3f548a65764214d7adf74c74992465c90498f84a07b19b829ae70e0bfb)
 #
 # - nodeenv
 # - cython
 # - anyio
 # - coverage[toml]>=6.2
 # - pytest
 # - pytest-cov
@@ -47,34 +47,35 @@
 # - asyncpg>=0.29.0
 # - redis
 # - google-cloud-spanner
 #
 
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   elasticsearch7
     #   elasticsearch8
 aioodbc==0.5.0
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
 anyio==4.3.0
+    # via
+    #   starlette
+    #   watchfiles
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 astroid==3.1.0
     # via pylint
 async-timeout==4.0.3
-    # via
-    #   asyncpg
-    #   redis
+    # via asyncpg
 asyncmy==0.2.9
 asyncpg==0.29.0
     # via asyncpg-stubs
 asyncpg-stubs==0.29.1
 attrs==23.2.0
     # via aiohttp
 auto-pytabs==0.4.0
@@ -106,14 +107,15 @@
 click==8.1.7
     # via
     #   harlequin
     #   pytest-click
     #   rich-click
     #   shandy-sqlfmt
     #   sphinx-click
+    #   uvicorn
 colorama==0.4.6
     # via sphinx-autobuild
 coverage==7.4.4
     # via pytest-cov
 cryptography==42.0.5
     # via
     #   oracledb
@@ -126,33 +128,33 @@
     # via google-cloud-spanner
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
-docutils==0.20.1
+docutils==0.21.1
     # via
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-click
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-toolbox
 domdf-python-tools==3.8.0.post2
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-duckdb==0.10.1
+duckdb==0.10.2
     # via harlequin
 elastic-transport==8.13.0
     # via elasticsearch8
-elasticsearch7==7.17.9
+elasticsearch7==7.9.1
 elasticsearch8==8.13.0
 execnet==2.1.1
     # via pytest-xdist
 filelock==3.13.4
     # via
     #   cachecontrol
     #   sphinx-toolbox
@@ -186,20 +188,22 @@
     #   google-api-core
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpc-interceptor
     #   grpcio-status
 grpcio-status==1.62.1
     # via google-api-core
-harlequin==1.16.2
+h11==0.14.0
+    # via uvicorn
+harlequin==1.17.0
 html5lib==1.1
     # via sphinx-toolbox
 identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
@@ -211,16 +215,14 @@
     # via
     #   shandy-sqlfmt
     #   sphinx
     #   sphinx-jinja2-compat
 linkify-it-py==2.0.3
     # via markdown-it-py
 litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git@c5ce66aadc8f910c24f54bf0d172798c237a67eb
-livereload==2.6.3
-    # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.5
     # via
@@ -242,16 +244,18 @@
 mypy-extensions==1.0.0
     # via mypy
 natsort==8.4.0
     # via domdf-python-tools
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
-    # via pyarrow
-oracledb==2.1.1
+    # via
+    #   harlequin
+    #   pyarrow
+oracledb==2.1.2
 packaging==24.0
     # via
     #   pydata-sphinx-theme
     #   pytest
     #   pytest-sugar
     #   sphinx
 platformdirs==4.2.0
@@ -339,45 +343,43 @@
     # via harlequin
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.3.5
+ruff==0.3.7
     # via auto-pytabs
-setuptools==69.2.0
+setuptools==69.5.1
     # via nodeenv
 shandy-sqlfmt==0.21.2
     # via harlequin
 six==1.16.0
-    # via
-    #   html5lib
-    #   livereload
+    # via html5lib
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.6
     # via
     #   auto-pytabs
     #   autodocsumm
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-autodoc-typehints
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-toolbox
-sphinx-autobuild==2024.2.4
-sphinx-autodoc-typehints==2.0.0
+sphinx-autobuild==2024.4.16
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-click==5.1.0
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
     # via litestar-sphinx-theme
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
@@ -395,16 +397,18 @@
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-mermaid==0.9.2
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via google-cloud-spanner
+starlette==0.37.2
+    # via sphinx-autobuild
 tabulate==0.9.0
     # via sphinx-toolbox
 termcolor==2.4.0
     # via pytest-sugar
 textual==0.49.0
     # via
     #   harlequin
@@ -414,60 +418,69 @@
     # via harlequin
 textual-textarea==0.11.3
     # via harlequin
 tomlkit==0.12.4
     # via
     #   harlequin
     #   pylint
-tornado==6.4
-    # via livereload
 tqdm==4.66.2
     # via shandy-sqlfmt
 tree-sitter==0.20.4
     # via
     #   textual
     #   tree-sitter-languages
 tree-sitter-languages==1.9.1
     # via
     #   textual
     #   textual-textarea
+types-cffi==1.16.0.20240331
+    # via types-pyopenssl
 types-click==7.1.8
 types-decorator==5.1.8.20240310
 types-docutils==0.20.0.20240406
-types-pyopenssl==24.0.0.20240311
+types-pyopenssl==24.0.0.20240417
     # via types-redis
 types-pyyaml==6.0.12.20240311
-types-redis==4.6.0.20240409
+types-redis==4.6.0.20240417
+types-setuptools==69.5.0.20240415
+    # via types-cffi
 types-six==1.16.21.20240311
 typing-extensions==4.11.0
     # via
     #   asyncpg-stubs
     #   domdf-python-tools
     #   mypy
     #   psycopg
     #   pydata-sphinx-theme
     #   rich-click
     #   sphinx-toolbox
     #   textual
 uc-micro-py==1.0.3
     # via linkify-it-py
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   elastic-transport
     #   elasticsearch7
     #   requests
+uvicorn==0.29.0
+    # via sphinx-autobuild
 vcrpy==6.0.1
     # via pytest-vcr
-virtualenv==20.25.1
+virtualenv==20.25.3
     # via pre-commit
+watchfiles==0.21.0
+    # via sphinx-autobuild
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
+websockets==12.0
+    # via sphinx-autobuild
 wrapt==1.16.0
     # via
     #   deprecated
     #   vcrpy
 yarl==1.9.4
     # via
     #   aiohttp
+    #   elasticsearch7
     #   vcrpy
```

### Comparing `pytest_databases-0.2.5/requirements/requirements-docs.txt` & `pytest_databases-0.3.0/requirements/requirements-docs.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,32 +33,33 @@
 # - asyncpg>=0.29.0
 # - redis
 # - google-cloud-spanner
 #
 
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   elasticsearch7
     #   elasticsearch8
 aioodbc==0.5.0
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
 anyio==4.3.0
+    # via
+    #   starlette
+    #   watchfiles
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 async-timeout==4.0.3
-    # via
-    #   asyncpg
-    #   redis
+    # via asyncpg
 asyncmy==0.2.9
 asyncpg==0.29.0
 attrs==23.2.0
     # via aiohttp
 auto-pytabs==0.4.0
 autodocsumm==0.2.12
     # via sphinx-toolbox
@@ -83,28 +84,29 @@
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   pytest-click
     #   sphinx-click
+    #   uvicorn
 colorama==0.4.6
     # via sphinx-autobuild
 coverage==7.4.4
     # via pytest-cov
 cryptography==42.0.5
     # via oracledb
 cssutils==2.10.2
     # via dict2css
 cython==3.0.10
 deprecated==1.2.14
     # via google-cloud-spanner
 dict2css==0.3.0.post1
     # via sphinx-toolbox
-docutils==0.20.1
+docutils==0.21.1
     # via
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-click
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-toolbox
@@ -112,15 +114,15 @@
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 elastic-transport==8.13.0
     # via elasticsearch8
-elasticsearch7==7.17.9
+elasticsearch7==7.9.1
 elasticsearch8==8.13.0
 execnet==2.1.1
     # via pytest-xdist
 filelock==3.13.4
     # via
     #   cachecontrol
     #   sphinx-toolbox
@@ -153,47 +155,47 @@
     #   google-api-core
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpc-interceptor
     #   grpcio-status
 grpcio-status==1.62.1
     # via google-api-core
+h11==0.14.0
+    # via uvicorn
 html5lib==1.1
     # via sphinx-toolbox
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.3
     # via
     #   sphinx
     #   sphinx-jinja2-compat
 litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git@c5ce66aadc8f910c24f54bf0d172798c237a67eb
-livereload==2.6.3
-    # via sphinx-autobuild
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
 msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 natsort==8.4.0
     # via domdf-python-tools
 nodeenv==1.8.0
-oracledb==2.1.1
+oracledb==2.1.2
 packaging==24.0
     # via
     #   pydata-sphinx-theme
     #   pytest
     #   pytest-sugar
     #   sphinx
 platformdirs==4.2.0
@@ -257,43 +259,41 @@
     #   sphinx
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.3.5
+ruff==0.3.7
     # via auto-pytabs
-setuptools==69.2.0
+setuptools==69.5.1
     # via nodeenv
 six==1.16.0
-    # via
-    #   html5lib
-    #   livereload
+    # via html5lib
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.6
     # via
     #   auto-pytabs
     #   autodocsumm
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-autodoc-typehints
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-toolbox
-sphinx-autobuild==2024.2.4
-sphinx-autodoc-typehints==2.0.0
+sphinx-autobuild==2024.4.16
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-click==5.1.0
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
     # via litestar-sphinx-theme
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
@@ -311,38 +311,45 @@
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-mermaid==0.9.2
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via google-cloud-spanner
+starlette==0.37.2
+    # via sphinx-autobuild
 tabulate==0.9.0
     # via sphinx-toolbox
 termcolor==2.4.0
     # via pytest-sugar
-tornado==6.4
-    # via livereload
 typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   psycopg
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   elastic-transport
     #   elasticsearch7
     #   requests
+uvicorn==0.29.0
+    # via sphinx-autobuild
 vcrpy==6.0.1
     # via pytest-vcr
+watchfiles==0.21.0
+    # via sphinx-autobuild
 webencodings==0.5.1
     # via html5lib
+websockets==12.0
+    # via sphinx-autobuild
 wrapt==1.16.0
     # via
     #   deprecated
     #   vcrpy
 yarl==1.9.4
     # via
     #   aiohttp
+    #   elasticsearch7
     #   vcrpy
```

### Comparing `pytest_databases-0.2.5/scripts/__init__.py` & `pytest_databases-0.3.0/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/scripts/build_docs.py` & `pytest_databases-0.3.0/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/src/pytest_databases/__init__.py` & `pytest_databases-0.3.0/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/src/pytest_databases/__metadata__.py` & `pytest_databases-0.3.0/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/src/pytest_databases/helpers.py` & `pytest_databases-0.3.0/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 
 import asyncio
 import os
 import re
 import subprocess  # noqa: S404
 import sys
 import timeit
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 
 import pytest
 
 from pytest_databases.helpers import simple_string_hash, wrap_sync
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable, Generator
+    from pathlib import Path
 
 
 async def wait_until_responsive(
     check: Callable[..., Awaitable],
     timeout: float,
     pause: float,
     **kwargs: Any,
@@ -72,17 +72,17 @@
 
 
 class DockerServiceRegistry:
     def __init__(self, worker_id: str, compose_project_name: str = COMPOSE_PROJECT_NAME) -> None:
         self._running_services: set[str] = set()
         self.docker_ip = self._get_docker_ip()
         self._base_command = ["docker-compose"] if USE_LEGACY_DOCKER_COMPOSE else ["docker", "compose"]
+        self._compose_files: list[str] = []
         self._base_command.extend(
             [
-                f"--file={Path(__file__).parent / 'docker-compose.yml'}",
                 f"--project-name={compose_project_name}-{worker_id}",
             ],
         )
 
     @staticmethod
     def _get_docker_ip() -> str:
         docker_host = os.environ.get("DOCKER_HOST", "").strip()
@@ -92,29 +92,31 @@
         if match := re.match(r"^tcp://(.+?):\d+$", docker_host):
             return match[1]
 
         msg = f'Invalid value for DOCKER_HOST: "{docker_host}".'
         raise ValueError(msg)
 
     def run_command(self, *args: str) -> None:
-        command = [*self._base_command, *args]
+        command = [*self._base_command, *self._compose_files, *args]
         subprocess.run(command, check=True, capture_output=True)
 
     async def start(
         self,
         name: str,
+        docker_compose_files: list[Path],
         *,
         check: Callable[..., Any],
         timeout: float = 30,
         pause: float = 0.1,
         **kwargs: Any,
     ) -> None:
         if SKIP_DOCKER_COMPOSE:
             self._running_services.add(name)
         if name not in self._running_services:
+            self._compose_files = [f"--file={compose_file}" for compose_file in docker_compose_files]
             self.run_command("up", "--force-recreate", "-d", name)
             self._running_services.add(name)
 
         await wait_until_responsive(
             check=wrap_sync(check),
             timeout=timeout,
             pause=pause,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/cockroachdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import psycopg
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -54,25 +55,38 @@
 
 
 @pytest.fixture()
 def cockroachdb_driver_opts() -> dict[str, str]:
     return {"sslmode": "disable"}
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.cockroachdb.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_cockroachdb_service_name() -> str:
+    return "cockroachdb"
+
+
 @pytest.fixture(autouse=False)
 async def cockroachdb_service(
     docker_services: DockerServiceRegistry,
+    default_cockroachdb_service_name: str,
+    docker_compose_files: list[Path],
     cockroachdb_port: int,
     cockroachdb_database: str,
     cockroachdb_driver_opts: dict[str, str],
 ) -> None:
     os.environ["COCKROACHDB_DATABASE"] = cockroachdb_database
     os.environ["COCKROACHDB_PORT"] = str(cockroachdb_port)
     await docker_services.start(
-        "cockroachdb",
+        name=default_cockroachdb_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=60,
         pause=1,
         check=cockroachdb_responsive,
         port=cockroachdb_port,
         database=cockroachdb_database,
         driver_opts=cockroachdb_driver_opts,
     )
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/dragonfly.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from redis.asyncio import Redis as AsyncRedis
 from redis.exceptions import ConnectionError as RedisConnectionError
 
 if TYPE_CHECKING:
@@ -45,11 +46,31 @@
 
 
 @pytest.fixture()
 def dragonfly_port() -> int:
     return 6398
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.dragonfly.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_dragonfly_service_name() -> str:
+    return "dragonfly"
+
+
 @pytest.fixture(autouse=False)
-async def dragonfly_service(docker_services: DockerServiceRegistry, dragonfly_port: int) -> None:
+async def dragonfly_service(
+    docker_services: DockerServiceRegistry,
+    default_dragonfly_service_name: str,
+    docker_compose_files: list[Path],
+    dragonfly_port: int,
+) -> None:
     os.environ["DRAGONFLY_PORT"] = str(dragonfly_port)
-    await docker_services.start("dragonfly", check=dragonfly_responsive, port=dragonfly_port)
+    await docker_services.start(
+        name=default_dragonfly_service_name,
+        docker_compose_files=docker_compose_files,
+        check=dragonfly_responsive,
+        port=dragonfly_port,
+    )
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/elastic_search.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/elastic_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from elasticsearch7 import AsyncElasticsearch as Elasticsearch7
 from elasticsearch7 import AsyncElasticsearch as Elasticsearch8
 
 if TYPE_CHECKING:
@@ -79,47 +80,86 @@
 
 
 @pytest.fixture
 def elasticsearch8_port() -> int:
     return 9201
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.elasticsearch.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_elasticsearch_service_name() -> str:
+    return "elasticsearch8"
+
+
+@pytest.fixture(autouse=False)
 async def elasticsearch7_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     elasticsearch7_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
 ) -> None:
     await docker_services.start(
         "elasticsearch7",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=elasticsearch7_responsive,
         port=elasticsearch7_port,
         database=elasticsearch_database,
         user=elasticsearch_user,
         password=elasticsearch_password,
         scheme=elasticsearch_scheme,
     )
 
 
-@pytest.fixture
+@pytest.fixture(autouse=False)
 async def elasticsearch8_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     elasticsearch8_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
 ) -> None:
     await docker_services.start(
         "elasticsearch8",
+        docker_compose_files=docker_compose_files,
+        timeout=45,
+        pause=1,
+        check=elasticsearch8_responsive,
+        port=elasticsearch8_port,
+        database=elasticsearch_database,
+        user=elasticsearch_user,
+        password=elasticsearch_password,
+        scheme=elasticsearch_scheme,
+    )
+
+
+@pytest.fixture(autouse=False)
+async def elasticsearch_service(
+    docker_services: DockerServiceRegistry,
+    default_elasticsearch_service_name: str,
+    docker_compose_files: list[Path],
+    elasticsearch8_port: int,
+    elasticsearch_database: str,
+    elasticsearch_user: str,
+    elasticsearch_password: str,
+    elasticsearch_scheme: str,
+) -> None:
+    await docker_services.start(
+        name=default_elasticsearch_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=elasticsearch8_responsive,
         port=elasticsearch8_port,
         database=elasticsearch_database,
         user=elasticsearch_user,
         password=elasticsearch_password,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/keydb.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from redis.asyncio import Redis as AsyncRedis
 from redis.exceptions import ConnectionError as RedisConnectionError
 
 if TYPE_CHECKING:
@@ -45,11 +46,31 @@
 
 
 @pytest.fixture()
 def keydb_port() -> int:
     return 6396
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.keydb.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_keydb_service_name() -> str:
+    return "keydb"
+
+
 @pytest.fixture(autouse=False)
-async def keydb_service(docker_services: DockerServiceRegistry, keydb_port: int) -> None:
+async def keydb_service(
+    docker_services: DockerServiceRegistry,
+    default_keydb_service_name: str,
+    docker_compose_files: list[Path],
+    keydb_port: int,
+) -> None:
     os.environ["KEYDB_PORT"] = str(keydb_port)
-    await docker_services.start("keydb", check=keydb_responsive, port=keydb_port)
+    await docker_services.start(
+        name=default_keydb_service_name,
+        docker_compose_files=docker_compose_files,
+        check=keydb_responsive,
+        port=keydb_port,
+    )
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/mariadb.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import contextlib
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import asyncmy
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -78,66 +79,75 @@
 
 @pytest.fixture()
 def mariadb113_port() -> int:
     return 3359
 
 
 @pytest.fixture()
-def mariadb_default_version() -> str:
+def default_mariadb_service_name() -> str:
     return "mariadb113"
 
 
 @pytest.fixture()
 def mariadb_port(mariadb113_port: int) -> int:
     return mariadb113_port
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.mariadb.yml")]
+
+
 @pytest.fixture()
 async def mariadb113_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     mariadb113_port: int,
     mariadb_database: str,
     mariadb_user: str,
     mariadb_password: str,
     mariadb_root_password: str,
 ) -> None:
     os.environ["MARIADB_ROOT_PASSWORD"] = mariadb_root_password
     os.environ["MARIADB_PASSWORD"] = mariadb_password
     os.environ["MARIADB_USER"] = mariadb_user
     os.environ["MARIADB_DATABASE"] = mariadb_database
     os.environ["MARIADB113_PORT"] = str(mariadb113_port)
     await docker_services.start(
         "mariadb113",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mariadb_responsive,
         port=mariadb113_port,
         database=mariadb_database,
         user=mariadb_user,
         password=mariadb_password,
     )
 
 
 @pytest.fixture()
 async def mariadb_service(
     docker_services: DockerServiceRegistry,
-    mariadb_default_version: str,
+    default_mariadb_service_name: str,
+    docker_compose_files: list[Path],
     mariadb_port: int,
     mariadb_database: str,
     mariadb_user: str,
     mariadb_password: str,
     mariadb_root_password: str,
 ) -> None:
     os.environ["MARIADB_ROOT_PASSWORD"] = mariadb_root_password
     os.environ["MARIADB_PASSWORD"] = mariadb_password
     os.environ["MARIADB_USER"] = mariadb_user
     os.environ["MARIADB_DATABASE"] = mariadb_database
-    os.environ[f"{mariadb_default_version.upper()}_PORT"] = str(mariadb_port)
+    os.environ[f"{default_mariadb_service_name.upper()}_PORT"] = str(mariadb_port)
     await docker_services.start(
-        mariadb_default_version,
+        name=default_mariadb_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mariadb_responsive,
         port=mariadb_port,
         database=mariadb_database,
         user=mariadb_user,
         password=mariadb_password,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/mssql.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import asyncio
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import aioodbc
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -66,61 +67,70 @@
 
 @pytest.fixture()
 def mssql2022_port() -> int:
     return 4133
 
 
 @pytest.fixture()
-def mssql_default_version() -> str:
-    return "mssql2022"
-
-
-@pytest.fixture()
 def mssql_port(mssql2022_port: int) -> int:
     return mssql2022_port
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.mssql.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_mssql_service_name() -> str:
+    return "mssql2022"
+
+
 @pytest.fixture(autouse=False)
 async def mssql2022_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     docker_ip: str,
     mssql2022_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
 ) -> None:
     os.environ["MSSQL_PASSWORD"] = mssql_password
     os.environ["MSSQL_USER"] = mssql_user
     os.environ["MSSQL_DATABASE"] = mssql_database
     os.environ["MSSQL2022_PORT"] = str(mssql2022_port)
     connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql2022_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
     await docker_services.start(
         "mssql2022",
+        docker_compose_files=docker_compose_files,
         timeout=120,
         pause=1,
         check=mssql_responsive,
         connstring=connstring,
     )
 
 
 @pytest.fixture(autouse=False)
 async def mssql_service(
     docker_services: DockerServiceRegistry,
+    default_mssql_service_name: str,
+    docker_compose_files: list[Path],
     docker_ip: str,
-    mssql_default_version: str,
     mssql_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
 ) -> None:
     connstring = f"encrypt=no; TrustServerCertificate=yes; driver={{ODBC Driver 18 for SQL Server}}; server={docker_ip},{mssql_port}; database={mssql_database}; UID={mssql_user}; PWD={mssql_password}"
     os.environ["MSSQL_PASSWORD"] = mssql_password
     os.environ["MSSQL_USER"] = mssql_user
     os.environ["MSSQL_DATABASE"] = mssql_database
-    os.environ[f"{mssql_default_version.upper()}_PORT"] = str(mssql_port)
+    os.environ[f"{default_mssql_service_name.upper()}_PORT"] = str(mssql_port)
     await docker_services.start(
-        mssql_default_version,
+        name=default_mssql_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=120,
         pause=1,
         check=mssql_responsive,
         connstring=connstring,
     )
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import contextlib
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import asyncmy
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -83,123 +84,136 @@
 
 @pytest.fixture()
 def mysql57_port() -> int:
     return 3361
 
 
 @pytest.fixture()
-def mysql8_port() -> int:
-    return 3360
+def default_mysql_service_name() -> str:
+    return "mysql8"
 
 
 @pytest.fixture()
-def mysql_default_version() -> str:
-    return "mysql8"
+def mysql8_port() -> int:
+    return 3360
 
 
 @pytest.fixture()
 def mysql_port(mysql8_port: int) -> int:
     return mysql8_port
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.mysql.yml")]
+
+
 @pytest.fixture(autouse=False)
 async def mysql8_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     mysql8_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
 ) -> None:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL8_PORT"] = str(mysql8_port)
     await docker_services.start(
         "mysql8",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql8_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def mysql57_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     mysql57_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
 ) -> None:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL57_PORT"] = str(mysql57_port)
     await docker_services.start(
         "mysql57",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql57_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def mysql56_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     mysql56_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
 ) -> None:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
     os.environ["MYSQL56_PORT"] = str(mysql56_port)
     await docker_services.start(
         "mysql56",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql56_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def mysql_service(
     docker_services: DockerServiceRegistry,
-    mysql_default_version: str,
+    default_mysql_service_name: str,
+    docker_compose_files: list[Path],
     mysql_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
     mysql_root_password: str,
 ) -> None:
     os.environ["MYSQL_ROOT_PASSWORD"] = mysql_root_password
     os.environ["MYSQL_PASSWORD"] = mysql_password
     os.environ["MYSQL_USER"] = mysql_user
     os.environ["MYSQL_DATABASE"] = mysql_database
-    os.environ[f"{mysql_default_version.upper()}_PORT"] = str(mysql_port)
+    os.environ[f"{default_mysql_service_name.upper()}_PORT"] = str(mysql_port)
     await docker_services.start(
-        mysql_default_version,
+        name=default_mysql_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=mysql_responsive,
         port=mysql_port,
         database=mysql_database,
         user=mysql_user,
         password=mysql_password,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/oracle.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import oracledb
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -87,93 +88,104 @@
 
 @pytest.fixture()
 def oracle23c_port() -> int:
     return 1513
 
 
 @pytest.fixture()
-def oracle_default_version() -> str:
+def default_oracle_service_name() -> str:
     return "oracle23c"
 
 
 @pytest.fixture()
 def oracle_port(oracle23c_port: int) -> int:
     return oracle23c_port
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.oracle.yml")]
+
+
 @pytest.fixture(autouse=False)
 async def oracle23c_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     oracle23c_port: int,
     oracle23c_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
 ) -> None:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE23C_SERVICE_NAME"] = oracle23c_service_name
     os.environ["ORACLE23C_PORT"] = str(oracle23c_port)
     await docker_services.start(
         "oracle23c",
+        docker_compose_files=docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle23c_port,
         service_name=oracle23c_service_name,
         user=oracle_user,
         password=oracle_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def oracle18c_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     oracle18c_port: int,
     oracle18c_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
 ) -> None:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE18C_SERVICE_NAME"] = oracle18c_service_name
     os.environ["ORACLE18C_PORT"] = str(oracle18c_port)
     await docker_services.start(
         "oracle18c",
+        docker_compose_files=docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle18c_port,
         service_name=oracle18c_service_name,
         user=oracle_user,
         password=oracle_password,
     )
 
 
 # alias to the latest
 @pytest.fixture(autouse=False)
 async def oracle_service(
     docker_services: DockerServiceRegistry,
-    oracle_default_version: str,
+    default_oracle_service_name: str,
+    docker_compose_files: list[Path],
     oracle_port: int,
     oracle_service_name: str,
     oracle_system_password: str,
     oracle_user: str,
     oracle_password: str,
 ) -> None:
     os.environ["ORACLE_PASSWORD"] = oracle_password
     os.environ["ORACLE_SYSTEM_PASSWORD"] = oracle_system_password
     os.environ["ORACLE_USER"] = oracle_user
     os.environ["ORACLE_SERVICE_NAME"] = oracle_service_name
-    os.environ[f"{oracle_default_version.upper()}_PORT"] = str(oracle_port)
+    os.environ[f"{default_oracle_service_name.upper()}_PORT"] = str(oracle_port)
     await docker_services.start(
-        oracle_default_version,
+        name=default_oracle_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=90,
         pause=1,
         check=oracle_responsive,
         port=oracle_port,
         service_name=oracle_service_name,
         user=oracle_user,
         password=oracle_password,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/postgres.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import asyncpg
 import pytest
 
 if TYPE_CHECKING:
     from pytest_databases.docker import DockerServiceRegistry
@@ -94,159 +95,176 @@
 
 @pytest.fixture()
 def postgres16_port() -> int:
     return 5427
 
 
 @pytest.fixture()
-def postgres_default_version() -> str:
+def default_postgres_service_name() -> str:
     return "postgres16"
 
 
 @pytest.fixture()
 def postgres_port(postgres16_port: int) -> int:
     return postgres16_port
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.postgres.yml")]
+
+
 @pytest.fixture(autouse=False)
 async def postgres12_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     postgres12_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES12_PORT"] = str(postgres12_port)
     await docker_services.start(
         "postgres12",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres12_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def postgres13_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     postgres13_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES13_PORT"] = str(postgres13_port)
     await docker_services.start(
         "postgres13",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres13_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def postgres14_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     postgres14_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES14_PORT"] = str(postgres14_port)
     await docker_services.start(
         "postgres14",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres14_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def postgres15_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     postgres15_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES15_PORT"] = str(postgres15_port)
     await docker_services.start(
         "postgres15",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres15_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
 
 
 @pytest.fixture(autouse=False)
 async def postgres16_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     postgres16_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
     os.environ["POSTGRES16_PORT"] = str(postgres16_port)
     await docker_services.start(
         "postgres16",
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres16_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
     )
 
 
 # alias to the latest
 @pytest.fixture(autouse=False)
 async def postgres_service(
     docker_services: DockerServiceRegistry,
-    postgres_default_version: str,
+    default_postgres_service_name: str,
+    docker_compose_files: list[Path],
     postgres_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
     os.environ["POSTGRES_PASSWORD"] = postgres_password
     os.environ["POSTGRES_USER"] = postgres_user
     os.environ["POSTGRES_DATABASE"] = postgres_database
-    os.environ[f"{postgres_default_version.upper()}_PORT"] = str(postgres_port)
+    os.environ[f"{default_postgres_service_name.upper()}_PORT"] = str(postgres_port)
     await docker_services.start(
-        postgres_default_version,
+        name=default_postgres_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=45,
         pause=1,
         check=postgres_responsive,
         port=postgres_port,
         database=postgres_database,
         user=postgres_user,
         password=postgres_password,
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/redis.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from redis.asyncio import Redis as AsyncRedis
 from redis.exceptions import ConnectionError as RedisConnectionError
 
 if TYPE_CHECKING:
@@ -45,11 +46,31 @@
 
 
 @pytest.fixture()
 def redis_port() -> int:
     return 6397
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.redis.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_redis_service_name() -> str:
+    return "redis"
+
+
 @pytest.fixture(autouse=False)
-async def redis_service(docker_services: DockerServiceRegistry, redis_port: int) -> None:
+async def redis_service(
+    docker_services: DockerServiceRegistry,
+    default_redis_service_name: str,
+    docker_compose_files: list[Path],
+    redis_port: int,
+) -> None:
     os.environ["REDIS_PORT"] = str(redis_port)
-    await docker_services.start("redis", check=redis_responsive, port=redis_port)
+    await docker_services.start(
+        name=default_redis_service_name,
+        docker_compose_files=docker_compose_files,
+        check=redis_responsive,
+        port=redis_port,
+    )
```

### Comparing `pytest_databases-0.2.5/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.3.0/src/pytest_databases/docker/spanner.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 
 from __future__ import annotations
 
 import contextlib
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from google.auth.credentials import AnonymousCredentials, Credentials
 from google.cloud import spanner
 
 if TYPE_CHECKING:
@@ -81,31 +82,44 @@
 
 
 @pytest.fixture
 def spanner_credentials() -> Credentials:
     return AnonymousCredentials()
 
 
+@pytest.fixture(scope="session")
+def docker_compose_files() -> list[Path]:
+    return [Path(Path(__file__).parent / "docker-compose.spanner.yml")]
+
+
+@pytest.fixture(scope="session")
+def default_spanner_service_name() -> str:
+    return "spanner"
+
+
 @pytest.fixture(autouse=False)
 async def spanner_service(
     docker_services: DockerServiceRegistry,
+    default_spanner_service_name: str,
+    docker_compose_files: list[Path],
     docker_ip: str,
     spanner_port: int,
     spanner_instance: str,
     spanner_database: str,
     spanner_project: str,
     spanner_credentials: Credentials,
 ) -> None:
     os.environ["SPANNER_EMULATOR_HOST"] = f"{docker_ip}:{spanner_port}"
     os.environ["SPANNER_DATABASE"] = spanner_database
     os.environ["SPANNER_INSTANCE"] = spanner_instance
     os.environ["SPANNER_PORT"] = str(spanner_port)
     os.environ["GOOGLE_CLOUD_PROJECT"] = spanner_project
     await docker_services.start(
-        "spanner",
+        name=default_spanner_service_name,
+        docker_compose_files=docker_compose_files,
         timeout=60,
         check=spanner_responsive,
         spanner_port=spanner_port,
         spanner_instance=spanner_instance,
         spanner_database=spanner_database,
         spanner_project=spanner_project,
         spanner_credentials=spanner_credentials,
```

### Comparing `pytest_databases-0.2.5/tests/__init__.py` & `pytest_databases-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/conftest.py` & `pytest_databases-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/__init__.py` & `pytest_databases-0.3.0/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/test_cockroachdb.py` & `pytest_databases-0.3.0/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/test_dragonfly.py` & `pytest_databases-0.3.0/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/test_elasticsearch.py` & `pytest_databases-0.3.0/tests/docker/test_elasticsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,35 +29,39 @@
 import pytest
 from elasticsearch7 import AsyncElasticsearch as Elasticsearch7
 from elasticsearch8 import AsyncElasticsearch as Elasticsearch8
 
 from pytest_databases.docker.elastic_search import elasticsearch7_responsive, elasticsearch8_responsive
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from pytest_databases.docker import DockerServiceRegistry
 
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.elastic_search",
 ]
 
 
 @pytest.fixture
 async def elasticsearch7_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     elasticsearch7_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
 ) -> AsyncGenerator[Any, Any]:
     """Overwrites fixture to stop container after the test."""
     try:
         await docker_services.start(
             "elasticsearch7",
+            docker_compose_files=docker_compose_files,
             timeout=45,
             pause=1,
             check=elasticsearch7_responsive,
             port=elasticsearch7_port,
             database=elasticsearch_database,
             user=elasticsearch_user,
             password=elasticsearch_password,
@@ -67,24 +71,26 @@
     finally:
         docker_services.stop("elasticsearch7")
 
 
 @pytest.fixture
 async def elasticsearch8_service(
     docker_services: DockerServiceRegistry,
+    docker_compose_files: list[Path],
     elasticsearch8_port: int,
     elasticsearch_database: str,
     elasticsearch_user: str,
     elasticsearch_password: str,
     elasticsearch_scheme: str,
 ) -> AsyncGenerator[Any, Any]:
     """Overwrites fixture to stop container after the test."""
     try:
         await docker_services.start(
             "elasticsearch8",
+            docker_compose_files=docker_compose_files,
             timeout=45,
             pause=1,
             check=elasticsearch8_responsive,
             port=elasticsearch8_port,
             database=elasticsearch_database,
             user=elasticsearch_user,
             password=elasticsearch_password,
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_keydb.py` & `pytest_databases-0.3.0/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/test_mariadb.py` & `pytest_databases-0.3.0/tests/docker/test_mariadb.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.mariadb",
 ]
 
 
 async def test_mariadb_default_config(
-    mariadb_default_version: str,
+    default_mariadb_service_name: str,
     mariadb_port: int,
     mariadb_database: str,
     mariadb_user: str,
     mariadb_password: str,
 ) -> None:
-    assert mariadb_default_version == "mariadb113"
+    assert default_mariadb_service_name == "mariadb113"
     assert mariadb_port == 3359
     assert mariadb_database == "db"
     assert mariadb_user == "app"
     assert mariadb_password == "super-secret"
 
 
 async def test_mariadb_113_config(
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_mssql.py` & `pytest_databases-0.3.0/tests/docker/test_mssql.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,21 +55,21 @@
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.mssql",
 ]
 
 
 async def test_mssql_default_config(
-    mssql_default_version: str,
+    default_mssql_service_name: str,
     mssql_port: int,
     mssql_database: str,
     mssql_user: str,
     mssql_password: str,
 ) -> None:
-    assert mssql_default_version == "mssql2022"
+    assert default_mssql_service_name == "mssql2022"
     assert mssql_port == 4133
     assert mssql_database == "master"
     assert mssql_user == "sa"
     assert mssql_password == "Super-secret1"
 
 
 async def test_mssql_2022_config(
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_mysql.py` & `pytest_databases-0.3.0/tests/docker/test_mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.mysql",
 ]
 
 
 async def test_mysql_default_config(
-    mysql_default_version: str,
+    default_mysql_service_name: str,
     mysql_port: int,
     mysql_database: str,
     mysql_user: str,
     mysql_password: str,
 ) -> None:
-    assert mysql_default_version == "mysql8"
+    assert default_mysql_service_name == "mysql8"
     assert mysql_port == 3360
     assert mysql_database == "db"
     assert mysql_user == "app"
     assert mysql_password == "super-secret"
 
 
 async def test_mysql_8_config(
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_oracle.py` & `pytest_databases-0.3.0/tests/docker/test_oracle.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 def test_oracle_default_config(
     oracle_user: str,
     oracle_password: str,
     oracle_service_name: str,
     oracle_port: int,
     oracle23c_port: int,
-    oracle_default_version: str,
+    default_oracle_service_name: str,
 ) -> None:
-    assert oracle_default_version == "oracle23c"
+    assert default_oracle_service_name == "oracle23c"
     assert oracle_user == "app"
     assert oracle_password == "super-secret"
     assert oracle_service_name == "FREEPDB1"
     assert oracle_port == 1513
     assert oracle_port == oracle23c_port
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_postgres.py` & `pytest_databases-0.3.0/tests/docker/test_postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 pytestmark = pytest.mark.anyio
 pytest_plugins = [
     "pytest_databases.docker.postgres",
 ]
 
 
 async def test_postgres_default_config(
-    postgres_default_version: str,
+    default_postgres_service_name: str,
     postgres_port: int,
     postgres_database: str,
     postgres_user: str,
     postgres_password: str,
 ) -> None:
-    assert postgres_default_version == "postgres16"
+    assert default_postgres_service_name == "postgres16"
     assert postgres_port == 5427
     assert postgres_database == "postgres"
     assert postgres_user == "postgres"
     assert postgres_password == "super-secret"
 
 
 async def test_postgres_12_config(
```

### Comparing `pytest_databases-0.2.5/tests/docker/test_redis.py` & `pytest_databases-0.3.0/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/tests/docker/test_spanner.py` & `pytest_databases-0.3.0/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/.gitignore` & `pytest_databases-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/LICENSE` & `pytest_databases-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.5/README.md` & `pytest_databases-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |
-| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
+| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
 
 > [!WARNING] > **Pre-Release Alpha Stage**
@@ -40,15 +40,16 @@
 
 `pytest-databases` currently utilizes `docker compose` (or the legacy `docker-compose`) commands to manage the startup and shutdown of each database service. The following databases are currently available:
 
 - **Postgres**: Version 12, 13, 14, 15, and 16 are available
 - **MySQL**: Version 5.6, 5.7 and 8 are available
 - **Oracle**: Version 18c XE and 23C Free are available
 - **SQL Server**: Version 2022 is available
-- **Spanner**: The latest cloud-emulator from Google is available
+- **Google AlloyDB Omni**: Simplified Omni installation for easy testing.
+- **Google Spanner**: The latest cloud-emulator from Google is available
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
 
 ## Contributing
```

### Comparing `pytest_databases-0.2.5/pyproject.toml` & `pytest_databases-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.5"
+version = "0.3.0"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
   "oracle",
   "mssql",
   "duckdb",
   "bigquery",
   "spanner",
+  "alloydb",
+  "alloydbomni",
   "cockroachdb",
   "redis",
   "elasticsearch",
 ]
 # options under https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -100,15 +102,26 @@
   "pytest-cov",
   "pytest-mock",
   "pytest-vcr",
   "pytest-sugar",
   "pytest-click",
   "pytest-xdist",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner", "redis", "elasticsearch7", "elasticsearch8"]
+features = [
+  "oracle",
+  "mysql",
+  "mssql",
+  "postgres",
+  "spanner",
+  "cockroachdb",
+  "spanner",
+  "redis",
+  "elasticsearch7",
+  "elasticsearch8",
+]
 template = "default"
 type = "virtual"
 
 [tool.hatch.envs.test.env-vars]
 PYTHONPATH = "."
 PYTHONUNBUFFERED = "1"
 SOURCE_DATE_EPOCH = "1580601600"
@@ -146,15 +159,26 @@
   "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git",
   "sphinx-click>=5.0.1",
   "sphinx-toolbox>=3.5.0",
   "sphinx-design>=0.5.0",
   "sphinxcontrib-mermaid>=0.9.2",
   "auto-pytabs[sphinx]>=0.4.0",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner", "redis", "elasticsearch7", "elasticsearch8"]
+features = [
+  "oracle",
+  "mysql",
+  "mssql",
+  "postgres",
+  "spanner",
+  "cockroachdb",
+  "spanner",
+  "redis",
+  "elasticsearch7",
+  "elasticsearch8",
+]
 lock-filename = "requirements/requirements-docs.txt"
 pip-compile-constraint = "default"
 python = "3.11"
 template = "test"
 type = "pip-compile"
 
 [tool.hatch.envs.docs.env-vars]
@@ -207,15 +231,25 @@
   "types-six",
   "types-decorator",
   "types-pyyaml",
   "asyncpg-stubs",
   "types-docutils",
   "types-redis",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "cockroachdb", "spanner", "redis", "elasticsearch7", "elasticsearch8"]
+features = [
+  "oracle",
+  "mysql",
+  "mssql",
+  "postgres",
+  "cockroachdb",
+  "spanner",
+  "redis",
+  "elasticsearch7",
+  "elasticsearch8",
+]
 lock-filename = "requirements/requirements-dev.txt"
 path = ".venv/"
 pip-compile-constraint = "docs"
 python = "3.11"
 template = "docs"
 type = "pip-compile"
 
@@ -235,15 +269,25 @@
   "types-six",
   "types-decorator",
   "types-pyyaml",
   "asyncpg-stubs",
   "types-docutils",
   "types-redis",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "redis", "elasticsearch7", "elasticsearch8"]
+features = [
+  "oracle",
+  "mysql",
+  "mssql",
+  "postgres",
+  "spanner",
+  "cockroachdb",
+  "redis",
+  "elasticsearch7",
+  "elasticsearch8",
+]
 python = "3.11"
 template = "docs"
 
 [tool.hatch.envs.lint.scripts]
 check = ["style", "typing"]
 fix = [
   "typing",
```

### Comparing `pytest_databases-0.2.5/PKG-INFO` & `pytest_databases-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.2.5
+Version: 0.3.0
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: bigquery,cockroachdb,database,duckdb,elasticsearch,migration,mssql,mysql,oracle,postgres,redis,spanner
+Keywords: alloydb,alloydbomni,bigquery,cockroachdb,database,duckdb,elasticsearch,migration,mssql,mysql,oracle,postgres,redis,spanner
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -61,16 +61,16 @@
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |
-| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
+| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
 
 > [!WARNING] > **Pre-Release Alpha Stage**
@@ -88,15 +88,16 @@
 
 `pytest-databases` currently utilizes `docker compose` (or the legacy `docker-compose`) commands to manage the startup and shutdown of each database service. The following databases are currently available:
 
 - **Postgres**: Version 12, 13, 14, 15, and 16 are available
 - **MySQL**: Version 5.6, 5.7 and 8 are available
 - **Oracle**: Version 18c XE and 23C Free are available
 - **SQL Server**: Version 2022 is available
-- **Spanner**: The latest cloud-emulator from Google is available
+- **Google AlloyDB Omni**: Simplified Omni installation for easy testing.
+- **Google Spanner**: The latest cloud-emulator from Google is available
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
 
 ## Contributing
```

