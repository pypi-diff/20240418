# Comparing `tmp/dagster-plus-1.7.2rc2.tar.gz` & `tmp/dagster-plus-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-plus-1.7.2rc2.tar", last modified: Tue Apr 16 20:40:49 2024, max compression
+gzip compressed data, was "dagster-plus-1.7.2rc3.tar", last modified: Thu Apr 18 21:22:02 2024, max compression
```

## Comparing `dagster-plus-1.7.2rc2.tar` & `dagster-plus-1.7.2rc3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.796630 dagster-plus-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)     4558 2024-04-16 20:40:49.796630 dagster-plus-1.7.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3056 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.712630 dagster-plus-1.7.2rc2/dagster_plus/
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.716630 dagster-plus-1.7.2rc2/dagster_plus/agent/
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.716630 dagster-plus-1.7.2rc2/dagster_plus/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7581 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45462 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.724629 dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9294 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/defs.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/mutation.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.724629 dagster-plus-1.7.2rc2/dagster_plus/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19247 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.724629 dagster-plus-1.7.2rc2/dagster_plus/artifacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.728630 dagster-plus-1.7.2rc2/dagster_plus/auth/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.732630 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.732630 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     7964 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3233 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.740630 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7064 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)     9357 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3807 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.740630 dagster-plus-1.7.2rc2/dagster_plus/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.740630 dagster-plus-1.7.2rc2/dagster_plus/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3096 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.740630 dagster-plus-1.7.2rc2/dagster_plus/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17254 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.744630 dagster-plus-1.7.2rc2/dagster_plus/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.744630 dagster-plus-1.7.2rc2/dagster_plus/instance/
--rw-r--r--   0 root         (0) root         (0)    23058 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.748630 dagster-plus-1.7.2rc2/dagster_plus/metrics/
--rw-r--r--   0 root         (0) root         (0)    10090 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.748630 dagster-plus-1.7.2rc2/dagster_plus/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.752630 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.752630 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.756630 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.756630 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2114 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17842 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12796 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3321 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.760630 dagster-plus-1.7.2rc2/dagster_plus/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.760630 dagster-plus-1.7.2rc2/dagster_plus/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.764630 dagster-plus-1.7.2rc2/dagster_plus/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1618 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.764630 dagster-plus-1.7.2rc2/dagster_plus/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4750 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.768630 dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16297 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    46228 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.772630 dagster-plus-1.7.2rc2/dagster_plus/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6446 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    18838 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.776630 dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7574 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.776630 dagster-plus-1.7.2rc2/dagster_plus/util/
--rw-r--r--   0 root         (0) root         (0)     2778 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.776630 dagster-plus-1.7.2rc2/dagster_plus/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.780630 dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.780630 dagster-plus-1.7.2rc2/dagster_plus/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12974 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.784630 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28817 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    28613 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.788630 dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26243 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)     9824 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.792630 dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14244 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    83988 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-16 20:27:17.000000 dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:49.716630 dagster-plus-1.7.2rc2/dagster_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4558 2024-04-16 20:40:49.000000 dagster-plus-1.7.2rc2/dagster_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4175 2024-04-16 20:40:49.000000 dagster-plus-1.7.2rc2/dagster_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:40:49.000000 dagster-plus-1.7.2rc2/dagster_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-16 20:40:49.000000 dagster-plus-1.7.2rc2/dagster_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 20:40:49.000000 dagster-plus-1.7.2rc2/dagster_plus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:40:49.796630 dagster-plus-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3095 2024-04-16 20:27:18.000000 dagster-plus-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.387936 dagster-plus-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-04-18 21:22:02.387936 dagster-plus-1.7.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3056 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.299936 dagster-plus-1.7.2rc3/dagster_plus/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.303936 dagster-plus-1.7.2rc3/dagster_plus/agent/
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.303936 dagster-plus-1.7.2rc3/dagster_plus/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7581 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45462 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.307936 dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9294 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.307936 dagster-plus-1.7.2rc3/dagster_plus/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19247 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.307936 dagster-plus-1.7.2rc3/dagster_plus/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.311936 dagster-plus-1.7.2rc3/dagster_plus/auth/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.311936 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.315936 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.323936 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9357 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.323936 dagster-plus-1.7.2rc3/dagster_plus/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.327936 dagster-plus-1.7.2rc3/dagster_plus/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.327936 dagster-plus-1.7.2rc3/dagster_plus/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17254 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.327936 dagster-plus-1.7.2rc3/dagster_plus/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.331936 dagster-plus-1.7.2rc3/dagster_plus/instance/
+-rw-r--r--   0 root         (0) root         (0)    23059 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.331936 dagster-plus-1.7.2rc3/dagster_plus/metrics/
+-rw-r--r--   0 root         (0) root         (0)    10090 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.331936 dagster-plus-1.7.2rc3/dagster_plus/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.335936 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.335936 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.343936 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.343936 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17842 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.347936 dagster-plus-1.7.2rc3/dagster_plus/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.347936 dagster-plus-1.7.2rc3/dagster_plus/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.351936 dagster-plus-1.7.2rc3/dagster_plus/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.351936 dagster-plus-1.7.2rc3/dagster_plus/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.359936 dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16297 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46228 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.359936 dagster-plus-1.7.2rc3/dagster_plus/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18838 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.363936 dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7574 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.363936 dagster-plus-1.7.2rc3/dagster_plus/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.367936 dagster-plus-1.7.2rc3/dagster_plus/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.371936 dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.371936 dagster-plus-1.7.2rc3/dagster_plus/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12974 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.379937 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28817 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28613 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.379937 dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26243 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9824 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.387936 dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14244 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    83988 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:02.299936 dagster-plus-1.7.2rc3/dagster_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-04-18 21:22:02.000000 dagster-plus-1.7.2rc3/dagster_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4175 2024-04-18 21:22:02.000000 dagster-plus-1.7.2rc3/dagster_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:22:02.000000 dagster-plus-1.7.2rc3/dagster_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-18 21:22:02.000000 dagster-plus-1.7.2rc3/dagster_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-18 21:22:02.000000 dagster-plus-1.7.2rc3/dagster_plus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 21:22:02.387936 dagster-plus-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-18 21:10:30.000000 dagster-plus-1.7.2rc3/setup.py
```

### Comparing `dagster-plus-1.7.2rc2/PKG-INFO` & `dagster-plus-1.7.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-plus
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-plus-1.7.2rc2/README.md` & `dagster-plus-1.7.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/agent/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/agent/cli/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/agent/dagster_cloud_agent.py` & `dagster-plus-1.7.2rc3/dagster_plus/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/agent/queries.py` & `dagster-plus-1.7.2rc3/dagster_plus/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/defs.py` & `dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/defs.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/anomaly_detection/types.py` & `dagster-plus-1.7.2rc3/dagster_plus/anomaly_detection/types.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/api/dagster_cloud_api.py` & `dagster-plus-1.7.2rc3/dagster_plus/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/auth/constants.py` & `dagster-plus-1.7.2rc3/dagster_plus/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/bigquery_utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/insights_utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/insights_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/metrics_utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/query.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/definitions.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/insights_snowflake_resource.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/dagster_insights/snowflake/snowflake_utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/execution/cloud_run_launcher/process.py` & `dagster-plus-1.7.2rc3/dagster_plus/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/execution/monitoring/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/execution/utils/process.py` & `dagster-plus-1.7.2rc3/dagster_plus/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/instance/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,14 +410,15 @@
                                 as_type=DagsterCloudUserCodeLauncher
                             )
                         )
                         self._user_code_launcher.register_instance(self)
                     except Exception:
                         logger = logging.getLogger("dagster_cloud")
                         logger.exception("Failed to load user code launcher from dagster_plus")
+
                         # Raise the original error if the rehydration fails with the dagster_plus path
                         raise e
                 else:
                     raise e
 
         return self._user_code_launcher
```

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/metrics/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/client.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/compile.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/cli/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/manager.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/registry.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/server/server.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/pex/grpc/types.py` & `dagster-plus-1.7.2rc3/dagster_plus/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/secrets/loader.py` & `dagster-plus-1.7.2rc3/dagster_plus/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/serverless/io_manager.py` & `dagster-plus-1.7.2rc3/dagster_plus/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/client.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/compute_logs/compute_log_manager.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/queries.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/storage.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/event_logs/utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/runs/queries.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/runs/storage.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/queries.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/storage/schedules/storage.py` & `dagster-plus-1.7.2rc3/dagster_plus/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/util/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/util/container_resources.py` & `dagster-plus-1.7.2rc3/dagster_plus/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/docker.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/ecs.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/config_schema/kubernetes.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/docker/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/client.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/launcher.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/run_launcher.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/service.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/ecs/utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/launcher.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/kubernetes/utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/__init__.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/process.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/user_code_launcher.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus/workspace/user_code_launcher/utils.py` & `dagster-plus-1.7.2rc3/dagster_plus/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus.egg-info/PKG-INFO` & `dagster-plus-1.7.2rc3/dagster_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-plus
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-plus-1.7.2rc2/dagster_plus.egg-info/SOURCES.txt` & `dagster-plus-1.7.2rc3/dagster_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-plus-1.7.2rc2/dagster_plus.egg-info/requires.txt` & `dagster-plus-1.7.2rc3/dagster_plus.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-dagster==1.7.2rc2
-dagster-plus-cli==1.7.2rc2
+dagster==1.7.2rc3
+dagster-plus-cli==1.7.2rc3
 pex<3,>=2.1.132
 questionary
 requests
 typer[all]
 
 [docker]
 docker
-dagster_docker==0.23.2rc2
+dagster_docker==0.23.2rc3
 
 [ecs]
-dagster_aws==0.23.2rc2
+dagster_aws==0.23.2rc3
 boto3
 
 [insights]
 pyarrow
 
 [kubernetes]
 kubernetes
-dagster_k8s==0.23.2rc2
+dagster_k8s==0.23.2rc3
 
 [pex]
 boto3
 
 [sandbox]
 supervisor
 
@@ -43,9 +43,9 @@
 types-PyYAML
 types-requests
 dagster-cloud-test-infra
 dbt-core
 dbt-snowflake
 dbt-postgres
 dbt-duckdb
-dagster-dbt==0.23.2rc2
-dagster_k8s==0.23.2rc2
+dagster-dbt==0.23.2rc3
+dagster_k8s==0.23.2rc3
```

### Comparing `dagster-plus-1.7.2rc2/setup.py` & `dagster-plus-1.7.2rc3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_plus_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.2rc2",
-        "dagster-plus-cli==1.7.2rc2",
+        "dagster==1.7.2rc3",
+        "dagster-plus-cli==1.7.2rc3",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -62,21 +62,21 @@
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
             "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.23.2rc2",
-            "dagster_k8s==0.23.2rc2",
+            "dagster-dbt==0.23.2rc3",
+            "dagster_k8s==0.23.2rc3",
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.23.2rc2"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.23.2rc2"],
-        "ecs": ["dagster_aws==0.23.2rc2", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.2rc3"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.2rc3"],
+        "ecs": ["dagster_aws==0.23.2rc3", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

