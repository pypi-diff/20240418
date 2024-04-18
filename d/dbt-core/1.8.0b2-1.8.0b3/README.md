# Comparing `tmp/dbt-core-1.8.0b2.tar.gz` & `tmp/dbt_core-1.8.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.8.0b2.tar", last modified: Wed Apr  3 15:20:18 2024, max compression
+gzip compressed data, was "dbt_core-1.8.0b3.tar", last modified: Thu Apr 18 16:22:42 2024, max compression
```

## Comparing `dbt-core-1.8.0b2.tar` & `dbt_core-1.8.0b3.tar`

### file list

```diff
@@ -1,262 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.672722 dbt-core-1.8.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.672722 dbt-core-1.8.0b2/dbt/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.676722 dbt-core-1.8.0b2/dbt/artifacts/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.676722 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/saved_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_layer_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/source_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/sql_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/unit_test_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31410 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    67660 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64188 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    55019 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/semantic_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.668722 dbt-core-1.8.0b2/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    98530 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/core_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    53554 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    49734 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    34960 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.668722 dbt-core-1.8.0b2/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/mp_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.700722 dbt-core-1.8.0b2/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    78171 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)    17600 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)    14964 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    23685 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.700722 dbt-core-1.8.0b2/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/selected_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.704722 dbt-core-1.8.0b2/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17771 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/task/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)  1509632 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26636 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20263 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/exceptions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/saved_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_layer_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/source_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/sql_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/unit_test_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.507873 dbt_core-1.8.0b3/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31410 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.507873 dbt_core-1.8.0b3/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67660 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/query_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64188 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55031 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.487873 dbt_core-1.8.0b3/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99855 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/core_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54812 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49139 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35018 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.487873 dbt_core-1.8.0b3/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/mp_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.523873 dbt_core-1.8.0b3/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80055 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24969 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.523873 dbt_core-1.8.0b3/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/selected_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.527873 dbt_core-1.8.0b3/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/task/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1509632 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18691 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/setup.py
```

### Comparing `dbt-core-1.8.0b2/PKG-INFO` & `dbt_core-1.8.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,20 +21,20 @@
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
-Requires-Dist: pathspec<0.12,>=0.9
-Requires-Dist: sqlparse<0.5,>=0.2.3
+Requires-Dist: pathspec<0.13,>=0.9
+Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
-Requires-Dist: dbt-common<2.0
+Requires-Dist: dbt-common<2.0,>=1.0.1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b3 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
 Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
-pathspec<0.12,>=0.9 Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-
+pathspec<0.13,>=0.9 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: dbt-
 extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
-common<2.0 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+common<2.0,>=1.0.1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
 packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
```

### Comparing `dbt-core-1.8.0b2/README.md` & `dbt_core-1.8.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/__init__.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/base.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/types.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/components.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/components.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/config.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     CompareBehavior,
     MergeBehavior,
 )
 from dbt_common.contracts.config.metadata import Metadata, ShowBehavior
 from dbt_common.contracts.config.materialization import OnConfigurationChangeOption
 from dbt.artifacts.resources.base import Docs
 from dbt.artifacts.resources.types import ModelHookType
-from dbt.contracts.graph.utils import validate_color
+from dbt.artifacts.utils.validation import validate_color
 from dbt import hooks
 from mashumaro.jsonschema.annotations import Pattern
 
 
 def list_str() -> List[str]:
     return []
```

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/exposure.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/exposure.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/generic_test.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/macro.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/macro.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/metric.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/metric.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/model.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/model.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/saved_query.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/seed.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_layer_components.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_layer_components.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_model.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 @dataclass
 class NodeRelation(dbtClassMixin):
     alias: str
     schema_name: str  # TODO: Could this be called simply "schema" so we could reuse StateRelation?
     database: Optional[str] = None
-    relation_name: Optional[str] = None
+    relation_name: Optional[str] = ""
 
 
 # ====================================
 # Dimension objects
 # Dimension protocols: https://github.com/dbt-labs/dbt-semantic-interfaces/blob/main/dbt_semantic_interfaces/protocols/dimension.py
 # ====================================
```

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/singular_test.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/snapshot.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/source_definition.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/source_definition.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/unit_test_definition.py` & `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/unit_test_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         metadata=MergeBehavior.Update.meta(),
     )
 
 
 class UnitTestFormat(StrEnum):
     CSV = "csv"
     Dict = "dict"
+    SQL = "sql"
 
 
 @dataclass
 class UnitTestInputFixture(dbtClassMixin):
     input: str
     rows: Optional[Union[str, List[Dict[str, Any]]]] = None
     format: UnitTestFormat = UnitTestFormat.Dict
```

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/base.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import dataclasses
 from datetime import datetime
+import functools
+from mashumaro.jsonschema import build_json_schema
+from mashumaro.jsonschema.dialects import DRAFT_2020_12
 from typing import ClassVar, Type, TypeVar, Dict, Any, Optional
 
 from dbt_common.clients.system import write_json, read_json
-from dbt.exceptions import (
-    DbtInternalError,
-    DbtRuntimeError,
-    IncompatibleSchemaError,
-)
-from dbt.version import __version__
-
+from dbt_common.exceptions import DbtInternalError, DbtRuntimeError
 from dbt_common.events.functions import get_metadata_vars
 from dbt_common.invocation import get_invocation_id
 from dbt_common.dataclass_schema import dbtClassMixin
 
-from mashumaro.jsonschema import build_json_schema
-from mashumaro.jsonschema.dialects import DRAFT_2020_12
-import functools
+from dbt.version import __version__
+from dbt.artifacts.exceptions import IncompatibleSchemaError
 
 
 BASE_SCHEMAS_URL = "https://schemas.getdbt.com/"
 SCHEMA_PATH = "dbt/{name}/v{version}.json"
 
 
 @dataclasses.dataclass
```

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/catalog.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/freshness.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/manifest.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/results.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from dbt.contracts.graph.nodes import ResultNode
-from dbt_common.events.functions import fire_event
-from dbt.events.types import TimingInfoCollected
-from dbt_common.events.contextvars import get_node_info
 from dbt_common.events.helpers import datetime_to_json_string
-from dbt.logger import TimingProcessor
 from dbt_common.utils import cast_to_str, cast_to_int
 from dbt_common.dataclass_schema import dbtClassMixin, StrEnum
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
@@ -41,21 +37,14 @@
 
     def __enter__(self):
         self.timing_info.begin()
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.timing_info.end()
         self.callback(self.timing_info)
-        # Note: when legacy logger is removed, we can remove the following line
-        with TimingProcessor(self.timing_info):
-            fire_event(
-                TimingInfoCollected(
-                    timing_info=self.timing_info.to_msg_dict(), node_info=get_node_info()
-                )
-            )
 
 
 class RunningStatus(StrEnum):
     Started = "started"
     Compiling = "compiling"
     Executing = "executing"
```

### Comparing `dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py` & `dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/upgrade_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/exceptions.py` & `dbt_core-1.8.0b3/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/flags.py` & `dbt_core-1.8.0b3/dbt/cli/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,14 +348,19 @@
         if getattr(self, "WARN_ERROR_OPTIONS", None) is not None:
             functions.WARN_ERROR_OPTIONS = getattr(self, "WARN_ERROR_OPTIONS")
 
         # Set globals for common.jinja
         if getattr(self, "MACRO_DEBUGGING", None) is not None:
             jinja.MACRO_DEBUGGING = getattr(self, "MACRO_DEBUGGING")
 
+    # This is here to prevent mypy from complaining about all of the
+    # attributes which we added dynamically.
+    def __getattr__(self, name: str) -> Any:
+        return super().__get_attribute__(name)  # type: ignore
+
 
 CommandParams = List[str]
 
 
 def command_params(command: CliCommand, args_dict: Dict[str, Any]) -> CommandParams:
     """Given a command and a dict, returns a list of strings representing
     the CLI params for that command. The order of this list is consistent with
```

### Comparing `dbt-core-1.8.0b2/dbt/cli/main.py` & `dbt_core-1.8.0b3/dbt/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,14 @@
 @requires.preflight
 def debug(ctx, **kwargs):
     """Show information on the current dbt environment and check dependencies, then test the database connection. Not to be confused with the --debug option which increases verbosity."""
     from dbt.task.debug import DebugTask
 
     task = DebugTask(
         ctx.obj["flags"],
-        None,
     )
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
 
 
@@ -460,15 +459,15 @@
 @p.vars
 @requires.postflight
 @requires.preflight
 def init(ctx, **kwargs):
     """Initialize a new dbt project."""
     from dbt.task.init import InitTask
 
-    task = InitTask(ctx.obj["flags"], None)
+    task = InitTask(ctx.obj["flags"])
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
 
 
 # dbt list
```

### Comparing `dbt-core-1.8.0b2/dbt/cli/option_types.py` & `dbt_core-1.8.0b3/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/options.py` & `dbt_core-1.8.0b3/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/params.py` & `dbt_core-1.8.0b3/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/requires.py` & `dbt_core-1.8.0b3/dbt/cli/requires.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from dbt.cli.exceptions import (
     ExceptionExit,
     ResultExit,
 )
 from dbt.cli.flags import Flags
 from dbt.config import RuntimeConfig
 from dbt.config.runtime import load_project, load_profile, UnsetProfile
-from dbt.context.manifest import generate_query_header_context
+from dbt.context.query_header import generate_query_header_context
 
 from dbt_common.events.base_types import EventLevel
 from dbt_common.events.functions import (
     fire_event,
     LOG_VERSION,
 )
 from dbt.events.logging import setup_event_logger
```

### Comparing `dbt-core-1.8.0b2/dbt/cli/resolvers.py` & `dbt_core-1.8.0b3/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/cli/types.py` & `dbt_core-1.8.0b3/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/clients/git.py` & `dbt_core-1.8.0b3/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/clients/jinja.py` & `dbt_core-1.8.0b3/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/clients/jinja_static.py` & `dbt_core-1.8.0b3/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/clients/registry.py` & `dbt_core-1.8.0b3/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/clients/yaml_helper.py` & `dbt_core-1.8.0b3/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/compilation.py` & `dbt_core-1.8.0b3/dbt/compilation.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,14 @@
 
 class Compiler:
     def __init__(self, config) -> None:
         self.config = config
 
     def initialize(self):
         make_directory(self.config.project_target_path)
-        make_directory(self.config.packages_install_path)
 
     # creates a ModelContext which is converted to
     # a dict for jinja rendering of SQL
     def _create_node_context(
         self,
         node: ManifestSQLNode,
         manifest: Manifest,
```

### Comparing `dbt-core-1.8.0b2/dbt/config/profile.py` & `dbt_core-1.8.0b3/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/config/project.py` & `dbt_core-1.8.0b3/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/config/renderer.py` & `dbt_core-1.8.0b3/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/config/runtime.py` & `dbt_core-1.8.0b3/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/config/selectors.py` & `dbt_core-1.8.0b3/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/config/utils.py` & `dbt_core-1.8.0b3/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/constants.py` & `dbt_core-1.8.0b3/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/base.py` & `dbt_core-1.8.0b3/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/configured.py` & `dbt_core-1.8.0b3/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/context_config.py` & `dbt_core-1.8.0b3/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/docs.py` & `dbt_core-1.8.0b3/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/exceptions_jinja.py` & `dbt_core-1.8.0b3/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/macro_resolver.py` & `dbt_core-1.8.0b3/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/macros.py` & `dbt_core-1.8.0b3/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/manifest.py` & `dbt_core-1.8.0b3/dbt/context/manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,17 +67,7 @@
             dct.update(self.namespace)
 
         return dct
 
     @contextproperty()
     def context_macro_stack(self):
         return self.macro_stack
-
-
-class QueryHeaderContext(ManifestContext):
-    def __init__(self, config: AdapterRequiredConfig, manifest: Manifest) -> None:
-        super().__init__(config, manifest, config.project_name)
-
-
-def generate_query_header_context(config: AdapterRequiredConfig, manifest: Manifest):
-    ctx = QueryHeaderContext(config, manifest)
-    return ctx.to_dict()
```

### Comparing `dbt-core-1.8.0b2/dbt/context/providers.py` & `dbt_core-1.8.0b3/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/secret.py` & `dbt_core-1.8.0b3/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/context/target.py` & `dbt_core-1.8.0b3/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/files.py` & `dbt_core-1.8.0b3/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/manifest.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/metrics.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/model_config.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/model_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         lowercased.append("".join("[{}{}]".format(s.upper(), s.lower()) for s in pattern))
     return "^({})$".format("|".join(lowercased))
 
 
 @dataclass
 class UnitTestNodeConfig(NodeConfig):
     expected_rows: List[Dict[str, Any]] = field(default_factory=list)
+    expected_sql: Optional[str] = None
 
 
 @dataclass
 class EmptySnapshotConfig(NodeConfig):
     materialized: str = "snapshot"
     unique_key: Optional[str] = None  # override NodeConfig unique_key definition
```

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/node_args.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/nodes.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -987,15 +987,15 @@
 
         return self.checksum == other.checksum
 
 
 @dataclass
 class UnitTestFileFixture(BaseNode):
     resource_type: Literal[NodeType.Fixture]
-    rows: Optional[List[Dict[str, Any]]] = None
+    rows: Optional[Union[List[Dict[str, Any]], str]] = None
 
 
 # ====================================
 # Snapshot node
 # ====================================
```

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/semantic_manifest.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/unparsed.py` & `dbt_core-1.8.0b3/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/graph/utils.py` & `dbt_core-1.8.0b3/dbt/artifacts/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/project.py` & `dbt_core-1.8.0b3/dbt/contracts/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -292,14 +292,15 @@
             deprecations.warn(
                 "project-test-config", deprecated_path="tests", exp_path="data_tests"
             )
 
 
 @dataclass
 class ProjectFlags(ExtensibleDbtClassMixin):
+    allow_spaces_in_model_names: Optional[bool] = True
     cache_selected_only: Optional[bool] = None
     debug: Optional[bool] = None
     fail_fast: Optional[bool] = None
     indirect_selection: Optional[str] = None
     log_format: Optional[str] = None
     log_format_file: Optional[str] = None
     log_level: Optional[str] = None
@@ -316,15 +317,18 @@
     version_check: Optional[bool] = None
     warn_error: Optional[bool] = None
     warn_error_options: Optional[Dict[str, Union[str, List[str]]]] = None
     write_json: Optional[bool] = None
 
     @property
     def project_only_flags(self) -> Dict[str, Any]:
-        return {"source_freshness_run_project_hooks": self.source_freshness_run_project_hooks}
+        return {
+            "source_freshness_run_project_hooks": self.source_freshness_run_project_hooks,
+            "allow_spaces_in_model_names": self.allow_spaces_in_model_names,
+        }
 
 
 @dataclass
 class ProfileConfig(dbtClassMixin):
     profile_name: str
     target_name: str
     threads: int
```

### Comparing `dbt-core-1.8.0b2/dbt/contracts/results.py` & `dbt_core-1.8.0b3/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/selection.py` & `dbt_core-1.8.0b3/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/sql.py` & `dbt_core-1.8.0b3/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/contracts/state.py` & `dbt_core-1.8.0b3/dbt/contracts/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Optional
 
 from dbt.contracts.graph.manifest import Manifest
+from dbt.artifacts.exceptions import IncompatibleSchemaError
 from dbt.artifacts.schemas.manifest import WritableManifest
 from dbt.artifacts.schemas.freshness import FreshnessExecutionResultArtifact
 from dbt.artifacts.schemas.run import RunResultsArtifact
 from dbt_common.events.functions import fire_event
 from dbt.events.types import WarnStateTargetEqual
-from dbt.exceptions import IncompatibleSchemaError
 
 
 def load_result_state(results_path) -> Optional[RunResultsArtifact]:
     if results_path.exists() and results_path.is_file():
         try:
             return RunResultsArtifact.read_and_check_versions(str(results_path))
         except IncompatibleSchemaError as exc:
```

### Comparing `dbt-core-1.8.0b2/dbt/contracts/util.py` & `dbt_core-1.8.0b3/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deprecations.py` & `dbt_core-1.8.0b3/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deps/base.py` & `dbt_core-1.8.0b3/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deps/git.py` & `dbt_core-1.8.0b3/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deps/local.py` & `dbt_core-1.8.0b3/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deps/registry.py` & `dbt_core-1.8.0b3/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/deps/resolver.py` & `dbt_core-1.8.0b3/dbt/deps/resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Dict, List, NoReturn, Union, Type, Iterator, Set, Any
+from typing import Dict, List, NoReturn, Type, Iterator, Set, Any
 
 from dbt.exceptions import (
     DuplicateDependencyToRootError,
     DuplicateProjectDependencyError,
     MismatchedDependencyTypeError,
     DbtInternalError,
 )
@@ -13,22 +13,21 @@
 from dbt.deps.base import BasePackage, PinnedPackage, UnpinnedPackage
 from dbt.deps.local import LocalUnpinnedPackage
 from dbt.deps.tarball import TarballUnpinnedPackage
 from dbt.deps.git import GitUnpinnedPackage
 from dbt.deps.registry import RegistryUnpinnedPackage
 
 from dbt.contracts.project import (
+    PackageSpec,
     LocalPackage,
     TarballPackage,
     GitPackage,
     RegistryPackage,
 )
 
-PackageContract = Union[LocalPackage, TarballPackage, GitPackage, RegistryPackage]
-
 
 @dataclass
 class PackageListing:
     packages: Dict[str, UnpinnedPackage] = field(default_factory=dict)
 
     def __len__(self):
         return len(self.packages)
@@ -64,15 +63,15 @@
             existing: UnpinnedPackage = self.packages[key]
             if not isinstance(existing, type(package)):
                 self._mismatched_types(existing, package)
             self.packages[key] = existing.incorporate(package)
         else:
             self.packages[key] = package
 
-    def update_from(self, src: List[PackageContract]) -> None:
+    def update_from(self, src: List[PackageSpec]) -> None:
         pkg: UnpinnedPackage
         for contract in src:
             if isinstance(contract, LocalPackage):
                 pkg = LocalUnpinnedPackage.from_contract(contract)
             elif isinstance(contract, TarballPackage):
                 pkg = TarballUnpinnedPackage.from_contract(contract)
             elif isinstance(contract, GitPackage):
@@ -80,17 +79,15 @@
             elif isinstance(contract, RegistryPackage):
                 pkg = RegistryUnpinnedPackage.from_contract(contract)
             else:
                 raise DbtInternalError("Invalid package type {}".format(type(contract)))
             self.incorporate(pkg)
 
     @classmethod
-    def from_contracts(
-        cls: Type["PackageListing"], src: List[PackageContract]
-    ) -> "PackageListing":
+    def from_contracts(cls: Type["PackageListing"], src: List[PackageSpec]) -> "PackageListing":
         self = cls({})
         self.update_from(src)
         return self
 
     def resolved(self) -> List[PinnedPackage]:
         return [p.resolved() for p in self.packages.values()]
 
@@ -110,15 +107,15 @@
             raise DuplicateProjectDependencyError(project_name)
         elif project_name == project.project_name:
             raise DuplicateDependencyToRootError(project_name)
         seen.add(project_name)
 
 
 def resolve_packages(
-    packages: List[PackageContract],
+    packages: List[PackageSpec],
     project: Project,
     cli_vars: Dict[str, Any],
 ) -> List[PinnedPackage]:
     pending = PackageListing.from_contracts(packages)
     final = PackageListing()
 
     renderer = PackageRenderer(cli_vars)
@@ -133,15 +130,15 @@
         pending = next_pending
 
     resolved = final.resolved()
     _check_for_duplicate_project_names(resolved, project, renderer)
     return resolved
 
 
-def resolve_lock_packages(packages: List[PackageContract]) -> List[PinnedPackage]:
+def resolve_lock_packages(packages: List[PackageSpec]) -> List[PinnedPackage]:
     lock_packages = PackageListing.from_contracts(packages)
     final = PackageListing()
 
     for package in lock_packages:
         final.incorporate(package)
 
     resolved = final.resolved()
```

### Comparing `dbt-core-1.8.0b2/dbt/deps/tarball.py` & `dbt_core-1.8.0b3/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/docs/source/_ext/dbt_click.py` & `dbt_core-1.8.0b3/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/docs/source/conf.py` & `dbt_core-1.8.0b3/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/events/base_types.py` & `dbt_core-1.8.0b3/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/events/core_types_pb2.py` & `dbt_core-1.8.0b3/dbt/events/core_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"t\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"t\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"G\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\"S\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"I\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"W\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"P\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"X\n\x1cSpacesInModelNameDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\t\"\x84\x01\n\x1fSpacesInModelNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.SpacesInModelNameDeprecation\"k\n$TotalModelNamesWithSpacesDeprecation\x12\x1b\n\x13\x63ount_invalid_names\x18\x01 \x01(\x05\x12\x17\n\x0fshow_debug_hint\x18\x02 \x01(\x08\x12\r\n\x05level\x18\x03 \x01(\t\"\x94\x01\n\'TotalModelNamesWithSpacesDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.TotalModelNamesWithSpacesDeprecation\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"t\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"t\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"G\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\"S\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"I\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"W\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"P\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core_types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_COREEVENTINFO_EXTRAENTRY']._options = None
@@ -171,576 +171,584 @@
   _globals['_TESTSCONFIGDEPRECATION']._serialized_end=6422
   _globals['_TESTSCONFIGDEPRECATIONMSG']._serialized_start=6424
   _globals['_TESTSCONFIGDEPRECATIONMSG']._serialized_end=6544
   _globals['_PROJECTFLAGSMOVEDDEPRECATION']._serialized_start=6546
   _globals['_PROJECTFLAGSMOVEDDEPRECATION']._serialized_end=6576
   _globals['_PROJECTFLAGSMOVEDDEPRECATIONMSG']._serialized_start=6579
   _globals['_PROJECTFLAGSMOVEDDEPRECATIONMSG']._serialized_end=6711
-  _globals['_DEPRECATEDMODEL']._serialized_start=6713
-  _globals['_DEPRECATEDMODEL']._serialized_end=6799
-  _globals['_DEPRECATEDMODELMSG']._serialized_start=6801
-  _globals['_DEPRECATEDMODELMSG']._serialized_end=6907
-  _globals['_INPUTFILEDIFFERROR']._serialized_start=6909
-  _globals['_INPUTFILEDIFFERROR']._serialized_end=6964
-  _globals['_INPUTFILEDIFFERRORMSG']._serialized_start=6966
-  _globals['_INPUTFILEDIFFERRORMSG']._serialized_end=7078
-  _globals['_INVALIDVALUEFORFIELD']._serialized_start=7080
-  _globals['_INVALIDVALUEFORFIELD']._serialized_end=7143
-  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_start=7145
-  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_end=7261
-  _globals['_VALIDATIONWARNING']._serialized_start=7263
-  _globals['_VALIDATIONWARNING']._serialized_end=7344
-  _globals['_VALIDATIONWARNINGMSG']._serialized_start=7346
-  _globals['_VALIDATIONWARNINGMSG']._serialized_end=7456
-  _globals['_PARSEPERFINFOPATH']._serialized_start=7458
-  _globals['_PARSEPERFINFOPATH']._serialized_end=7491
-  _globals['_PARSEPERFINFOPATHMSG']._serialized_start=7493
-  _globals['_PARSEPERFINFOPATHMSG']._serialized_end=7603
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_start=7605
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_end=7654
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_start=7657
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_end=7799
-  _globals['_PARTIALPARSINGERROR']._serialized_start=7802
-  _globals['_PARTIALPARSINGERROR']._serialized_end=7936
-  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_start=7890
-  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_end=7936
-  _globals['_PARTIALPARSINGERRORMSG']._serialized_start=7938
-  _globals['_PARTIALPARSINGERRORMSG']._serialized_end=8052
-  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_start=8054
-  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_end=8081
-  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_start=8083
-  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_end=8209
-  _globals['_UNABLETOPARTIALPARSE']._serialized_start=8211
-  _globals['_UNABLETOPARTIALPARSE']._serialized_end=8249
-  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_start=8251
-  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_end=8367
-  _globals['_STATECHECKVARSHASH']._serialized_start=8369
-  _globals['_STATECHECKVARSHASH']._serialized_end=8471
-  _globals['_STATECHECKVARSHASHMSG']._serialized_start=8473
-  _globals['_STATECHECKVARSHASHMSG']._serialized_end=8585
-  _globals['_PARTIALPARSINGNOTENABLED']._serialized_start=8587
-  _globals['_PARTIALPARSINGNOTENABLED']._serialized_end=8613
-  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_start=8615
-  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_end=8739
-  _globals['_PARSEDFILELOADFAILED']._serialized_start=8741
-  _globals['_PARSEDFILELOADFAILED']._serialized_end=8808
-  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_start=8810
-  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_end=8926
-  _globals['_PARTIALPARSINGENABLED']._serialized_start=8928
-  _globals['_PARTIALPARSINGENABLED']._serialized_end=9000
-  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_start=9002
-  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_end=9120
-  _globals['_PARTIALPARSINGFILE']._serialized_start=9122
-  _globals['_PARTIALPARSINGFILE']._serialized_end=9178
-  _globals['_PARTIALPARSINGFILEMSG']._serialized_start=9180
-  _globals['_PARTIALPARSINGFILEMSG']._serialized_end=9292
-  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_start=9295
-  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_end=9470
-  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_start=9473
-  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_end=9611
-  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_start=9613
-  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_end=9668
-  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_start=9670
-  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_end=9794
-  _globals['_SEEDINCREASED']._serialized_start=9796
-  _globals['_SEEDINCREASED']._serialized_end=9847
-  _globals['_SEEDINCREASEDMSG']._serialized_start=9849
-  _globals['_SEEDINCREASEDMSG']._serialized_end=9951
-  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_start=9953
-  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_end=10015
-  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_start=10017
-  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_end=10141
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_start=10143
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_end=10211
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_start=10214
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_end=10350
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_start=10352
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_end=10444
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_start=10447
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_end=10585
-  _globals['_UNUSEDTABLES']._serialized_start=10587
-  _globals['_UNUSEDTABLES']._serialized_end=10624
-  _globals['_UNUSEDTABLESMSG']._serialized_start=10626
-  _globals['_UNUSEDTABLESMSG']._serialized_end=10726
-  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_start=10729
-  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_end=10864
-  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_start=10866
-  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_end=10988
-  _globals['_NONODEFORYAMLKEY']._serialized_start=10990
-  _globals['_NONODEFORYAMLKEY']._serialized_end=11065
-  _globals['_NONODEFORYAMLKEYMSG']._serialized_start=11067
-  _globals['_NONODEFORYAMLKEYMSG']._serialized_end=11175
-  _globals['_MACRONOTFOUNDFORPATCH']._serialized_start=11177
-  _globals['_MACRONOTFOUNDFORPATCH']._serialized_end=11220
-  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_start=11222
-  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_end=11340
-  _globals['_NODENOTFOUNDORDISABLED']._serialized_start=11343
-  _globals['_NODENOTFOUNDORDISABLED']._serialized_end=11527
-  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_start=11529
-  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_end=11649
-  _globals['_JINJALOGWARNING']._serialized_start=11651
-  _globals['_JINJALOGWARNING']._serialized_end=11723
-  _globals['_JINJALOGWARNINGMSG']._serialized_start=11725
-  _globals['_JINJALOGWARNINGMSG']._serialized_end=11831
-  _globals['_JINJALOGINFO']._serialized_start=11833
-  _globals['_JINJALOGINFO']._serialized_end=11902
-  _globals['_JINJALOGINFOMSG']._serialized_start=11904
-  _globals['_JINJALOGINFOMSG']._serialized_end=12004
-  _globals['_JINJALOGDEBUG']._serialized_start=12006
-  _globals['_JINJALOGDEBUG']._serialized_end=12076
-  _globals['_JINJALOGDEBUGMSG']._serialized_start=12078
-  _globals['_JINJALOGDEBUGMSG']._serialized_end=12180
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_start=12183
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_end=12357
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_start=12360
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_end=12496
-  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_start=12499
-  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_end=12697
-  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_start=12700
-  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_end=12832
-  _globals['_DEPRECATEDREFERENCE']._serialized_start=12835
-  _globals['_DEPRECATEDREFERENCE']._serialized_end=13024
-  _globals['_DEPRECATEDREFERENCEMSG']._serialized_start=13026
-  _globals['_DEPRECATEDREFERENCEMSG']._serialized_end=13140
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_start=13142
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_end=13202
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_start=13205
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_end=13353
-  _globals['_PARSEINLINENODEERROR']._serialized_start=13355
-  _globals['_PARSEINLINENODEERROR']._serialized_end=13432
-  _globals['_PARSEINLINENODEERRORMSG']._serialized_start=13434
-  _globals['_PARSEINLINENODEERRORMSG']._serialized_end=13550
-  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_start=13552
-  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_end=13592
-  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_start=13594
-  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_end=13720
-  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_start=13723
-  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_end=14117
-  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_start=14119
-  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_end=14245
-  _globals['_WARNSTATETARGETEQUAL']._serialized_start=14247
-  _globals['_WARNSTATETARGETEQUAL']._serialized_end=14289
-  _globals['_WARNSTATETARGETEQUALMSG']._serialized_start=14291
-  _globals['_WARNSTATETARGETEQUALMSG']._serialized_end=14407
-  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_start=14409
-  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_end=14446
-  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_start=14448
-  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_end=14568
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_start=14570
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_end=14617
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_start=14620
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_end=14754
-  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_start=14756
-  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_end=14803
-  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_start=14806
-  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_end=14936
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_start=14938
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_end=14990
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_start=14993
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_end=15143
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_start=15145
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_end=15191
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_start=15194
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_end=15332
-  _globals['_GITNOTHINGTODO']._serialized_start=15334
-  _globals['_GITNOTHINGTODO']._serialized_end=15363
-  _globals['_GITNOTHINGTODOMSG']._serialized_start=15365
-  _globals['_GITNOTHINGTODOMSG']._serialized_end=15469
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_start=15471
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_end=15540
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_start=15543
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_end=15681
-  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_start=15683
-  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_end=15725
-  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_start=15727
-  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_end=15849
-  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_start=15851
-  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_end=15892
-  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_start=15895
-  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_end=16023
-  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_start=16025
-  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_end=16086
-  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_start=16089
-  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_end=16219
-  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_start=16221
-  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_end=16316
-  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_start=16319
-  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_end=16453
-  _globals['_DEPSNOPACKAGESFOUND']._serialized_start=16455
-  _globals['_DEPSNOPACKAGESFOUND']._serialized_end=16476
-  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_start=16478
-  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_end=16592
-  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_start=16594
-  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_end=16641
-  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_start=16643
-  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_end=16765
-  _globals['_DEPSINSTALLINFO']._serialized_start=16767
-  _globals['_DEPSINSTALLINFO']._serialized_end=16806
-  _globals['_DEPSINSTALLINFOMSG']._serialized_start=16808
-  _globals['_DEPSINSTALLINFOMSG']._serialized_end=16914
-  _globals['_DEPSUPDATEAVAILABLE']._serialized_start=16916
-  _globals['_DEPSUPDATEAVAILABLE']._serialized_end=16961
-  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_start=16963
-  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_end=17077
-  _globals['_DEPSUPTODATE']._serialized_start=17079
-  _globals['_DEPSUPTODATE']._serialized_end=17093
-  _globals['_DEPSUPTODATEMSG']._serialized_start=17095
-  _globals['_DEPSUPTODATEMSG']._serialized_end=17195
-  _globals['_DEPSLISTSUBDIRECTORY']._serialized_start=17197
-  _globals['_DEPSLISTSUBDIRECTORY']._serialized_end=17241
-  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_start=17243
-  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_end=17359
-  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_start=17361
-  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_end=17407
-  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_start=17410
-  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_end=17538
-  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_start=17540
-  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_end=17586
-  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_start=17589
-  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_end=17727
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_start=17729
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_end=17795
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_start=17798
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_end=17938
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_start=17940
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_end=17990
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_start=17993
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_end=18129
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_start=18131
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_end=18181
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_start=18184
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_end=18320
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_start=18322
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_end=18375
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_start=18378
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_end=18520
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_start=18522
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_end=18573
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_start=18576
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_end=18714
-  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_start=18716
-  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_end=18756
-  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_start=18758
-  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_end=18882
-  _globals['_DEPSUNPINNED']._serialized_start=18884
-  _globals['_DEPSUNPINNED']._serialized_end=18929
-  _globals['_DEPSUNPINNEDMSG']._serialized_start=18931
-  _globals['_DEPSUNPINNEDMSG']._serialized_end=19031
-  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_start=19033
-  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_end=19080
-  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_start=19083
-  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_end=19213
-  _globals['_DEPSLOCKUPDATING']._serialized_start=19215
-  _globals['_DEPSLOCKUPDATING']._serialized_end=19256
-  _globals['_DEPSLOCKUPDATINGMSG']._serialized_start=19258
-  _globals['_DEPSLOCKUPDATINGMSG']._serialized_end=19366
-  _globals['_DEPSADDPACKAGE']._serialized_start=19368
-  _globals['_DEPSADDPACKAGE']._serialized_end=19450
-  _globals['_DEPSADDPACKAGEMSG']._serialized_start=19452
-  _globals['_DEPSADDPACKAGEMSG']._serialized_end=19556
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_start=19559
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_end=19726
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_start=19673
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_end=19726
-  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_start=19728
-  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_end=19854
-  _globals['_DEPSVERSIONMISSING']._serialized_start=19856
-  _globals['_DEPSVERSIONMISSING']._serialized_end=19892
-  _globals['_DEPSVERSIONMISSINGMSG']._serialized_start=19894
-  _globals['_DEPSVERSIONMISSINGMSG']._serialized_end=20006
-  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_start=20008
-  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_end=20055
-  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_start=20057
-  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_end=20179
-  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_start=20181
-  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_end=20223
-  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_start=20226
-  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_end=20356
-  _globals['_COMPILECOMPLETE']._serialized_start=20358
-  _globals['_COMPILECOMPLETE']._serialized_end=20375
-  _globals['_COMPILECOMPLETEMSG']._serialized_start=20377
-  _globals['_COMPILECOMPLETEMSG']._serialized_end=20483
-  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_start=20485
-  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_end=20509
-  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_start=20511
-  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_end=20631
-  _globals['_SEEDHEADER']._serialized_start=20633
-  _globals['_SEEDHEADER']._serialized_end=20661
-  _globals['_SEEDHEADERMSG']._serialized_start=20663
-  _globals['_SEEDHEADERMSG']._serialized_end=20759
-  _globals['_SQLRUNNEREXCEPTION']._serialized_start=20761
-  _globals['_SQLRUNNEREXCEPTION']._serialized_end=20854
-  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_start=20856
-  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_end=20968
-  _globals['_LOGTESTRESULT']._serialized_start=20971
-  _globals['_LOGTESTRESULT']._serialized_end=21139
-  _globals['_LOGTESTRESULTMSG']._serialized_start=21141
-  _globals['_LOGTESTRESULTMSG']._serialized_end=21243
-  _globals['_LOGSTARTLINE']._serialized_start=21245
-  _globals['_LOGSTARTLINE']._serialized_end=21352
-  _globals['_LOGSTARTLINEMSG']._serialized_start=21354
-  _globals['_LOGSTARTLINEMSG']._serialized_end=21454
-  _globals['_LOGMODELRESULT']._serialized_start=21457
-  _globals['_LOGMODELRESULT']._serialized_end=21606
-  _globals['_LOGMODELRESULTMSG']._serialized_start=21608
-  _globals['_LOGMODELRESULTMSG']._serialized_end=21712
-  _globals['_LOGSNAPSHOTRESULT']._serialized_start=21715
-  _globals['_LOGSNAPSHOTRESULT']._serialized_end=21989
-  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_start=21947
-  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_end=21989
-  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_start=21991
-  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_end=22101
-  _globals['_LOGSEEDRESULT']._serialized_start=22104
-  _globals['_LOGSEEDRESULT']._serialized_end=22289
-  _globals['_LOGSEEDRESULTMSG']._serialized_start=22291
-  _globals['_LOGSEEDRESULTMSG']._serialized_end=22393
-  _globals['_LOGFRESHNESSRESULT']._serialized_start=22396
-  _globals['_LOGFRESHNESSRESULT']._serialized_end=22569
-  _globals['_LOGFRESHNESSRESULTMSG']._serialized_start=22571
-  _globals['_LOGFRESHNESSRESULTMSG']._serialized_end=22683
-  _globals['_LOGNODENOOPRESULT']._serialized_start=22686
-  _globals['_LOGNODENOOPRESULT']._serialized_end=22838
-  _globals['_LOGNODENOOPRESULTMSG']._serialized_start=22840
-  _globals['_LOGNODENOOPRESULTMSG']._serialized_end=22950
-  _globals['_LOGCANCELLINE']._serialized_start=22952
-  _globals['_LOGCANCELLINE']._serialized_end=22986
-  _globals['_LOGCANCELLINEMSG']._serialized_start=22988
-  _globals['_LOGCANCELLINEMSG']._serialized_end=23090
-  _globals['_DEFAULTSELECTOR']._serialized_start=23092
-  _globals['_DEFAULTSELECTOR']._serialized_end=23123
-  _globals['_DEFAULTSELECTORMSG']._serialized_start=23125
-  _globals['_DEFAULTSELECTORMSG']._serialized_end=23231
-  _globals['_NODESTART']._serialized_start=23233
-  _globals['_NODESTART']._serialized_end=23286
-  _globals['_NODESTARTMSG']._serialized_start=23288
-  _globals['_NODESTARTMSG']._serialized_end=23382
-  _globals['_NODEFINISHED']._serialized_start=23384
-  _globals['_NODEFINISHED']._serialized_end=23487
-  _globals['_NODEFINISHEDMSG']._serialized_start=23489
-  _globals['_NODEFINISHEDMSG']._serialized_end=23589
-  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_start=23591
-  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_end=23634
-  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_start=23637
-  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_end=23767
-  _globals['_CONCURRENCYLINE']._serialized_start=23769
-  _globals['_CONCURRENCYLINE']._serialized_end=23848
-  _globals['_CONCURRENCYLINEMSG']._serialized_start=23850
-  _globals['_CONCURRENCYLINEMSG']._serialized_end=23956
-  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_start=23958
-  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_end=24027
-  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_start=24029
-  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_end=24155
-  _globals['_NODECOMPILING']._serialized_start=24157
-  _globals['_NODECOMPILING']._serialized_end=24214
-  _globals['_NODECOMPILINGMSG']._serialized_start=24216
-  _globals['_NODECOMPILINGMSG']._serialized_end=24318
-  _globals['_NODEEXECUTING']._serialized_start=24320
-  _globals['_NODEEXECUTING']._serialized_end=24377
-  _globals['_NODEEXECUTINGMSG']._serialized_start=24379
-  _globals['_NODEEXECUTINGMSG']._serialized_end=24481
-  _globals['_LOGHOOKSTARTLINE']._serialized_start=24483
-  _globals['_LOGHOOKSTARTLINE']._serialized_end=24592
-  _globals['_LOGHOOKSTARTLINEMSG']._serialized_start=24594
-  _globals['_LOGHOOKSTARTLINEMSG']._serialized_end=24702
-  _globals['_LOGHOOKENDLINE']._serialized_start=24705
-  _globals['_LOGHOOKENDLINE']._serialized_end=24852
-  _globals['_LOGHOOKENDLINEMSG']._serialized_start=24854
-  _globals['_LOGHOOKENDLINEMSG']._serialized_end=24958
-  _globals['_SKIPPINGDETAILS']._serialized_start=24961
-  _globals['_SKIPPINGDETAILS']._serialized_end=25108
-  _globals['_SKIPPINGDETAILSMSG']._serialized_start=25110
-  _globals['_SKIPPINGDETAILSMSG']._serialized_end=25216
-  _globals['_NOTHINGTODO']._serialized_start=25218
-  _globals['_NOTHINGTODO']._serialized_end=25231
-  _globals['_NOTHINGTODOMSG']._serialized_start=25233
-  _globals['_NOTHINGTODOMSG']._serialized_end=25331
-  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_start=25333
-  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_end=25377
-  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_start=25380
-  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_end=25514
-  _globals['_ENDRUNRESULT']._serialized_start=25517
-  _globals['_ENDRUNRESULT']._serialized_end=25664
-  _globals['_ENDRUNRESULTMSG']._serialized_start=25666
-  _globals['_ENDRUNRESULTMSG']._serialized_end=25766
-  _globals['_NONODESSELECTED']._serialized_start=25768
-  _globals['_NONODESSELECTED']._serialized_end=25785
-  _globals['_NONODESSELECTEDMSG']._serialized_start=25787
-  _globals['_NONODESSELECTEDMSG']._serialized_end=25893
-  _globals['_COMMANDCOMPLETED']._serialized_start=25895
-  _globals['_COMMANDCOMPLETED']._serialized_end=26014
-  _globals['_COMMANDCOMPLETEDMSG']._serialized_start=26016
-  _globals['_COMMANDCOMPLETEDMSG']._serialized_end=26124
-  _globals['_SHOWNODE']._serialized_start=26126
-  _globals['_SHOWNODE']._serialized_end=26233
-  _globals['_SHOWNODEMSG']._serialized_start=26235
-  _globals['_SHOWNODEMSG']._serialized_end=26327
-  _globals['_COMPILEDNODE']._serialized_start=26329
-  _globals['_COMPILEDNODE']._serialized_end=26441
-  _globals['_COMPILEDNODEMSG']._serialized_start=26443
-  _globals['_COMPILEDNODEMSG']._serialized_end=26543
-  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_start=26545
-  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_end=26643
-  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_start=26645
-  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_end=26767
-  _globals['_INTERNALERRORONRUN']._serialized_start=26769
-  _globals['_INTERNALERRORONRUN']._serialized_end=26864
-  _globals['_INTERNALERRORONRUNMSG']._serialized_start=26866
-  _globals['_INTERNALERRORONRUNMSG']._serialized_end=26978
-  _globals['_GENERICEXCEPTIONONRUN']._serialized_start=26980
-  _globals['_GENERICEXCEPTIONONRUN']._serialized_end=27097
-  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_start=27099
-  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_end=27217
-  _globals['_NODECONNECTIONRELEASEERROR']._serialized_start=27219
-  _globals['_NODECONNECTIONRELEASEERROR']._serialized_end=27297
-  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_start=27300
-  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_end=27428
-  _globals['_FOUNDSTATS']._serialized_start=27430
-  _globals['_FOUNDSTATS']._serialized_end=27461
-  _globals['_FOUNDSTATSMSG']._serialized_start=27463
-  _globals['_FOUNDSTATSMSG']._serialized_end=27559
-  _globals['_MAINKEYBOARDINTERRUPT']._serialized_start=27561
-  _globals['_MAINKEYBOARDINTERRUPT']._serialized_end=27584
-  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_start=27586
-  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_end=27704
-  _globals['_MAINENCOUNTEREDERROR']._serialized_start=27706
-  _globals['_MAINENCOUNTEREDERROR']._serialized_end=27741
-  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_start=27743
-  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_end=27859
-  _globals['_MAINSTACKTRACE']._serialized_start=27861
-  _globals['_MAINSTACKTRACE']._serialized_end=27898
-  _globals['_MAINSTACKTRACEMSG']._serialized_start=27900
-  _globals['_MAINSTACKTRACEMSG']._serialized_end=28004
-  _globals['_TIMINGINFOCOLLECTED']._serialized_start=28006
-  _globals['_TIMINGINFOCOLLECTED']._serialized_end=28118
-  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_start=28120
-  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_end=28234
-  _globals['_LOGDEBUGSTACKTRACE']._serialized_start=28236
-  _globals['_LOGDEBUGSTACKTRACE']._serialized_end=28274
-  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_start=28276
-  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_end=28388
-  _globals['_CHECKCLEANPATH']._serialized_start=28390
-  _globals['_CHECKCLEANPATH']._serialized_end=28420
-  _globals['_CHECKCLEANPATHMSG']._serialized_start=28422
-  _globals['_CHECKCLEANPATHMSG']._serialized_end=28526
-  _globals['_CONFIRMCLEANPATH']._serialized_start=28528
-  _globals['_CONFIRMCLEANPATH']._serialized_end=28560
-  _globals['_CONFIRMCLEANPATHMSG']._serialized_start=28562
-  _globals['_CONFIRMCLEANPATHMSG']._serialized_end=28670
-  _globals['_PROTECTEDCLEANPATH']._serialized_start=28672
-  _globals['_PROTECTEDCLEANPATH']._serialized_end=28706
-  _globals['_PROTECTEDCLEANPATHMSG']._serialized_start=28708
-  _globals['_PROTECTEDCLEANPATHMSG']._serialized_end=28820
-  _globals['_FINISHEDCLEANPATHS']._serialized_start=28822
-  _globals['_FINISHEDCLEANPATHS']._serialized_end=28842
-  _globals['_FINISHEDCLEANPATHSMSG']._serialized_start=28844
-  _globals['_FINISHEDCLEANPATHSMSG']._serialized_end=28956
-  _globals['_OPENCOMMAND']._serialized_start=28958
-  _globals['_OPENCOMMAND']._serialized_end=29011
-  _globals['_OPENCOMMANDMSG']._serialized_start=29013
-  _globals['_OPENCOMMANDMSG']._serialized_end=29111
-  _globals['_SERVINGDOCSPORT']._serialized_start=29113
-  _globals['_SERVINGDOCSPORT']._serialized_end=29161
-  _globals['_SERVINGDOCSPORTMSG']._serialized_start=29163
-  _globals['_SERVINGDOCSPORTMSG']._serialized_end=29269
-  _globals['_SERVINGDOCSACCESSINFO']._serialized_start=29271
-  _globals['_SERVINGDOCSACCESSINFO']._serialized_end=29308
-  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_start=29310
-  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_end=29428
-  _globals['_SERVINGDOCSEXITINFO']._serialized_start=29430
-  _globals['_SERVINGDOCSEXITINFO']._serialized_end=29451
-  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_start=29453
-  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_end=29567
-  _globals['_RUNRESULTWARNING']._serialized_start=29569
-  _globals['_RUNRESULTWARNING']._serialized_end=29685
-  _globals['_RUNRESULTWARNINGMSG']._serialized_start=29687
-  _globals['_RUNRESULTWARNINGMSG']._serialized_end=29795
-  _globals['_RUNRESULTFAILURE']._serialized_start=29797
-  _globals['_RUNRESULTFAILURE']._serialized_end=29913
-  _globals['_RUNRESULTFAILUREMSG']._serialized_start=29915
-  _globals['_RUNRESULTFAILUREMSG']._serialized_end=30023
-  _globals['_STATSLINE']._serialized_start=30025
-  _globals['_STATSLINE']._serialized_end=30132
-  _globals['_STATSLINE_STATSENTRY']._serialized_start=30088
-  _globals['_STATSLINE_STATSENTRY']._serialized_end=30132
-  _globals['_STATSLINEMSG']._serialized_start=30134
-  _globals['_STATSLINEMSG']._serialized_end=30228
-  _globals['_RUNRESULTERROR']._serialized_start=30230
-  _globals['_RUNRESULTERROR']._serialized_end=30301
-  _globals['_RUNRESULTERRORMSG']._serialized_start=30303
-  _globals['_RUNRESULTERRORMSG']._serialized_end=30407
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=30409
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=30492
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=30494
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=30616
-  _globals['_SQLCOMPILEDPATH']._serialized_start=30618
-  _globals['_SQLCOMPILEDPATH']._serialized_end=30691
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=30693
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=30799
-  _globals['_CHECKNODETESTFAILURE']._serialized_start=30801
-  _globals['_CHECKNODETESTFAILURE']._serialized_end=30888
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=30890
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=31006
-  _globals['_ENDOFRUNSUMMARY']._serialized_start=31008
-  _globals['_ENDOFRUNSUMMARY']._serialized_end=31095
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=31097
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=31203
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=31205
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=31290
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=31292
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=31406
-  _globals['_ENSUREGITINSTALLED']._serialized_start=31408
-  _globals['_ENSUREGITINSTALLED']._serialized_end=31428
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=31430
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=31542
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=31544
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=31570
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=31572
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=31696
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=31698
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=31723
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=31725
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=31847
-  _globals['_DISABLETRACKING']._serialized_start=31849
-  _globals['_DISABLETRACKING']._serialized_end=31866
-  _globals['_DISABLETRACKINGMSG']._serialized_start=31868
-  _globals['_DISABLETRACKINGMSG']._serialized_end=31974
-  _globals['_SENDINGEVENT']._serialized_start=31976
-  _globals['_SENDINGEVENT']._serialized_end=32006
-  _globals['_SENDINGEVENTMSG']._serialized_start=32008
-  _globals['_SENDINGEVENTMSG']._serialized_end=32108
-  _globals['_SENDEVENTFAILURE']._serialized_start=32110
-  _globals['_SENDEVENTFAILURE']._serialized_end=32128
-  _globals['_SENDEVENTFAILUREMSG']._serialized_start=32130
-  _globals['_SENDEVENTFAILUREMSG']._serialized_end=32238
-  _globals['_FLUSHEVENTS']._serialized_start=32240
-  _globals['_FLUSHEVENTS']._serialized_end=32253
-  _globals['_FLUSHEVENTSMSG']._serialized_start=32255
-  _globals['_FLUSHEVENTSMSG']._serialized_end=32353
-  _globals['_FLUSHEVENTSFAILURE']._serialized_start=32355
-  _globals['_FLUSHEVENTSFAILURE']._serialized_end=32375
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=32377
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=32489
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=32491
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=32536
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=32538
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=32664
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=32666
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=32746
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=32748
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=32870
-  _globals['_DEBUGCMDOUT']._serialized_start=32872
-  _globals['_DEBUGCMDOUT']._serialized_end=32898
-  _globals['_DEBUGCMDOUTMSG']._serialized_start=32900
-  _globals['_DEBUGCMDOUTMSG']._serialized_end=32998
-  _globals['_DEBUGCMDRESULT']._serialized_start=33000
-  _globals['_DEBUGCMDRESULT']._serialized_end=33029
-  _globals['_DEBUGCMDRESULTMSG']._serialized_start=33031
-  _globals['_DEBUGCMDRESULTMSG']._serialized_end=33135
-  _globals['_LISTCMDOUT']._serialized_start=33137
-  _globals['_LISTCMDOUT']._serialized_end=33162
-  _globals['_LISTCMDOUTMSG']._serialized_start=33164
-  _globals['_LISTCMDOUTMSG']._serialized_end=33260
-  _globals['_RESOURCEREPORT']._serialized_start=33263
-  _globals['_RESOURCEREPORT']._serialized_end=33499
-  _globals['_RESOURCEREPORTMSG']._serialized_start=33501
-  _globals['_RESOURCEREPORTMSG']._serialized_end=33605
+  _globals['_SPACESINMODELNAMEDEPRECATION']._serialized_start=6713
+  _globals['_SPACESINMODELNAMEDEPRECATION']._serialized_end=6801
+  _globals['_SPACESINMODELNAMEDEPRECATIONMSG']._serialized_start=6804
+  _globals['_SPACESINMODELNAMEDEPRECATIONMSG']._serialized_end=6936
+  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATION']._serialized_start=6938
+  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATION']._serialized_end=7045
+  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATIONMSG']._serialized_start=7048
+  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATIONMSG']._serialized_end=7196
+  _globals['_DEPRECATEDMODEL']._serialized_start=7198
+  _globals['_DEPRECATEDMODEL']._serialized_end=7284
+  _globals['_DEPRECATEDMODELMSG']._serialized_start=7286
+  _globals['_DEPRECATEDMODELMSG']._serialized_end=7392
+  _globals['_INPUTFILEDIFFERROR']._serialized_start=7394
+  _globals['_INPUTFILEDIFFERROR']._serialized_end=7449
+  _globals['_INPUTFILEDIFFERRORMSG']._serialized_start=7451
+  _globals['_INPUTFILEDIFFERRORMSG']._serialized_end=7563
+  _globals['_INVALIDVALUEFORFIELD']._serialized_start=7565
+  _globals['_INVALIDVALUEFORFIELD']._serialized_end=7628
+  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_start=7630
+  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_end=7746
+  _globals['_VALIDATIONWARNING']._serialized_start=7748
+  _globals['_VALIDATIONWARNING']._serialized_end=7829
+  _globals['_VALIDATIONWARNINGMSG']._serialized_start=7831
+  _globals['_VALIDATIONWARNINGMSG']._serialized_end=7941
+  _globals['_PARSEPERFINFOPATH']._serialized_start=7943
+  _globals['_PARSEPERFINFOPATH']._serialized_end=7976
+  _globals['_PARSEPERFINFOPATHMSG']._serialized_start=7978
+  _globals['_PARSEPERFINFOPATHMSG']._serialized_end=8088
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_start=8090
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_end=8139
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_start=8142
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_end=8284
+  _globals['_PARTIALPARSINGERROR']._serialized_start=8287
+  _globals['_PARTIALPARSINGERROR']._serialized_end=8421
+  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_start=8375
+  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_end=8421
+  _globals['_PARTIALPARSINGERRORMSG']._serialized_start=8423
+  _globals['_PARTIALPARSINGERRORMSG']._serialized_end=8537
+  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_start=8539
+  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_end=8566
+  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_start=8568
+  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_end=8694
+  _globals['_UNABLETOPARTIALPARSE']._serialized_start=8696
+  _globals['_UNABLETOPARTIALPARSE']._serialized_end=8734
+  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_start=8736
+  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_end=8852
+  _globals['_STATECHECKVARSHASH']._serialized_start=8854
+  _globals['_STATECHECKVARSHASH']._serialized_end=8956
+  _globals['_STATECHECKVARSHASHMSG']._serialized_start=8958
+  _globals['_STATECHECKVARSHASHMSG']._serialized_end=9070
+  _globals['_PARTIALPARSINGNOTENABLED']._serialized_start=9072
+  _globals['_PARTIALPARSINGNOTENABLED']._serialized_end=9098
+  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_start=9100
+  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_end=9224
+  _globals['_PARSEDFILELOADFAILED']._serialized_start=9226
+  _globals['_PARSEDFILELOADFAILED']._serialized_end=9293
+  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_start=9295
+  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_end=9411
+  _globals['_PARTIALPARSINGENABLED']._serialized_start=9413
+  _globals['_PARTIALPARSINGENABLED']._serialized_end=9485
+  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_start=9487
+  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_end=9605
+  _globals['_PARTIALPARSINGFILE']._serialized_start=9607
+  _globals['_PARTIALPARSINGFILE']._serialized_end=9663
+  _globals['_PARTIALPARSINGFILEMSG']._serialized_start=9665
+  _globals['_PARTIALPARSINGFILEMSG']._serialized_end=9777
+  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_start=9780
+  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_end=9955
+  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_start=9958
+  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_end=10096
+  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_start=10098
+  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_end=10153
+  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_start=10155
+  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_end=10279
+  _globals['_SEEDINCREASED']._serialized_start=10281
+  _globals['_SEEDINCREASED']._serialized_end=10332
+  _globals['_SEEDINCREASEDMSG']._serialized_start=10334
+  _globals['_SEEDINCREASEDMSG']._serialized_end=10436
+  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_start=10438
+  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_end=10500
+  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_start=10502
+  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_end=10626
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_start=10628
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_end=10696
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_start=10699
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_end=10835
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_start=10837
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_end=10929
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_start=10932
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_end=11070
+  _globals['_UNUSEDTABLES']._serialized_start=11072
+  _globals['_UNUSEDTABLES']._serialized_end=11109
+  _globals['_UNUSEDTABLESMSG']._serialized_start=11111
+  _globals['_UNUSEDTABLESMSG']._serialized_end=11211
+  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_start=11214
+  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_end=11349
+  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_start=11351
+  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_end=11473
+  _globals['_NONODEFORYAMLKEY']._serialized_start=11475
+  _globals['_NONODEFORYAMLKEY']._serialized_end=11550
+  _globals['_NONODEFORYAMLKEYMSG']._serialized_start=11552
+  _globals['_NONODEFORYAMLKEYMSG']._serialized_end=11660
+  _globals['_MACRONOTFOUNDFORPATCH']._serialized_start=11662
+  _globals['_MACRONOTFOUNDFORPATCH']._serialized_end=11705
+  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_start=11707
+  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_end=11825
+  _globals['_NODENOTFOUNDORDISABLED']._serialized_start=11828
+  _globals['_NODENOTFOUNDORDISABLED']._serialized_end=12012
+  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_start=12014
+  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_end=12134
+  _globals['_JINJALOGWARNING']._serialized_start=12136
+  _globals['_JINJALOGWARNING']._serialized_end=12208
+  _globals['_JINJALOGWARNINGMSG']._serialized_start=12210
+  _globals['_JINJALOGWARNINGMSG']._serialized_end=12316
+  _globals['_JINJALOGINFO']._serialized_start=12318
+  _globals['_JINJALOGINFO']._serialized_end=12387
+  _globals['_JINJALOGINFOMSG']._serialized_start=12389
+  _globals['_JINJALOGINFOMSG']._serialized_end=12489
+  _globals['_JINJALOGDEBUG']._serialized_start=12491
+  _globals['_JINJALOGDEBUG']._serialized_end=12561
+  _globals['_JINJALOGDEBUGMSG']._serialized_start=12563
+  _globals['_JINJALOGDEBUGMSG']._serialized_end=12665
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_start=12668
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_end=12842
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_start=12845
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_end=12981
+  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_start=12984
+  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_end=13182
+  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_start=13185
+  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_end=13317
+  _globals['_DEPRECATEDREFERENCE']._serialized_start=13320
+  _globals['_DEPRECATEDREFERENCE']._serialized_end=13509
+  _globals['_DEPRECATEDREFERENCEMSG']._serialized_start=13511
+  _globals['_DEPRECATEDREFERENCEMSG']._serialized_end=13625
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_start=13627
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_end=13687
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_start=13690
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_end=13838
+  _globals['_PARSEINLINENODEERROR']._serialized_start=13840
+  _globals['_PARSEINLINENODEERROR']._serialized_end=13917
+  _globals['_PARSEINLINENODEERRORMSG']._serialized_start=13919
+  _globals['_PARSEINLINENODEERRORMSG']._serialized_end=14035
+  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_start=14037
+  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_end=14077
+  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_start=14079
+  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_end=14205
+  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_start=14208
+  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_end=14602
+  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_start=14604
+  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_end=14730
+  _globals['_WARNSTATETARGETEQUAL']._serialized_start=14732
+  _globals['_WARNSTATETARGETEQUAL']._serialized_end=14774
+  _globals['_WARNSTATETARGETEQUALMSG']._serialized_start=14776
+  _globals['_WARNSTATETARGETEQUALMSG']._serialized_end=14892
+  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_start=14894
+  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_end=14931
+  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_start=14933
+  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_end=15053
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_start=15055
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_end=15102
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_start=15105
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_end=15239
+  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_start=15241
+  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_end=15288
+  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_start=15291
+  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_end=15421
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_start=15423
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_end=15475
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_start=15478
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_end=15628
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_start=15630
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_end=15676
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_start=15679
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_end=15817
+  _globals['_GITNOTHINGTODO']._serialized_start=15819
+  _globals['_GITNOTHINGTODO']._serialized_end=15848
+  _globals['_GITNOTHINGTODOMSG']._serialized_start=15850
+  _globals['_GITNOTHINGTODOMSG']._serialized_end=15954
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_start=15956
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_end=16025
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_start=16028
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_end=16166
+  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_start=16168
+  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_end=16210
+  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_start=16212
+  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_end=16334
+  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_start=16336
+  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_end=16377
+  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_start=16380
+  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_end=16508
+  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_start=16510
+  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_end=16571
+  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_start=16574
+  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_end=16704
+  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_start=16706
+  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_end=16801
+  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_start=16804
+  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_end=16938
+  _globals['_DEPSNOPACKAGESFOUND']._serialized_start=16940
+  _globals['_DEPSNOPACKAGESFOUND']._serialized_end=16961
+  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_start=16963
+  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_end=17077
+  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_start=17079
+  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_end=17126
+  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_start=17128
+  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_end=17250
+  _globals['_DEPSINSTALLINFO']._serialized_start=17252
+  _globals['_DEPSINSTALLINFO']._serialized_end=17291
+  _globals['_DEPSINSTALLINFOMSG']._serialized_start=17293
+  _globals['_DEPSINSTALLINFOMSG']._serialized_end=17399
+  _globals['_DEPSUPDATEAVAILABLE']._serialized_start=17401
+  _globals['_DEPSUPDATEAVAILABLE']._serialized_end=17446
+  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_start=17448
+  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_end=17562
+  _globals['_DEPSUPTODATE']._serialized_start=17564
+  _globals['_DEPSUPTODATE']._serialized_end=17578
+  _globals['_DEPSUPTODATEMSG']._serialized_start=17580
+  _globals['_DEPSUPTODATEMSG']._serialized_end=17680
+  _globals['_DEPSLISTSUBDIRECTORY']._serialized_start=17682
+  _globals['_DEPSLISTSUBDIRECTORY']._serialized_end=17726
+  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_start=17728
+  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_end=17844
+  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_start=17846
+  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_end=17892
+  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_start=17895
+  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_end=18023
+  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_start=18025
+  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_end=18071
+  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_start=18074
+  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_end=18212
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_start=18214
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_end=18280
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_start=18283
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_end=18423
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_start=18425
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_end=18475
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_start=18478
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_end=18614
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_start=18616
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_end=18666
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_start=18669
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_end=18805
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_start=18807
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_end=18860
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_start=18863
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_end=19005
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_start=19007
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_end=19058
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_start=19061
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_end=19199
+  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_start=19201
+  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_end=19241
+  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_start=19243
+  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_end=19367
+  _globals['_DEPSUNPINNED']._serialized_start=19369
+  _globals['_DEPSUNPINNED']._serialized_end=19414
+  _globals['_DEPSUNPINNEDMSG']._serialized_start=19416
+  _globals['_DEPSUNPINNEDMSG']._serialized_end=19516
+  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_start=19518
+  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_end=19565
+  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_start=19568
+  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_end=19698
+  _globals['_DEPSLOCKUPDATING']._serialized_start=19700
+  _globals['_DEPSLOCKUPDATING']._serialized_end=19741
+  _globals['_DEPSLOCKUPDATINGMSG']._serialized_start=19743
+  _globals['_DEPSLOCKUPDATINGMSG']._serialized_end=19851
+  _globals['_DEPSADDPACKAGE']._serialized_start=19853
+  _globals['_DEPSADDPACKAGE']._serialized_end=19935
+  _globals['_DEPSADDPACKAGEMSG']._serialized_start=19937
+  _globals['_DEPSADDPACKAGEMSG']._serialized_end=20041
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_start=20044
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_end=20211
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_start=20158
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_end=20211
+  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_start=20213
+  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_end=20339
+  _globals['_DEPSVERSIONMISSING']._serialized_start=20341
+  _globals['_DEPSVERSIONMISSING']._serialized_end=20377
+  _globals['_DEPSVERSIONMISSINGMSG']._serialized_start=20379
+  _globals['_DEPSVERSIONMISSINGMSG']._serialized_end=20491
+  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_start=20493
+  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_end=20540
+  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_start=20542
+  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_end=20664
+  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_start=20666
+  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_end=20708
+  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_start=20711
+  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_end=20841
+  _globals['_COMPILECOMPLETE']._serialized_start=20843
+  _globals['_COMPILECOMPLETE']._serialized_end=20860
+  _globals['_COMPILECOMPLETEMSG']._serialized_start=20862
+  _globals['_COMPILECOMPLETEMSG']._serialized_end=20968
+  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_start=20970
+  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_end=20994
+  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_start=20996
+  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_end=21116
+  _globals['_SEEDHEADER']._serialized_start=21118
+  _globals['_SEEDHEADER']._serialized_end=21146
+  _globals['_SEEDHEADERMSG']._serialized_start=21148
+  _globals['_SEEDHEADERMSG']._serialized_end=21244
+  _globals['_SQLRUNNEREXCEPTION']._serialized_start=21246
+  _globals['_SQLRUNNEREXCEPTION']._serialized_end=21339
+  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_start=21341
+  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_end=21453
+  _globals['_LOGTESTRESULT']._serialized_start=21456
+  _globals['_LOGTESTRESULT']._serialized_end=21624
+  _globals['_LOGTESTRESULTMSG']._serialized_start=21626
+  _globals['_LOGTESTRESULTMSG']._serialized_end=21728
+  _globals['_LOGSTARTLINE']._serialized_start=21730
+  _globals['_LOGSTARTLINE']._serialized_end=21837
+  _globals['_LOGSTARTLINEMSG']._serialized_start=21839
+  _globals['_LOGSTARTLINEMSG']._serialized_end=21939
+  _globals['_LOGMODELRESULT']._serialized_start=21942
+  _globals['_LOGMODELRESULT']._serialized_end=22091
+  _globals['_LOGMODELRESULTMSG']._serialized_start=22093
+  _globals['_LOGMODELRESULTMSG']._serialized_end=22197
+  _globals['_LOGSNAPSHOTRESULT']._serialized_start=22200
+  _globals['_LOGSNAPSHOTRESULT']._serialized_end=22474
+  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_start=22432
+  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_end=22474
+  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_start=22476
+  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_end=22586
+  _globals['_LOGSEEDRESULT']._serialized_start=22589
+  _globals['_LOGSEEDRESULT']._serialized_end=22774
+  _globals['_LOGSEEDRESULTMSG']._serialized_start=22776
+  _globals['_LOGSEEDRESULTMSG']._serialized_end=22878
+  _globals['_LOGFRESHNESSRESULT']._serialized_start=22881
+  _globals['_LOGFRESHNESSRESULT']._serialized_end=23054
+  _globals['_LOGFRESHNESSRESULTMSG']._serialized_start=23056
+  _globals['_LOGFRESHNESSRESULTMSG']._serialized_end=23168
+  _globals['_LOGNODENOOPRESULT']._serialized_start=23171
+  _globals['_LOGNODENOOPRESULT']._serialized_end=23323
+  _globals['_LOGNODENOOPRESULTMSG']._serialized_start=23325
+  _globals['_LOGNODENOOPRESULTMSG']._serialized_end=23435
+  _globals['_LOGCANCELLINE']._serialized_start=23437
+  _globals['_LOGCANCELLINE']._serialized_end=23471
+  _globals['_LOGCANCELLINEMSG']._serialized_start=23473
+  _globals['_LOGCANCELLINEMSG']._serialized_end=23575
+  _globals['_DEFAULTSELECTOR']._serialized_start=23577
+  _globals['_DEFAULTSELECTOR']._serialized_end=23608
+  _globals['_DEFAULTSELECTORMSG']._serialized_start=23610
+  _globals['_DEFAULTSELECTORMSG']._serialized_end=23716
+  _globals['_NODESTART']._serialized_start=23718
+  _globals['_NODESTART']._serialized_end=23771
+  _globals['_NODESTARTMSG']._serialized_start=23773
+  _globals['_NODESTARTMSG']._serialized_end=23867
+  _globals['_NODEFINISHED']._serialized_start=23869
+  _globals['_NODEFINISHED']._serialized_end=23972
+  _globals['_NODEFINISHEDMSG']._serialized_start=23974
+  _globals['_NODEFINISHEDMSG']._serialized_end=24074
+  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_start=24076
+  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_end=24119
+  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_start=24122
+  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_end=24252
+  _globals['_CONCURRENCYLINE']._serialized_start=24254
+  _globals['_CONCURRENCYLINE']._serialized_end=24333
+  _globals['_CONCURRENCYLINEMSG']._serialized_start=24335
+  _globals['_CONCURRENCYLINEMSG']._serialized_end=24441
+  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_start=24443
+  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_end=24512
+  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_start=24514
+  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_end=24640
+  _globals['_NODECOMPILING']._serialized_start=24642
+  _globals['_NODECOMPILING']._serialized_end=24699
+  _globals['_NODECOMPILINGMSG']._serialized_start=24701
+  _globals['_NODECOMPILINGMSG']._serialized_end=24803
+  _globals['_NODEEXECUTING']._serialized_start=24805
+  _globals['_NODEEXECUTING']._serialized_end=24862
+  _globals['_NODEEXECUTINGMSG']._serialized_start=24864
+  _globals['_NODEEXECUTINGMSG']._serialized_end=24966
+  _globals['_LOGHOOKSTARTLINE']._serialized_start=24968
+  _globals['_LOGHOOKSTARTLINE']._serialized_end=25077
+  _globals['_LOGHOOKSTARTLINEMSG']._serialized_start=25079
+  _globals['_LOGHOOKSTARTLINEMSG']._serialized_end=25187
+  _globals['_LOGHOOKENDLINE']._serialized_start=25190
+  _globals['_LOGHOOKENDLINE']._serialized_end=25337
+  _globals['_LOGHOOKENDLINEMSG']._serialized_start=25339
+  _globals['_LOGHOOKENDLINEMSG']._serialized_end=25443
+  _globals['_SKIPPINGDETAILS']._serialized_start=25446
+  _globals['_SKIPPINGDETAILS']._serialized_end=25593
+  _globals['_SKIPPINGDETAILSMSG']._serialized_start=25595
+  _globals['_SKIPPINGDETAILSMSG']._serialized_end=25701
+  _globals['_NOTHINGTODO']._serialized_start=25703
+  _globals['_NOTHINGTODO']._serialized_end=25716
+  _globals['_NOTHINGTODOMSG']._serialized_start=25718
+  _globals['_NOTHINGTODOMSG']._serialized_end=25816
+  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_start=25818
+  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_end=25862
+  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_start=25865
+  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_end=25999
+  _globals['_ENDRUNRESULT']._serialized_start=26002
+  _globals['_ENDRUNRESULT']._serialized_end=26149
+  _globals['_ENDRUNRESULTMSG']._serialized_start=26151
+  _globals['_ENDRUNRESULTMSG']._serialized_end=26251
+  _globals['_NONODESSELECTED']._serialized_start=26253
+  _globals['_NONODESSELECTED']._serialized_end=26270
+  _globals['_NONODESSELECTEDMSG']._serialized_start=26272
+  _globals['_NONODESSELECTEDMSG']._serialized_end=26378
+  _globals['_COMMANDCOMPLETED']._serialized_start=26380
+  _globals['_COMMANDCOMPLETED']._serialized_end=26499
+  _globals['_COMMANDCOMPLETEDMSG']._serialized_start=26501
+  _globals['_COMMANDCOMPLETEDMSG']._serialized_end=26609
+  _globals['_SHOWNODE']._serialized_start=26611
+  _globals['_SHOWNODE']._serialized_end=26718
+  _globals['_SHOWNODEMSG']._serialized_start=26720
+  _globals['_SHOWNODEMSG']._serialized_end=26812
+  _globals['_COMPILEDNODE']._serialized_start=26814
+  _globals['_COMPILEDNODE']._serialized_end=26926
+  _globals['_COMPILEDNODEMSG']._serialized_start=26928
+  _globals['_COMPILEDNODEMSG']._serialized_end=27028
+  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_start=27030
+  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_end=27128
+  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_start=27130
+  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_end=27252
+  _globals['_INTERNALERRORONRUN']._serialized_start=27254
+  _globals['_INTERNALERRORONRUN']._serialized_end=27349
+  _globals['_INTERNALERRORONRUNMSG']._serialized_start=27351
+  _globals['_INTERNALERRORONRUNMSG']._serialized_end=27463
+  _globals['_GENERICEXCEPTIONONRUN']._serialized_start=27465
+  _globals['_GENERICEXCEPTIONONRUN']._serialized_end=27582
+  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_start=27584
+  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_end=27702
+  _globals['_NODECONNECTIONRELEASEERROR']._serialized_start=27704
+  _globals['_NODECONNECTIONRELEASEERROR']._serialized_end=27782
+  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_start=27785
+  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_end=27913
+  _globals['_FOUNDSTATS']._serialized_start=27915
+  _globals['_FOUNDSTATS']._serialized_end=27946
+  _globals['_FOUNDSTATSMSG']._serialized_start=27948
+  _globals['_FOUNDSTATSMSG']._serialized_end=28044
+  _globals['_MAINKEYBOARDINTERRUPT']._serialized_start=28046
+  _globals['_MAINKEYBOARDINTERRUPT']._serialized_end=28069
+  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_start=28071
+  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_end=28189
+  _globals['_MAINENCOUNTEREDERROR']._serialized_start=28191
+  _globals['_MAINENCOUNTEREDERROR']._serialized_end=28226
+  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_start=28228
+  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_end=28344
+  _globals['_MAINSTACKTRACE']._serialized_start=28346
+  _globals['_MAINSTACKTRACE']._serialized_end=28383
+  _globals['_MAINSTACKTRACEMSG']._serialized_start=28385
+  _globals['_MAINSTACKTRACEMSG']._serialized_end=28489
+  _globals['_TIMINGINFOCOLLECTED']._serialized_start=28491
+  _globals['_TIMINGINFOCOLLECTED']._serialized_end=28603
+  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_start=28605
+  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_end=28719
+  _globals['_LOGDEBUGSTACKTRACE']._serialized_start=28721
+  _globals['_LOGDEBUGSTACKTRACE']._serialized_end=28759
+  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_start=28761
+  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_end=28873
+  _globals['_CHECKCLEANPATH']._serialized_start=28875
+  _globals['_CHECKCLEANPATH']._serialized_end=28905
+  _globals['_CHECKCLEANPATHMSG']._serialized_start=28907
+  _globals['_CHECKCLEANPATHMSG']._serialized_end=29011
+  _globals['_CONFIRMCLEANPATH']._serialized_start=29013
+  _globals['_CONFIRMCLEANPATH']._serialized_end=29045
+  _globals['_CONFIRMCLEANPATHMSG']._serialized_start=29047
+  _globals['_CONFIRMCLEANPATHMSG']._serialized_end=29155
+  _globals['_PROTECTEDCLEANPATH']._serialized_start=29157
+  _globals['_PROTECTEDCLEANPATH']._serialized_end=29191
+  _globals['_PROTECTEDCLEANPATHMSG']._serialized_start=29193
+  _globals['_PROTECTEDCLEANPATHMSG']._serialized_end=29305
+  _globals['_FINISHEDCLEANPATHS']._serialized_start=29307
+  _globals['_FINISHEDCLEANPATHS']._serialized_end=29327
+  _globals['_FINISHEDCLEANPATHSMSG']._serialized_start=29329
+  _globals['_FINISHEDCLEANPATHSMSG']._serialized_end=29441
+  _globals['_OPENCOMMAND']._serialized_start=29443
+  _globals['_OPENCOMMAND']._serialized_end=29496
+  _globals['_OPENCOMMANDMSG']._serialized_start=29498
+  _globals['_OPENCOMMANDMSG']._serialized_end=29596
+  _globals['_SERVINGDOCSPORT']._serialized_start=29598
+  _globals['_SERVINGDOCSPORT']._serialized_end=29646
+  _globals['_SERVINGDOCSPORTMSG']._serialized_start=29648
+  _globals['_SERVINGDOCSPORTMSG']._serialized_end=29754
+  _globals['_SERVINGDOCSACCESSINFO']._serialized_start=29756
+  _globals['_SERVINGDOCSACCESSINFO']._serialized_end=29793
+  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_start=29795
+  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_end=29913
+  _globals['_SERVINGDOCSEXITINFO']._serialized_start=29915
+  _globals['_SERVINGDOCSEXITINFO']._serialized_end=29936
+  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_start=29938
+  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_end=30052
+  _globals['_RUNRESULTWARNING']._serialized_start=30054
+  _globals['_RUNRESULTWARNING']._serialized_end=30170
+  _globals['_RUNRESULTWARNINGMSG']._serialized_start=30172
+  _globals['_RUNRESULTWARNINGMSG']._serialized_end=30280
+  _globals['_RUNRESULTFAILURE']._serialized_start=30282
+  _globals['_RUNRESULTFAILURE']._serialized_end=30398
+  _globals['_RUNRESULTFAILUREMSG']._serialized_start=30400
+  _globals['_RUNRESULTFAILUREMSG']._serialized_end=30508
+  _globals['_STATSLINE']._serialized_start=30510
+  _globals['_STATSLINE']._serialized_end=30617
+  _globals['_STATSLINE_STATSENTRY']._serialized_start=30573
+  _globals['_STATSLINE_STATSENTRY']._serialized_end=30617
+  _globals['_STATSLINEMSG']._serialized_start=30619
+  _globals['_STATSLINEMSG']._serialized_end=30713
+  _globals['_RUNRESULTERROR']._serialized_start=30715
+  _globals['_RUNRESULTERROR']._serialized_end=30786
+  _globals['_RUNRESULTERRORMSG']._serialized_start=30788
+  _globals['_RUNRESULTERRORMSG']._serialized_end=30892
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=30894
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=30977
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=30979
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=31101
+  _globals['_SQLCOMPILEDPATH']._serialized_start=31103
+  _globals['_SQLCOMPILEDPATH']._serialized_end=31176
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=31178
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=31284
+  _globals['_CHECKNODETESTFAILURE']._serialized_start=31286
+  _globals['_CHECKNODETESTFAILURE']._serialized_end=31373
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=31375
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=31491
+  _globals['_ENDOFRUNSUMMARY']._serialized_start=31493
+  _globals['_ENDOFRUNSUMMARY']._serialized_end=31580
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=31582
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=31688
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=31690
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=31775
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=31777
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=31891
+  _globals['_ENSUREGITINSTALLED']._serialized_start=31893
+  _globals['_ENSUREGITINSTALLED']._serialized_end=31913
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=31915
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=32027
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=32029
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=32055
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=32057
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=32181
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=32183
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=32208
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=32210
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=32332
+  _globals['_DISABLETRACKING']._serialized_start=32334
+  _globals['_DISABLETRACKING']._serialized_end=32351
+  _globals['_DISABLETRACKINGMSG']._serialized_start=32353
+  _globals['_DISABLETRACKINGMSG']._serialized_end=32459
+  _globals['_SENDINGEVENT']._serialized_start=32461
+  _globals['_SENDINGEVENT']._serialized_end=32491
+  _globals['_SENDINGEVENTMSG']._serialized_start=32493
+  _globals['_SENDINGEVENTMSG']._serialized_end=32593
+  _globals['_SENDEVENTFAILURE']._serialized_start=32595
+  _globals['_SENDEVENTFAILURE']._serialized_end=32613
+  _globals['_SENDEVENTFAILUREMSG']._serialized_start=32615
+  _globals['_SENDEVENTFAILUREMSG']._serialized_end=32723
+  _globals['_FLUSHEVENTS']._serialized_start=32725
+  _globals['_FLUSHEVENTS']._serialized_end=32738
+  _globals['_FLUSHEVENTSMSG']._serialized_start=32740
+  _globals['_FLUSHEVENTSMSG']._serialized_end=32838
+  _globals['_FLUSHEVENTSFAILURE']._serialized_start=32840
+  _globals['_FLUSHEVENTSFAILURE']._serialized_end=32860
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=32862
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=32974
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=32976
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=33021
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=33023
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=33149
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=33151
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=33231
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=33233
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=33355
+  _globals['_DEBUGCMDOUT']._serialized_start=33357
+  _globals['_DEBUGCMDOUT']._serialized_end=33383
+  _globals['_DEBUGCMDOUTMSG']._serialized_start=33385
+  _globals['_DEBUGCMDOUTMSG']._serialized_end=33483
+  _globals['_DEBUGCMDRESULT']._serialized_start=33485
+  _globals['_DEBUGCMDRESULT']._serialized_end=33514
+  _globals['_DEBUGCMDRESULTMSG']._serialized_start=33516
+  _globals['_DEBUGCMDRESULTMSG']._serialized_end=33620
+  _globals['_LISTCMDOUT']._serialized_start=33622
+  _globals['_LISTCMDOUT']._serialized_end=33647
+  _globals['_LISTCMDOUTMSG']._serialized_start=33649
+  _globals['_LISTCMDOUTMSG']._serialized_end=33745
+  _globals['_RESOURCEREPORT']._serialized_start=33748
+  _globals['_RESOURCEREPORT']._serialized_end=33984
+  _globals['_RESOURCEREPORTMSG']._serialized_start=33986
+  _globals['_RESOURCEREPORTMSG']._serialized_end=34090
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt-core-1.8.0b2/dbt/events/logging.py` & `dbt_core-1.8.0b3/dbt/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/events/types.py` & `dbt_core-1.8.0b3/dbt/events/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from dbt.constants import MAXIMUM_SEED_SIZE_NAME, PIN_PACKAGE_URL
-from dbt_common.ui import warning_tag, line_wrap_message, green, yellow, red
+from dbt_common.ui import error_tag, warning_tag, line_wrap_message, green, yellow, red
 from dbt_common.events.base_types import EventLevel
 from dbt_common.events.format import (
     format_fancy_output_line,
     timestamp_to_datetime_string,
     pluralize,
 )
 from dbt.events.base_types import WarnLevel, InfoLevel, DebugLevel, ErrorLevel, DynamicLevel
@@ -409,14 +409,51 @@
             "User config should be moved from the 'config' key in profiles.yml to the 'flags' "
             "key in dbt_project.yml."
         )
         # Can't use line_wrap_message here because flags.printer_width isn't available yet
         return warning_tag(f"Deprecated functionality\n\n{description}")
 
 
+class SpacesInModelNameDeprecation(DynamicLevel):
+    def code(self) -> str:
+        return "D014"
+
+    def message(self) -> str:
+        version = ".v" + self.model_version if self.model_version else ""
+        description = (
+            f"Model `{self.model_name}{version}` has spaces in its name. This is deprecated and "
+            "may cause errors when using dbt."
+        )
+
+        if self.level == EventLevel.ERROR.value:
+            description = error_tag(description)
+        elif self.level == EventLevel.WARN.value:
+            description = warning_tag(description)
+
+        return line_wrap_message(description)
+
+
+class TotalModelNamesWithSpacesDeprecation(DynamicLevel):
+    def code(self) -> str:
+        return "D015"
+
+    def message(self) -> str:
+        description = f"Spaces in model names found in {self.count_invalid_names} model(s), which is deprecated."
+
+        if self.show_debug_hint:
+            description += " Run again with `--debug` to see them all."
+
+        if self.level == EventLevel.ERROR.value:
+            description = error_tag(description)
+        elif self.level == EventLevel.WARN.value:
+            description = warning_tag(description)
+
+        return line_wrap_message(description)
+
+
 # =======================================================
 # I - Project parsing
 # =======================================================
 
 
 class InputFileDiffError(DebugLevel):
     def code(self) -> str:
@@ -1095,15 +1132,15 @@
 
 
 class NoNodesForSelectionCriteria(WarnLevel):
     def code(self) -> str:
         return "M030"
 
     def message(self) -> str:
-        return f"The selection criterion '{self.spec_raw}' does not match any nodes"
+        return f"The selection criterion '{self.spec_raw}' does not match any enabled nodes"
 
 
 class DepsLockUpdating(InfoLevel):
     def code(self):
         return "M031"
 
     def message(self) -> str:
```

### Comparing `dbt-core-1.8.0b2/dbt/exceptions.py` & `dbt_core-1.8.0b3/dbt/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     DbtValidationError,
     CommandResultError,
 )
 from dbt.node_types import NodeType, AccessType, REFABLE_NODE_TYPES
 
 from dbt_common.dataclass_schema import ValidationError
 
+from dbt.constants import SECRET_ENV_PREFIX
+
 
 if TYPE_CHECKING:
     import agate
 
 
 class ContractBreakingChangeError(DbtRuntimeError):
     CODE = 10016
@@ -73,42 +75,14 @@
         super().__init__(msg)
 
     def __reduce__(self):
         # see https://stackoverflow.com/a/36342588 for why this is necessary
         return (JSONValidationError, (self.typename, self.errors))
 
 
-class IncompatibleSchemaError(DbtRuntimeError):
-    def __init__(self, expected: str, found: Optional[str] = None) -> None:
-        self.expected = expected
-        self.found = found
-        self.filename = "input file"
-
-        super().__init__(msg=self.get_message())
-
-    def add_filename(self, filename: str):
-        self.filename = filename
-        self.msg = self.get_message()
-
-    def get_message(self) -> str:
-        found_str = "nothing"
-        if self.found is not None:
-            found_str = f'"{self.found}"'
-
-        msg = (
-            f'Expected a schema version of "{self.expected}" in '
-            f"{self.filename}, but found {found_str}. Are you running with a "
-            f"different version of dbt?"
-        )
-        return msg
-
-    CODE = 10014
-    MESSAGE = "Incompatible Schema"
-
-
 class AliasError(DbtValidationError):
     pass
 
 
 class DependencyError(Exception):
     CODE = 10006
     MESSAGE = "Dependency Error"
@@ -357,15 +331,18 @@
         else:
             node_name = "<Configuration>"
 
         dct = {k: self.merged[k] for k in self.merged}
         pretty_vars = json.dumps(dct, sort_keys=True, indent=4)
 
         msg = f"Required var '{self.var_name}' not found in config:\nVars supplied to {node_name} = {pretty_vars}"
-        return msg
+        return scrub_secrets(msg, self.var_secrets())
+
+    def var_secrets(self) -> List[str]:
+        return [v for k, v in self.merged.items() if k.startswith(SECRET_ENV_PREFIX) and v.strip()]
 
 
 class PackageNotFoundForMacroError(CompilationError):
     def __init__(self, package_name: str) -> None:
         self.package_name = package_name
         msg = f"Could not find package '{self.package_name}'"
         super().__init__(msg=msg)
```

### Comparing `dbt-core-1.8.0b2/dbt/flags.py` & `dbt_core-1.8.0b3/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/graph/cli.py` & `dbt_core-1.8.0b3/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/graph/graph.py` & `dbt_core-1.8.0b3/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/graph/queue.py` & `dbt_core-1.8.0b3/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/graph/selector.py` & `dbt_core-1.8.0b3/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/graph/selector_methods.py` & `dbt_core-1.8.0b3/dbt/graph/selector_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,16 @@
                 yield unique_id
 
 
 class GroupSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included in the specified group"""
         for unique_id, node in self.groupable_nodes(included_nodes):
-            if selector == node.config.get("group"):
+            node_group = node.config.get("group")
+            if node_group and fnmatch(node_group, selector):
                 yield unique_id
 
 
 class AccessSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields model nodes matching the specified access level"""
         for unique_id, node in self.parsed_nodes(included_nodes):
```

### Comparing `dbt-core-1.8.0b2/dbt/graph/selector_spec.py` & `dbt_core-1.8.0b3/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/include/README.md` & `dbt_core-1.8.0b3/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/include/starter_project/README.md` & `dbt_core-1.8.0b3/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/include/starter_project/dbt_project.yml` & `dbt_core-1.8.0b3/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/internal_deprecations.py` & `dbt_core-1.8.0b3/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/logger.py` & `dbt_core-1.8.0b3/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/node_types.py` & `dbt_core-1.8.0b3/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/__init__.py` & `dbt_core-1.8.0b3/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/analysis.py` & `dbt_core-1.8.0b3/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/base.py` & `dbt_core-1.8.0b3/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/common.py` & `dbt_core-1.8.0b3/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/docs.py` & `dbt_core-1.8.0b3/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/fixtures.py` & `dbt_core-1.8.0b3/dbt/parser/fixtures.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,22 +22,27 @@
     def generate_unique_id(self, resource_name: str, _: Optional[str] = None) -> str:
         return f"fixture.{self.project.project_name}.{resource_name}"
 
     def parse_file(self, file_block: FileBlock):
         assert isinstance(file_block.file, FixtureSourceFile)
         unique_id = self.generate_unique_id(file_block.name)
 
+        if file_block.file.path.relative_path.endswith(".sql"):
+            rows = file_block.file.contents  # type: ignore
+        else:  # endswith('.csv')
+            rows = self.get_rows(file_block.file.contents)  # type: ignore
+
         fixture = UnitTestFileFixture(
             name=file_block.name,
             path=file_block.file.path.relative_path,
             original_file_path=file_block.path.original_file_path,
             package_name=self.project.project_name,
             unique_id=unique_id,
             resource_type=NodeType.Fixture,
-            rows=self.get_rows(file_block.file.contents),
+            rows=rows,
         )
         self.manifest.add_fixture(file_block.file, fixture)
 
     def get_rows(self, contents) -> List[Dict[str, Any]]:
         rows = []
         dummy_file = StringIO(contents)
         reader = csv.DictReader(dummy_file)
```

### Comparing `dbt-core-1.8.0b2/dbt/parser/generic_test.py` & `dbt_core-1.8.0b3/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/generic_test_builders.py` & `dbt_core-1.8.0b3/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/hooks.py` & `dbt_core-1.8.0b3/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/macros.py` & `dbt_core-1.8.0b3/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/manifest.py` & `dbt_core-1.8.0b3/dbt/parser/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     Union,
     Tuple,
     Set,
 )
 from itertools import chain
 import time
 
-from dbt.context.manifest import generate_query_header_context
+from dbt.context.query_header import generate_query_header_context
 from dbt.contracts.graph.semantic_manifest import SemanticManifest
 from dbt_common.events.base_types import EventLevel
+from dbt_common.exceptions.base import DbtValidationError
 import dbt_common.utils
 import json
 import pprint
 from dbt.mp_context import get_mp_context
 import msgpack
 
 import dbt.exceptions
@@ -39,14 +40,15 @@
     get_adapter_package_names,
     register_adapter,
 )
 from dbt.constants import (
     MANIFEST_FILE_NAME,
     PARTIAL_PARSE_FILE_NAME,
     SEMANTIC_MANIFEST_FILE_NAME,
+    SECRET_ENV_PREFIX,
 )
 from dbt_common.helper_types import PathSet
 from dbt_common.events.functions import fire_event, get_invocation_id, warn_or_error
 from dbt_common.events.types import (
     Note,
 )
 from dbt.events.types import (
@@ -58,14 +60,16 @@
     PartialParsingNotEnabled,
     ParsedFileLoadFailed,
     InvalidDisabledTargetInTestNode,
     NodeNotFoundOrDisabled,
     StateCheckVarsHash,
     DeprecatedModel,
     DeprecatedReference,
+    SpacesInModelNameDeprecation,
+    TotalModelNamesWithSpacesDeprecation,
     UpcomingReferenceDeprecation,
 )
 from dbt.logger import DbtProcessState
 from dbt.node_types import NodeType, AccessType
 from dbt.clients.jinja import get_rendered, MacroStack
 from dbt.clients.jinja_static import statically_extract_macro_calls
 from dbt_common.clients.system import (
@@ -109,14 +113,15 @@
 )
 from dbt.artifacts.resources import NodeRelation, NodeVersion, FileHash
 from dbt.artifacts.schemas.base import Writable
 from dbt.exceptions import (
     TargetNotFoundError,
     AmbiguousAliasError,
     InvalidAccessTypeError,
+    scrub_secrets,
 )
 from dbt.parser.base import Parser
 from dbt.parser.analysis import AnalysisParser
 from dbt.parser.generic_test import GenericTestParser
 from dbt.parser.singular_test import SingularTestParser
 from dbt.parser.docs import DocumentationParser
 from dbt.parser.fixtures import FixtureParser
@@ -516,14 +521,15 @@
                 # parent and child maps will be rebuilt by write_manifest
 
         if not self.skip_parsing or external_nodes_modified:
             # write out the fully parsed manifest
             self.write_manifest_for_partial_parse()
 
         self.check_for_model_deprecations()
+        self.check_for_spaces_in_model_names()
 
         return self.manifest
 
     def safe_update_project_parser_files_partially(self, project_parser_files: Dict) -> Dict:
         if self.saved_manifest is None:
             return project_parser_files
 
@@ -617,14 +623,55 @@
                                 ref_model_name=resolved_ref.name,
                                 ref_model_version=version_to_str(resolved_ref.version),
                                 ref_model_latest_version=str(resolved_ref.latest_version),
                                 ref_model_deprecation_date=resolved_ref.deprecation_date.isoformat(),
                             )
                         )
 
+    def check_for_spaces_in_model_names(self):
+        """Validates that model names do not contain spaces
+
+        If `DEBUG` flag is `False`, logs only first bad model name
+        If `DEBUG` flag is `True`, logs every bad model name
+        If `ALLOW_SPACES_IN_MODEL_NAMES` is `False`, logs are `ERROR` level and an exception is raised if any names are bad
+        If `ALLOW_SPACES_IN_MODEL_NAMES` is `True`, logs are `WARN` level
+        """
+        improper_model_names = 0
+        level = (
+            EventLevel.WARN
+            if self.root_project.args.ALLOW_SPACES_IN_MODEL_NAMES
+            else EventLevel.ERROR
+        )
+
+        for node in self.manifest.nodes.values():
+            if isinstance(node, ModelNode) and " " in node.name:
+                if improper_model_names == 0 or self.root_project.args.DEBUG:
+                    fire_event(
+                        SpacesInModelNameDeprecation(
+                            model_name=node.name,
+                            model_version=version_to_str(node.version),
+                            level=level.value,
+                        ),
+                        level=level,
+                    )
+                improper_model_names += 1
+
+        if improper_model_names > 0:
+            fire_event(
+                TotalModelNamesWithSpacesDeprecation(
+                    count_invalid_names=improper_model_names,
+                    show_debug_hint=(not self.root_project.args.DEBUG),
+                    level=level.value,
+                ),
+                level=level,
+            )
+
+            if level == EventLevel.ERROR:
+                raise DbtValidationError("Model names cannot contain spaces")
+
     def load_and_parse_macros(self, project_parser_files):
         for project in self.all_projects.values():
             if project.project_name not in project_parser_files:
                 continue
             parser_files = project_parser_files[project.project_name]
             if "MacroParser" in parser_files:
                 parser = MacroParser(project, self.manifest)
@@ -831,21 +878,14 @@
             != manifest.state_check.project_env_vars_hash
         ):
             fire_event(
                 UnableToPartialParse(reason="env vars used in dbt_project.yml have changed")
             )
             valid = False
             reparse_reason = ReparseReason.proj_env_vars_changed
-        if (
-            self.manifest.state_check.profile_env_vars_hash
-            != manifest.state_check.profile_env_vars_hash
-        ):
-            fire_event(UnableToPartialParse(reason="env vars used in profiles.yml have changed"))
-            valid = False
-            reparse_reason = ReparseReason.prof_env_vars_changed
 
         missing_keys = {
             k
             for k in self.manifest.state_check.project_hashes
             if k not in manifest.state_check.project_hashes
         }
         if missing_keys:
@@ -947,67 +987,69 @@
         # Create a FileHash of vars string, profile name and target name
         # This does not capture vars in dbt_project, just the command line
         # arg vars, but since any changes to that file will cause state_check
         # to not pass, it doesn't matter.  If we move to more granular checking
         # of env_vars, that would need to change.
         # We are using the parsed cli_vars instead of config.args.vars, in order
         # to sort them and avoid reparsing because of ordering issues.
+        secret_vars = [
+            v for k, v in config.cli_vars.items() if k.startswith(SECRET_ENV_PREFIX) and v.strip()
+        ]
         stringified_cli_vars = pprint.pformat(config.cli_vars)
         vars_hash = FileHash.from_contents(
             "\x00".join(
                 [
                     stringified_cli_vars,
                     getattr(config.args, "profile", "") or "",
                     getattr(config.args, "target", "") or "",
                     __version__,
                 ]
             )
         )
         fire_event(
             StateCheckVarsHash(
                 checksum=vars_hash.checksum,
-                vars=stringified_cli_vars,
+                vars=scrub_secrets(stringified_cli_vars, secret_vars),
                 profile=config.args.profile,
                 target=config.args.target,
                 version=__version__,
             )
         )
 
         # Create a FileHash of the env_vars in the project
         key_list = list(config.project_env_vars.keys())
         key_list.sort()
         env_var_str = ""
         for key in key_list:
             env_var_str += f"{key}:{config.project_env_vars[key]}|"
         project_env_vars_hash = FileHash.from_contents(env_var_str)
 
-        # Create a FileHash of the env_vars in the project
-        key_list = list(config.profile_env_vars.keys())
-        key_list.sort()
-        env_var_str = ""
-        for key in key_list:
-            env_var_str += f"{key}:{config.profile_env_vars[key]}|"
-        profile_env_vars_hash = FileHash.from_contents(env_var_str)
-
-        # Create a FileHash of the profile file
-        profile_path = os.path.join(get_flags().PROFILES_DIR, "profiles.yml")
-        with open(profile_path) as fp:
-            profile_hash = FileHash.from_contents(fp.read())
+        # Create a hash of the connection_info, which user has access to in
+        # jinja context. Thus attributes here may affect the parsing result.
+        # Ideally we should not expose all of the connection info to the jinja.
+
+        # Renaming this variable mean that we will have to do a whole lot more
+        # change to make sure the previous manifest can be loaded correctly.
+        # This is an example of naming should be chosen based on the functionality
+        # rather than the implementation details.
+        connection_keys = list(config.credentials.connection_info())
+        # avoid reparsing because of ordering issues
+        connection_keys.sort()
+        profile_hash = FileHash.from_contents(pprint.pformat(connection_keys))
 
         # Create a FileHashes for dbt_project for all dependencies
         project_hashes = {}
         for name, project in all_projects.items():
             path = os.path.join(project.project_root, "dbt_project.yml")
             with open(path) as fp:
                 project_hashes[name] = FileHash.from_contents(fp.read())
 
         # Create the ManifestStateCheck object
         state_check = ManifestStateCheck(
             project_env_vars_hash=project_env_vars_hash,
-            profile_env_vars_hash=profile_env_vars_hash,
             vars_hash=vars_hash,
             profile_hash=profile_hash,
             project_hashes=project_hashes,
         )
         return state_check
 
     def save_macros_to_adapter(self, adapter):
```

### Comparing `dbt-core-1.8.0b2/dbt/parser/models.py` & `dbt_core-1.8.0b3/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/partial.py` & `dbt_core-1.8.0b3/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/read_files.py` & `dbt_core-1.8.0b3/dbt/parser/read_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,19 +141,19 @@
     fp_list = filesystem_search(project, paths, extension, ignore_spec)
     # file block list
     fb_list = []
     for fp in fp_list:
         if parse_file_type == ParseFileType.Seed:
             fb_list.append(load_seed_source_file(fp, project.project_name))
         # singular tests live in /tests but only generic tests live
-        # in /tests/generic so we want to skip those
+        # in /tests/generic and fixtures in /tests/fixture so we want to skip those
         else:
             if parse_file_type == ParseFileType.SingularTest:
                 path = pathlib.Path(fp.relative_path)
-                if path.parts[0] == "generic":
+                if path.parts[0] in ["generic", "fixtures"]:
                     continue
             file = load_source_file(fp, parse_file_type, project.project_name, saved_files)
             # only append the list if it has contents. added to fix #3568
             if file:
                 fb_list.append(file)
     return fb_list
 
@@ -427,12 +427,12 @@
         ParseFileType.Schema: {
             "paths": project.all_source_paths,
             "extensions": [".yml", ".yaml"],
             "parser": "SchemaParser",
         },
         ParseFileType.Fixture: {
             "paths": project.fixture_paths,
-            "extensions": [".csv"],
+            "extensions": [".csv", ".sql"],
             "parser": "FixtureParser",
         },
     }
     return file_types
```

### Comparing `dbt-core-1.8.0b2/dbt/parser/schema_generic_tests.py` & `dbt_core-1.8.0b3/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/schema_renderer.py` & `dbt_core-1.8.0b3/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/schema_yaml_readers.py` & `dbt_core-1.8.0b3/dbt/parser/schema_yaml_readers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/schemas.py` & `dbt_core-1.8.0b3/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/search.py` & `dbt_core-1.8.0b3/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/seeds.py` & `dbt_core-1.8.0b3/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/singular_test.py` & `dbt_core-1.8.0b3/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/snapshots.py` & `dbt_core-1.8.0b3/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/sources.py` & `dbt_core-1.8.0b3/dbt/parser/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         ):
             # Metadata-based freshness is being used by default for this node,
             # but is not available through the configured adapter, so warn the
             # user that freshness info will not be collected for this node at
             # runtime.
             fire_event(
                 FreshnessConfigProblem(
-                    msg=f"The configured adapter does not support metadata-based freshness. A loaded_at_field must be specified for source '{source.name}'."
+                    msg=f"The configured adapter does not support metadata-based freshness. A loaded_at_field must be specified for source '{source.name}.{table.name}'."
                 )
             )
 
         # relation name is added after instantiation because the adapter does
         # not provide the relation name for a UnpatchedSourceDefinition object
         parsed_source.relation_name = self._get_relation_name(parsed_source)
         return parsed_source
```

### Comparing `dbt-core-1.8.0b2/dbt/parser/sql.py` & `dbt_core-1.8.0b3/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/parser/unit_tests.py` & `dbt_core-1.8.0b3/dbt/parser/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,24 +64,32 @@
         # Create UnitTestNode based on model being tested. Since selection has
         # already been done, we don't have to care about fields that are necessary
         # for selection.
         # Note: no depends_on, that's added later using input nodes
         name = test_case.name
         if tested_node.is_versioned:
             name = name + f"_v{tested_node.version}"
+        expected_sql: Optional[str] = None
+        if test_case.expect.format == UnitTestFormat.SQL:
+            expected_rows: List[Dict[str, Any]] = []
+            expected_sql = test_case.expect.rows  # type: ignore
+        else:
+            assert isinstance(test_case.expect.rows, List)
+            expected_rows = deepcopy(test_case.expect.rows)
+
+        assert isinstance(expected_rows, List)
         unit_test_node = UnitTestNode(
             name=name,
             resource_type=NodeType.Unit,
             package_name=test_case.package_name,
             path=get_pseudo_test_path(name, test_case.original_file_path),
             original_file_path=test_case.original_file_path,
             unique_id=test_case.unique_id,
             config=UnitTestNodeConfig(
-                materialized="unit",
-                expected_rows=deepcopy(test_case.expect.rows),  # type:ignore
+                materialized="unit", expected_rows=expected_rows, expected_sql=expected_sql
             ),
             raw_code=tested_node.raw_code,
             database=tested_node.database,
             schema=tested_node.schema,
             alias=name,
             fqn=test_case.unique_id.split("."),
             checksum=FileHash.empty(),
@@ -128,15 +136,15 @@
                 "original_file_path": unit_test_node.original_file_path,
                 "config": ModelConfig(materialized="ephemeral"),
                 "database": original_input_node.database,
                 "alias": original_input_node.identifier,
                 "schema": original_input_node.schema,
                 "fqn": original_input_node.fqn,
                 "checksum": FileHash.empty(),
-                "raw_code": self._build_fixture_raw_code(given.rows, None),
+                "raw_code": self._build_fixture_raw_code(given.rows, None, given.format),
                 "package_name": original_input_node.package_name,
                 "unique_id": f"model.{original_input_node.package_name}.{input_name}",
                 "name": input_name,
                 "path": f"{input_name}.sql",
             }
 
             if original_input_node.resource_type in (
@@ -168,20 +176,23 @@
             # Populate this_input_node_unique_id if input fixture represents node being tested
             if original_input_node == tested_node:
                 unit_test_node.this_input_node_unique_id = input_node.unique_id
 
             # Add unique ids of input_nodes to depends_on
             unit_test_node.depends_on.nodes.append(input_node.unique_id)
 
-    def _build_fixture_raw_code(self, rows, column_name_to_data_types) -> str:
+    def _build_fixture_raw_code(self, rows, column_name_to_data_types, fixture_format) -> str:
         # We're not currently using column_name_to_data_types, but leaving here for
         # possible future use.
-        return ("{{{{ get_fixture_sql({rows}, {column_name_to_data_types}) }}}}").format(
-            rows=rows, column_name_to_data_types=column_name_to_data_types
-        )
+        if fixture_format == UnitTestFormat.SQL:
+            return rows
+        else:
+            return ("{{{{ get_fixture_sql({rows}, {column_name_to_data_types}) }}}}").format(
+                rows=rows, column_name_to_data_types=column_name_to_data_types
+            )
 
     def _get_original_input_node(self, input: str, tested_node: ModelNode, test_case_name: str):
         """
         Returns the original input node as defined in the project given an input reference
         and the node being tested.
 
         input: str representing how input node is referenced in tested model sql
@@ -348,21 +359,37 @@
             if not (isinstance(ut_fixture.rows, str) or isinstance(ut_fixture.fixture, str)):
                 raise ParsingError(
                     f"Unit test {unit_test_definition.name} has {fixture_type} rows or fixtures "
                     f"which do not match format {ut_fixture.format}.  Expected string."
                 )
 
             if ut_fixture.fixture:
-                # find fixture file object and store unit_test_definition unique_id
-                fixture = self._get_fixture(ut_fixture.fixture, self.project.project_name)
-                fixture_source_file = self.manifest.files[fixture.file_id]
-                fixture_source_file.unit_tests.append(unit_test_definition.unique_id)
-                ut_fixture.rows = fixture.rows
+                ut_fixture.rows = self.get_fixture_file_rows(
+                    ut_fixture.fixture, self.project.project_name, unit_test_definition.unique_id
+                )
             else:
                 ut_fixture.rows = self._convert_csv_to_list_of_dicts(ut_fixture.rows)
+        elif ut_fixture.format == UnitTestFormat.SQL:
+            if not (isinstance(ut_fixture.rows, str) or isinstance(ut_fixture.fixture, str)):
+                raise ParsingError(
+                    f"Unit test {unit_test_definition.name} has {fixture_type} rows or fixtures "
+                    f"which do not match format {ut_fixture.format}.  Expected string."
+                )
+
+            if ut_fixture.fixture:
+                ut_fixture.rows = self.get_fixture_file_rows(
+                    ut_fixture.fixture, self.project.project_name, unit_test_definition.unique_id
+                )
+
+    def get_fixture_file_rows(self, fixture_name, project_name, utdef_unique_id):
+        # find fixture file object and store unit_test_definition unique_id
+        fixture = self._get_fixture(fixture_name, project_name)
+        fixture_source_file = self.manifest.files[fixture.file_id]
+        fixture_source_file.unit_tests.append(utdef_unique_id)
+        return fixture.rows
 
     def _convert_csv_to_list_of_dicts(self, csv_string: str) -> List[Dict[str, Any]]:
         dummy_file = StringIO(csv_string)
         reader = csv.DictReader(dummy_file)
         rows = []
         for row in reader:
             rows.append(row)
```

### Comparing `dbt-core-1.8.0b2/dbt/plugins/__init__.py` & `dbt_core-1.8.0b3/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/plugins/manager.py` & `dbt_core-1.8.0b3/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/plugins/manifest.py` & `dbt_core-1.8.0b3/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/base.py` & `dbt_core-1.8.0b3/dbt/task/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import threading
 import time
 import traceback
 from abc import ABCMeta, abstractmethod
 from contextlib import nullcontext
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, Union, Set
+from typing import Any, Dict, List, Optional, Set
 
 from dbt.compilation import Compiler
 import dbt_common.exceptions.base
 import dbt.exceptions
 from dbt import tracking
-from dbt.config import RuntimeConfig, Project
+from dbt.cli.flags import Flags
+from dbt.config import RuntimeConfig
 from dbt.config.profile import read_profile
 from dbt.constants import DBT_PROJECT_FILE_NAME
 from dbt.contracts.graph.manifest import Manifest
 from dbt.artifacts.resources.types import NodeType
 from dbt.artifacts.schemas.results import TimingInfo, collect_timing_info
 from dbt.artifacts.schemas.results import NodeStatus, RunningStatus, RunStatus
 from dbt.artifacts.schemas.run import RunResult
@@ -45,20 +46,14 @@
 )
 from dbt.flags import get_flags
 from dbt.graph import Graph
 from dbt.logger import log_manager
 from dbt.task.printer import print_run_result_error
 
 
-class NoneConfig:
-    @classmethod
-    def from_args(cls, args):
-        return None
-
-
 def read_profiles(profiles_dir=None):
     """This is only used for some error handling"""
     if profiles_dir is None:
         profiles_dir = get_flags().PROFILES_DIR
 
     raw_profiles = read_profile(profiles_dir)
 
@@ -67,53 +62,32 @@
     else:
         profiles = {k: v for (k, v) in raw_profiles.items() if k != "config"}
 
     return profiles
 
 
 class BaseTask(metaclass=ABCMeta):
-    ConfigType: Union[Type[NoneConfig], Type[Project]] = NoneConfig
-
-    def __init__(self, args, config, project=None) -> None:
+    def __init__(self, args: Flags) -> None:
         self.args = args
-        self.config = config
-        self.project = config if isinstance(config, Project) else project
 
     @classmethod
-    def pre_init_hook(cls, args):
+    def pre_init_hook(cls, args: Flags):
         """A hook called before the task is initialized."""
         if args.log_format == "json":
             log_manager.format_json()
         else:
             log_manager.format_text()
 
     @classmethod
     def set_log_format(cls):
         if get_flags().LOG_FORMAT == "json":
             log_manager.format_json()
         else:
             log_manager.format_text()
 
-    @classmethod
-    def from_args(cls, args, *pargs, **kwargs):
-        try:
-            # This is usually RuntimeConfig
-            config = cls.ConfigType.from_args(args)
-        except dbt.exceptions.DbtProjectError as exc:
-            fire_event(LogDbtProjectError(exc=str(exc)))
-
-            tracking.track_invalid_invocation(args=args, result_type=exc.result_type)
-            raise dbt_common.exceptions.DbtRuntimeError("Could not run dbt") from exc
-        except dbt.exceptions.DbtProfileError as exc:
-            all_profile_names = list(read_profiles(get_flags().PROFILES_DIR).keys())
-            fire_event(LogDbtProfileError(exc=str(exc), profiles=all_profile_names))
-            tracking.track_invalid_invocation(args=args, result_type=exc.result_type)
-            raise dbt_common.exceptions.DbtRuntimeError("Could not run dbt") from exc
-        return cls(args, config, *pargs, **kwargs)
-
     @abstractmethod
     def run(self):
         raise dbt_common.exceptions.base.NotImplementedError("Not Implemented")
 
     def interpret_results(self, results):
         return True
 
@@ -149,18 +123,19 @@
     return nearest_project_dir
 
 
 # TODO: look into deprecating this class in favor of several small functions that
 # produce the same behavior. currently this class only contains manifest compilation,
 # holding a manifest, and moving direcories.
 class ConfiguredTask(BaseTask):
-    ConfigType = RuntimeConfig
-
-    def __init__(self, args, config, manifest: Optional[Manifest] = None) -> None:
-        super().__init__(args, config)
+    def __init__(
+        self, args: Flags, config: RuntimeConfig, manifest: Optional[Manifest] = None
+    ) -> None:
+        super().__init__(args)
+        self.config = config
         self.graph: Optional[Graph] = None
         self.manifest = manifest
         self.compiler = Compiler(self.config)
 
     def compile_manifest(self):
         if self.manifest is None:
             raise DbtInternalError("compile_manifest called before manifest was loaded")
@@ -170,17 +145,30 @@
         self.graph = self.compiler.compile(self.manifest)
 
         compile_time = time.perf_counter() - start_compile_manifest
         if dbt.tracking.active_user is not None:
             dbt.tracking.track_runnable_timing({"graph_compilation_elapsed": compile_time})
 
     @classmethod
-    def from_args(cls, args, *pargs, **kwargs):
+    def from_args(cls, args: Flags, *pargs, **kwargs):
         move_to_nearest_project_dir(args.project_dir)
-        return super().from_args(args, *pargs, **kwargs)
+        try:
+            # This is usually RuntimeConfig
+            config = RuntimeConfig.from_args(args)
+        except dbt.exceptions.DbtProjectError as exc:
+            fire_event(LogDbtProjectError(exc=str(exc)))
+
+            tracking.track_invalid_invocation(args=args, result_type=exc.result_type)
+            raise dbt_common.exceptions.DbtRuntimeError("Could not run dbt") from exc
+        except dbt.exceptions.DbtProfileError as exc:
+            all_profile_names = list(read_profiles(get_flags().PROFILES_DIR).keys())
+            fire_event(LogDbtProfileError(exc=str(exc), profiles=all_profile_names))
+            tracking.track_invalid_invocation(args=args, result_type=exc.result_type)
+            raise dbt_common.exceptions.DbtRuntimeError("Could not run dbt") from exc
+        return cls(args, config, *pargs, **kwargs)
 
 
 class ExecutionContext:
     """During execution and error handling, dbt makes use of mutable state:
     timing information and the newest (compiled vs executed) form of the node.
     """
 
@@ -483,15 +471,15 @@
 
     def do_skip(self, cause=None):
         self.skip = True
         self.skip_cause = cause
 
 
 def resource_types_from_args(
-    args, all_resource_values: Set[NodeType], default_resource_values: Set[NodeType]
+    args: Flags, all_resource_values: Set[NodeType], default_resource_values: Set[NodeType]
 ) -> Set[NodeType]:
 
     if not args.resource_types:
         resource_types = default_resource_values
     else:
         # This is a list of strings, not NodeTypes
         arg_resource_types = set(args.resource_types)
```

### Comparing `dbt-core-1.8.0b2/dbt/task/build.py` & `dbt_core-1.8.0b3/dbt/task/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from .run import RunTask, ModelRunner as run_model_runner
 from .snapshot import SnapshotRunner as snapshot_model_runner
 from .seed import SeedRunner as seed_runner
 from .test import TestRunner as test_runner
 
 from dbt.artifacts.schemas.results import NodeStatus, RunStatus
 from dbt.artifacts.schemas.run import RunResult
+from dbt.cli.flags import Flags
+from dbt.config.runtime import RuntimeConfig
+from dbt.contracts.graph.manifest import Manifest
 from dbt.graph import ResourceTypeSelector, GraphQueue, Graph
 from dbt.node_types import NodeType
 from dbt.task.test import TestSelector
 from dbt.task.base import BaseRunner, resource_types_from_args
 from dbt_common.events.functions import fire_event
 from dbt.events.types import LogNodeNoOpResult
 from dbt.exceptions import DbtInternalError
@@ -70,15 +73,15 @@
         NodeType.Seed: seed_runner,
         NodeType.Test: test_runner,
         NodeType.Unit: test_runner,
         NodeType.SavedQuery: SavedQueryRunner,
     }
     ALL_RESOURCE_VALUES = frozenset({x for x in RUNNER_MAP.keys()})
 
-    def __init__(self, args, config, manifest) -> None:
+    def __init__(self, args: Flags, config: RuntimeConfig, manifest: Manifest) -> None:
         super().__init__(args, config, manifest)
         self.selected_unit_tests: Set = set()
         self.model_to_unit_test_map: Dict[str, List] = {}
 
     def resource_types(self, no_unit_tests=False):
         resource_types = resource_types_from_args(
             self.args, set(self.ALL_RESOURCE_VALUES), set(self.ALL_RESOURCE_VALUES)
```

### Comparing `dbt-core-1.8.0b2/dbt/task/clean.py` & `dbt_core-1.8.0b3/dbt/task/clean.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,28 @@
 from dbt_common.events.functions import fire_event
 from dbt.events.types import (
     CheckCleanPath,
     ConfirmCleanPath,
     FinishedCleanPaths,
 )
 from dbt_common.exceptions import DbtRuntimeError
+from dbt.cli.flags import Flags
+from dbt.config.project import Project
 from dbt.task.base import (
     BaseTask,
     move_to_nearest_project_dir,
 )
 
 
 class CleanTask(BaseTask):
+    def __init__(self, args: Flags, config: Project):
+        super().__init__(args)
+        self.config = config
+        self.project = config
+
     def run(self):
         """
         This function takes all the paths in the target file
         and cleans the project paths that are not protected.
         """
         project_dir = move_to_nearest_project_dir(self.args.project_dir)
```

### Comparing `dbt-core-1.8.0b2/dbt/task/clone.py` & `dbt_core-1.8.0b3/dbt/task/clone.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/compile.py` & `dbt_core-1.8.0b3/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/debug.py` & `dbt_core-1.8.0b3/dbt/task/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DebugCmdOut,
     DebugCmdResult,
 )
 import dbt_common.clients.system
 import dbt.exceptions
 import dbt_common.exceptions
 from dbt.adapters.factory import get_adapter, register_adapter
+from dbt.cli.flags import Flags
 from dbt.config import PartialProject, Project, Profile
 from dbt.config.renderer import DbtProjectYamlRenderer, ProfileRenderer
 from dbt.artifacts.schemas.results import RunStatus
 from dbt.clients.yaml_helper import load_yaml_text
 from dbt.links import ProfileConfigDocs
 from dbt_common.ui import green, red
 from dbt_common.events.format import pluralize
@@ -73,16 +74,16 @@
 
 class DebugRunStatus(Flag):
     SUCCESS = True
     FAIL = False
 
 
 class DebugTask(BaseTask):
-    def __init__(self, args, config) -> None:
-        super().__init__(args, config)
+    def __init__(self, args: Flags) -> None:
+        super().__init__(args)
         self.profiles_dir = args.PROFILES_DIR
         self.profile_path = os.path.join(self.profiles_dir, "profiles.yml")
         try:
             self.project_dir = get_nearest_project_dir(self.args.project_dir)
         except dbt_common.exceptions.DbtBaseException:
             # we probably couldn't find a project directory. Set project dir
             # to whatever was given, or default to the current directory.
@@ -93,21 +94,14 @@
         self.project_path = os.path.join(self.project_dir, "dbt_project.yml")
         self.cli_vars: Dict[str, Any] = args.vars
 
         # set by _load_*
         self.profile: Optional[Profile] = None
         self.raw_profile_data: Optional[Dict[str, Any]] = None
         self.profile_name: Optional[str] = None
-        self.project: Optional[Project] = None
-
-    @property
-    def project_profile(self):
-        if self.project is None:
-            return None
-        return self.project.profile_name
 
     def run(self) -> bool:
         # WARN: this is a legacy workflow that is not compatible with other runtime flags
         if self.args.config_dir:
             fire_event(
                 OpenCommand(
                     open_cmd=dbt_common.clients.system.open_dir_cmd(),
```

### Comparing `dbt-core-1.8.0b2/dbt/task/deps.py` & `dbt_core-1.8.0b3/dbt/task/deps.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from dbt.config.renderer import PackageRenderer
 from dbt.config.project import package_config_from_data, load_yml_dict
 from dbt.constants import PACKAGE_LOCK_FILE_NAME, PACKAGE_LOCK_HASH_KEY
 from dbt.deps.base import downloads_directory
 from dbt.deps.resolver import resolve_lock_packages, resolve_packages
 from dbt.deps.registry import RegistryPinnedPackage
-from dbt.contracts.project import Package
+from dbt.contracts.project import PackageSpec
 
 
 from dbt_common.events.functions import fire_event
 from dbt_common.events.types import (
     Formatting,
 )
 from dbt.events.types import (
@@ -40,15 +40,15 @@
 
 
 class dbtPackageDumper(yaml.Dumper):
     def increase_indent(self, flow=False, indentless=False):
         return super(dbtPackageDumper, self).increase_indent(flow, False)
 
 
-def _create_sha1_hash(packages: List[Package]) -> str:
+def _create_sha1_hash(packages: List[PackageSpec]) -> str:
     """Create a SHA1 hash of the packages list,
     this is used to determine if the packages for current execution matches
     the previous lock.
 
     Args:
         list[Packages]: list of packages specified that are already rendered
 
@@ -90,22 +90,23 @@
         packages_yml_entry[version_key] = version
 
     return packages_yml_entry
 
 
 class DepsTask(BaseTask):
     def __init__(self, args: Any, project: Project) -> None:
+        super().__init__(args=args)
         # N.B. This is a temporary fix for a bug when using relative paths via
         # --project-dir with deps.  A larger overhaul of our path handling methods
         # is needed to fix this the "right" way.
         # See GH-7615
         project.project_root = str(Path(project.project_root).resolve())
+        self.project = project
 
         move_to_nearest_project_dir(project.project_root)
-        super().__init__(args=args, config=None, project=project)
         self.cli_vars = args.vars
 
     def track_package_install(
         self, package_name: str, source_type: str, version: Optional[str]
     ) -> None:
         # Hub packages do not need to be hashed, as they are public
         if source_type == "local":
```

### Comparing `dbt-core-1.8.0b2/dbt/task/docs/generate.py` & `dbt_core-1.8.0b3/dbt/task/docs/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/docs/index.html` & `dbt_core-1.8.0b3/dbt/task/docs/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/docs/serve.py` & `dbt_core-1.8.0b3/dbt/task/docs/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/init.py` & `dbt_core-1.8.0b3/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/list.py` & `dbt_core-1.8.0b3/dbt/task/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     Exposure,
     SourceDefinition,
     Metric,
     SavedQuery,
     SemanticModel,
     UnitTestDefinition,
 )
+from dbt.cli.flags import Flags
+from dbt.config.runtime import RuntimeConfig
+from dbt.contracts.graph.manifest import Manifest
 from dbt.flags import get_flags
 from dbt.graph import ResourceTypeSelector
 from dbt.task.base import resource_types_from_args
 from dbt.task.runnable import GraphRunnableTask
 from dbt.task.test import TestSelector
 from dbt.node_types import NodeType
 from dbt_common.events.functions import (
@@ -50,15 +53,15 @@
             "resource_type",
             "source_name",
             "original_file_path",
             "unique_id",
         )
     )
 
-    def __init__(self, args, config, manifest) -> None:
+    def __init__(self, args: Flags, config: RuntimeConfig, manifest: Manifest) -> None:
         super().__init__(args, config, manifest)
         if self.args.models:
             if self.args.select:
                 raise DbtRuntimeError('"models" and "select" are mutually exclusive arguments')
             if self.args.resource_types:
                 raise DbtRuntimeError(
                     '"models" and "resource_type" are mutually exclusive ' "arguments"
```

### Comparing `dbt-core-1.8.0b2/dbt/task/printer.py` & `dbt_core-1.8.0b3/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/retry.py` & `dbt_core-1.8.0b3/dbt/task/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "test": CliCommand.TEST,
     "run": CliCommand.RUN,
     "run-operation": CliCommand.RUN_OPERATION,
 }
 
 
 class RetryTask(ConfiguredTask):
-    def __init__(self, args, config) -> None:
+    def __init__(self, args: Flags, config: RuntimeConfig) -> None:
         # load previous run results
         state_path = args.state or config.target_path
         self.previous_results = load_result_state(
             Path(config.project_root) / Path(state_path) / "run_results.json"
         )
         if not self.previous_results:
             raise DbtRuntimeError(
```

### Comparing `dbt-core-1.8.0b2/dbt/task/run.py` & `dbt_core-1.8.0b3/dbt/task/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     print_run_end_messages,
     get_counts,
 )
 from datetime import datetime
 from dbt import tracking
 from dbt import utils
 from dbt.adapters.base import BaseRelation
+from dbt.cli.flags import Flags
 from dbt.clients.jinja import MacroGenerator
+from dbt.config.runtime import RuntimeConfig
 from dbt.context.providers import generate_runtime_model_context
 from dbt.contracts.graph.nodes import HookNode, ResultNode
+from dbt.contracts.graph.manifest import Manifest
 from dbt.artifacts.schemas.results import NodeStatus, RunStatus, RunningStatus, BaseResult
 from dbt.artifacts.schemas.run import RunResult
 from dbt.artifacts.resources import Hook
 from dbt.exceptions import (
     CompilationError,
     DbtInternalError,
     DbtRuntimeError,
@@ -301,15 +304,15 @@
         for relation in self._materialization_relations(result, model):
             self.adapter.cache_added(relation.incorporate(dbt_created=True))
 
         return self._build_run_model_result(model, context)
 
 
 class RunTask(CompileTask):
-    def __init__(self, args, config, manifest) -> None:
+    def __init__(self, args: Flags, config: RuntimeConfig, manifest: Manifest) -> None:
         super().__init__(args, config, manifest)
         self.ran_hooks: List[HookNode] = []
         self._total_executed = 0
 
     def index_offset(self, value: int) -> int:
         return self._total_executed + value
```

### Comparing `dbt-core-1.8.0b2/dbt/task/run_operation.py` & `dbt_core-1.8.0b3/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/runnable.py` & `dbt_core-1.8.0b3/dbt/task/runnable.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import dbt_common.utils.formatting
 
 import dbt.exceptions
 import dbt.tracking
 import dbt.utils
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.factory import get_adapter
+from dbt.cli.flags import Flags
+from dbt.config.runtime import RuntimeConfig
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import ResultNode
 from dbt.artifacts.schemas.results import NodeStatus, RunningStatus, RunStatus, BaseResult
 from dbt.artifacts.schemas.run import RunExecutionResult, RunResult
 from dbt.contracts.state import PreviousState
 from dbt_common.events.contextvars import log_contextvars, task_contextvars
 from dbt_common.events.functions import fire_event, warn_or_error
@@ -61,16 +63,17 @@
 RESULT_FILE_NAME = "run_results.json"
 RUNNING_STATE = DbtProcessState("running")
 
 
 class GraphRunnableTask(ConfiguredTask):
     MARK_DEPENDENT_ERRORS_STATUSES = [NodeStatus.Error]
 
-    def __init__(self, args, config, manifest) -> None:
+    def __init__(self, args: Flags, config: RuntimeConfig, manifest: Manifest) -> None:
         super().__init__(args, config, manifest)
+        self.config = config
         self._flattened_nodes: Optional[List[ResultNode]] = None
         self._raise_next_tick: Optional[DbtRuntimeError] = None
         self._skipped_children: Dict[str, Optional[RunResult]] = {}
         self.job_queue: Optional[GraphQueue] = None
         self.node_results: List[BaseResult] = []
         self.num_nodes: int = 0
         self.previous_state: Optional[PreviousState] = None
@@ -119,15 +122,17 @@
             # use pre-defined selector (--selector) with default: true
             fire_event(DefaultSelector(name=default_selector_name))
             spec = self.config.get_selector(default_selector_name)
         else:
             # This is what's used with no default selector and no selection
             # use --select and --exclude args
             spec = parse_difference(self.selection_arg, self.exclusion_arg, indirect_selection)
-        return spec
+        # mypy complains because the return values of get_selector and parse_difference
+        # are different
+        return spec  # type: ignore
 
     @abstractmethod
     def get_node_selector(self) -> NodeSelector:
         raise NotImplementedError(f"get_node_selector not implemented for task {type(self)}")
 
     def defer_to_manifest(self, adapter, selected_uids: AbstractSet[str]):
         deferred_manifest = self._get_deferred_manifest()
@@ -619,15 +624,17 @@
             schema = relation.schema
             with adapter.connection_named(f"create_{db}_{schema}"):
                 adapter.create_schema(relation)
 
         list_futures = []
         create_futures = []
 
-        with dbt_common.utils.executor(self.config) as tpe:
+        # TODO: following has a mypy issue because profile and project config
+        # defines threads as int and HasThreadingConfig defines it as Optional[int]
+        with dbt_common.utils.executor(self.config) as tpe:  # type: ignore
             for req in required_databases:
                 if req.database is None:
                     name = "list_schemas"
                 else:
                     name = f"list_{req.database}"
                 fut = tpe.submit_connected(adapter, name, list_schemas, req)
                 list_futures.append(fut)
```

### Comparing `dbt-core-1.8.0b2/dbt/task/seed.py` & `dbt_core-1.8.0b3/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/show.py` & `dbt_core-1.8.0b3/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/snapshot.py` & `dbt_core-1.8.0b3/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/sql.py` & `dbt_core-1.8.0b3/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/task/test.py` & `dbt_core-1.8.0b3/dbt/task/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     should_error: bool
     adapter_response: Dict[str, Any]
     diff: Optional[UnitTestDiff] = None
 
 
 class TestRunner(CompileRunner):
     _ANSI_ESCAPE = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
+    _LOG_TEST_RESULT_EVENTS = LogTestResult
 
     def describe_node_name(self):
         if self.node.resource_type == NodeType.Unit:
             name = f"{self.node.model}::{self.node.versioned_name}"
             return name
         else:
             return self.node.name
@@ -98,15 +99,15 @@
     def describe_node(self):
         return f"{self.node.resource_type} {self.describe_node_name()}"
 
     def print_result_line(self, result):
         model = result.node
 
         fire_event(
-            LogTestResult(
+            self._LOG_TEST_RESULT_EVENTS(
                 name=self.describe_node_name(),
                 status=str(result.status),
                 index=self.node_index,
                 num_models=self.num_nodes,
                 execution_time=result.execution_time,
                 node_info=model.node_info,
                 num_failures=result.failures,
@@ -276,15 +277,17 @@
         message = None
         failures = 0
         if severity == "ERROR" and result.should_error:
             status = TestStatus.Fail
             message = f"Got {num_errors}, configured to fail if {test.config.error_if}"
             failures = result.failures
         elif result.should_warn:
-            if get_flags().WARN_ERROR:
+            if get_flags().WARN_ERROR or get_flags().WARN_ERROR_OPTIONS.includes(
+                self._LOG_TEST_RESULT_EVENTS.__name__
+            ):
                 status = TestStatus.Fail
                 message = f"Got {num_errors}, configured to fail if {test.config.warn_if}"
             else:
                 status = TestStatus.Warn
                 message = f"Got {num_errors}, configured to warn if {test.config.warn_if}"
             failures = result.failures
         else:
```

### Comparing `dbt-core-1.8.0b2/dbt/tests/fixtures/project.py` & `dbt_core-1.8.0b3/dbt/tests/fixtures/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 from pathlib import Path
+from typing import Mapping
+
 import pytest  # type: ignore
 import random
 from argparse import Namespace
 from datetime import datetime
 import warnings
 import yaml
 
@@ -489,19 +491,26 @@
                 order by table_name
                 """
         sql = sql.format("{} ilike '{}'".format("table_schema", self.test_schema))
         result = self.run_sql(sql, fetch="all")
         return {model_name: materialization for (model_name, materialization) in result}
 
 
+@pytest.fixture(scope="class")
+def environment() -> Mapping[str, str]:
+    # By default, fixture initialization is done with the following environment
+    # from the os, but this fixture provides a way to customize the environment.
+    return os.environ
+
+
 # Housekeeping that needs to be done before we start setting up any test fixtures.
 @pytest.fixture(scope="class")
-def initialization() -> None:
+def initialization(environment) -> None:
     # Create an "invocation context," which dbt application code relies on.
-    set_invocation_context(os.environ)
+    set_invocation_context(environment)
 
     # Enable caches used between test runs, for better testing performance.
     enable_test_caching()
 
 
 # This is the main fixture that is used in all functional tests. It pulls in the other
 # fixtures that are necessary to set up a dbt project, and saves some of the information
```

### Comparing `dbt-core-1.8.0b2/dbt/tests/util.py` & `dbt_core-1.8.0b3/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/tracking.py` & `dbt_core-1.8.0b3/dbt/tracking.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from contextlib import contextmanager
 from datetime import datetime
 from typing import Optional
 
 import logbook
 import pytz
 import requests
+from packaging.version import Version
 from snowplow_tracker import Emitter, SelfDescribingJson, Subject, Tracker
+from snowplow_tracker import __version__ as snowplow_version  # type: ignore
 from snowplow_tracker import logger as sp_logger
 
 from dbt import version as dbt_version
 from dbt.clients.yaml_helper import safe_load, yaml  # noqa:F401
 from dbt_common.events.functions import fire_event, get_invocation_id
 from dbt.events.types import (
     DisableTracking,
@@ -45,25 +47,33 @@
 PROJECT_ID_SPEC = "iglu:com.dbt/project_id/jsonschema/1-0-1"
 RESOURCE_COUNTS = "iglu:com.dbt/resource_counts/jsonschema/1-0-1"
 RPC_REQUEST_SPEC = "iglu:com.dbt/rpc_request/jsonschema/1-0-1"
 RUNNABLE_TIMING = "iglu:com.dbt/runnable/jsonschema/1-0-0"
 RUN_MODEL_SPEC = "iglu:com.dbt/run_model/jsonschema/1-0-3"
 PLUGIN_GET_NODES = "iglu:com.dbt/plugin_get_nodes/jsonschema/1-0-0"
 
+SNOWPLOW_TRACKER_VERSION = Version(snowplow_version)
+
+# workaround in case real snowplow tracker is in the env
+# the argument was renamed in https://github.com/snowplow/snowplow-python-tracker/commit/39fd50a3aff98a5efdd5c5c7fb5518fe4761305b
+INIT_KW_ARGS = (
+    {"buffer_size": 30} if SNOWPLOW_TRACKER_VERSION < Version("0.13.0") else {"batch_size": 30}
+)
+
 
 class TimeoutEmitter(Emitter):
     def __init__(self) -> None:
         super().__init__(
             COLLECTOR_URL,
             protocol=COLLECTOR_PROTOCOL,
-            buffer_size=30,
             on_failure=self.handle_failure,
             method="post",
             # don't set this.
             byte_limit=None,
+            **INIT_KW_ARGS,
         )
 
     @staticmethod
     def handle_failure(num_ok, unsent):
         # num_ok will always be 0, unsent will always be 1 entry long, because
         # the buffer is length 1, so not much to talk about
         fire_event(DisableTracking())
@@ -100,15 +110,15 @@
 
         self._log_result("GET", r.status_code)
         return r
 
 
 emitter = TimeoutEmitter()
 tracker = Tracker(
-    emitter,
+    emitters=emitter,
     namespace="cf",
     app_id="dbt",
 )
 
 
 class User:
     def __init__(self, cookie_dir) -> None:
```

### Comparing `dbt-core-1.8.0b2/dbt/utils.py` & `dbt_core-1.8.0b3/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b2/dbt/version.py` & `dbt_core-1.8.0b3/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,9 +225,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.8.0b2"
+__version__ = "1.8.0b3"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.8.0b2/dbt_core.egg-info/PKG-INFO` & `dbt_core-1.8.0b3/dbt_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,20 +21,20 @@
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
-Requires-Dist: pathspec<0.12,>=0.9
-Requires-Dist: sqlparse<0.5,>=0.2.3
+Requires-Dist: pathspec<0.13,>=0.9
+Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
-Requires-Dist: dbt-common<2.0
+Requires-Dist: dbt-common<2.0,>=1.0.1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b3 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
 Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
-pathspec<0.12,>=0.9 Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-
+pathspec<0.13,>=0.9 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: dbt-
 extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
-common<2.0 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+common<2.0,>=1.0.1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
 packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
```

### Comparing `dbt-core-1.8.0b2/dbt_core.egg-info/SOURCES.txt` & `dbt_core-1.8.0b3/dbt_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 dbt/profiler.py
 dbt/py.typed
 dbt/selected_resources.py
 dbt/tracking.py
 dbt/utils.py
 dbt/version.py
 dbt/artifacts/__init__.py
+dbt/artifacts/exceptions/__init__.py
+dbt/artifacts/exceptions/schemas.py
 dbt/artifacts/resources/__init__.py
 dbt/artifacts/resources/base.py
 dbt/artifacts/resources/types.py
 dbt/artifacts/resources/v1/analysis.py
 dbt/artifacts/resources/v1/components.py
 dbt/artifacts/resources/v1/config.py
 dbt/artifacts/resources/v1/documentation.py
@@ -57,14 +59,15 @@
 dbt/artifacts/schemas/manifest/v12/__init__.py
 dbt/artifacts/schemas/manifest/v12/manifest.py
 dbt/artifacts/schemas/run/__init__.py
 dbt/artifacts/schemas/run/v5/__init__.py
 dbt/artifacts/schemas/run/v5/run.py
 dbt/artifacts/schemas/upgrades/__init__.py
 dbt/artifacts/schemas/upgrades/upgrade_manifest.py
+dbt/artifacts/utils/validation.py
 dbt/cli/__init__.py
 dbt/cli/context.py
 dbt/cli/exceptions.py
 dbt/cli/flags.py
 dbt/cli/main.py
 dbt/cli/option_types.py
 dbt/cli/options.py
@@ -91,14 +94,15 @@
 dbt/context/context_config.py
 dbt/context/docs.py
 dbt/context/exceptions_jinja.py
 dbt/context/macro_resolver.py
 dbt/context/macros.py
 dbt/context/manifest.py
 dbt/context/providers.py
+dbt/context/query_header.py
 dbt/context/secret.py
 dbt/context/target.py
 dbt/contracts/__init__.py
 dbt/contracts/files.py
 dbt/contracts/project.py
 dbt/contracts/results.py
 dbt/contracts/selection.py
@@ -107,18 +111,16 @@
 dbt/contracts/util.py
 dbt/contracts/graph/__init__.py
 dbt/contracts/graph/manifest.py
 dbt/contracts/graph/metrics.py
 dbt/contracts/graph/model_config.py
 dbt/contracts/graph/node_args.py
 dbt/contracts/graph/nodes.py
-dbt/contracts/graph/searcher.py
 dbt/contracts/graph/semantic_manifest.py
 dbt/contracts/graph/unparsed.py
-dbt/contracts/graph/utils.py
 dbt/deps/__init__.py
 dbt/deps/base.py
 dbt/deps/git.py
 dbt/deps/local.py
 dbt/deps/registry.py
 dbt/deps/resolver.py
 dbt/deps/tarball.py
```

### Comparing `dbt-core-1.8.0b2/setup.py` & `dbt_core-1.8.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.8.0b2"
+package_version = "1.8.0b3"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -62,24 +62,24 @@
         "click>=8.0.2,<9.0",
         "networkx>=2.3,<4.0",
         "protobuf>=4.0.0,<5",
         "requests<3.0.0",  # should match dbt-common
         # ----
         # These packages are major-version-0. Keep upper bounds on upcoming minor versions (which could have breaking changes)
         # and check compatibility / bump in each new minor version of dbt-core.
-        "pathspec>=0.9,<0.12",
-        "sqlparse>=0.2.3,<0.5",
+        "pathspec>=0.9,<0.13",
+        "sqlparse>=0.5.0,<0.6.0",
         # ----
         # These are major-version-0 packages also maintained by dbt-labs.
         # Accept patches but avoid automatically updating past a set minor version range.
         "dbt-extractor>=0.5.0,<=0.6",
         "minimal-snowplow-tracker>=0.0.2,<0.1",
         "dbt-semantic-interfaces>=0.5.1,<0.6",
         # Minor versions for these are expected to be backwards-compatible
-        "dbt-common<2.0",
+        "dbt-common>=1.0.1,<2.0",
         "dbt-adapters>=0.1.0a2,<2.0",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "daff>=1.3.46",
```

