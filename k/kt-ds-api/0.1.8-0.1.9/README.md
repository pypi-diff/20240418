# Comparing `tmp/kt-ds-api-0.1.8.tar.gz` & `tmp/kt-ds-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kt-ds-api-0.1.8.tar", last modified: Mon Nov 13 00:04:03 2023, max compression
+gzip compressed data, was "kt-ds-api-0.1.9.tar", last modified: Wed Nov 15 05:40:10 2023, max compression
```

## Comparing `kt-ds-api-0.1.8.tar` & `kt-ds-api-0.1.9.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.736725 kt-ds-api-0.1.8/
--rw-rw-rw-   0        0        0       95 2023-11-13 00:04:03.735724 kt-ds-api-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:02.998092 kt-ds-api-0.1.8/kt_ds_api.egg-info/
--rw-rw-rw-   0        0        0       95 2023-11-13 00:04:02.000000 kt-ds-api-0.1.8/kt_ds_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11645 2023-11-13 00:04:02.000000 kt-ds-api-0.1.8/kt_ds_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 00:04:02.000000 kt-ds-api-0.1.8/kt_ds_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-30 13:33:09.000000 kt-ds-api-0.1.8/kt_ds_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-11-13 00:04:02.000000 kt-ds-api-0.1.8/kt_ds_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-13 00:04:03.736725 kt-ds-api-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-10-30 13:21:52.000000 kt-ds-api-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:02.998092 kt-ds-api-0.1.8/spaceone/
--rw-rw-rw-   0        0        0       64 2023-10-30 13:21:52.000000 kt-ds-api-0.1.8/spaceone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.008179 kt-ds-api-0.1.8/spaceone/api/
--rw-rw-rw-   0        0        0       14 2023-10-30 13:21:52.000000 kt-ds-api-0.1.8/spaceone/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.010726 kt-ds-api-0.1.8/spaceone/api/board/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:08.000000 kt-ds-api-0.1.8/spaceone/api/board/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.018844 kt-ds-api-0.1.8/spaceone/api/board/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:08.000000 kt-ds-api-0.1.8/spaceone/api/board/v1/__init__.py
--rw-rw-rw-   0        0        0     9126 2023-11-13 00:02:35.000000 kt-ds-api-0.1.8/spaceone/api/board/v1/board_pb2.py
--rw-rw-rw-   0        0        0    16100 2023-11-13 00:02:35.000000 kt-ds-api-0.1.8/spaceone/api/board/v1/board_pb2_grpc.py
--rw-rw-rw-   0        0        0    11744 2023-11-13 00:02:35.000000 kt-ds-api-0.1.8/spaceone/api/board/v1/post_pb2.py
--rw-rw-rw-   0        0        0    17722 2023-11-13 00:02:35.000000 kt-ds-api-0.1.8/spaceone/api/board/v1/post_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.018844 kt-ds-api-0.1.8/spaceone/api/config/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:47.000000 kt-ds-api-0.1.8/spaceone/api/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.031484 kt-ds-api-0.1.8/spaceone/api/config/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:47.000000 kt-ds-api-0.1.8/spaceone/api/config/v1/__init__.py
--rw-rw-rw-   0        0        0     8852 2023-11-13 00:02:19.000000 kt-ds-api-0.1.8/spaceone/api/config/v1/domain_config_pb2.py
--rw-rw-rw-   0        0        0    13539 2023-11-13 00:02:19.000000 kt-ds-api-0.1.8/spaceone/api/config/v1/domain_config_pb2_grpc.py
--rw-rw-rw-   0        0        0     8679 2023-11-13 00:02:20.000000 kt-ds-api-0.1.8/spaceone/api/config/v1/user_config_pb2.py
--rw-rw-rw-   0        0        0    13353 2023-11-13 00:02:20.000000 kt-ds-api-0.1.8/spaceone/api/config/v1/user_config_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.039517 kt-ds-api-0.1.8/spaceone/api/core/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:21:55.000000 kt-ds-api-0.1.8/spaceone/api/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.050166 kt-ds-api-0.1.8/spaceone/api/core/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:21:55.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/__init__.py
--rw-rw-rw-   0        0        0     5009 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/handler_pb2.py
--rw-rw-rw-   0        0        0      159 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/handler_pb2_grpc.py
--rw-rw-rw-   0        0        0    13065 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/query_pb2.py
--rw-rw-rw-   0        0        0      159 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/query_pb2_grpc.py
--rw-rw-rw-   0        0        0     1637 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/server_info_pb2.py
--rw-rw-rw-   0        0        0     2768 2023-11-13 00:01:21.000000 kt-ds-api-0.1.8/spaceone/api/core/v1/server_info_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.050166 kt-ds-api-0.1.8/spaceone/api/cost_analysis/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:00.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.070300 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:00.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/__init__.py
--rw-rw-rw-   0        0        0     3771 2023-11-13 00:02:24.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/cost_pb2.py
--rw-rw-rw-   0        0        0     2877 2023-11-13 00:02:24.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py
--rw-rw-rw-   0        0        0     3338 2023-11-13 00:02:24.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/data_source_pb2.py
--rw-rw-rw-   0        0        0     4840 2023-11-13 00:02:25.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py
--rw-rw-rw-   0        0        0     3736 2023-11-13 00:02:25.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/job_pb2.py
--rw-rw-rw-   0        0        0     2869 2023-11-13 00:02:25.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.131381 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:00.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/__init__.py
--rw-rw-rw-   0        0        0    14478 2023-11-13 00:02:26.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_pb2.py
--rw-rw-rw-   0        0        0    22607 2023-11-13 00:02:26.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py
--rw-rw-rw-   0        0        0     5153 2023-11-13 00:02:26.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_usage_pb2.py
--rw-rw-rw-   0        0        0     5494 2023-11-13 00:02:26.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py
--rw-rw-rw-   0        0        0    12312 2023-11-13 00:02:26.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_pb2.py
--rw-rw-rw-   0        0        0    20553 2023-11-13 00:02:27.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py
--rw-rw-rw-   0        0        0    10011 2023-11-13 00:02:27.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py
--rw-rw-rw-   0        0        0    17427 2023-11-13 00:02:27.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py
--rw-rw-rw-   0        0        0     9863 2023-11-13 00:02:28.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/custom_widget_pb2.py
--rw-rw-rw-   0        0        0    16546 2023-11-13 00:02:28.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/custom_widget_pb2_grpc.py
--rw-rw-rw-   0        0        0    17315 2023-11-13 00:02:28.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_pb2.py
--rw-rw-rw-   0        0        0    34869 2023-11-13 00:02:28.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py
--rw-rw-rw-   0        0        0    15939 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py
--rw-rw-rw-   0        0        0    20408 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py
--rw-rw-rw-   0        0        0     7230 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/exchange_rate_pb2.py
--rw-rw-rw-   0        0        0    14041 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/exchange_rate_pb2_grpc.py
--rw-rw-rw-   0        0        0     8043 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_pb2.py
--rw-rw-rw-   0        0        0    10734 2023-11-13 00:02:29.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_pb2_grpc.py
--rw-rw-rw-   0        0        0     6985 2023-11-13 00:02:30.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_task_pb2.py
--rw-rw-rw-   0        0        0     8631 2023-11-13 00:02:30.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py
--rw-rw-rw-   0        0        0     5544 2023-11-13 00:02:30.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2.py
--rw-rw-rw-   0        0        0     8965 2023-11-13 00:02:30.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2_grpc.py
--rw-rw-rw-   0        0        0    13445 2023-11-13 00:02:31.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/public_dashboard_pb2.py
--rw-rw-rw-   0        0        0    24608 2023-11-13 00:02:31.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/public_dashboard_pb2_grpc.py
--rw-rw-rw-   0        0        0    11436 2023-11-13 00:02:31.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/schedule_pb2.py
--rw-rw-rw-   0        0        0    15330 2023-11-13 00:02:31.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/schedule_pb2_grpc.py
--rw-rw-rw-   0        0        0    13178 2023-11-13 00:02:32.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/user_dashboard_pb2.py
--rw-rw-rw-   0        0        0    23182 2023-11-13 00:02:32.000000 kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/user_dashboard_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.141446 kt-ds-api-0.1.8/spaceone/api/dashboard/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:15.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.151824 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:15.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/__init__.py
--rw-rw-rw-   0        0        0    10411 2023-11-13 00:02:40.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/custom_widget_pb2.py
--rw-rw-rw-   0        0        0    11905 2023-11-13 00:02:40.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/custom_widget_pb2_grpc.py
--rw-rw-rw-   0        0        0    21126 2023-11-13 00:02:40.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/domain_dashboard_pb2.py
--rw-rw-rw-   0        0        0    19798 2023-11-13 00:02:40.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/domain_dashboard_pb2_grpc.py
--rw-rw-rw-   0        0        0    21462 2023-11-13 00:02:41.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/project_dashboard_pb2.py
--rw-rw-rw-   0        0        0    19927 2023-11-13 00:02:41.000000 kt-ds-api-0.1.8/spaceone/api/dashboard/v1/project_dashboard_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.151824 kt-ds-api-0.1.8/spaceone/api/file_manager/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:11.000000 kt-ds-api-0.1.8/spaceone/api/file_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.161851 kt-ds-api-0.1.8/spaceone/api/file_manager/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:23:11.000000 kt-ds-api-0.1.8/spaceone/api/file_manager/v1/__init__.py
--rw-rw-rw-   0        0        0    11080 2023-11-13 00:02:38.000000 kt-ds-api-0.1.8/spaceone/api/file_manager/v1/file_pb2.py
--rw-rw-rw-   0        0        0    13154 2023-11-13 00:02:38.000000 kt-ds-api-0.1.8/spaceone/api/file_manager/v1/file_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.170410 kt-ds-api-0.1.8/spaceone/api/identity/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:02.000000 kt-ds-api-0.1.8/spaceone/api/identity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.171928 kt-ds-api-0.1.8/spaceone/api/identity/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:02.000000 kt-ds-api-0.1.8/spaceone/api/identity/plugin/__init__.py
--rw-rw-rw-   0        0        0     6889 2023-11-13 00:01:24.000000 kt-ds-api-0.1.8/spaceone/api/identity/plugin/auth_pb2.py
--rw-rw-rw-   0        0        0     7868 2023-11-13 00:01:24.000000 kt-ds-api-0.1.8/spaceone/api/identity/plugin/auth_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.243322 kt-ds-api-0.1.8/spaceone/api/identity/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:02.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/__init__.py
--rw-rw-rw-   0        0        0     8834 2023-11-13 00:01:25.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/api_key_pb2.py
--rw-rw-rw-   0        0        0    13106 2023-11-13 00:01:25.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/api_key_pb2_grpc.py
--rw-rw-rw-   0        0        0     1589 2023-11-13 00:01:25.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/authorization_pb2.py
--rw-rw-rw-   0        0        0     2786 2023-11-13 00:01:25.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/authorization_pb2_grpc.py
--rw-rw-rw-   0        0        0     6327 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_owner_pb2.py
--rw-rw-rw-   0        0        0     8183 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_owner_pb2_grpc.py
--rw-rw-rw-   0        0        0    14524 2023-11-13 00:01:26.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_pb2.py
--rw-rw-rw-   0        0        0    21983 2023-11-13 00:01:26.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_pb2_grpc.py
--rw-rw-rw-   0        0        0     3881 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/endpoint_pb2.py
--rw-rw-rw-   0        0        0     2732 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/endpoint_pb2_grpc.py
--rw-rw-rw-   0        0        0     8644 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/policy_pb2.py
--rw-rw-rw-   0        0        0    11326 2023-11-13 00:01:27.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/policy_pb2_grpc.py
--rw-rw-rw-   0        0        0    20379 2023-11-13 00:01:28.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/project_group_pb2.py
--rw-rw-rw-   0        0        0    21293 2023-11-13 00:01:29.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/project_group_pb2_grpc.py
--rw-rw-rw-   0        0        0    19158 2023-11-13 00:01:28.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/project_pb2.py
--rw-rw-rw-   0        0        0    29819 2023-11-13 00:01:28.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/project_pb2_grpc.py
--rw-rw-rw-   0        0        0     9395 2023-11-13 00:01:29.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/provider_pb2.py
--rw-rw-rw-   0        0        0    11481 2023-11-13 00:01:29.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/provider_pb2_grpc.py
--rw-rw-rw-   0        0        0    10569 2023-11-13 00:01:30.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/role_binding_pb2.py
--rw-rw-rw-   0        0        0    11781 2023-11-13 00:01:30.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/role_binding_pb2_grpc.py
--rw-rw-rw-   0        0        0    11296 2023-11-13 00:01:30.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/role_pb2.py
--rw-rw-rw-   0        0        0    11165 2023-11-13 00:01:30.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/role_pb2_grpc.py
--rw-rw-rw-   0        0        0    10865 2023-11-13 00:01:31.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/service_account_pb2.py
--rw-rw-rw-   0        0        0    12018 2023-11-13 00:01:31.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/service_account_pb2_grpc.py
--rw-rw-rw-   0        0        0     3218 2023-11-13 00:01:31.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/token_pb2.py
--rw-rw-rw-   0        0        0     4410 2023-11-13 00:01:31.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/token_pb2_grpc.py
--rw-rw-rw-   0        0        0    15790 2023-11-13 00:01:32.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/user_pb2.py
--rw-rw-rw-   0        0        0    20705 2023-11-13 00:01:32.000000 kt-ds-api-0.1.8/spaceone/api/identity/v1/user_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.243322 kt-ds-api-0.1.8/spaceone/api/inventory/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:29.000000 kt-ds-api-0.1.8/spaceone/api/inventory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.251514 kt-ds-api-0.1.8/spaceone/api/inventory/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:29.000000 kt-ds-api-0.1.8/spaceone/api/inventory/plugin/__init__.py
--rw-rw-rw-   0        0        0     5821 2023-11-13 00:01:44.000000 kt-ds-api-0.1.8/spaceone/api/inventory/plugin/collector_pb2.py
--rw-rw-rw-   0        0        0     6982 2023-11-13 00:01:44.000000 kt-ds-api-0.1.8/spaceone/api/inventory/plugin/collector_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.320054 kt-ds-api-0.1.8/spaceone/api/inventory/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:29.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/__init__.py
--rw-rw-rw-   0        0        0     6295 2023-11-13 00:01:44.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/change_history_pb2.py
--rw-rw-rw-   0        0        0     4653 2023-11-13 00:01:44.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/change_history_pb2_grpc.py
--rw-rw-rw-   0        0        0    13338 2023-11-13 00:01:45.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_pb2.py
--rw-rw-rw-   0        0        0    23915 2023-11-13 00:01:45.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py
--rw-rw-rw-   0        0        0     5296 2023-11-13 00:01:45.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_tag_pb2.py
--rw-rw-rw-   0        0        0     4735 2023-11-13 00:01:45.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_tag_pb2_grpc.py
--rw-rw-rw-   0        0        0    11463 2023-11-13 00:01:46.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_type_pb2.py
--rw-rw-rw-   0        0        0    17823 2023-11-13 00:01:46.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py
--rw-rw-rw-   0        0        0    26939 2023-11-13 00:01:46.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/collector_pb2.py
--rw-rw-rw-   0        0        0    45613 2023-11-13 00:01:46.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/collector_pb2_grpc.py
--rw-rw-rw-   0        0        0     6229 2023-11-13 00:01:47.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_pb2.py
--rw-rw-rw-   0        0        0    10829 2023-11-13 00:01:47.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_pb2_grpc.py
--rw-rw-rw-   0        0        0     8400 2023-11-13 00:01:47.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_task_pb2.py
--rw-rw-rw-   0        0        0    10854 2023-11-13 00:01:47.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_task_pb2_grpc.py
--rw-rw-rw-   0        0        0     8331 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/note_pb2.py
--rw-rw-rw-   0        0        0    11595 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/note_pb2_grpc.py
--rw-rw-rw-   0        0        0     8888 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/region_pb2.py
--rw-rw-rw-   0        0        0    15623 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/region_pb2_grpc.py
--rw-rw-rw-   0        0        0    10822 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/resource_group_pb2.py
--rw-rw-rw-   0        0        0    18633 2023-11-13 00:01:48.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/resource_group_pb2_grpc.py
--rw-rw-rw-   0        0        0    15572 2023-11-13 00:01:49.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/server_pb2.py
--rw-rw-rw-   0        0        0    13130 2023-11-13 00:01:49.000000 kt-ds-api-0.1.8/spaceone/api/inventory/v1/server_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.320054 kt-ds-api-0.1.8/spaceone/api/monitoring/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:37.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.365441 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:37.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/__init__.py
--rw-rw-rw-   0        0        0     3227 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/data_source_pb2.py
--rw-rw-rw-   0        0        0     4901 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py
--rw-rw-rw-   0        0        0     3716 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/event_pb2.py
--rw-rw-rw-   0        0        0     2936 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/event_pb2_grpc.py
--rw-rw-rw-   0        0        0     3086 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/log_pb2.py
--rw-rw-rw-   0        0        0     2714 2023-11-13 00:01:51.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/log_pb2_grpc.py
--rw-rw-rw-   0        0        0     4889 2023-11-13 00:01:52.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/metric_pb2.py
--rw-rw-rw-   0        0        0     4868 2023-11-13 00:01:52.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/metric_pb2_grpc.py
--rw-rw-rw-   0        0        0     3320 2023-11-13 00:01:52.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/webhook_pb2.py
--rw-rw-rw-   0        0        0     4865 2023-11-13 00:01:52.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.457215 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:37.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/__init__.py
--rw-rw-rw-   0        0        0    19229 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/alert_pb2.py
--rw-rw-rw-   0        0        0    32376 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/alert_pb2_grpc.py
--rw-rw-rw-   0        0        0    14879 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/data_source_pb2.py
--rw-rw-rw-   0        0        0    29312 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/data_source_pb2_grpc.py
--rw-rw-rw-   0        0        0    15551 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/escalation_policy_pb2.py
--rw-rw-rw-   0        0        0    19800 2023-11-13 00:01:53.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py
--rw-rw-rw-   0        0        0     8148 2023-11-13 00:01:54.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_pb2.py
--rw-rw-rw-   0        0        0    12965 2023-11-13 00:01:54.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_pb2_grpc.py
--rw-rw-rw-   0        0        0    16897 2023-11-13 00:01:54.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_rule_pb2.py
--rw-rw-rw-   0        0        0    20365 2023-11-13 00:01:54.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py
--rw-rw-rw-   0        0        0     2857 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/log_pb2.py
--rw-rw-rw-   0        0        0     2664 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/log_pb2_grpc.py
--rw-rw-rw-   0        0        0    11647 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/maintenance_window_pb2.py
--rw-rw-rw-   0        0        0    17707 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/maintenance_window_pb2_grpc.py
--rw-rw-rw-   0        0        0     5444 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/metric_pb2.py
--rw-rw-rw-   0        0        0     7689 2023-11-13 00:01:55.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/metric_pb2_grpc.py
--rw-rw-rw-   0        0        0     8364 2023-11-13 00:01:56.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/note_pb2.py
--rw-rw-rw-   0        0        0    14119 2023-11-13 00:01:56.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/note_pb2_grpc.py
--rw-rw-rw-   0        0        0    12030 2023-11-13 00:01:56.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/project_alert_config_pb2.py
--rw-rw-rw-   0        0        0    16871 2023-11-13 00:01:56.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py
--rw-rw-rw-   0        0        0    13969 2023-11-13 00:01:57.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/webhook_pb2.py
--rw-rw-rw-   0        0        0    26926 2023-11-13 00:01:57.000000 kt-ds-api-0.1.8/spaceone/api/monitoring/v1/webhook_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.460214 kt-ds-api-0.1.8/spaceone/api/notification/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:41.000000 kt-ds-api-0.1.8/spaceone/api/notification/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.476214 kt-ds-api-0.1.8/spaceone/api/notification/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:41.000000 kt-ds-api-0.1.8/spaceone/api/notification/plugin/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-11-13 00:02:05.000000 kt-ds-api-0.1.8/spaceone/api/notification/plugin/notification_pb2.py
--rw-rw-rw-   0        0        0     4596 2023-11-13 00:02:05.000000 kt-ds-api-0.1.8/spaceone/api/notification/plugin/notification_pb2_grpc.py
--rw-rw-rw-   0        0        0     3189 2023-11-13 00:02:05.000000 kt-ds-api-0.1.8/spaceone/api/notification/plugin/protocol_pb2.py
--rw-rw-rw-   0        0        0     5016 2023-11-13 00:02:05.000000 kt-ds-api-0.1.8/spaceone/api/notification/plugin/protocol_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.523756 kt-ds-api-0.1.8/spaceone/api/notification/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:41.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/__init__.py
--rw-rw-rw-   0        0        0    14203 2023-11-13 00:02:06.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_pb2.py
--rw-rw-rw-   0        0        0    20070 2023-11-13 00:02:06.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_pb2_grpc.py
--rw-rw-rw-   0        0        0     5276 2023-11-13 00:02:06.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_usage_pb2.py
--rw-rw-rw-   0        0        0     5480 2023-11-13 00:02:06.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_usage_pb2_grpc.py
--rw-rw-rw-   0        0        0    17683 2023-11-13 00:02:07.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/project_channel_pb2.py
--rw-rw-rw-   0        0        0    27678 2023-11-13 00:02:07.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/project_channel_pb2_grpc.py
--rw-rw-rw-   0        0        0    15094 2023-11-13 00:02:07.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/protocol_pb2.py
--rw-rw-rw-   0        0        0    28786 2023-11-13 00:02:07.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/protocol_pb2_grpc.py
--rw-rw-rw-   0        0        0     7849 2023-11-13 00:02:08.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/quota_pb2.py
--rw-rw-rw-   0        0        0    13903 2023-11-13 00:02:08.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/quota_pb2_grpc.py
--rw-rw-rw-   0        0        0    16112 2023-11-13 00:02:08.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/user_channel_pb2.py
--rw-rw-rw-   0        0        0    27452 2023-11-13 00:02:08.000000 kt-ds-api-0.1.8/spaceone/api/notification/v1/user_channel_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.526748 kt-ds-api-0.1.8/spaceone/api/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:13.000000 kt-ds-api-0.1.8/spaceone/api/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.541745 kt-ds-api-0.1.8/spaceone/api/plugin/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:13.000000 kt-ds-api-0.1.8/spaceone/api/plugin/v1/__init__.py
--rw-rw-rw-   0        0        0     4492 2023-11-13 00:01:38.000000 kt-ds-api-0.1.8/spaceone/api/plugin/v1/plugin_pb2.py
--rw-rw-rw-   0        0        0     5093 2023-11-13 00:01:38.000000 kt-ds-api-0.1.8/spaceone/api/plugin/v1/plugin_pb2_grpc.py
--rw-rw-rw-   0        0        0    15826 2023-11-13 00:01:38.000000 kt-ds-api-0.1.8/spaceone/api/plugin/v1/supervisor_pb2.py
--rw-rw-rw-   0        0        0    26433 2023-11-13 00:01:39.000000 kt-ds-api-0.1.8/spaceone/api/plugin/v1/supervisor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.544744 kt-ds-api-0.1.8/spaceone/api/provisioning/
--rw-rw-rw-   0        0        0        0 2023-10-31 00:05:13.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.611207 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/
--rw-rw-rw-   0        0        0        0 2023-10-31 00:05:13.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/__init__.py
--rw-rw-rw-   0        0        0    12523 2023-11-13 00:02:43.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_pb2.py
--rw-rw-rw-   0        0        0    17218 2023-11-13 00:02:43.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_pb2_grpc.py
--rw-rw-rw-   0        0        0     7919 2023-11-13 00:02:44.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_history_pb2.py
--rw-rw-rw-   0        0        0     7318 2023-11-13 00:02:44.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_history_pb2_grpc.py
--rw-rw-rw-   0        0        0    12116 2023-11-13 00:02:43.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_pb2.py
--rw-rw-rw-   0        0        0    12872 2023-11-13 00:02:43.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_pb2_grpc.py
--rw-rw-rw-   0        0        0      951 2023-11-13 00:02:44.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/consumers_pb2.py
--rw-rw-rw-   0        0        0      903 2023-11-13 00:02:44.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/consumers_pb2_grpc.py
--rw-rw-rw-   0        0        0     9138 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_group_pb2.py
--rw-rw-rw-   0        0        0    12635 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_group_pb2_grpc.py
--rw-rw-rw-   0        0        0    10761 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_pb2.py
--rw-rw-rw-   0        0        0    11967 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_pb2_grpc.py
--rw-rw-rw-   0        0        0     9259 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_tag_pb2.py
--rw-rw-rw-   0        0        0    12407 2023-11-13 00:02:45.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_tag_pb2_grpc.py
--rw-rw-rw-   0        0        0    11394 2023-11-13 00:02:46.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_pb2.py
--rw-rw-rw-   0        0        0    15077 2023-11-13 00:02:46.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_pb2_grpc.py
--rw-rw-rw-   0        0        0     7645 2023-11-13 00:02:47.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_history_pb2.py
--rw-rw-rw-   0        0        0     7204 2023-11-13 00:02:47.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_history_pb2_grpc.py
--rw-rw-rw-   0        0        0    11740 2023-11-13 00:02:46.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_pb2.py
--rw-rw-rw-   0        0        0    12644 2023-11-13 00:02:46.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_pb2_grpc.py
--rw-rw-rw-   0        0        0     7959 2023-11-13 00:02:47.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/transmission_history_pb2.py
--rw-rw-rw-   0        0        0     9226 2023-11-13 00:02:47.000000 kt-ds-api-0.1.8/spaceone/api/provisioning/v1/transmission_history_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.614211 kt-ds-api-0.1.8/spaceone/api/repository/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:08.000000 kt-ds-api-0.1.8/spaceone/api/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.639206 kt-ds-api-0.1.8/spaceone/api/repository/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:08.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/__init__.py
--rw-rw-rw-   0        0        0    14221 2023-11-13 00:01:35.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/plugin_pb2.py
--rw-rw-rw-   0        0        0    29261 2023-11-13 00:01:35.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/plugin_pb2_grpc.py
--rw-rw-rw-   0        0        0    10282 2023-11-13 00:01:35.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/policy_pb2.py
--rw-rw-rw-   0        0        0    15964 2023-11-13 00:01:35.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/policy_pb2_grpc.py
--rw-rw-rw-   0        0        0     9305 2023-11-13 00:01:36.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/repository_pb2.py
--rw-rw-rw-   0        0        0    14137 2023-11-13 00:01:36.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/repository_pb2_grpc.py
--rw-rw-rw-   0        0        0    10176 2023-11-13 00:01:36.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/schema_pb2.py
--rw-rw-rw-   0        0        0    15467 2023-11-13 00:01:36.000000 kt-ds-api-0.1.8/spaceone/api/repository/v1/schema_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.642207 kt-ds-api-0.1.8/spaceone/api/sample/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:21:52.000000 kt-ds-api-0.1.8/spaceone/api/sample/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.659206 kt-ds-api-0.1.8/spaceone/api/sample/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:21:52.000000 kt-ds-api-0.1.8/spaceone/api/sample/v1/__init__.py
--rw-rw-rw-   0        0        0     2032 2023-11-13 00:01:17.000000 kt-ds-api-0.1.8/spaceone/api/sample/v1/helloworld_pb2.py
--rw-rw-rw-   0        0        0     2703 2023-11-13 00:01:17.000000 kt-ds-api-0.1.8/spaceone/api/sample/v1/helloworld_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.662207 kt-ds-api-0.1.8/spaceone/api/secret/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:18.000000 kt-ds-api-0.1.8/spaceone/api/secret/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.695726 kt-ds-api-0.1.8/spaceone/api/secret/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:18.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/__init__.py
--rw-rw-rw-   0        0        0    11668 2023-11-13 00:01:41.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_group_pb2.py
--rw-rw-rw-   0        0        0    15293 2023-11-13 00:01:41.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_group_pb2_grpc.py
--rw-rw-rw-   0        0        0    11883 2023-11-13 00:01:41.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_pb2.py
--rw-rw-rw-   0        0        0    19449 2023-11-13 00:01:41.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_pb2_grpc.py
--rw-rw-rw-   0        0        0    11152 2023-11-13 00:01:42.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/trusted_secret_pb2.py
--rw-rw-rw-   0        0        0    17527 2023-11-13 00:01:42.000000 kt-ds-api-0.1.8/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.700726 kt-ds-api-0.1.8/spaceone/api/statistics/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:45.000000 kt-ds-api-0.1.8/spaceone/api/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.707727 kt-ds-api-0.1.8/spaceone/api/statistics/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:45.000000 kt-ds-api-0.1.8/spaceone/api/statistics/plugin/__init__.py
--rw-rw-rw-   0        0        0     3955 2023-11-13 00:02:12.000000 kt-ds-api-0.1.8/spaceone/api/statistics/plugin/storage_pb2.py
--rw-rw-rw-   0        0        0     6207 2023-11-13 00:02:12.000000 kt-ds-api-0.1.8/spaceone/api/statistics/plugin/storage_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 00:04:03.732726 kt-ds-api-0.1.8/spaceone/api/statistics/v1/
--rw-rw-rw-   0        0        0        0 2023-10-30 13:22:45.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/__init__.py
--rw-rw-rw-   0        0        0     5752 2023-11-13 00:02:13.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/history_pb2.py
--rw-rw-rw-   0        0        0     7655 2023-11-13 00:02:13.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/history_pb2_grpc.py
--rw-rw-rw-   0        0        0     9047 2023-11-13 00:02:14.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/resource_pb2.py
--rw-rw-rw-   0        0        0     7684 2023-11-13 00:02:14.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/resource_pb2_grpc.py
--rw-rw-rw-   0        0        0    11875 2023-11-13 00:02:15.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/schedule_pb2.py
--rw-rw-rw-   0        0        0    76967 2023-11-13 00:02:15.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/schedule_pb2_grpc.py
--rw-rw-rw-   0        0        0    13587 2023-11-13 00:02:16.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/storage_pb2.py
--rw-rw-rw-   0        0        0    18596 2023-11-13 00:02:16.000000 kt-ds-api-0.1.8/spaceone/api/statistics/v1/storage_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.437454 kt-ds-api-0.1.9/
+-rw-rw-rw-   0        0        0       95 2023-11-15 05:40:10.436454 kt-ds-api-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.695454 kt-ds-api-0.1.9/kt_ds_api.egg-info/
+-rw-rw-rw-   0        0        0       95 2023-11-15 05:40:09.000000 kt-ds-api-0.1.9/kt_ds_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11645 2023-11-15 05:40:09.000000 kt-ds-api-0.1.9/kt_ds_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-15 05:40:09.000000 kt-ds-api-0.1.9/kt_ds_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-15 05:40:09.000000 kt-ds-api-0.1.9/kt_ds_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-11-15 05:40:09.000000 kt-ds-api-0.1.9/kt_ds_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-15 05:40:10.437454 kt-ds-api-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.695454 kt-ds-api-0.1.9/spaceone/
+-rw-rw-rw-   0        0        0       64 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.695454 kt-ds-api-0.1.9/spaceone/api/
+-rw-rw-rw-   0        0        0       14 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.695454 kt-ds-api-0.1.9/spaceone/api/board/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.713642 kt-ds-api-0.1.9/spaceone/api/board/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/v1/__init__.py
+-rw-rw-rw-   0        0        0     9126 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/v1/board_pb2.py
+-rw-rw-rw-   0        0        0    16100 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/v1/board_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11744 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/v1/post_pb2.py
+-rw-rw-rw-   0        0        0    17722 2023-11-15 05:33:52.000000 kt-ds-api-0.1.9/spaceone/api/board/v1/post_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.715640 kt-ds-api-0.1.9/spaceone/api/config/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:39.000000 kt-ds-api-0.1.9/spaceone/api/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.726393 kt-ds-api-0.1.9/spaceone/api/config/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:39.000000 kt-ds-api-0.1.9/spaceone/api/config/v1/__init__.py
+-rw-rw-rw-   0        0        0     8852 2023-11-15 05:33:38.000000 kt-ds-api-0.1.9/spaceone/api/config/v1/domain_config_pb2.py
+-rw-rw-rw-   0        0        0    13539 2023-11-15 05:33:38.000000 kt-ds-api-0.1.9/spaceone/api/config/v1/domain_config_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8679 2023-11-15 05:33:39.000000 kt-ds-api-0.1.9/spaceone/api/config/v1/user_config_pb2.py
+-rw-rw-rw-   0        0        0    13353 2023-11-15 05:33:39.000000 kt-ds-api-0.1.9/spaceone/api/config/v1/user_config_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.728692 kt-ds-api-0.1.9/spaceone/api/core/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.747016 kt-ds-api-0.1.9/spaceone/api/core/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/__init__.py
+-rw-rw-rw-   0        0        0     5009 2023-11-15 05:32:54.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/handler_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-11-15 05:32:54.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/handler_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13065 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/query_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/query_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1637 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/server_info_pb2.py
+-rw-rw-rw-   0        0        0     2768 2023-11-15 05:32:55.000000 kt-ds-api-0.1.9/spaceone/api/core/v1/server_info_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.749016 kt-ds-api-0.1.9/spaceone/api/cost_analysis/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:50.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.764951 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:50.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/__init__.py
+-rw-rw-rw-   0        0        0     3771 2023-11-15 05:33:42.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/cost_pb2.py
+-rw-rw-rw-   0        0        0     2877 2023-11-15 05:33:42.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3338 2023-11-15 05:33:43.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/data_source_pb2.py
+-rw-rw-rw-   0        0        0     4840 2023-11-15 05:33:43.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3736 2023-11-15 05:33:44.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/job_pb2.py
+-rw-rw-rw-   0        0        0     2869 2023-11-15 05:33:44.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.848839 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:50.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/__init__.py
+-rw-rw-rw-   0        0        0    14478 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_pb2.py
+-rw-rw-rw-   0        0        0    22607 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5153 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_usage_pb2.py
+-rw-rw-rw-   0        0        0     5494 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12312 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_pb2.py
+-rw-rw-rw-   0        0        0    20553 2023-11-15 05:33:45.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10011 2023-11-15 05:33:46.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py
+-rw-rw-rw-   0        0        0    17427 2023-11-15 05:33:46.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9863 2023-11-15 05:33:46.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/custom_widget_pb2.py
+-rw-rw-rw-   0        0        0    16546 2023-11-15 05:33:46.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/custom_widget_pb2_grpc.py
+-rw-rw-rw-   0        0        0    17315 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_pb2.py
+-rw-rw-rw-   0        0        0    34869 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15939 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py
+-rw-rw-rw-   0        0        0    20408 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7230 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/exchange_rate_pb2.py
+-rw-rw-rw-   0        0        0    14041 2023-11-15 05:33:47.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/exchange_rate_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8043 2023-11-15 05:33:48.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_pb2.py
+-rw-rw-rw-   0        0        0    10734 2023-11-15 05:33:48.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6985 2023-11-15 05:33:48.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_task_pb2.py
+-rw-rw-rw-   0        0        0     8631 2023-11-15 05:33:48.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5544 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2.py
+-rw-rw-rw-   0        0        0     8965 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13445 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/public_dashboard_pb2.py
+-rw-rw-rw-   0        0        0    24608 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/public_dashboard_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11436 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/schedule_pb2.py
+-rw-rw-rw-   0        0        0    15330 2023-11-15 05:33:49.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/schedule_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13178 2023-11-15 05:33:50.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/user_dashboard_pb2.py
+-rw-rw-rw-   0        0        0    23182 2023-11-15 05:33:50.000000 kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/user_dashboard_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.850840 kt-ds-api-0.1.9/spaceone/api/dashboard/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.862834 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/__init__.py
+-rw-rw-rw-   0        0        0    10411 2023-11-15 05:33:56.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/custom_widget_pb2.py
+-rw-rw-rw-   0        0        0    11905 2023-11-15 05:33:56.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/custom_widget_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21126 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/domain_dashboard_pb2.py
+-rw-rw-rw-   0        0        0    19798 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/domain_dashboard_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21462 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/project_dashboard_pb2.py
+-rw-rw-rw-   0        0        0    19927 2023-11-15 05:33:57.000000 kt-ds-api-0.1.9/spaceone/api/dashboard/v1/project_dashboard_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.868813 kt-ds-api-0.1.9/spaceone/api/file_manager/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:54.000000 kt-ds-api-0.1.9/spaceone/api/file_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.874817 kt-ds-api-0.1.9/spaceone/api/file_manager/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:54.000000 kt-ds-api-0.1.9/spaceone/api/file_manager/v1/__init__.py
+-rw-rw-rw-   0        0        0    11080 2023-11-15 05:33:54.000000 kt-ds-api-0.1.9/spaceone/api/file_manager/v1/file_pb2.py
+-rw-rw-rw-   0        0        0    13154 2023-11-15 05:33:54.000000 kt-ds-api-0.1.9/spaceone/api/file_manager/v1/file_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.877771 kt-ds-api-0.1.9/spaceone/api/identity/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:04.000000 kt-ds-api-0.1.9/spaceone/api/identity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.883775 kt-ds-api-0.1.9/spaceone/api/identity/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:04.000000 kt-ds-api-0.1.9/spaceone/api/identity/plugin/__init__.py
+-rw-rw-rw-   0        0        0     6889 2023-11-15 05:32:57.000000 kt-ds-api-0.1.9/spaceone/api/identity/plugin/auth_pb2.py
+-rw-rw-rw-   0        0        0     7868 2023-11-15 05:32:57.000000 kt-ds-api-0.1.9/spaceone/api/identity/plugin/auth_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.961342 kt-ds-api-0.1.9/spaceone/api/identity/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:04.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/__init__.py
+-rw-rw-rw-   0        0        0     8834 2023-11-15 05:32:58.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/api_key_pb2.py
+-rw-rw-rw-   0        0        0    13106 2023-11-15 05:32:58.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/api_key_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1589 2023-11-15 05:32:58.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/authorization_pb2.py
+-rw-rw-rw-   0        0        0     2786 2023-11-15 05:32:58.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/authorization_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6327 2023-11-15 05:32:59.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_owner_pb2.py
+-rw-rw-rw-   0        0        0     8183 2023-11-15 05:32:59.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_owner_pb2_grpc.py
+-rw-rw-rw-   0        0        0    14524 2023-11-15 05:32:59.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_pb2.py
+-rw-rw-rw-   0        0        0    21983 2023-11-15 05:32:59.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3881 2023-11-15 05:33:00.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/endpoint_pb2.py
+-rw-rw-rw-   0        0        0     2732 2023-11-15 05:33:00.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/endpoint_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8644 2023-11-15 05:33:00.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/policy_pb2.py
+-rw-rw-rw-   0        0        0    11326 2023-11-15 05:33:00.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/policy_pb2_grpc.py
+-rw-rw-rw-   0        0        0    20379 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/project_group_pb2.py
+-rw-rw-rw-   0        0        0    21293 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/project_group_pb2_grpc.py
+-rw-rw-rw-   0        0        0    19158 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/project_pb2.py
+-rw-rw-rw-   0        0        0    29819 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/project_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9395 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/provider_pb2.py
+-rw-rw-rw-   0        0        0    11481 2023-11-15 05:33:01.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/provider_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10569 2023-11-15 05:33:02.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/role_binding_pb2.py
+-rw-rw-rw-   0        0        0    11781 2023-11-15 05:33:02.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/role_binding_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11296 2023-11-15 05:33:02.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/role_pb2.py
+-rw-rw-rw-   0        0        0    11165 2023-11-15 05:33:02.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/role_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10865 2023-11-15 05:33:03.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/service_account_pb2.py
+-rw-rw-rw-   0        0        0    12018 2023-11-15 05:33:03.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/service_account_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3218 2023-11-15 05:33:03.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/token_pb2.py
+-rw-rw-rw-   0        0        0     4410 2023-11-15 05:33:03.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/token_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15832 2023-11-15 05:33:04.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/user_pb2.py
+-rw-rw-rw-   0        0        0    20705 2023-11-15 05:33:04.000000 kt-ds-api-0.1.9/spaceone/api/identity/v1/user_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.961342 kt-ds-api-0.1.9/spaceone/api/inventory/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:20.000000 kt-ds-api-0.1.9/spaceone/api/inventory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:09.968484 kt-ds-api-0.1.9/spaceone/api/inventory/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:20.000000 kt-ds-api-0.1.9/spaceone/api/inventory/plugin/__init__.py
+-rw-rw-rw-   0        0        0     5821 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/plugin/collector_pb2.py
+-rw-rw-rw-   0        0        0     6982 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/plugin/collector_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.021950 kt-ds-api-0.1.9/spaceone/api/inventory/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:20.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/__init__.py
+-rw-rw-rw-   0        0        0     6295 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/change_history_pb2.py
+-rw-rw-rw-   0        0        0     4653 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/change_history_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13338 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_pb2.py
+-rw-rw-rw-   0        0        0    23915 2023-11-15 05:33:16.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5296 2023-11-15 05:33:17.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_tag_pb2.py
+-rw-rw-rw-   0        0        0     4735 2023-11-15 05:33:17.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_tag_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11463 2023-11-15 05:33:17.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_type_pb2.py
+-rw-rw-rw-   0        0        0    17823 2023-11-15 05:33:17.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py
+-rw-rw-rw-   0        0        0    26939 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/collector_pb2.py
+-rw-rw-rw-   0        0        0    45613 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/collector_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6229 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_pb2.py
+-rw-rw-rw-   0        0        0    10829 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8400 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_task_pb2.py
+-rw-rw-rw-   0        0        0    10854 2023-11-15 05:33:18.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_task_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8331 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/note_pb2.py
+-rw-rw-rw-   0        0        0    11595 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/note_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8888 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/region_pb2.py
+-rw-rw-rw-   0        0        0    15623 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/region_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10822 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/resource_group_pb2.py
+-rw-rw-rw-   0        0        0    18633 2023-11-15 05:33:19.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/resource_group_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15572 2023-11-15 05:33:20.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/server_pb2.py
+-rw-rw-rw-   0        0        0    13130 2023-11-15 05:33:20.000000 kt-ds-api-0.1.9/spaceone/api/inventory/v1/server_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.024951 kt-ds-api-0.1.9/spaceone/api/monitoring/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:28.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.050804 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:28.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/__init__.py
+-rw-rw-rw-   0        0        0     3227 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/data_source_pb2.py
+-rw-rw-rw-   0        0        0     4901 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3716 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/event_pb2.py
+-rw-rw-rw-   0        0        0     2936 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/event_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3086 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/log_pb2.py
+-rw-rw-rw-   0        0        0     2714 2023-11-15 05:33:22.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/log_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4889 2023-11-15 05:33:23.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/metric_pb2.py
+-rw-rw-rw-   0        0        0     4868 2023-11-15 05:33:23.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/metric_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3320 2023-11-15 05:33:23.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/webhook_pb2.py
+-rw-rw-rw-   0        0        0     4865 2023-11-15 05:33:23.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.098512 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:28.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/__init__.py
+-rw-rw-rw-   0        0        0    19229 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/alert_pb2.py
+-rw-rw-rw-   0        0        0    32376 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/alert_pb2_grpc.py
+-rw-rw-rw-   0        0        0    14879 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/data_source_pb2.py
+-rw-rw-rw-   0        0        0    29312 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/data_source_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15551 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/escalation_policy_pb2.py
+-rw-rw-rw-   0        0        0    19800 2023-11-15 05:33:24.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8148 2023-11-15 05:33:25.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_pb2.py
+-rw-rw-rw-   0        0        0    12965 2023-11-15 05:33:25.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16897 2023-11-15 05:33:25.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_rule_pb2.py
+-rw-rw-rw-   0        0        0    20365 2023-11-15 05:33:25.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2857 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/log_pb2.py
+-rw-rw-rw-   0        0        0     2664 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/log_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11647 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/maintenance_window_pb2.py
+-rw-rw-rw-   0        0        0    17707 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/maintenance_window_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5444 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/metric_pb2.py
+-rw-rw-rw-   0        0        0     7689 2023-11-15 05:33:26.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/metric_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8364 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/note_pb2.py
+-rw-rw-rw-   0        0        0    14119 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/note_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12030 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/project_alert_config_pb2.py
+-rw-rw-rw-   0        0        0    16871 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13969 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/webhook_pb2.py
+-rw-rw-rw-   0        0        0    26926 2023-11-15 05:33:27.000000 kt-ds-api-0.1.9/spaceone/api/monitoring/v1/webhook_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.098512 kt-ds-api-0.1.9/spaceone/api/notification/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.115032 kt-ds-api-0.1.9/spaceone/api/notification/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-11-15 05:33:29.000000 kt-ds-api-0.1.9/spaceone/api/notification/plugin/notification_pb2.py
+-rw-rw-rw-   0        0        0     4596 2023-11-15 05:33:29.000000 kt-ds-api-0.1.9/spaceone/api/notification/plugin/notification_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3189 2023-11-15 05:33:30.000000 kt-ds-api-0.1.9/spaceone/api/notification/plugin/protocol_pb2.py
+-rw-rw-rw-   0        0        0     5016 2023-11-15 05:33:30.000000 kt-ds-api-0.1.9/spaceone/api/notification/plugin/protocol_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.155646 kt-ds-api-0.1.9/spaceone/api/notification/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/__init__.py
+-rw-rw-rw-   0        0        0    14203 2023-11-15 05:33:30.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_pb2.py
+-rw-rw-rw-   0        0        0    20070 2023-11-15 05:33:30.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5276 2023-11-15 05:33:30.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_usage_pb2.py
+-rw-rw-rw-   0        0        0     5480 2023-11-15 05:33:31.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_usage_pb2_grpc.py
+-rw-rw-rw-   0        0        0    17683 2023-11-15 05:33:31.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/project_channel_pb2.py
+-rw-rw-rw-   0        0        0    27678 2023-11-15 05:33:31.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/project_channel_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15094 2023-11-15 05:33:31.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/protocol_pb2.py
+-rw-rw-rw-   0        0        0    28786 2023-11-15 05:33:31.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/protocol_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7849 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/quota_pb2.py
+-rw-rw-rw-   0        0        0    13903 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/quota_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16112 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/user_channel_pb2.py
+-rw-rw-rw-   0        0        0    27452 2023-11-15 05:33:32.000000 kt-ds-api-0.1.9/spaceone/api/notification/v1/user_channel_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.159647 kt-ds-api-0.1.9/spaceone/api/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.173611 kt-ds-api-0.1.9/spaceone/api/plugin/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/v1/__init__.py
+-rw-rw-rw-   0        0        0     4492 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/v1/plugin_pb2.py
+-rw-rw-rw-   0        0        0     5093 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/v1/plugin_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15826 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/v1/supervisor_pb2.py
+-rw-rw-rw-   0        0        0    26433 2023-11-15 05:33:10.000000 kt-ds-api-0.1.9/spaceone/api/plugin/v1/supervisor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.177377 kt-ds-api-0.1.9/spaceone/api/provisioning/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.275470 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/__init__.py
+-rw-rw-rw-   0        0        0    12523 2023-11-15 05:33:59.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_pb2.py
+-rw-rw-rw-   0        0        0    17218 2023-11-15 05:33:59.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7919 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_history_pb2.py
+-rw-rw-rw-   0        0        0     7318 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_history_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12116 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_pb2.py
+-rw-rw-rw-   0        0        0    12872 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_pb2_grpc.py
+-rw-rw-rw-   0        0        0      951 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/consumers_pb2.py
+-rw-rw-rw-   0        0        0      903 2023-11-15 05:34:00.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/consumers_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9138 2023-11-15 05:34:01.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_group_pb2.py
+-rw-rw-rw-   0        0        0    12635 2023-11-15 05:34:01.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_group_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10761 2023-11-15 05:34:01.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_pb2.py
+-rw-rw-rw-   0        0        0    11967 2023-11-15 05:34:01.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9259 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_tag_pb2.py
+-rw-rw-rw-   0        0        0    12407 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_tag_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11394 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_pb2.py
+-rw-rw-rw-   0        0        0    15077 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7645 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_history_pb2.py
+-rw-rw-rw-   0        0        0     7204 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_history_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11740 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_pb2.py
+-rw-rw-rw-   0        0        0    12644 2023-11-15 05:34:02.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7959 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/transmission_history_pb2.py
+-rw-rw-rw-   0        0        0     9226 2023-11-15 05:34:03.000000 kt-ds-api-0.1.9/spaceone/api/provisioning/v1/transmission_history_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.278477 kt-ds-api-0.1.9/spaceone/api/repository/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.365920 kt-ds-api-0.1.9/spaceone/api/repository/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/__init__.py
+-rw-rw-rw-   0        0        0    14221 2023-11-15 05:33:06.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/plugin_pb2.py
+-rw-rw-rw-   0        0        0    29261 2023-11-15 05:33:06.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/plugin_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10282 2023-11-15 05:33:06.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/policy_pb2.py
+-rw-rw-rw-   0        0        0    15964 2023-11-15 05:33:06.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/policy_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9305 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/repository_pb2.py
+-rw-rw-rw-   0        0        0    14137 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/repository_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10176 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/schema_pb2.py
+-rw-rw-rw-   0        0        0    15467 2023-11-15 05:33:07.000000 kt-ds-api-0.1.9/spaceone/api/repository/v1/schema_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.368189 kt-ds-api-0.1.9/spaceone/api/sample/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/api/sample/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.379742 kt-ds-api-0.1.9/spaceone/api/sample/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/api/sample/v1/__init__.py
+-rw-rw-rw-   0        0        0     2032 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/api/sample/v1/helloworld_pb2.py
+-rw-rw-rw-   0        0        0     2703 2023-11-15 05:32:52.000000 kt-ds-api-0.1.9/spaceone/api/sample/v1/helloworld_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.384743 kt-ds-api-0.1.9/spaceone/api/secret/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:14.000000 kt-ds-api-0.1.9/spaceone/api/secret/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.400036 kt-ds-api-0.1.9/spaceone/api/secret/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:14.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/__init__.py
+-rw-rw-rw-   0        0        0    11668 2023-11-15 05:33:13.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_group_pb2.py
+-rw-rw-rw-   0        0        0    15293 2023-11-15 05:33:13.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_group_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11883 2023-11-15 05:33:13.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_pb2.py
+-rw-rw-rw-   0        0        0    19449 2023-11-15 05:33:13.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11152 2023-11-15 05:33:14.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/trusted_secret_pb2.py
+-rw-rw-rw-   0        0        0    17527 2023-11-15 05:33:14.000000 kt-ds-api-0.1.9/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.400036 kt-ds-api-0.1.9/spaceone/api/statistics/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:36.000000 kt-ds-api-0.1.9/spaceone/api/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.411180 kt-ds-api-0.1.9/spaceone/api/statistics/plugin/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:36.000000 kt-ds-api-0.1.9/spaceone/api/statistics/plugin/__init__.py
+-rw-rw-rw-   0        0        0     3955 2023-11-15 05:33:34.000000 kt-ds-api-0.1.9/spaceone/api/statistics/plugin/storage_pb2.py
+-rw-rw-rw-   0        0        0     6207 2023-11-15 05:33:34.000000 kt-ds-api-0.1.9/spaceone/api/statistics/plugin/storage_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-11-15 05:40:10.434454 kt-ds-api-0.1.9/spaceone/api/statistics/v1/
+-rw-rw-rw-   0        0        0        0 2023-11-15 05:33:36.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/__init__.py
+-rw-rw-rw-   0        0        0     5752 2023-11-15 05:33:34.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/history_pb2.py
+-rw-rw-rw-   0        0        0     7655 2023-11-15 05:33:35.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/history_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9047 2023-11-15 05:33:35.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/resource_pb2.py
+-rw-rw-rw-   0        0        0     7684 2023-11-15 05:33:35.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/resource_pb2_grpc.py
+-rw-rw-rw-   0        0        0    11875 2023-11-15 05:33:35.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/schedule_pb2.py
+-rw-rw-rw-   0        0        0    76967 2023-11-15 05:33:35.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/schedule_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13587 2023-11-15 05:33:36.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/storage_pb2.py
+-rw-rw-rw-   0        0        0    18596 2023-11-15 05:33:36.000000 kt-ds-api-0.1.9/spaceone/api/statistics/v1/storage_pb2_grpc.py
```

### Comparing `kt-ds-api-0.1.8/kt_ds_api.egg-info/SOURCES.txt` & `kt-ds-api-0.1.9/kt_ds_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/setup.py` & `kt-ds-api-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/board/v1/board_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/board/v1/board_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/board/v1/board_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/board/v1/board_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/board/v1/post_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/board/v1/post_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/board/v1/post_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/board/v1/post_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/config/v1/domain_config_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/config/v1/domain_config_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/config/v1/domain_config_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/config/v1/domain_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/config/v1/user_config_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/config/v1/user_config_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/config/v1/user_config_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/config/v1/user_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/core/v1/handler_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/core/v1/handler_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/core/v1/query_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/core/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/core/v1/server_info_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/core/v1/server_info_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/core/v1/server_info_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/core/v1/server_info_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/cost_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/cost_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/data_source_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/job_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/job_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_usage_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/custom_widget_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/custom_widget_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/custom_widget_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/custom_widget_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/exchange_rate_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/exchange_rate_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/exchange_rate_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/exchange_rate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_task_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_task_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/monthly_exchange_rate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/public_dashboard_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/public_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/public_dashboard_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/public_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/schedule_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/schedule_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/user_dashboard_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/user_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/cost_analysis/v1/user_dashboard_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/cost_analysis/v1/user_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/custom_widget_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/custom_widget_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/custom_widget_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/custom_widget_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/domain_dashboard_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/domain_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/domain_dashboard_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/domain_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/project_dashboard_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/project_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/dashboard/v1/project_dashboard_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/dashboard/v1/project_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/file_manager/v1/file_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/file_manager/v1/file_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/file_manager/v1/file_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/file_manager/v1/file_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/plugin/auth_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/plugin/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/plugin/auth_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/plugin/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/api_key_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/api_key_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/api_key_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/authorization_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/authorization_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/authorization_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_owner_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_owner_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_owner_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_owner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/domain_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/domain_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/endpoint_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/endpoint_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/endpoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/policy_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/policy_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/policy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/project_group_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/project_group_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/project_group_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/project_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/project_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/project_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/provider_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/provider_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/role_binding_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/role_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/role_binding_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/role_binding_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/role_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/role_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/service_account_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/service_account_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/service_account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/token_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/token_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/token_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/user_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/user_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v1 import query_pb2 as spaceone_dot_api_dot_core_dot_v1_dot_query__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#spaceone/api/identity/v1/user.proto\x12\x18spaceone.api.identity.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v1/query.proto\"\xa0\x02\n\x11\x43reateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tuser_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x06 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\n \x01(\t\"\xb1\x01\n\x11UpdateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\n \x01(\t\"~\n\x19SetRequiredActionsRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12=\n\x07\x61\x63tions\x18\x02 \x03(\x0e\x32,.spaceone.api.identity.v1.UserRequiredAction\x12\x11\n\tdomain_id\x18\x03 \x01(\t\"1\n\x0bUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"B\n\x0eGetUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\x12\x0c\n\x04only\x18\x03 \x03(\t\"\xf6\x01\n\tUserQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v1.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tuser_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x07 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x11\n\tdomain_id\x18\x0b \x01(\t\"\xef\x03\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x37\n\x05state\x18\x03 \x01(\x0e\x32(.spaceone.api.identity.v1.UserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tuser_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x06 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12\x46\n\x10required_actions\x18\t \x03(\x0e\x32,.spaceone.api.identity.v1.UserRequiredAction\x12%\n\x04tags\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x18\n\x10last_accessed_at\x18\x0b \x01(\t\x12\x12\n\ncreated_at\x18\x0c \x01(\t\x12\x11\n\tdomain_id\x18\r \x01(\t\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"U\n\tUsersInfo\x12\x33\n\x07results\x18\x01 \x03(\x0b\x32\".spaceone.api.identity.v1.UserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"X\n\rUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v1.StatisticsQuery\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"F\n\x0e\x46indUserSearch\x12\x11\n\x07user_id\x18\x01 \x01(\tH\x00\x12\x11\n\x07keyword\x18\x02 \x01(\tH\x00\x42\x0e\n\x0csearch_alias\"\\\n\rFindUserQuery\x12\x38\n\x06search\x18\x01 \x01(\x0b\x32(.spaceone.api.identity.v1.FindUserSearch\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"c\n\x0c\x46indUserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"]\n\rFindUsersInfo\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.spaceone.api.identity.v1.FindUserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05*8\n\x0bUserBackend\x12\x10\n\x0cNONE_BACKEND\x10\x00\x12\t\n\x05LOCAL\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02*6\n\x08UserType\x12\x12\n\x0eNONE_USER_TYPE\x10\x00\x12\x08\n\x04USER\x10\x01\x12\x0c\n\x08\x41PI_USER\x10\x02*K\n\x12UserRequiredAction\x12\x13\n\x0fUPDATE_PASSWORD\x10\x00\x12 \n\x1cPASS_PREVENT_LOGIN_DUPLICATE\x10\x01\x32\xe1\n\n\x04User\x12u\n\x06\x63reate\x12+.spaceone.api.identity.v1.CreateUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x12/identity/v1/users\x12u\n\x06update\x12+.spaceone.api.identity.v1.UpdateUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1a\x82\xd3\xe4\x93\x02\x14\x1a\x12/identity/v1/users\x12\xa0\x01\n\x14set_required_actions\x12\x33.spaceone.api.identity.v1.SetRequiredActionsRequest\x1a\".spaceone.api.identity.v1.UserInfo\"/\x82\xd3\xe4\x93\x02)\"\'/identity/v1/users/set-required-actions\x12\x7f\n\x06\x65nable\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"*\x82\xd3\xe4\x93\x02$\x1a\"/identity/v1/user/{user_id}/enable\x12\x81\x01\n\x07\x64isable\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"+\x82\xd3\xe4\x93\x02%\x1a#/identity/v1/user/{user_id}/disable\x12\x63\n\x06\x64\x65lete\x12%.spaceone.api.identity.v1.UserRequest\x1a\x16.google.protobuf.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14*\x12/identity/v1/users\x12x\n\x03get\x12(.spaceone.api.identity.v1.GetUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/identity/v1/user/{user_id}\x12\x89\x01\n\x04list\x12#.spaceone.api.identity.v1.UserQuery\x1a#.spaceone.api.identity.v1.UsersInfo\"7\x82\xd3\xe4\x93\x02\x31\x12\x12/identity/v1/usersZ\x1b\"\x19/identity/v1/users/search\x12i\n\x04stat\x12\'.spaceone.api.identity.v1.UserStatQuery\x1a\x17.google.protobuf.Struct\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/stat\x12y\n\x04\x66ind\x12\'.spaceone.api.identity.v1.FindUserQuery\x1a\'.spaceone.api.identity.v1.FindUsersInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/find\x12r\n\x04sync\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/syncb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#spaceone/api/identity/v1/user.proto\x12\x18spaceone.api.identity.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v1/query.proto\"\xa0\x02\n\x11\x43reateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tuser_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x06 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\n \x01(\t\"\xc7\x01\n\x11UpdateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x14\n\x0cold_password\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x10\n\x08language\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\n \x01(\t\"~\n\x19SetRequiredActionsRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12=\n\x07\x61\x63tions\x18\x02 \x03(\x0e\x32,.spaceone.api.identity.v1.UserRequiredAction\x12\x11\n\tdomain_id\x18\x03 \x01(\t\"1\n\x0bUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"B\n\x0eGetUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\x12\x0c\n\x04only\x18\x03 \x03(\t\"\xf6\x01\n\tUserQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v1.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tuser_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x07 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x11\n\tdomain_id\x18\x0b \x01(\t\"\xef\x03\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x37\n\x05state\x18\x03 \x01(\x0e\x32(.spaceone.api.identity.v1.UserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tuser_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v1.UserType\x12\x36\n\x07\x62\x61\x63kend\x18\x06 \x01(\x0e\x32%.spaceone.api.identity.v1.UserBackend\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12\x46\n\x10required_actions\x18\t \x03(\x0e\x32,.spaceone.api.identity.v1.UserRequiredAction\x12%\n\x04tags\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x18\n\x10last_accessed_at\x18\x0b \x01(\t\x12\x12\n\ncreated_at\x18\x0c \x01(\t\x12\x11\n\tdomain_id\x18\r \x01(\t\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"U\n\tUsersInfo\x12\x33\n\x07results\x18\x01 \x03(\x0b\x32\".spaceone.api.identity.v1.UserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"X\n\rUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v1.StatisticsQuery\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"F\n\x0e\x46indUserSearch\x12\x11\n\x07user_id\x18\x01 \x01(\tH\x00\x12\x11\n\x07keyword\x18\x02 \x01(\tH\x00\x42\x0e\n\x0csearch_alias\"\\\n\rFindUserQuery\x12\x38\n\x06search\x18\x01 \x01(\x0b\x32(.spaceone.api.identity.v1.FindUserSearch\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"c\n\x0c\x46indUserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"]\n\rFindUsersInfo\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.spaceone.api.identity.v1.FindUserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05*8\n\x0bUserBackend\x12\x10\n\x0cNONE_BACKEND\x10\x00\x12\t\n\x05LOCAL\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02*6\n\x08UserType\x12\x12\n\x0eNONE_USER_TYPE\x10\x00\x12\x08\n\x04USER\x10\x01\x12\x0c\n\x08\x41PI_USER\x10\x02*K\n\x12UserRequiredAction\x12\x13\n\x0fUPDATE_PASSWORD\x10\x00\x12 \n\x1cPASS_PREVENT_LOGIN_DUPLICATE\x10\x01\x32\xe1\n\n\x04User\x12u\n\x06\x63reate\x12+.spaceone.api.identity.v1.CreateUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x12/identity/v1/users\x12u\n\x06update\x12+.spaceone.api.identity.v1.UpdateUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1a\x82\xd3\xe4\x93\x02\x14\x1a\x12/identity/v1/users\x12\xa0\x01\n\x14set_required_actions\x12\x33.spaceone.api.identity.v1.SetRequiredActionsRequest\x1a\".spaceone.api.identity.v1.UserInfo\"/\x82\xd3\xe4\x93\x02)\"\'/identity/v1/users/set-required-actions\x12\x7f\n\x06\x65nable\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"*\x82\xd3\xe4\x93\x02$\x1a\"/identity/v1/user/{user_id}/enable\x12\x81\x01\n\x07\x64isable\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"+\x82\xd3\xe4\x93\x02%\x1a#/identity/v1/user/{user_id}/disable\x12\x63\n\x06\x64\x65lete\x12%.spaceone.api.identity.v1.UserRequest\x1a\x16.google.protobuf.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14*\x12/identity/v1/users\x12x\n\x03get\x12(.spaceone.api.identity.v1.GetUserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/identity/v1/user/{user_id}\x12\x89\x01\n\x04list\x12#.spaceone.api.identity.v1.UserQuery\x1a#.spaceone.api.identity.v1.UsersInfo\"7\x82\xd3\xe4\x93\x02\x31\x12\x12/identity/v1/usersZ\x1b\"\x19/identity/v1/users/search\x12i\n\x04stat\x12\'.spaceone.api.identity.v1.UserStatQuery\x1a\x17.google.protobuf.Struct\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/stat\x12y\n\x04\x66ind\x12\'.spaceone.api.identity.v1.FindUserQuery\x1a\'.spaceone.api.identity.v1.FindUsersInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/find\x12r\n\x04sync\x12%.spaceone.api.identity.v1.UserRequest\x1a\".spaceone.api.identity.v1.UserInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/identity/v1/users/syncb\x06proto3')
 
 _USERBACKEND = DESCRIPTOR.enum_types_by_name['UserBackend']
 UserBackend = enum_type_wrapper.EnumTypeWrapper(_USERBACKEND)
 _USERTYPE = DESCRIPTOR.enum_types_by_name['UserType']
 UserType = enum_type_wrapper.EnumTypeWrapper(_USERTYPE)
 _USERREQUIREDACTION = DESCRIPTOR.enum_types_by_name['UserRequiredAction']
 UserRequiredAction = enum_type_wrapper.EnumTypeWrapper(_USERREQUIREDACTION)
@@ -164,44 +164,44 @@
   _USER.methods_by_name['list']._serialized_options = b'\202\323\344\223\0021\022\022/identity/v1/usersZ\033\"\031/identity/v1/users/search'
   _USER.methods_by_name['stat']._options = None
   _USER.methods_by_name['stat']._serialized_options = b'\202\323\344\223\002\031\"\027/identity/v1/users/stat'
   _USER.methods_by_name['find']._options = None
   _USER.methods_by_name['find']._serialized_options = b'\202\323\344\223\002\031\"\027/identity/v1/users/find'
   _USER.methods_by_name['sync']._options = None
   _USER.methods_by_name['sync']._serialized_options = b'\202\323\344\223\002\031\"\027/identity/v1/users/sync'
-  _USERBACKEND._serialized_start=2192
-  _USERBACKEND._serialized_end=2248
-  _USERTYPE._serialized_start=2250
-  _USERTYPE._serialized_end=2304
-  _USERREQUIREDACTION._serialized_start=2306
-  _USERREQUIREDACTION._serialized_end=2381
+  _USERBACKEND._serialized_start=2214
+  _USERBACKEND._serialized_end=2270
+  _USERTYPE._serialized_start=2272
+  _USERTYPE._serialized_end=2326
+  _USERREQUIREDACTION._serialized_start=2328
+  _USERREQUIREDACTION._serialized_end=2403
   _CREATEUSERREQUEST._serialized_start=189
   _CREATEUSERREQUEST._serialized_end=477
   _UPDATEUSERREQUEST._serialized_start=480
-  _UPDATEUSERREQUEST._serialized_end=657
-  _SETREQUIREDACTIONSREQUEST._serialized_start=659
-  _SETREQUIREDACTIONSREQUEST._serialized_end=785
-  _USERREQUEST._serialized_start=787
-  _USERREQUEST._serialized_end=836
-  _GETUSERREQUEST._serialized_start=838
-  _GETUSERREQUEST._serialized_end=904
-  _USERQUERY._serialized_start=907
-  _USERQUERY._serialized_end=1153
-  _USERINFO._serialized_start=1156
-  _USERINFO._serialized_end=1651
-  _USERINFO_STATE._serialized_start=1594
-  _USERINFO_STATE._serialized_end=1651
-  _USERSINFO._serialized_start=1653
-  _USERSINFO._serialized_end=1738
-  _USERSTATQUERY._serialized_start=1740
-  _USERSTATQUERY._serialized_end=1828
-  _FINDUSERSEARCH._serialized_start=1830
-  _FINDUSERSEARCH._serialized_end=1900
-  _FINDUSERQUERY._serialized_start=1902
-  _FINDUSERQUERY._serialized_end=1994
-  _FINDUSERINFO._serialized_start=1996
-  _FINDUSERINFO._serialized_end=2095
-  _FINDUSERSINFO._serialized_start=2097
-  _FINDUSERSINFO._serialized_end=2190
-  _USER._serialized_start=2384
-  _USER._serialized_end=3761
+  _UPDATEUSERREQUEST._serialized_end=679
+  _SETREQUIREDACTIONSREQUEST._serialized_start=681
+  _SETREQUIREDACTIONSREQUEST._serialized_end=807
+  _USERREQUEST._serialized_start=809
+  _USERREQUEST._serialized_end=858
+  _GETUSERREQUEST._serialized_start=860
+  _GETUSERREQUEST._serialized_end=926
+  _USERQUERY._serialized_start=929
+  _USERQUERY._serialized_end=1175
+  _USERINFO._serialized_start=1178
+  _USERINFO._serialized_end=1673
+  _USERINFO_STATE._serialized_start=1616
+  _USERINFO_STATE._serialized_end=1673
+  _USERSINFO._serialized_start=1675
+  _USERSINFO._serialized_end=1760
+  _USERSTATQUERY._serialized_start=1762
+  _USERSTATQUERY._serialized_end=1850
+  _FINDUSERSEARCH._serialized_start=1852
+  _FINDUSERSEARCH._serialized_end=1922
+  _FINDUSERQUERY._serialized_start=1924
+  _FINDUSERQUERY._serialized_end=2016
+  _FINDUSERINFO._serialized_start=2018
+  _FINDUSERINFO._serialized_end=2117
+  _FINDUSERSINFO._serialized_start=2119
+  _FINDUSERSINFO._serialized_end=2212
+  _USER._serialized_start=2406
+  _USER._serialized_end=3783
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kt-ds-api-0.1.8/spaceone/api/identity/v1/user_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/identity/v1/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/plugin/collector_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/plugin/collector_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/plugin/collector_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/plugin/collector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/change_history_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/change_history_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/change_history_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/change_history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_tag_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_tag_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_tag_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_tag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_type_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_type_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/collector_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/collector_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/collector_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/collector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_task_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_task_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/job_task_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/job_task_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/note_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/note_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/note_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/note_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/region_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/region_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/region_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/resource_group_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/resource_group_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/resource_group_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/resource_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/server_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/server_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/inventory/v1/server_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/inventory/v1/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/data_source_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/event_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/event_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/event_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/log_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/log_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/log_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/metric_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/metric_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/metric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/webhook_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/alert_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/alert_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/data_source_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/data_source_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/escalation_policy_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/escalation_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_rule_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_rule_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/log_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/log_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/maintenance_window_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/maintenance_window_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/maintenance_window_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/maintenance_window_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/metric_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/metric_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/metric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/note_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/note_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/note_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/note_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/project_alert_config_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/project_alert_config_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/webhook_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/monitoring/v1/webhook_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/monitoring/v1/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/plugin/notification_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/plugin/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/plugin/notification_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/plugin/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/plugin/protocol_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/plugin/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/plugin/protocol_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/plugin/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_usage_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/notification_usage_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/notification_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/project_channel_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/project_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/project_channel_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/project_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/protocol_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/protocol_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/quota_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/quota_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/quota_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/user_channel_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/user_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/notification/v1/user_channel_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/notification/v1/user_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/plugin/v1/plugin_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/plugin/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/plugin/v1/plugin_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/plugin/v1/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/plugin/v1/supervisor_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/plugin/v1/supervisor_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/plugin/v1/supervisor_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/plugin/v1/supervisor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_history_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_history_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_history_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/catalog_resource_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/catalog_resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/consumers_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/consumers_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/consumers_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/consumers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_group_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_group_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_group_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_tag_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_tag_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/resource_tag_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/resource_tag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_history_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_history_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_history_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/stack_resource_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/stack_resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/transmission_history_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/transmission_history_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/provisioning/v1/transmission_history_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/provisioning/v1/transmission_history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/plugin_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/plugin_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/policy_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/policy_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/policy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/repository_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/repository_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/schema_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/repository/v1/schema_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/repository/v1/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/sample/v1/helloworld_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/sample/v1/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/sample/v1/helloworld_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/sample/v1/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_group_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_group_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_group_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/secret_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/trusted_secret_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/trusted_secret_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/plugin/storage_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/plugin/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/plugin/storage_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/plugin/storage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/history_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/history_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/history_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/resource_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/resource_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/schedule_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/schedule_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/storage_pb2.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `kt-ds-api-0.1.8/spaceone/api/statistics/v1/storage_pb2_grpc.py` & `kt-ds-api-0.1.9/spaceone/api/statistics/v1/storage_pb2_grpc.py`

 * *Files identical despite different names*

