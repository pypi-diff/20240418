# Comparing `tmp/alibabacloud_dingtalk-2.0.95.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.95.tar", last modified: Mon Apr 15 10:46:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.96.tar", last modified: Thu Apr 18 04:15:40 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.95.tar` & `alibabacloud_dingtalk-2.0.96.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/
--rw-r--r--   0 root         (0) root         (0)   120327 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2650 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18818 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12444 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71584 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101499 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143706 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   201494 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334068 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418722 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   257462 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   615355 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136761 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208587 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25614 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31620 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   161460 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58076 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94327 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77172 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133813 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198336 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413640 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494302 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   740928 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/
+-rw-r--r--   0 root         (0) root         (0)   121863 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21346 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23757 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12444 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71584 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101499 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143706 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   201494 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   257462 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   615355 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25614 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31620 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   161460 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77172 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133813 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198336 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413640 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494302 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   751756 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.95/ChangeLog.md` & `alibabacloud_dingtalk-2.0.96/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-15 Version: 2.0.95
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-04-09 Version: 2.0.94
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-02 Version: 2.0.93
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-26 Version: 2.0.92
```

### Comparing `alibabacloud_dingtalk-2.0.95/LICENSE` & `alibabacloud_dingtalk-2.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/PKG-INFO` & `alibabacloud_dingtalk-2.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.95
+Version: 2.0.96
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.95/README-CN.md` & `alibabacloud_dingtalk-2.0.96/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/README.md` & `alibabacloud_dingtalk-2.0.96/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -303,14 +303,112 @@
         self,
         request: dingtalkai_interaction__1__0_models.ReplyRequest,
     ) -> dingtalkai_interaction__1__0_models.ReplyResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkai_interaction__1__0_models.ReplyHeaders()
         return await self.reply_with_options_async(request, headers, runtime)
 
+    def send_with_options(
+        self,
+        request: dingtalkai_interaction__1__0_models.SendRequest,
+        headers: dingtalkai_interaction__1__0_models.SendHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkai_interaction__1__0_models.SendResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.content_type):
+            body['contentType'] = request.content_type
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='Send',
+            version='aiInteraction_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/aiInteraction/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkai_interaction__1__0_models.SendResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def send_with_options_async(
+        self,
+        request: dingtalkai_interaction__1__0_models.SendRequest,
+        headers: dingtalkai_interaction__1__0_models.SendHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkai_interaction__1__0_models.SendResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.content_type):
+            body['contentType'] = request.content_type
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='Send',
+            version='aiInteraction_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/aiInteraction/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkai_interaction__1__0_models.SendResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def send(
+        self,
+        request: dingtalkai_interaction__1__0_models.SendRequest,
+    ) -> dingtalkai_interaction__1__0_models.SendResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkai_interaction__1__0_models.SendHeaders()
+        return self.send_with_options(request, headers, runtime)
+
+    async def send_async(
+        self,
+        request: dingtalkai_interaction__1__0_models.SendRequest,
+    ) -> dingtalkai_interaction__1__0_models.SendResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkai_interaction__1__0_models.SendHeaders()
+        return await self.send_with_options_async(request, headers, runtime)
+
     def update_with_options(
         self,
         request: dingtalkai_interaction__1__0_models.UpdateRequest,
         headers: dingtalkai_interaction__1__0_models.UpdateHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkai_interaction__1__0_models.UpdateResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -501,14 +501,189 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ReplyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SendHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SendRequest(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        content_type: str = None,
+        open_conversation_id: str = None,
+        union_id: str = None,
+    ):
+        self.content = content
+        self.content_type = content_type
+        self.open_conversation_id = open_conversation_id
+        self.union_id = union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['content'] = self.content
+        if self.content_type is not None:
+            result['contentType'] = self.content_type
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('contentType') is not None:
+            self.content_type = m.get('contentType')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class SendResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class SendResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SendResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SendResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SendResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SendResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SendResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9336,23 +9336,266 @@
         if m.get('systemToken') is not None:
             self.system_token = m.get('systemToken')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
+class GetOperationRecordsResponseBodyResultDomainListOperatorAgentIdList(TeaModel):
+    def __init__(
+        self,
+        department_description: str = None,
+        display_name: str = None,
+        display_name_in_english: str = None,
+        order_number: str = None,
+        personal_photo: str = None,
+        status: str = None,
+        user_id: str = None,
+        user_information: str = None,
+    ):
+        self.department_description = department_description
+        self.display_name = display_name
+        self.display_name_in_english = display_name_in_english
+        self.order_number = order_number
+        self.personal_photo = personal_photo
+        self.status = status
+        self.user_id = user_id
+        self.user_information = user_information
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_description is not None:
+            result['departmentDescription'] = self.department_description
+        if self.display_name is not None:
+            result['displayName'] = self.display_name
+        if self.display_name_in_english is not None:
+            result['displayNameInEnglish'] = self.display_name_in_english
+        if self.order_number is not None:
+            result['orderNumber'] = self.order_number
+        if self.personal_photo is not None:
+            result['personalPhoto'] = self.personal_photo
+        if self.status is not None:
+            result['status'] = self.status
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_information is not None:
+            result['userInformation'] = self.user_information
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('departmentDescription') is not None:
+            self.department_description = m.get('departmentDescription')
+        if m.get('displayName') is not None:
+            self.display_name = m.get('displayName')
+        if m.get('displayNameInEnglish') is not None:
+            self.display_name_in_english = m.get('displayNameInEnglish')
+        if m.get('orderNumber') is not None:
+            self.order_number = m.get('orderNumber')
+        if m.get('personalPhoto') is not None:
+            self.personal_photo = m.get('personalPhoto')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userInformation') is not None:
+            self.user_information = m.get('userInformation')
+        return self
+
+
+class GetOperationRecordsResponseBodyResultDomainList(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        active_time_gmt: str = None,
+        activity_id: str = None,
+        digital_signature: str = None,
+        files: str = None,
+        format_action: str = None,
+        operate_time_gmt: str = None,
+        operate_type: str = None,
+        operator: str = None,
+        operator_agent_id_list: List[GetOperationRecordsResponseBodyResultDomainListOperatorAgentIdList] = None,
+        operator_display_name: str = None,
+        operator_name: str = None,
+        operator_nick_name: str = None,
+        operator_photo_url: str = None,
+        operator_status: str = None,
+        process_instance_id: str = None,
+        remark: str = None,
+        show_name: str = None,
+        size: int = None,
+        task_execute_type: str = None,
+        task_hold_time_gmt: int = None,
+        task_id: str = None,
+        task_type: str = None,
+        type: str = None,
+    ):
+        self.action = action
+        self.active_time_gmt = active_time_gmt
+        self.activity_id = activity_id
+        self.digital_signature = digital_signature
+        self.files = files
+        self.format_action = format_action
+        self.operate_time_gmt = operate_time_gmt
+        self.operate_type = operate_type
+        self.operator = operator
+        self.operator_agent_id_list = operator_agent_id_list
+        self.operator_display_name = operator_display_name
+        self.operator_name = operator_name
+        self.operator_nick_name = operator_nick_name
+        self.operator_photo_url = operator_photo_url
+        self.operator_status = operator_status
+        self.process_instance_id = process_instance_id
+        self.remark = remark
+        self.show_name = show_name
+        self.size = size
+        self.task_execute_type = task_execute_type
+        self.task_hold_time_gmt = task_hold_time_gmt
+        self.task_id = task_id
+        self.task_type = task_type
+        self.type = type
+
+    def validate(self):
+        if self.operator_agent_id_list:
+            for k in self.operator_agent_id_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['action'] = self.action
+        if self.active_time_gmt is not None:
+            result['activeTimeGMT'] = self.active_time_gmt
+        if self.activity_id is not None:
+            result['activityId'] = self.activity_id
+        if self.digital_signature is not None:
+            result['digitalSignature'] = self.digital_signature
+        if self.files is not None:
+            result['files'] = self.files
+        if self.format_action is not None:
+            result['formatAction'] = self.format_action
+        if self.operate_time_gmt is not None:
+            result['operateTimeGMT'] = self.operate_time_gmt
+        if self.operate_type is not None:
+            result['operateType'] = self.operate_type
+        if self.operator is not None:
+            result['operator'] = self.operator
+        result['operatorAgentIdList'] = []
+        if self.operator_agent_id_list is not None:
+            for k in self.operator_agent_id_list:
+                result['operatorAgentIdList'].append(k.to_map() if k else None)
+        if self.operator_display_name is not None:
+            result['operatorDisplayName'] = self.operator_display_name
+        if self.operator_name is not None:
+            result['operatorName'] = self.operator_name
+        if self.operator_nick_name is not None:
+            result['operatorNickName'] = self.operator_nick_name
+        if self.operator_photo_url is not None:
+            result['operatorPhotoUrl'] = self.operator_photo_url
+        if self.operator_status is not None:
+            result['operatorStatus'] = self.operator_status
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.show_name is not None:
+            result['showName'] = self.show_name
+        if self.size is not None:
+            result['size'] = self.size
+        if self.task_execute_type is not None:
+            result['taskExecuteType'] = self.task_execute_type
+        if self.task_hold_time_gmt is not None:
+            result['taskHoldTimeGMT'] = self.task_hold_time_gmt
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        if self.task_type is not None:
+            result['taskType'] = self.task_type
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        if m.get('activeTimeGMT') is not None:
+            self.active_time_gmt = m.get('activeTimeGMT')
+        if m.get('activityId') is not None:
+            self.activity_id = m.get('activityId')
+        if m.get('digitalSignature') is not None:
+            self.digital_signature = m.get('digitalSignature')
+        if m.get('files') is not None:
+            self.files = m.get('files')
+        if m.get('formatAction') is not None:
+            self.format_action = m.get('formatAction')
+        if m.get('operateTimeGMT') is not None:
+            self.operate_time_gmt = m.get('operateTimeGMT')
+        if m.get('operateType') is not None:
+            self.operate_type = m.get('operateType')
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        self.operator_agent_id_list = []
+        if m.get('operatorAgentIdList') is not None:
+            for k in m.get('operatorAgentIdList'):
+                temp_model = GetOperationRecordsResponseBodyResultDomainListOperatorAgentIdList()
+                self.operator_agent_id_list.append(temp_model.from_map(k))
+        if m.get('operatorDisplayName') is not None:
+            self.operator_display_name = m.get('operatorDisplayName')
+        if m.get('operatorName') is not None:
+            self.operator_name = m.get('operatorName')
+        if m.get('operatorNickName') is not None:
+            self.operator_nick_name = m.get('operatorNickName')
+        if m.get('operatorPhotoUrl') is not None:
+            self.operator_photo_url = m.get('operatorPhotoUrl')
+        if m.get('operatorStatus') is not None:
+            self.operator_status = m.get('operatorStatus')
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('showName') is not None:
+            self.show_name = m.get('showName')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('taskExecuteType') is not None:
+            self.task_execute_type = m.get('taskExecuteType')
+        if m.get('taskHoldTimeGMT') is not None:
+            self.task_hold_time_gmt = m.get('taskHoldTimeGMT')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        if m.get('taskType') is not None:
+            self.task_type = m.get('taskType')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
 class GetOperationRecordsResponseBodyResult(TeaModel):
     def __init__(
         self,
         action: str = None,
         action_exit: str = None,
         active_time_gmt: str = None,
         activity_id: str = None,
         data_id: int = None,
         digital_sign: str = None,
+        domain_list: List[GetOperationRecordsResponseBodyResultDomainList] = None,
         files: str = None,
         operate_time_gmt: str = None,
         operate_type: str = None,
         operator_display_name: str = None,
         operator_name: str = None,
         operator_nick_name: str = None,
         operator_photo_url: str = None,
@@ -9370,14 +9613,15 @@
     ):
         self.action = action
         self.action_exit = action_exit
         self.active_time_gmt = active_time_gmt
         self.activity_id = activity_id
         self.data_id = data_id
         self.digital_sign = digital_sign
+        self.domain_list = domain_list
         self.files = files
         self.operate_time_gmt = operate_time_gmt
         self.operate_type = operate_type
         self.operator_display_name = operator_display_name
         self.operator_name = operator_name
         self.operator_nick_name = operator_nick_name
         self.operator_photo_url = operator_photo_url
@@ -9390,15 +9634,18 @@
         self.task_execute_type = task_execute_type
         self.task_hold_time_gmt = task_hold_time_gmt
         self.task_id = task_id
         self.task_type = task_type
         self.type = type
 
     def validate(self):
-        pass
+        if self.domain_list:
+            for k in self.domain_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -9410,14 +9657,18 @@
             result['activeTimeGMT'] = self.active_time_gmt
         if self.activity_id is not None:
             result['activityId'] = self.activity_id
         if self.data_id is not None:
             result['dataId'] = self.data_id
         if self.digital_sign is not None:
             result['digitalSign'] = self.digital_sign
+        result['domainList'] = []
+        if self.domain_list is not None:
+            for k in self.domain_list:
+                result['domainList'].append(k.to_map() if k else None)
         if self.files is not None:
             result['files'] = self.files
         if self.operate_time_gmt is not None:
             result['operateTimeGMT'] = self.operate_time_gmt
         if self.operate_type is not None:
             result['operateType'] = self.operate_type
         if self.operator_display_name is not None:
@@ -9462,14 +9713,19 @@
             self.active_time_gmt = m.get('activeTimeGMT')
         if m.get('activityId') is not None:
             self.activity_id = m.get('activityId')
         if m.get('dataId') is not None:
             self.data_id = m.get('dataId')
         if m.get('digitalSign') is not None:
             self.digital_sign = m.get('digitalSign')
+        self.domain_list = []
+        if m.get('domainList') is not None:
+            for k in m.get('domainList'):
+                temp_model = GetOperationRecordsResponseBodyResultDomainList()
+                self.domain_list.append(temp_model.from_map(k))
         if m.get('files') is not None:
             self.files = m.get('files')
         if m.get('operateTimeGMT') is not None:
             self.operate_time_gmt = m.get('operateTimeGMT')
         if m.get('operateType') is not None:
             self.operate_type = m.get('operateType')
         if m.get('operatorDisplayName') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.95
+Version: 2.0.96
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.95/setup.py` & `alibabacloud_dingtalk-2.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 15/04/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

