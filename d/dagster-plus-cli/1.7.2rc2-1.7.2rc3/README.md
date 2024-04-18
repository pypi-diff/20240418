# Comparing `tmp/dagster-plus-cli-1.7.2rc2.tar.gz` & `tmp/dagster-plus-cli-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-plus-cli-1.7.2rc2.tar", last modified: Tue Apr 16 20:41:00 2024, max compression
+gzip compressed data, was "dagster-plus-cli-1.7.2rc3.tar", last modified: Thu Apr 18 21:22:13 2024, max compression
```

## Comparing `dagster-plus-cli-1.7.2rc2.tar` & `dagster-plus-cli-1.7.2rc3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.372652 dagster-plus-cli-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)      130 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-16 20:41:00.372652 dagster-plus-cli-1.7.2rc2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.320652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.324652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.324652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4947 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.328652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    29680 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4122 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4120 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      507 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.332652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.332652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17055 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.336652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4422 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.336652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.336652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.340652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.340652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1525 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18354 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.344652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.348652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4797 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    12940 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.352652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.352652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.364652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9422 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13812 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4654 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5406 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6219 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7105 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2461 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6770 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20455 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3487 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.324652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2922 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 20:41:00.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:00.372652 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16161 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8864 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:41:00.372652 dagster-plus-cli-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 20:27:17.000000 dagster-plus-cli-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.060011 dagster-plus-cli-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-18 21:22:13.060011 dagster-plus-cli-1.7.2rc3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.012010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.016010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.016010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.020010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    30023 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      507 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.024011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.024011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17055 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.024011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.024011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.028010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.028010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.032010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18354 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.032010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.040011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.040011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.040011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.052011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9422 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    14434 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20455 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.016010 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2922 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-18 21:22:12.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:13.060011 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8864 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 21:22:13.060011 dagster-plus-cli-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-18 21:10:30.000000 dagster-plus-cli-1.7.2rc3/setup.py
```

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/branch_deployment/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
     source = metrics.get_source()
     if source == CliEventTags.source.github:
         event = github_context.get_github_event(project_dir)
         msg = f"Your pull request at commit `{event.github_sha}` is automatically being deployed to Dagster Cloud."
         event.update_pr_comment(
             msg + "\n\n" + report.markdown_report(location_states),
             orig_author="github-actions[bot]",
-            orig_text=msg,
+            orig_text="Dagster Cloud",  # used to identify original comment
         )
     else:
         raise ui.error("'dagster-cloud ci notify' is only available within Github actions.")
 
 
 @app.command(help="List locations in the current build session")
 def locations_list(
@@ -784,8 +784,12 @@
                 ui.print("Download complete.")
 
             elif deployment_name == source_deployment:
                 ui.print(f"Uploading {source_deployment} manifest.")
                 upload_organization_artifact(key, project.manifest_path)
                 ui.print("Upload complete")
 
-        ui.print("Project ready")
+            else:
+                ui.warn(
+                    f"Deployment named {deployment_name} does not match source deployment {source_deployment}, taking no action. "
+                    f"If this is the desired dbt state artifacts to upload, set the cli flags `--source-deployment {deployment_name}`."
+                )
```

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/checks.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/report.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/ci/state.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/config.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/commands.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/job/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/metrics.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/organization/saml/commands.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/run/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/Dockerfile` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/serverless/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/commands/workspace/__init__.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/config_utils.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/alert_types.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/artifacts.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/docker_runner.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/errors.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/graphql_client.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/headers/impl.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/code_location.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/deploy.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/deps.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import os.path
 import re
 import subprocess
 import sys
 import tempfile
 from dataclasses import dataclass
-from typing import List, Optional, Tuple
+from typing import List, Mapping, Optional, Sequence, Tuple
 
 import click
 import pkg_resources
 from packaging import version
 
 from dagster_plus_cli import ui
 from dagster_plus_cli.core import docker_runner
@@ -184,14 +184,44 @@
         if self.stdout:
             lines.append("\nOutput:\n" + util.indent(self.stdout))
         if self.stderr:
             lines.append("\nError:\n" + util.indent(self.stderr))
         return "".join(lines)
 
 
+def get_and_check_dependency_versions_from_distributions(
+    distribution_names: Sequence[str],
+) -> Mapping[str, str]:
+    dep_names = ["dagster", "dagster_cloud", "dagster_plus"]
+    dep_versions = {}
+
+    # the distributions are named something like 'dagster-1.0.14-py3-none-any.whl'
+    # and 'dagster_cloud-1.1.7-py3-none-any.whl'
+    for name in distribution_names:
+        for dep_name in dep_names:
+            pattern = re.compile(f"{dep_name}-(.+?)-py")
+            match = pattern.match(name)
+            if match:
+                dep_versions[dep_name] = match.group(1)
+                break
+
+    if "dagster" not in dep_versions:
+        raise ValueError("The dagster package dependency was expected but not found.")
+    print(f"Found package dagster version {dep_versions['dagster']}.")
+
+    if "dagster_cloud" not in dep_versions and "dagster_plus" not in dep_versions:
+        raise ValueError(
+            "Either the dagster_cloud or dagster_plus package dependency was expected but not found."
+        )
+    for dep_name in ["dagster_cloud", "dagster_plus"]:
+        if dep_name in dep_versions:
+            print(f"Found package {dep_name} version {dep_versions[dep_name]}.")
+    return dep_versions
+
+
 def build_deps_from_requirements(
     requirements: DepsRequirements,
     output_directory: str,
     build_method: BuildMethod,
 ) -> Tuple[str, str]:
     os.makedirs(output_directory, exist_ok=True)
     deps_requirements_filename = f"deps-requirements-{requirements.hash}.txt"
@@ -251,30 +281,15 @@
     pex_info = util.get_pex_info(tmp_pex_path)
     pex_hash = pex_info["pex_hash"]
     final_pex_path = os.path.join(output_directory, f"deps-{pex_hash}.pex")
     os.rename(tmp_pex_path, final_pex_path)
     logging.info("Wrote deps pex: %r", final_pex_path)
 
     distribution_names = pex_info["distributions"].keys()
-    # the distributions are named something like 'dagster-1.0.14-py3-none-any.whl'
-    # and 'dagster_cloud-1.1.7-py3-none-any.whl'
-    dep_names = ["dagster", "dagster_cloud"]
-    dep_versions = {}
-    for name in distribution_names:
-        for dep_name in dep_names:
-            pattern = re.compile(f"{dep_name}-(.+?)-py")
-            match = pattern.match(name)
-            if match:
-                dep_versions[dep_name] = match.group(1)
-                break
-
-    for dep_name in dep_names:
-        if dep_name not in dep_versions:
-            raise ValueError(f"The {dep_name} package dependency was expected but not found.")
-        print(f"Found package {dep_name} version {dep_versions[dep_name]}.")
+    dep_versions = get_and_check_dependency_versions_from_distributions(distribution_names)
 
     return final_pex_path, dep_versions["dagster"]
 
 
 def build_deps_from_requirements_file(
     deps_requirements_path: str,
     output_pex_path: str,
```

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/git_context.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/github_context.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/gitlab_context.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/parse_workspace.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/pex_registry.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/selftest.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/source.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pex_builder/util.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/pydantic_yaml.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/pydantic_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Use a pydantic definition to validate dagster_cloud.yaml."""
 
 from typing import Any, Dict, List, Optional
 
 import yaml
-from dagster._config.pythonic_config.pydantic_compat_layer import compat_model_validator
+from dagster._model.pydantic_compat_layer import compat_model_validator
 from pydantic import BaseModel, Extra, Field, validator
 
 
 class CodeSource(BaseModel, extra=Extra.forbid):
     package_name: Optional[str] = None
     module_name: Optional[str] = None
     python_file: Optional[str] = None
```

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/core/workspace.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/docker_utils.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/entrypoint.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/gql.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/pex_utils.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/types.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/ui.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli/utils.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli.egg-info/SOURCES.txt` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_check.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_ci_commands.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_gql.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/dagster_plus_cli_tests/test_metrics.py` & `dagster-plus-cli-1.7.2rc3/dagster_plus_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-cli-1.7.2rc2/setup.py` & `dagster-plus-cli-1.7.2rc3/setup.py`

 * *Files identical despite different names*

