# Comparing `tmp/tc-core-analyzer-lib-1.2.0.tar.gz` & `tmp/tc_core_analyzer_lib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-core-analyzer-lib-1.2.0.tar", last modified: Thu Mar  7 04:20:05 2024, max compression
+gzip compressed data, was "tc_core_analyzer_lib-1.3.0.tar", last modified: Thu Apr 18 07:53:09 2024, max compression
```

## Comparing `tc-core-analyzer-lib-1.2.0.tar` & `tc_core_analyzer_lib-1.3.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.394663 tc-core-analyzer-lib-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-07 04:20:05.394663 tc-core-analyzer-lib-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 04:20:05.394663 tc-core-analyzer-lib-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.382663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/assess_engagement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.382663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.386663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_all_active_fourteen_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_mention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_replies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_consistently_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_consistently_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_newly_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_vital.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_lone_actions_all_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_lone_thr_actions_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_mention_active_members_from_int_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_newly_active_continuous_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_newly_active_discontinued_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_non_consistently_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_partially_consistently_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_still_active.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_thr_actions_all_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_vital.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.390663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_consistent.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_dropped.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_lurker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_disengaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_paused.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_returned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_unpaused.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_still_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_vital.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_check_past.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_check_prev_period.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_enum_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_graph_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.390663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.394663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_consistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_dropped.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_lurker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_remainder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_still_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_vital.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/check_past.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/check_prev_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/compute_interaction_per_acc.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-07 04:19:54.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/generate_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:20:05.394663 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-07 04:20:05.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-07 04:20:05.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 04:20:05.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-07 04:20:05.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-07 04:20:05.000000 tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.365215 tc_core_analyzer_lib-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-18 07:53:09.365215 tc_core_analyzer_lib-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:53:09.365215 tc_core_analyzer_lib-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.353215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/assess_engagement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.357215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.357215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_all_active_fourteen_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_mention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_replies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_consistently_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_consistently_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_newly_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_vital.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_lone_actions_all_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_lone_thr_actions_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_mention_active_members_from_int_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_newly_active_continuous_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_newly_active_discontinued_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_non_consistently_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_partially_consistently_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_still_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_thr_actions_all_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_vital.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.361215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_consistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_dropped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_lurker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_disengaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_paused.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_unpaused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_still_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_vital.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_check_past.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_check_prev_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_enum_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_graph_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.361215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.365215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_consistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_dropped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_lurker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_remainder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_still_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_vital.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/check_past.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/check_prev_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/compute_interaction_per_acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-18 07:53:01.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/generate_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:53:09.365215 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-18 07:53:09.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-18 07:53:09.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:53:09.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 07:53:09.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 07:53:09.000000 tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/top_level.txt
```

### Comparing `tc-core-analyzer-lib-1.2.0/PKG-INFO` & `tc_core_analyzer_lib-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-core-analyzer-lib
-Version: 1.2.0
+Version: 1.3.0
 Summary: TogetherCrew core analyzer library.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy==1.24.1
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov==4.0.0
```

### Comparing `tc-core-analyzer-lib-1.2.0/README.md` & `tc_core_analyzer_lib-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/assess_engagement.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/assess_engagement.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_active_members.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_active_members.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_all_active_fourteen_period.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_all_active_fourteen_period.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_mention.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_mention.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_reactions.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_reactions.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_assess_replies.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_assess_replies.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_consistently_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_consistently_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_members.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_members.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_consistently_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_consistently_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_newly_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_newly_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_vital.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_disengaged_were_vital.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_lone_actions_all_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_lone_actions_all_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_lone_thr_actions_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_lone_thr_actions_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_mention_active_members_from_int_matrix.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_mention_active_members_from_int_matrix.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_newly_active_continuous_period.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_newly_active_continuous_period.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_newly_active_discontinued_period.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_newly_active_discontinued_period.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_non_consistently_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_non_consistently_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_partially_consistently_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_partially_consistently_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_still_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_still_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_thr_actions_all_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_thr_actions_all_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/integration/test_vital.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/integration/test_vital.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_consistent.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_consistent.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_dropped.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_dropped.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_lurker.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_lurker.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_overlap.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_overlap.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_disengaged.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_disengaged.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_paused.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_paused.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_returned.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_returned.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_unpaused.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_remainder_unpaused.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_still_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_still_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_assess_vital.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_assess_vital.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_check_past.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_check_past.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/tests/unit/test_check_prev_period.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/tests/unit/test_check_prev_period.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_connected.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_connected.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_consistent.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_consistent.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_dropped.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_dropped.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_lurker.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_lurker.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_overlap.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_overlap.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_remainder.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_remainder.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_still_active.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_still_active.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/assess_vital.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/assess_vital.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/check_past.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/check_past.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/assessments/check_prev_period.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/assessments/check_prev_period.py`

 * *Files identical despite different names*

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib/utils/compute_interaction_per_acc.py` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib/utils/compute_interaction_per_acc.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,41 +92,53 @@
     all_degrees = np.array([val for (_, val) in graph.degree()])
 
     # compare total unweighted node degree to interaction threshold
     thr_uw_deg = np.where(all_degrees >= UW_DEG_THR)[0]
 
     # # # THRESHOLDED CONNECTIONS # # #
 
-    # make copy of graph for thresholding
-    thresh_graph = copy.deepcopy(graph)
-
-    # remove edges below threshold from copy
-    thresh_graph.remove_edges_from(
-        [
-            (n1, n2)
-            for n1, n2, w in thresh_graph.edges(data="weight")
-            if w < EDGE_STR_THR
-        ]
-    )
-
     # preparing matrix with no `action` and just interactions
     # actions were self-intereaction and are on diagonal
     matrix_interaction = copy.deepcopy(matrix)
     matrix_interaction[np.diag_indices_from(matrix_interaction)] = 0
     graph_interaction = make_graph(matrix_interaction)
 
+    # filtering the `at least interaction count` from the graph
+    graph_interaction_thresh = remove_edges_below_threshold(
+        graph_interaction, EDGE_STR_THR
+    )
+
     # get unweighted node degree value for each node from interaction network
-    all_degrees_thresh = np.array([val for (_, val) in graph_interaction.degree()])
+    all_degrees_thresh = np.array(
+        [val for (_, val) in graph_interaction_thresh.degree()]
+    )
 
     # compare total unweighted node degree after thresholding to threshold
     thr_uw_thr_deg = np.where(all_degrees_thresh > UW_THR_DEG_THR)[0]
 
     return (thr_ind, thr_uw_deg, thr_uw_thr_deg, graph)
 
 
+def remove_edges_below_threshold(
+    graph: DiGraph, EDGE_STR_THR: int, weight_name: str = "weight"
+) -> DiGraph:
+    """
+    remove the edges that has a weight below the threshold
+    """
+    graph_copy = copy.deepcopy(graph)
+    graph_copy.remove_edges_from(
+        [
+            (n1, n2)
+            for n1, n2, w in graph_copy.edges(data=weight_name)
+            if w < EDGE_STR_THR
+        ]
+    )
+    return graph_copy
+
+
 def get_analysis_vector(
     int_mat: dict[str, np.ndarray],
     activites: list[str],
     ignore_axis_0_activities: list[str],
     ignore_axis_1_activities: list[str],
 ):
     """
```

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/PKG-INFO` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-core-analyzer-lib
-Version: 1.2.0
+Version: 1.3.0
 Summary: TogetherCrew core analyzer library.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy==1.24.1
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov==4.0.0
```

### Comparing `tc-core-analyzer-lib-1.2.0/tc_core_analyzer_lib.egg-info/SOURCES.txt` & `tc_core_analyzer_lib-1.3.0/tc_core_analyzer_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

