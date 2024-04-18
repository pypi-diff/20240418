# Comparing `tmp/qbraid_core-0.1.3.tar.gz` & `tmp/qbraid_core-0.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_core-0.1.3.tar", last modified: Tue Apr 16 22:36:44 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.4.dev0.tar", last modified: Thu Apr 18 16:28:50 2024, max compression
```

## Comparing `qbraid_core-0.1.3.tar` & `qbraid_core-0.1.4.dev0.tar`

### file list

```diff
@@ -1,105 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.333411 qbraid_core-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.337411 qbraid_core-0.1.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.341411 qbraid_core-0.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.341411 qbraid_core-0.1.3/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.345411 qbraid_core-0.1.3/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/services/quantum/proxy_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 22:36:44.000000 qbraid_core-0.1.3/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:36:44.353411 qbraid_core-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/environments/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/environments/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/quantum/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/system/test_packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tests/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tests/top_level/test_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:36:44.349411 qbraid_core-0.1.3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-16 22:36:40.000000 qbraid_core-0.1.3/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.509451 qbraid_core-0.1.4.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.509451 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/quantum/test_aws_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/quantum/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tools/verify_headers.py
```

### Comparing `qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/workflows/docs.yml` & `qbraid_core-0.1.4.dev0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/workflows/format.yml` & `qbraid_core-0.1.4.dev0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/workflows/main.yml` & `qbraid_core-0.1.4.dev0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/workflows/publish.yml` & `qbraid_core-0.1.4.dev0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.github/workflows/test-publish.yml` & `qbraid_core-0.1.4.dev0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/.gitignore` & `qbraid_core-0.1.4.dev0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `qbraid_core-0.1.3/LICENSE` & `qbraid_core-0.1.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/PKG-INFO` & `qbraid_core-0.1.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.3
+Version: 0.1.4.dev0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -30,15 +30,15 @@
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 # qbraid-core
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/core/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-core.svg?color=blue)](https://pypi.org/project/qbraid-core/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-core.svg?color=blue)](https://pypi.org/project/qbraid-core/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
```

### Comparing `qbraid_core-0.1.3/README.md` & `qbraid_core-0.1.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/Makefile` & `qbraid_core-0.1.4.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.4.dev0/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/cards/python.png` & `qbraid_core-0.1.4.dev0/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/cards/terminal.png` & `qbraid_core-0.1.4.dev0/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/css/custom.css` & `qbraid_core-0.1.4.dev0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.4.dev0/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/favicon.ico` & `qbraid_core-0.1.4.dev0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/_static/logo.png` & `qbraid_core-0.1.4.dev0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/conf.py` & `qbraid_core-0.1.4.dev0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,48 +2,22 @@
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 # -- Project information -----------------------------------------------------
 
-project = "qBraid"
+import qbraid_core
+
+project = "qbraid-core"
 copyright = "2024, qBraid Development Team"
 author = "qBraid Development Team"
 
-import os
-
-try:
-    import tomllib
-
-    mode = "rb"
-except (ImportError, ModuleNotFoundError):
-    import toml as tomllib
-
-    mode = "r"
-
-
-def fetch_version():
-    """Get the version from the pyproject.toml file."""
-    try:
-        file_path = os.path.join(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
-            "pyproject.toml",
-        )
-
-        with open(file_path, mode) as file:
-            pyproject_toml = tomllib.load(file)
-            return pyproject_toml["project"]["version"]
-
-    except (FileNotFoundError, IOError) as err:
-        raise FileNotFoundError("Unable to find or read pyproject.toml") from err
-
-
 # Set the version
-version = fetch_version()
+version = qbraid_core.__version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `qbraid_core-0.1.3/docs/index.rst` & `qbraid_core-0.1.4.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/docs/make.bat` & `qbraid_core-0.1.4.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/pyproject.toml` & `qbraid_core-0.1.4.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.3"
+version = "0.1.4.dev0"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
@@ -32,15 +32,15 @@
 Documentation = "https://docs.qbraid.com/projects/core/en/latest/"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pylint", "pytest"]
-docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "sphinx-autodoc-typehints>=1.24,<2.1", "docutils<0.21"]
+docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "sphinx-autodoc-typehints>=1.24,<2.1", "docutils<0.22"]
 
 [tool.setuptools_scm]
 write_to = "qbraid_core/_version.py"
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310", "py311", "py312"]
```

### Comparing `qbraid_core-0.1.3/qbraid_core/__init__.py` & `qbraid_core-0.1.4.dev0/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/_compat.py` & `qbraid_core-0.1.4.dev0/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/client.py` & `qbraid_core-0.1.4.dev0/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/config.py` & `qbraid_core-0.1.4.dev0/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/exceptions.py` & `qbraid_core-0.1.4.dev0/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/registry.py` & `qbraid_core-0.1.4.dev0/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/retry.py` & `qbraid_core-0.1.4.dev0/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/quantum/client.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/services/quantum/proxy_braket.py` & `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy_braket.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,15 +49,23 @@
 
 
 def aws_configure(
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     region: Optional[str] = None,
 ) -> None:
-    """Initializes AWS configuration and credentials files."""
+    """
+    Initializes AWS configuration and credentials files with placeholder values.
+
+    This function ensures the existence of AWS config and credentials files in the user's home
+    directory. If these files do not already exist, it creates them and populates them with
+    placeholder values for the AWS access key and secret access key. While AWS credentials are not
+    required when submitting quantum tasks through qBraid, Amazon Braket requires these files to be
+    present to prevent configuration errors.
+    """
     aws_dir = Path.home() / ".aws"
     config_path = aws_dir / "config"
     credentials_path = aws_dir / "credentials"
     aws_access_key_id = aws_access_key_id or os.getenv("AWS_ACCESS_KEY_ID", "MYACCESSKEY")
     aws_secret_access_key = aws_secret_access_key or os.getenv(
         "AWS_SECRET_ACCESS_KEY", "MYSECRETKEY"
     )
```

### Comparing `qbraid_core-0.1.3/qbraid_core/sessions.py` & `qbraid_core-0.1.4.dev0/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/system/__init__.py` & `qbraid_core-0.1.4.dev0/qbraid_core/system/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,39 +16,49 @@
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
+   echo_log
+   extract_version
    is_exe
    is_valid_python
+   is_valid_semantic_version
    get_python_version_from_cfg
    get_python_version_from_exe
    get_venv_site_packages_path
    get_active_site_packages_path
    get_active_python_path
    get_local_package_path
    get_local_package_version
    get_latest_package_version
    python_paths_equivalent
    replace_str
-   echo_log
+
 
 Exceptions
 ------------
 
 .. autosummary::
    :toctree: ../stubs/
 
+   InvalidVersionError
    QbraidSystemError
    UnknownFileSystemObjectError
+   VersionNotFoundError
 
 """
-from .exceptions import QbraidSystemError, UnknownFileSystemObjectError
+from .exceptions import (
+    InvalidVersionError,
+    QbraidSystemError,
+    UnknownFileSystemObjectError,
+    VersionNotFoundError,
+)
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
     is_exe,
     is_valid_python,
     python_paths_equivalent,
@@ -58,7 +68,8 @@
     get_active_site_packages_path,
     get_latest_package_version,
     get_local_package_path,
     get_local_package_version,
     get_venv_site_packages_path,
 )
 from .threader import FileManager
+from .versions import extract_version, is_valid_semantic_version
```

### Comparing `qbraid_core-0.1.3/qbraid_core/system/executables.py` & `qbraid_core-0.1.4.dev0/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/system/generic.py` & `qbraid_core-0.1.4.dev0/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core/system/packages.py` & `qbraid_core-0.1.4.dev0/qbraid_core/system/packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 from typing import Optional, Union
 
 import requests
 
-from .exceptions import QbraidSystemError
+from .exceptions import QbraidSystemError, VersionNotFoundError
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
     python_paths_equivalent,
 )
 
@@ -147,17 +147,40 @@
 
     try:
         return version(package)
     except PackageNotFoundError as err:
         raise QbraidSystemError(f"{package} not found in the current environment.") from err
 
 
-def get_latest_package_version(package: str) -> str:
+def get_latest_package_version(package: str, prerelease: bool = False) -> str:
     """Retrieves the latest version of package from PyPI."""
     url = f"https://pypi.org/pypi/{package}/json"
     try:
         response = requests.get(url, timeout=5)
         response.raise_for_status()
-        data = response.json()
-        return data["info"]["version"]
     except requests.RequestException as err:
-        raise QbraidSystemError(f"Failed to retrieve latest {package} version from PyPI.") from err
+        raise VersionNotFoundError(
+            f"Failed to retrieve latest {package} version from PyPI."
+        ) from err
+
+    data = response.json()
+
+    if not prerelease:
+        try:
+            return data["info"]["version"]
+        except KeyError as err:
+            raise QbraidSystemError(
+                f"Failed to extract version from {package} package metadata."
+            ) from err
+
+    try:
+        all_versions = list(data["releases"].keys())
+    except KeyError as err:
+        raise QbraidSystemError(
+            f"Failed to extract version from {package} package metadata."
+        ) from err
+
+    if len(all_versions) == 0:
+        raise VersionNotFoundError(f"No versions found for {package}")
+
+    latest_version = all_versions[-1]
+    return latest_version
```

### Comparing `qbraid_core-0.1.3/qbraid_core/system/threader.py` & `qbraid_core-0.1.4.dev0/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.4.dev0/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.3
+Version: 0.1.4.dev0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -30,15 +30,15 @@
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 # qbraid-core
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/core/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-core.svg?color=blue)](https://pypi.org/project/qbraid-core/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-core.svg?color=blue)](https://pypi.org/project/qbraid-core/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
```

### Comparing `qbraid_core-0.1.3/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.4.dev0/qbraid_core.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 qbraid_core/sessions.py
 qbraid_core.egg-info/PKG-INFO
 qbraid_core.egg-info/SOURCES.txt
 qbraid_core.egg-info/dependency_links.txt
 qbraid_core.egg-info/requires.txt
 qbraid_core.egg-info/top_level.txt
 qbraid_core/services/__init__.py
+qbraid_core/services/admin/__init__.py
+qbraid_core/services/admin/client.py
 qbraid_core/services/environments/__init__.py
 qbraid_core/services/environments/client.py
 qbraid_core/services/environments/create.py
 qbraid_core/services/environments/exceptions.py
 qbraid_core/services/environments/paths.py
 qbraid_core/services/environments/state.py
 qbraid_core/services/environments/validate.py
@@ -56,26 +58,29 @@
 qbraid_core/services/quantum/proxy_braket.py
 qbraid_core/system/__init__.py
 qbraid_core/system/exceptions.py
 qbraid_core/system/executables.py
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
+qbraid_core/system/versions.py
 tests/__init__.py
 tests/environments/__init__.py
 tests/environments/conftest.py
 tests/environments/test_client.py
 tests/environments/test_create.py
 tests/environments/test_paths.py
 tests/environments/test_state.py
 tests/environments/test_validate.py
 tests/environments/fixtures/__init__.py
 tests/environments/fixtures/environments.py
+tests/quantum/test_aws_configure.py
 tests/quantum/test_proxy.py
 tests/system/test_executables.py
 tests/system/test_generic.py
 tests/system/test_packages.py
+tests/system/test_versions.py
 tests/top_level/test_client.py
 tests/top_level/test_compat.py
 tests/top_level/test_config.py
 tests/top_level/test_sessions.py
 tools/verify_headers.py
```

### Comparing `qbraid_core-0.1.3/tests/environments/fixtures/environments.py` & `qbraid_core-0.1.4.dev0/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/environments/test_client.py` & `qbraid_core-0.1.4.dev0/tests/environments/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/environments/test_create.py` & `qbraid_core-0.1.4.dev0/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/environments/test_paths.py` & `qbraid_core-0.1.4.dev0/tests/environments/test_paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/environments/test_state.py` & `qbraid_core-0.1.4.dev0/tests/environments/test_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/environments/test_validate.py` & `qbraid_core-0.1.4.dev0/tests/environments/test_validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/quantum/test_proxy.py` & `qbraid_core-0.1.4.dev0/tests/quantum/test_proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/system/test_executables.py` & `qbraid_core-0.1.4.dev0/tests/system/test_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/system/test_generic.py` & `qbraid_core-0.1.4.dev0/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/system/test_packages.py` & `qbraid_core-0.1.4.dev0/tests/system/test_packages.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/top_level/test_client.py` & `qbraid_core-0.1.4.dev0/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/top_level/test_compat.py` & `qbraid_core-0.1.4.dev0/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/top_level/test_config.py` & `qbraid_core-0.1.4.dev0/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tests/top_level/test_sessions.py` & `qbraid_core-0.1.4.dev0/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.3/tools/verify_headers.py` & `qbraid_core-0.1.4.dev0/tools/verify_headers.py`

 * *Files identical despite different names*

