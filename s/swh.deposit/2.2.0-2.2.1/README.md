# Comparing `tmp/swh.deposit-2.2.0.tar.gz` & `tmp/swh_deposit-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.deposit-2.2.0.tar", last modified: Fri Feb  2 10:30:27 2024, max compression
+gzip compressed data, was "swh_deposit-2.2.1.tar", last modified: Thu Apr 18 10:24:03 2024, max compression
```

## Comparing `swh.deposit-2.2.0.tar` & `swh_deposit-2.2.1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.243584 swh.deposit-2.2.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      350 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      207 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1065 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      831 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-02-02 10:30:27.243584 swh.deposit-2.2.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.147586 swh.deposit-2.2.0/bin/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/Makefile
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      130 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/content.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      322 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/create_deposit.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      381 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/create_deposit_atom.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      492 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/create_deposit_with_metadata.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/default-setup
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/download-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)       60 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/home.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      551 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/replace-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)       91 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/service-document.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      256 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/status.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      582 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/update-deposit-with-another-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      252 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/bin/update-status.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)      569 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.151586 swh.deposit-2.2.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.151586 swh.deposit-2.2.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.151586 swh.deposit-2.2.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.155586 swh.deposit-2.2.0/docs/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3230 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/api-documentation.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8816 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/metadata.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1504 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/register-account.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8033 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/use-cases.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14875 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/api/user-manual.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      653 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      169 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.155586 swh.deposit-2.2.0/docs/endpoints/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3371 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/collection.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1864 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/content.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2342 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/service-document.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3488 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/status.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      996 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/update-media.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      884 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/endpoints/update-metadata.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.159586 swh.deposit-2.2.0/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-authentication-basic.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      977 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-authentication-keycloak.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      929 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-create-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1151 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-delete-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1460 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-update-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1005 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-workflow-checking.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1208 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-workflow-loading.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1139 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/deposit-workflow-reception.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/images/status.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      372 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/index.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.159586 swh.deposit-2.2.0/docs/internals/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1646 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/internals/authentication.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/internals/dev-environment.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      299 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/internals/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3534 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/internals/loading-workflow.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4191 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/internals/prod-environment.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       60 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/metadata.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/spec-api.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.163586 swh.deposit-2.2.0/docs/specs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       59 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/blueprint.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1216 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/metadata_example.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13782 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/protocol-reference.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)    26123 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/spec-loading.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4118 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/specs/spec-meta-deposit.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/docs/user-manual.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1008 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2007 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      450 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements-server.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      138 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements-swh-server.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      155 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.131586 swh.deposit-2.2.0/resources/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.163586 swh.deposit-2.2.0/resources/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       46 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/resources/deposit/server.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-02-02 10:30:27.243584 swh.deposit-2.2.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.131586 swh.deposit-2.2.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.171585 swh.deposit-2.2.0/swh/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.175585 swh.deposit-2.2.0/swh/deposit/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17249 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/checks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6094 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/collection.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45116 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1362 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/content.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1827 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5311 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/edit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3140 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/edit_media.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.175585 swh.deposit-2.2.0/swh/deposit/api/private/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2624 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9121 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/deposit_check.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7287 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/deposit_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8441 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/deposit_read.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3892 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/deposit_update_status.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2713 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/private/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1455 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/service_document.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1615 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/state.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/sword_edit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1119 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/api/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/apps.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6082 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/auth.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.179585 swh.deposit-2.2.0/swh/deposit/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1215 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8348 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/cli/admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20150 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/cli/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28542 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4025 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6080 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/errors.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1345 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/exception.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.179585 swh.deposit-2.2.0/swh/deposit/fixtures/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/fixtures/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      194 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/fixtures/deposit_data.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/gunicorn_config.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.179585 swh.deposit-2.2.0/swh/deposit/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/loader/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1397 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/loader/checker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      657 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/loader/tasks.py
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1748 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/manage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.187585 swh.deposit-2.2.0/swh/deposit/migrations/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5264 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0002_depositrequest_archive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0003_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      367 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0004_delete_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      908 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0005_auto_20171019_1436.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      518 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0006_depositclient_url.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      450 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0007_auto_20171129_1609.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      917 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0008_auto_20171130_1513.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0009_deposit_parent.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0010_auto_20180110_0953.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      883 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0011_auto_20180115_1510.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0012_deposit_status_detail.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      817 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0014_auto_20180720_1221.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1359 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0015_depositrequest_typemigration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      878 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0016_auto_20190507_1408.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      612 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0017_auto_20190925_0906.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12150 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0018_migrate_swhids.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0019_auto_20200519_1035.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      582 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0020_auto_20200929_0855.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      858 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1857 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0022_auto_20220223_1542.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      897 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/migrations/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8981 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/models.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/parsers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/py.typed
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.187585 swh.deposit-2.2.0/swh/deposit/settings/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/settings/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3446 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/settings/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/settings/development.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4677 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/settings/production.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/settings/testing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.187585 swh.deposit-2.2.0/swh/deposit/static/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.191585 swh.deposit-2.2.0/swh/deposit/static/css/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16840 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/css/bootstrap-responsive.min.css
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8833 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/css/style.css
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.191585 swh.deposit-2.2.0/swh/deposit/static/img/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      868 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/arrow-up-small.png
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.191585 swh.deposit-2.2.0/swh/deposit/static/img/icons/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1961 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-32x32.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16114 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17138 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23808 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45250 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/swh-logo-deposit.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11585 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/img/swh-logo-deposit.svg
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/static/robots.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.195585 swh.deposit-2.2.0/swh/deposit/templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      505 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/api.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.195585 swh.deposit-2.2.0/swh/deposit/templates/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      492 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/collection_list.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      840 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/content.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/deposit_info.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/deposit_receipt.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/error.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1357 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/service_document.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1501 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/deposit/state.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1571 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/homepage.html
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/layout.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.195585 swh.deposit-2.2.0/swh/deposit/templates/rest_framework/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/templates/rest_framework/api.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.199585 swh.deposit-2.2.0/swh/deposit/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.207585 swh.deposit-2.2.0/swh/deposit/tests/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2730 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      941 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_basic_auth.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    43592 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_checks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3499 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4256 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_add_to_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5083 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    26349 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_atom.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10039 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_binary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14940 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_multipart.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8201 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_reuse_slug.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3860 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4356 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_delete.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_check.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12960 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6169 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_read_archive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17497 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_read_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6857 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_update_status.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4175 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_schedule.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5193 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_state.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4695 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18690 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update_atom.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13760 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update_binary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1781 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2435 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_get_file.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_keycloak_auth.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3586 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_parsers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3051 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/api/test_service_document.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.211585 swh.deposit-2.2.0/swh/deposit/tests/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/cli/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10494 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/cli/test_admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    38637 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/cli/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7496 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18049 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.135586 swh.deposit-2.2.0/swh/deposit/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.211585 swh.deposit-2.2.0/swh/deposit/tests/data/archives/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.223585 swh.deposit-2.2.0/swh/deposit/tests/data/atom/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/codemeta-sample.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       73 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1349 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       74 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-empty-body.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      208 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-ko.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      111 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-minimal.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      501 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      639 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      413 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      463 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      630 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      484 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data0.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      253 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data1.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data2.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data3.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      695 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1021 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-only-create-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-update-in-place.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      346 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/error-cli.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/error-with-decimal.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      527 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/atom/metadata.xml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.223585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.swh.test/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1209 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1164 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_test
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.223585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.list/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.223585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1240 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
--rw-r--r--   0 jenkins    (115) jenkins    (120)      792 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.227585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1218 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)      812 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.227585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.status/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1636 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.227585 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1217 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1634 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1635 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
--rw-r--r--   0 jenkins    (115) jenkins    (120)      750 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.231585 swh.deposit-2.2.0/swh/deposit/tests/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4190 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.135586 swh.deposit-2.2.0/swh/deposit/tests/loader/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.231585 swh.deposit-2.2.0/swh/deposit/tests/loader/data/http_example.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       20 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/http_example.org/hello.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       13 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/http_example.org/hello_you
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.231585 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2036 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
--rw-r--r--   0 jenkins    (115) jenkins    (120)   725946 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
--rw-r--r--   0 jenkins    (115) jenkins    (120)        5 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.235585 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_nowhere.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1233 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/test_checker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7064 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2387 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/loader/test_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2466 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7253 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_client_module.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1050 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2031 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_gunicorn_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      762 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5134 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_migrations.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7679 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests/test_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.235585 swh.deposit-2.2.0/swh/deposit/tests_migration/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/tests_migration/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1394 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7713 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.235585 swh.deposit-2.2.0/swh/deposit/xsd/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3808 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/xsd/codemeta.xsd
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2699 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/swh/deposit/xsd/swh.xsd
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-02-02 10:30:27.235585 swh.deposit-2.2.0/swh.deposit.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11667 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      109 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      755 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-02-02 10:30:27.000000 swh.deposit-2.2.0/swh.deposit.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1622 2024-02-02 10:30:20.000000 swh.deposit-2.2.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      350 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      207 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1507 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      831 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/bin/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/Makefile
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      130 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/content.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      322 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      381 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit_atom.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      492 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit_with_metadata.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/default-setup
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/download-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)       60 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/home.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      551 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/replace-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)       91 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/service-document.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      256 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/status.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      582 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/update-deposit-with-another-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      252 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/update-status.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      569 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3230 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/api-documentation.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8816 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/metadata.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1504 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/register-account.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8033 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/use-cases.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14875 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/user-manual.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      653 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      169 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/endpoints/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3371 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/collection.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1864 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/content.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2342 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/service-document.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3488 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/status.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      996 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/update-media.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      884 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/update-metadata.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-authentication-basic.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      977 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-authentication-keycloak.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      929 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-create-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1151 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-delete-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1460 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-update-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1005 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-checking.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1208 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-loading.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1139 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-reception.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/status.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      372 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/index.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/docs/internals/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1646 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/authentication.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/dev-environment.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      299 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3534 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/loading-workflow.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4191 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/prod-environment.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       60 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/metadata.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/spec-api.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/docs/specs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       59 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/blueprint.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1216 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/metadata_example.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13782 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/protocol-reference.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    26123 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/spec-loading.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4118 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/spec-meta-deposit.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/user-manual.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1008 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2007 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      461 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-server.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      138 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-swh-server.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      155 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.785169 swh_deposit-2.2.1/resources/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/resources/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       46 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/resources/deposit/server.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.785169 swh_deposit-2.2.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.817168 swh_deposit-2.2.1/swh/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17249 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/checks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6094 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/collection.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45766 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/content.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1827 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5311 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/edit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3140 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/edit_media.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/api/private/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2624 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9121 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_check.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7287 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8441 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_read.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3892 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_update_status.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2713 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1455 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/service_document.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1615 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/state.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/sword_edit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1119 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/apps.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6082 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/auth.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1215 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8348 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20150 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28542 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4025 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6080 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/errors.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1345 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/exception.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/fixtures/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/fixtures/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      194 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/fixtures/deposit_data.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/gunicorn_config.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1397 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      657 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/tasks.py
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1748 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/manage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/migrations/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5264 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0002_depositrequest_archive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0003_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      367 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0004_delete_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      908 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      518 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0006_depositclient_url.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      450 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0007_auto_20171129_1609.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      917 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0009_deposit_parent.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      883 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0012_deposit_status_detail.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      817 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1359 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      878 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      612 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12150 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0018_migrate_swhids.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      582 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      858 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1857 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      897 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8981 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/models.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/parsers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/py.typed
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/settings/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3446 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/development.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4677 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/production.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/testing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/css/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16840 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/css/bootstrap-responsive.min.css
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8833 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/css/style.css
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/img/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      868 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/arrow-up-small.png
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.833168 swh_deposit-2.2.1/swh/deposit/static/img/icons/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1961 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16114 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17138 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23808 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45250 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11585 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.svg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/robots.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.833168 swh_deposit-2.2.1/swh/deposit/templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      505 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/api.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.837168 swh_deposit-2.2.1/swh/deposit/templates/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      492 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/collection_list.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      840 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/content.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_info.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_receipt.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/error.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1357 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/service_document.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1501 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/state.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1571 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/homepage.html
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/layout.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.837168 swh_deposit-2.2.1/swh/deposit/templates/rest_framework/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/rest_framework/api.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.841168 swh_deposit-2.2.1/swh/deposit/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.849168 swh_deposit-2.2.1/swh/deposit/tests/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2730 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      941 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_basic_auth.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    43592 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_checks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3499 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4256 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5083 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    26349 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_atom.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10039 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_binary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14940 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_multipart.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8201 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3860 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4356 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_delete.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_check.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12960 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6169 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17497 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6857 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4175 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_schedule.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5193 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_state.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4695 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18690 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_atom.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13760 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_binary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1781 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2435 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_get_file.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_keycloak_auth.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3586 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_parsers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3051 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_service_document.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.853168 swh_deposit-2.2.1/swh/deposit/tests/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10494 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/test_admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    38637 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7496 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18049 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.789169 swh_deposit-2.2.1/swh/deposit/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.853168 swh_deposit-2.2.1/swh/deposit/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/atom/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       73 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1349 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       74 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-empty-body.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      208 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-ko.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      111 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-minimal.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      501 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      639 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      413 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      463 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      630 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      484 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data0.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      253 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data1.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data2.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data3.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      695 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1021 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-only-create-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-update-in-place.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      346 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-cli.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      527 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/metadata.xml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1209 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1164 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1240 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      792 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1218 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      812 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1636 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1217 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1634 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1635 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      750 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4190 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.789169 swh_deposit-2.2.1/swh/deposit/tests/loader/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       20 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/hello.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       13 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/hello_you
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2036 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   725946 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        5 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1233 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7064 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2387 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2466 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7253 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_client_module.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1050 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2031 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      762 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5134 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_migrations.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7679 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests_migration/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests_migration/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1394 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7713 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.873168 swh_deposit-2.2.1/swh/deposit/xsd/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3808 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/xsd/codemeta.xsd
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2699 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/xsd/swh.xsd
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.873168 swh_deposit-2.2.1/swh.deposit.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11667 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      109 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      755 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1289 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/tox.ini
```

### Comparing `swh.deposit-2.2.0/CODE_OF_CONDUCT.md` & `swh_deposit-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/LICENSE` & `swh_deposit-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/Makefile.local` & `swh_deposit-2.2.1/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/PKG-INFO` & `swh_deposit-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 2.2.0
+Version: 2.2.1
 Summary: Software Heritage deposit server
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-deposit
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-deposit/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-deposit/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-deposit.git
```

### Comparing `swh.deposit-2.2.0/README.rst` & `swh_deposit-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/bin/Makefile` & `swh_deposit-2.2.1/bin/Makefile`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/bin/replace-deposit-archive.sh` & `swh_deposit-2.2.1/bin/replace-deposit-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/bin/update-deposit-with-another-archive.sh` & `swh_deposit-2.2.1/bin/update-deposit-with-another-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/conftest.py` & `swh_deposit-2.2.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/README.rst` & `swh_deposit-2.2.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/api/api-documentation.rst` & `swh_deposit-2.2.1/docs/api/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/api/metadata.rst` & `swh_deposit-2.2.1/docs/api/metadata.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/api/register-account.rst` & `swh_deposit-2.2.1/docs/api/register-account.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/api/use-cases.rst` & `swh_deposit-2.2.1/docs/api/use-cases.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/api/user-manual.rst` & `swh_deposit-2.2.1/docs/api/user-manual.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/cli.rst` & `swh_deposit-2.2.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/collection.rst` & `swh_deposit-2.2.1/docs/endpoints/collection.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/content.rst` & `swh_deposit-2.2.1/docs/endpoints/content.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/service-document.rst` & `swh_deposit-2.2.1/docs/endpoints/service-document.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/status.rst` & `swh_deposit-2.2.1/docs/endpoints/status.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/update-media.rst` & `swh_deposit-2.2.1/docs/endpoints/update-media.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/endpoints/update-metadata.rst` & `swh_deposit-2.2.1/docs/endpoints/update-metadata.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-authentication-basic.uml` & `swh_deposit-2.2.1/docs/images/deposit-authentication-basic.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-authentication-keycloak.uml` & `swh_deposit-2.2.1/docs/images/deposit-authentication-keycloak.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-create-chart.uml` & `swh_deposit-2.2.1/docs/images/deposit-create-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-delete-chart.uml` & `swh_deposit-2.2.1/docs/images/deposit-delete-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-update-chart.uml` & `swh_deposit-2.2.1/docs/images/deposit-update-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-workflow-checking.uml` & `swh_deposit-2.2.1/docs/images/deposit-workflow-checking.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-workflow-loading.uml` & `swh_deposit-2.2.1/docs/images/deposit-workflow-loading.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/deposit-workflow-reception.uml` & `swh_deposit-2.2.1/docs/images/deposit-workflow-reception.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/images/status.uml` & `swh_deposit-2.2.1/docs/images/status.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/internals/authentication.rst` & `swh_deposit-2.2.1/docs/internals/authentication.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/internals/dev-environment.rst` & `swh_deposit-2.2.1/docs/internals/dev-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/internals/loading-workflow.rst` & `swh_deposit-2.2.1/docs/internals/loading-workflow.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/internals/prod-environment.rst` & `swh_deposit-2.2.1/docs/internals/prod-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/specs/metadata_example.xml` & `swh_deposit-2.2.1/docs/specs/metadata_example.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/specs/protocol-reference.rst` & `swh_deposit-2.2.1/docs/specs/protocol-reference.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/specs/spec-loading.rst` & `swh_deposit-2.2.1/docs/specs/spec-loading.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/docs/specs/spec-meta-deposit.rst` & `swh_deposit-2.2.1/docs/specs/spec-meta-deposit.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/mypy.ini` & `swh_deposit-2.2.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/pyproject.toml` & `swh_deposit-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/checks.py` & `swh_deposit-2.2.1/swh/deposit/api/checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/collection.py` & `swh_deposit-2.2.1/swh/deposit/api/collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/common.py` & `swh_deposit-2.2.1/swh/deposit/api/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (C) 2017-2022  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from abc import ABCMeta, abstractmethod
+import contextlib
 import datetime
 import hashlib
 import json
-from typing import Any, Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Dict, Iterator, Optional, Sequence, Tuple, Type, Union
 import uuid
 from xml.etree import ElementTree
 
 import attr
 from django.core.files.uploadedfile import UploadedFile
 from django.http import FileResponse, HttpResponse
 from django.shortcuts import render
@@ -234,26 +235,39 @@
             packaging=meta.get("HTTP_PACKAGING"),
             slug=meta.get("HTTP_SLUG"),
             on_behalf_of=meta.get("HTTP_ON_BEHALF_OF"),
             metadata_relevant=meta.get("HTTP_METADATA_RELEVANT"),
             swhid=meta.get("HTTP_X_CHECK_SWHID"),
         )
 
-    def _deposit_put(self, deposit: Deposit, in_progress: bool = False) -> None:
+    @contextlib.contextmanager
+    def _deposit_put(
+        self, deposit: Deposit, in_progress: bool = False
+    ) -> Iterator[None]:
         """Save/Update a deposit in db.
 
+        Acts as a context manager, ensuring the deposit object exists before entering
+        the block, and completes the deposit after (successfully) exiting the block.
+
         Args:
             deposit: deposit being updated/created
             in_progress: deposit status
         """
-        if in_progress is False:
-            self._complete_deposit(deposit)
-        else:
+        if in_progress:
             deposit.status = DEPOSIT_STATUS_PARTIAL
             deposit.save()
+            yield
+        else:
+            if deposit.pk is None:
+                # We need to save the Deposit to the database so DepositRequest objects
+                # can be created with the Deposit as foreign key
+                deposit.status = DEPOSIT_STATUS_PARTIAL
+                deposit.save()
+            yield
+            self._complete_deposit(deposit)
 
     def _complete_deposit(self, deposit: Deposit) -> None:
         """Marks the deposit as 'deposited', then schedule a check task if configured
         to do so."""
         deposit.complete_date = timezone.now()
         deposit.status = DEPOSIT_STATUS_DEPOSITED
         deposit.save()
@@ -475,24 +489,24 @@
         assert isinstance(filehandler, UploadedFile), filehandler
 
         self._check_file_length(filehandler, content_length)
         self._check_file_md5sum(filehandler, headers.content_md5sum)
 
         # actual storage of data
         archive_metadata = filehandler
-        self._deposit_put(
+        with self._deposit_put(
             deposit=deposit,
             in_progress=headers.in_progress,
-        )
-        self._deposit_request_put(
-            deposit,
-            {ARCHIVE_KEY: archive_metadata},
-            replace_metadata=replace_metadata,
-            replace_archives=replace_archives,
-        )
+        ):
+            self._deposit_request_put(
+                deposit,
+                {ARCHIVE_KEY: archive_metadata},
+                replace_metadata=replace_metadata,
+                replace_archives=replace_archives,
+            )
 
         return Receipt(
             deposit_id=deposit.id,
             deposit_date=deposit.reception_date,
             status=deposit.status,
             archive=filehandler.name,
         )
@@ -614,25 +628,25 @@
                 "The xml received is malformed. "
                 "Please ensure your metadata file is correctly formatted.",
             )
 
         self._set_deposit_origin_from_metadata(deposit, metadata_tree, headers)
 
         # actual storage of data
-        self._deposit_put(
+        with self._deposit_put(
             deposit=deposit,
             in_progress=headers.in_progress,
-        )
-        deposit_request_data = {
-            ARCHIVE_KEY: filehandler,
-            RAW_METADATA_KEY: raw_metadata,
-        }
-        self._deposit_request_put(
-            deposit, deposit_request_data, replace_metadata, replace_archives
-        )
+        ):
+            deposit_request_data = {
+                ARCHIVE_KEY: filehandler,
+                RAW_METADATA_KEY: raw_metadata,
+            }
+            self._deposit_request_put(
+                deposit, deposit_request_data, replace_metadata, replace_archives
+            )
 
         return Receipt(
             deposit_id=deposit.id,
             deposit_date=deposit.reception_date,
             archive=filehandler.name,
             status=deposit.status,
         )
@@ -893,25 +907,24 @@
             return Receipt(
                 deposit_id=deposit.id,
                 deposit_date=depo_request.date,
                 status=deposit.status,
                 archive=None,
             )
 
-        self._deposit_put(
+        with self._deposit_put(
             deposit=deposit,
             in_progress=headers.in_progress,
-        )
-
-        self._deposit_request_put(
-            deposit,
-            {RAW_METADATA_KEY: raw_metadata},
-            replace_metadata,
-            replace_archives,
-        )
+        ):
+            self._deposit_request_put(
+                deposit,
+                {RAW_METADATA_KEY: raw_metadata},
+                replace_metadata,
+                replace_archives,
+            )
 
         return Receipt(
             deposit_id=deposit.id,
             deposit_date=deposit.reception_date,
             status=deposit.status,
             archive=None,
         )
```

### Comparing `swh.deposit-2.2.0/swh/deposit/api/content.py` & `swh_deposit-2.2.1/swh/deposit/api/content.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/converters.py` & `swh_deposit-2.2.1/swh/deposit/api/converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/edit.py` & `swh_deposit-2.2.1/swh/deposit/api/edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/edit_media.py` & `swh_deposit-2.2.1/swh/deposit/api/edit_media.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/__init__.py` & `swh_deposit-2.2.1/swh/deposit/api/private/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/deposit_check.py` & `swh_deposit-2.2.1/swh/deposit/api/private/deposit_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/deposit_list.py` & `swh_deposit-2.2.1/swh/deposit/api/private/deposit_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/deposit_read.py` & `swh_deposit-2.2.1/swh/deposit/api/private/deposit_read.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/deposit_update_status.py` & `swh_deposit-2.2.1/swh/deposit/api/private/deposit_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/private/urls.py` & `swh_deposit-2.2.1/swh/deposit/api/private/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/service_document.py` & `swh_deposit-2.2.1/swh/deposit/api/service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/state.py` & `swh_deposit-2.2.1/swh/deposit/api/state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/sword_edit.py` & `swh_deposit-2.2.1/swh/deposit/api/sword_edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/urls.py` & `swh_deposit-2.2.1/swh/deposit/api/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/api/utils.py` & `swh_deposit-2.2.1/swh/deposit/api/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/auth.py` & `swh_deposit-2.2.1/swh/deposit/auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/cli/__init__.py` & `swh_deposit-2.2.1/swh/deposit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/cli/admin.py` & `swh_deposit-2.2.1/swh/deposit/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/cli/client.py` & `swh_deposit-2.2.1/swh/deposit/cli/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/client.py` & `swh_deposit-2.2.1/swh/deposit/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/config.py` & `swh_deposit-2.2.1/swh/deposit/config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/errors.py` & `swh_deposit-2.2.1/swh/deposit/errors.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/exception.py` & `swh_deposit-2.2.1/swh/deposit/exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/loader/checker.py` & `swh_deposit-2.2.1/swh/deposit/loader/checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/loader/tasks.py` & `swh_deposit-2.2.1/swh/deposit/loader/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/manage.py` & `swh_deposit-2.2.1/swh/deposit/manage.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0001_initial.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0002_depositrequest_archive.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0002_depositrequest_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0003_temporaryarchive.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0003_temporaryarchive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0005_auto_20171019_1436.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0006_depositclient_url.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0006_depositclient_url.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0008_auto_20171130_1513.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0009_deposit_parent.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0009_deposit_parent.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0010_auto_20180110_0953.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0011_auto_20180115_1510.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0014_auto_20180720_1221.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0015_depositrequest_typemigration.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0016_auto_20190507_1408.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0017_auto_20190925_0906.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0018_migrate_swhids.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0018_migrate_swhids.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0019_auto_20200519_1035.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0020_auto_20200929_0855.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0022_auto_20220223_1542.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py` & `swh_deposit-2.2.1/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/models.py` & `swh_deposit-2.2.1/swh/deposit/models.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/parsers.py` & `swh_deposit-2.2.1/swh/deposit/parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/settings/common.py` & `swh_deposit-2.2.1/swh/deposit/settings/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/settings/development.py` & `swh_deposit-2.2.1/swh/deposit/settings/development.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/settings/production.py` & `swh_deposit-2.2.1/swh/deposit/settings/production.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/settings/testing.py` & `swh_deposit-2.2.1/swh/deposit/settings/testing.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/css/bootstrap-responsive.min.css` & `swh_deposit-2.2.1/swh/deposit/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/css/style.css` & `swh_deposit-2.2.1/swh/deposit/static/css/style.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/arrow-up-small.png` & `swh_deposit-2.2.1/swh/deposit/static/img/arrow-up-small.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-32x32.png` & `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png` & `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png` & `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png` & `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/swh-logo-deposit.png` & `swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/static/img/swh-logo-deposit.svg` & `swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.svg`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/deposit/content.xml` & `swh_deposit-2.2.1/swh/deposit/templates/deposit/content.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/deposit/deposit_receipt.xml` & `swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_receipt.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/deposit/service_document.xml` & `swh_deposit-2.2.1/swh/deposit/templates/deposit/service_document.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/deposit/state.xml` & `swh_deposit-2.2.1/swh/deposit/templates/deposit/state.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/homepage.html` & `swh_deposit-2.2.1/swh/deposit/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/templates/layout.html` & `swh_deposit-2.2.1/swh/deposit/templates/layout.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/conftest.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_basic_auth.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_checks.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_add_to_origin.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_list.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_atom.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_binary.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_post_multipart.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_multipart.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_collection_reuse_slug.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_converters.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_delete.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_delete.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_check.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_list.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_read_archive.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_read_metadata.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_private_update_status.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_schedule.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_schedule.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_state.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update_atom.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_deposit_update_binary.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_exception.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_get_file.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_get_file.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_keycloak_auth.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_keycloak_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_parsers.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/api/test_service_document.py` & `swh_deposit-2.2.1/swh/deposit/tests/api/test_service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/cli/test_admin.py` & `swh_deposit-2.2.1/swh/deposit/tests/cli/test_admin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/cli/test_client.py` & `swh_deposit-2.2.1/swh/deposit/tests/cli/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/common.py` & `swh_deposit-2.2.1/swh/deposit/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/conftest.py` & `swh_deposit-2.2.1/swh/deposit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/codemeta-sample.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data2.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-data3.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data3.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/entry-list-deposits.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/error-with-decimal.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/atom/metadata.xml` & `swh_deposit-2.2.1/swh/deposit/tests/data/atom/metadata.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_test` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status` & `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/common.py` & `swh_deposit-2.2.1/swh/deposit/tests/loader/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/conftest.py` & `swh_deposit-2.2.1/swh/deposit/tests/loader/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta` & `swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw` & `swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/test_checker.py` & `swh_deposit-2.2.1/swh/deposit/tests/loader/test_checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/test_client.py` & `swh_deposit-2.2.1/swh/deposit/tests/loader/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/loader/test_tasks.py` & `swh_deposit-2.2.1/swh/deposit/tests/loader/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_backend.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_client_module.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_client_module.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_common.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_config.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_gunicorn_config.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_init.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_migrations.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/tests/test_utils.py` & `swh_deposit-2.2.1/swh/deposit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/urls.py` & `swh_deposit-2.2.1/swh/deposit/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/utils.py` & `swh_deposit-2.2.1/swh/deposit/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/xsd/codemeta.xsd` & `swh_deposit-2.2.1/swh/deposit/xsd/codemeta.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh/deposit/xsd/swh.xsd` & `swh_deposit-2.2.1/swh/deposit/xsd/swh.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh.deposit.egg-info/PKG-INFO` & `swh_deposit-2.2.1/swh.deposit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 2.2.0
+Version: 2.2.1
 Summary: Software Heritage deposit server
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-deposit
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-deposit/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-deposit/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-deposit.git
```

### Comparing `swh.deposit-2.2.0/swh.deposit.egg-info/SOURCES.txt` & `swh_deposit-2.2.1/swh.deposit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/swh.deposit.egg-info/requires.txt` & `swh_deposit-2.2.1/swh.deposit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `swh.deposit-2.2.0/tox.ini` & `swh_deposit-2.2.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,28 @@
   black
   flake8
   mypy
   py3-django2
   py3-django3
 
 [testenv]
+usedevelop = true
 extras =
   testing
 deps =
   dev: pdbpp
   pytest-cov
   django2: Django>=2,<3
   django3: Django>=3,<4
 commands =
   pytest --doctest-modules \
-         --rootdir {envsitepackagesdir} \
-         --cov={envsitepackagesdir}/swh/deposit \
+         --cov=swh/deposit \
          --cov-branch \
-         --ignore {envsitepackagesdir}/swh/deposit/settings/ \
-         {envsitepackagesdir}/swh/deposit \
+         swh/deposit \
          {posargs}
-# --rootdir (with --import-mode from pytest.ini) are required to make tests
-# that depends on the test file to be a proper submodule of the swh namespace
-# after migration to PEP420 (implicit namespace).
 
 [testenv:black]
 skip_install = true
 deps =
   black==23.1.0
 commands =
   {envpython} -m black --check swh
@@ -45,15 +41,15 @@
     --exclude=.tox,.git,__pycache__,.tox,.eggs,*.egg,swh/deposit/migrations
 
 [testenv:mypy]
 setenv = DJANGO_SETTINGS_MODULE=swh.deposit.settings.testing
 extras =
   testing
 deps =
-  mypy==1.0.1
+  mypy==1.8.0
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
```

