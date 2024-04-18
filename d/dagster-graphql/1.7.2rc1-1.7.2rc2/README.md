# Comparing `tmp/dagster-graphql-1.7.2rc1.tar.gz` & `tmp/dagster-graphql-1.7.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.7.2rc1.tar", last modified: Tue Apr 16 17:51:26 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.2rc2.tar", last modified: Tue Apr 16 20:27:53 2024, max compression
```

## Comparing `dagster-graphql-1.7.2rc1.tar` & `dagster-graphql-1.7.2rc2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.795215 dagster-graphql-1.7.2rc1/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18338 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    20532 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14499 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    29108 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15163 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9069 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10352 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    14555 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9774 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11979 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    55049 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    10990 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    20849 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    18785 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13742 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    11731 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28766 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     5440 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17797 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11060 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    40100 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1654 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32162 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    46584 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9135 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10196 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7078 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 17:51:26.811215 dagster-graphql-1.7.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1534 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.078977 dagster-graphql-1.7.2rc2/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.078977 dagster-graphql-1.7.2rc2/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.082977 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20532 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.082977 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    29108 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    14555 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.090977 dagster-graphql-1.7.2rc2/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    55049 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    20849 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18785 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13742 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    11731 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.090977 dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.090977 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    40100 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    46584 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:26:54.000000 dagster-graphql-1.7.2rc2/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:53.078977 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 20:27:52.000000 dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 20:27:53.094977 dagster-graphql-1.7.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-04-16 20:26:55.000000 dagster-graphql-1.7.2rc2/setup.py
```

### Comparing `dagster-graphql-1.7.2rc1/LICENSE` & `dagster-graphql-1.7.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/PKG-INFO` & `dagster-graphql-1.7.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.2rc1
+Version: 1.7.2rc2
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/cli.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/client/client.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/client/query.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/asset_selections.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/table.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.2rc2/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.2rc1
+Version: 1.7.2rc2
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.2rc2/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.2rc1/setup.py` & `dagster-graphql-1.7.2rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc1",
+        "dagster==1.7.2rc2",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

