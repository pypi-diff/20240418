# Comparing `tmp/cloudpss-hydrogen-4.0.0a6.tar.gz` & `tmp/cloudpss-hydrogen-4.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpss-hydrogen-4.0.0a6.tar", last modified: Tue Apr  9 10:21:38 2024, max compression
+gzip compressed data, was "dist\cloudpss-hydrogen-4.0.0a7.tar", last modified: Thu Apr 18 08:01:51 2024, max compression
```

## Comparing `cloudpss-hydrogen-4.0.0a6.tar` & `cloudpss-hydrogen-4.0.0a7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/
--rw-rw-rw-   0        0        0     2112 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/
--rw-rw-rw-   0        0        0      777 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/function/
--rw-rw-rw-   0        0        0     1629 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/function/__init__.py
--rw-rw-rw-   0        0        0       29 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/function/function.py
--rw-rw-rw-   0        0        0    14640 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/function/functionExecution.py
--rw-rw-rw-   0        0        0    13162 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/function/job.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/
--rw-rw-rw-   0        0        0    20757 2024-04-09 10:19:52.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/DataManageModel.py
--rw-rw-rw-   0        0        0     6721 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/EvaluationModel.py
--rw-rw-rw-   0        0        0     8522 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/IESLabPlan.py
--rw-rw-rw-   0        0        0     3934 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/IESLabSimulation.py
--rw-rw-rw-   0        0        0     4790 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/PlanModel.py
--rw-rw-rw-   0        0        0      186 2023-07-10 05:15:47.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/
--rw-rw-rw-   0        0        0      151 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/
--rw-rw-rw-   0        0        0       67 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/__init__.py
--rw-rw-rw-   0        0        0      734 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/component.py
--rw-rw-rw-   0        0        0     4582 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/diagram.py
--rw-rw-rw-   0        0        0      954 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/implement.py
--rw-rw-rw-   0        0        0     3770 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/jobDefinitions.py
--rw-rw-rw-   0        0        0    26956 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/model.py
--rw-rw-rw-   0        0        0     3736 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/revision.py
--rw-rw-rw-   0        0        0     2234 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/model/topology.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/project/
--rw-rw-rw-   0        0        0       51 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/project/__init__.py
--rw-rw-rw-   0        0        0    17700 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/project/project.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/
--rw-rw-rw-   0        0        0     5841 2023-07-10 05:15:47.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabEvaluationResult.py
--rw-rw-rw-   0        0        0     6862 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabPlanResult.py
--rw-rw-rw-   0        0        0     7863 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabTypicalDayResult.py
--rw-rw-rw-   0        0        0      241 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/__init__.py
--rw-rw-rw-   0        0        0     4096 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/receiver.py
--rw-rw-rw-   0        0        0    13125 2024-04-02 02:00:51.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/result.py
--rw-rw-rw-   0        0        0     5316 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/runner.py
--rw-rw-rw-   0        0        0     4162 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/storage.py
--rw-rw-rw-   0        0        0    11613 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/runner/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/
--rw-rw-rw-   0        0        0      291 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/__init__.py
--rw-rw-rw-   0        0        0      885 2024-04-02 03:50:05.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/dataEncoder.py
--rw-rw-rw-   0        0        0      255 2024-04-02 03:50:08.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/graphqlUtil.py
--rw-rw-rw-   0        0        0     1642 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/httprequests.py
--rw-rw-rw-   0        0        0      795 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/matlab.py
--rw-rw-rw-   0        0        0     2885 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/utils/yamlLoader.py
--rw-rw-rw-   0        0        0     1498 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/verify.py
--rw-rw-rw-   0        0        0       29 2024-04-09 10:21:34.000000 cloudpss-hydrogen-4.0.0a6/cloudpss/version.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-09 10:21:37.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1785 2024-04-09 10:21:37.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:21:37.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-09 10:21:37.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 10:21:37.000000 cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/setup.cfg
--rw-rw-rw-   0        0        0      855 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:21:38.000000 cloudpss-hydrogen-4.0.0a6/test/
--rw-rw-rw-   0        0        0      523 2023-12-27 12:07:35.000000 cloudpss-hydrogen-4.0.0a6/test/test-async.py
--rw-rw-rw-   0        0        0     1719 2023-12-27 12:10:15.000000 cloudpss-hydrogen-4.0.0a6/test/test-async2.py
--rw-rw-rw-   0        0        0      846 2023-12-28 08:14:48.000000 cloudpss-hydrogen-4.0.0a6/test/test-async3.py
--rw-rw-rw-   0        0        0      519 2024-03-07 08:20:22.000000 cloudpss-hydrogen-4.0.0a6/test/test-plot.py
--rw-rw-rw-   0        0        0     1097 2023-05-30 02:30:39.000000 cloudpss-hydrogen-4.0.0a6/test/test-sdk.py
--rw-rw-rw-   0        0        0     1359 2023-12-14 10:07:50.000000 cloudpss-hydrogen-4.0.0a6/test/test-sdk1.py
--rw-rw-rw-   0        0        0     3091 2023-05-30 02:30:39.000000 cloudpss-hydrogen-4.0.0a6/test/test-snapshot.py
--rw-rw-rw-   0        0        0     1247 2024-01-17 08:11:57.000000 cloudpss-hydrogen-4.0.0a6/test/test-topology.py
--rw-rw-rw-   0        0        0      298 2024-04-08 06:48:09.000000 cloudpss-hydrogen-4.0.0a6/test/test-yield.py
--rw-rw-rw-   0        0        0     1081 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a6/test/test.py
--rw-rw-rw-   0        0        0     1142 2023-09-27 07:50:35.000000 cloudpss-hydrogen-4.0.0a6/test/test7950.py
--rw-rw-rw-   0        0        0      854 2023-09-20 03:47:30.000000 cloudpss-hydrogen-4.0.0a6/test/testAsync.py
--rw-rw-rw-   0        0        0     1569 2023-09-25 06:50:28.000000 cloudpss-hydrogen-4.0.0a6/test/testEvent.py
--rw-rw-rw-   0        0        0     4762 2024-04-08 06:31:25.000000 cloudpss-hydrogen-4.0.0a6/test/testRt-test.py
--rw-rw-rw-   0        0        0     6556 2024-04-03 07:41:30.000000 cloudpss-hydrogen-4.0.0a6/test/testRt.py
--rw-rw-rw-   0        0        0     5127 2024-02-02 10:25:09.000000 cloudpss-hydrogen-4.0.0a6/test/testRt2.py
--rw-rw-rw-   0        0        0     2030 2024-01-24 08:48:01.000000 cloudpss-hydrogen-4.0.0a6/test/testSend.py
--rw-rw-rw-   0        0        0     5350 2023-07-31 07:18:47.000000 cloudpss-hydrogen-4.0.0a6/test/test_in_new_web_1.py
--rw-rw-rw-   0        0        0     2045 2024-01-18 02:22:57.000000 cloudpss-hydrogen-4.0.0a6/test/test_ws.py
--rw-rw-rw-   0        0        0     3542 2024-01-18 04:05:57.000000 cloudpss-hydrogen-4.0.0a6/test/test_ws2.py
--rw-rw-rw-   0        0        0      302 2023-09-21 09:28:41.000000 cloudpss-hydrogen-4.0.0a6/test/testb.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/
+-rw-rw-rw-   0        0        0     2112 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/
+-rw-rw-rw-   0        0        0      777 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/function/
+-rw-rw-rw-   0        0        0     1629 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/function/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/function/function.py
+-rw-rw-rw-   0        0        0    14640 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/function/functionExecution.py
+-rw-rw-rw-   0        0        0    13162 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/function/job.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/
+-rw-rw-rw-   0        0        0    20757 2024-04-09 10:19:52.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/DataManageModel.py
+-rw-rw-rw-   0        0        0     6721 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/EvaluationModel.py
+-rw-rw-rw-   0        0        0     8522 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/IESLabPlan.py
+-rw-rw-rw-   0        0        0     3934 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/IESLabSimulation.py
+-rw-rw-rw-   0        0        0     5184 2024-04-18 07:51:12.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/PlanModel.py
+-rw-rw-rw-   0        0        0      186 2023-07-10 05:15:47.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/
+-rw-rw-rw-   0        0        0      151 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/
+-rw-rw-rw-   0        0        0       67 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/component.py
+-rw-rw-rw-   0        0        0     4582 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/diagram.py
+-rw-rw-rw-   0        0        0      954 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/implement.py
+-rw-rw-rw-   0        0        0     3770 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/jobDefinitions.py
+-rw-rw-rw-   0        0        0    26956 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/model.py
+-rw-rw-rw-   0        0        0     3736 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/revision.py
+-rw-rw-rw-   0        0        0     2234 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/model/topology.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/project/
+-rw-rw-rw-   0        0        0       51 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/project/__init__.py
+-rw-rw-rw-   0        0        0    17700 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/project/project.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/
+-rw-rw-rw-   0        0        0     5841 2023-07-10 05:15:47.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabEvaluationResult.py
+-rw-rw-rw-   0        0        0     6862 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabPlanResult.py
+-rw-rw-rw-   0        0        0     7863 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabTypicalDayResult.py
+-rw-rw-rw-   0        0        0      241 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/__init__.py
+-rw-rw-rw-   0        0        0     4096 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/receiver.py
+-rw-rw-rw-   0        0        0    13125 2024-04-02 02:00:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/result.py
+-rw-rw-rw-   0        0        0     5316 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/runner.py
+-rw-rw-rw-   0        0        0     4162 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/storage.py
+-rw-rw-rw-   0        0        0    11613 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/runner/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/
+-rw-rw-rw-   0        0        0      291 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/__init__.py
+-rw-rw-rw-   0        0        0      885 2024-04-02 03:50:05.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/dataEncoder.py
+-rw-rw-rw-   0        0        0      255 2024-04-02 03:50:08.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/graphqlUtil.py
+-rw-rw-rw-   0        0        0     1642 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/httprequests.py
+-rw-rw-rw-   0        0        0      795 2023-01-12 12:36:01.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/matlab.py
+-rw-rw-rw-   0        0        0     2885 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/utils/yamlLoader.py
+-rw-rw-rw-   0        0        0     1498 2024-04-02 10:14:57.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/verify.py
+-rw-rw-rw-   0        0        0       29 2024-04-18 07:55:55.000000 cloudpss-hydrogen-4.0.0a7/cloudpss/version.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-18 08:01:50.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1785 2024-04-18 08:01:50.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 08:01:50.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-18 08:01:50.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 08:01:50.000000 cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:01:51.000000 cloudpss-hydrogen-4.0.0a7/test/
+-rw-rw-rw-   0        0        0      523 2023-12-27 12:07:35.000000 cloudpss-hydrogen-4.0.0a7/test/test-async.py
+-rw-rw-rw-   0        0        0     1719 2023-12-27 12:10:15.000000 cloudpss-hydrogen-4.0.0a7/test/test-async2.py
+-rw-rw-rw-   0        0        0      846 2023-12-28 08:14:48.000000 cloudpss-hydrogen-4.0.0a7/test/test-async3.py
+-rw-rw-rw-   0        0        0      519 2024-03-07 08:20:22.000000 cloudpss-hydrogen-4.0.0a7/test/test-plot.py
+-rw-rw-rw-   0        0        0     1097 2023-05-30 02:30:39.000000 cloudpss-hydrogen-4.0.0a7/test/test-sdk.py
+-rw-rw-rw-   0        0        0     1359 2023-12-14 10:07:50.000000 cloudpss-hydrogen-4.0.0a7/test/test-sdk1.py
+-rw-rw-rw-   0        0        0     3091 2023-05-30 02:30:39.000000 cloudpss-hydrogen-4.0.0a7/test/test-snapshot.py
+-rw-rw-rw-   0        0        0     1247 2024-01-17 08:11:57.000000 cloudpss-hydrogen-4.0.0a7/test/test-topology.py
+-rw-rw-rw-   0        0        0      298 2024-04-08 06:48:09.000000 cloudpss-hydrogen-4.0.0a7/test/test-yield.py
+-rw-rw-rw-   0        0        0     1081 2024-04-09 10:19:46.000000 cloudpss-hydrogen-4.0.0a7/test/test.py
+-rw-rw-rw-   0        0        0     1142 2023-09-27 07:50:35.000000 cloudpss-hydrogen-4.0.0a7/test/test7950.py
+-rw-rw-rw-   0        0        0      854 2023-09-20 03:47:30.000000 cloudpss-hydrogen-4.0.0a7/test/testAsync.py
+-rw-rw-rw-   0        0        0     1569 2023-09-25 06:50:28.000000 cloudpss-hydrogen-4.0.0a7/test/testEvent.py
+-rw-rw-rw-   0        0        0     4762 2024-04-08 06:31:25.000000 cloudpss-hydrogen-4.0.0a7/test/testRt-test.py
+-rw-rw-rw-   0        0        0     6556 2024-04-03 07:41:30.000000 cloudpss-hydrogen-4.0.0a7/test/testRt.py
+-rw-rw-rw-   0        0        0     5127 2024-02-02 10:25:09.000000 cloudpss-hydrogen-4.0.0a7/test/testRt2.py
+-rw-rw-rw-   0        0        0     2030 2024-01-24 08:48:01.000000 cloudpss-hydrogen-4.0.0a7/test/testSend.py
+-rw-rw-rw-   0        0        0     5350 2023-07-31 07:18:47.000000 cloudpss-hydrogen-4.0.0a7/test/test_in_new_web_1.py
+-rw-rw-rw-   0        0        0     2045 2024-01-18 02:22:57.000000 cloudpss-hydrogen-4.0.0a7/test/test_ws.py
+-rw-rw-rw-   0        0        0     3542 2024-01-18 04:05:57.000000 cloudpss-hydrogen-4.0.0a7/test/test_ws2.py
+-rw-rw-rw-   0        0        0      302 2023-09-21 09:28:41.000000 cloudpss-hydrogen-4.0.0a7/test/testb.py
```

### Comparing `cloudpss-hydrogen-4.0.0a6/PKG-INFO` & `cloudpss-hydrogen-4.0.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss-hydrogen
-Version: 4.0.0a6
+Version: 4.0.0a7
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
```

### Comparing `cloudpss-hydrogen-4.0.0a6/README.md` & `cloudpss-hydrogen-4.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/__init__.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/function/__init__.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/function/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/function/functionExecution.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/function/functionExecution.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/function/job.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/function/job.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/DataManageModel.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/DataManageModel.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/EvaluationModel.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/EvaluationModel.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/IESLabPlan.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/IESLabPlan.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/IESLabSimulation.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/IESLabSimulation.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/ieslab/PlanModel.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/ieslab/PlanModel.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,20 +30,33 @@
         '''
             获取当前算例的优化目标设置信息
 
             :return: enum 类型，代表经济性优化和环保性优化的类型
         '''
         try:
             data = self._fetchItemData(self._baseUri)
+            print(data)
             for e in OptimizationMode:
                 if (e.value == data['data']['optimizationpara']
                     ['OptimizationMode']):
                     return e
         except:
             return OptimizationMode['经济性']
+    
+    def GetGlobalConfig(self):
+        '''
+            获取当前算例的全局参数设置
+
+            :return: int 类型，代表储能动作灵敏度设置的值，默认为0.1
+        '''
+        try:
+            data = self._fetchItemData(self._baseUri)
+            return data['data']['optimizationpara']['StoSen']
+        except:
+            return 0.1
 
     def SetOptimizationInfo(self, optType):
         '''
             无对应接口
             设置当前算例的优化目标
 
             :param optType: enum 类型，代表经济性优化和环保性优化的类型
```

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/component.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/component.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/diagram.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/diagram.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/implements/implement.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/implements/implement.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/jobDefinitions.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/jobDefinitions.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/model.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/model.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/revision.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/revision.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/model/topology.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/model/topology.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/project/project.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/project/project.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabEvaluationResult.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabEvaluationResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabPlanResult.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabPlanResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/IESLabTypicalDayResult.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/IESLabTypicalDayResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/receiver.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/receiver.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/result.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/result.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/runner.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/runner.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/storage.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/storage.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/runner/transform.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/runner/transform.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/utils/dataEncoder.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/utils/dataEncoder.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/utils/httprequests.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/utils/httprequests.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/utils/matlab.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/utils/matlab.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/utils/yamlLoader.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/utils/yamlLoader.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss/verify.py` & `cloudpss-hydrogen-4.0.0a7/cloudpss/verify.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/PKG-INFO` & `cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss-hydrogen
-Version: 4.0.0a6
+Version: 4.0.0a7
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
```

### Comparing `cloudpss-hydrogen-4.0.0a6/cloudpss_hydrogen.egg-info/SOURCES.txt` & `cloudpss-hydrogen-4.0.0a7/cloudpss_hydrogen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/setup.py` & `cloudpss-hydrogen-4.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-async.py` & `cloudpss-hydrogen-4.0.0a7/test/test-async.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-async2.py` & `cloudpss-hydrogen-4.0.0a7/test/test-async2.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-async3.py` & `cloudpss-hydrogen-4.0.0a7/test/test-async3.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-plot.py` & `cloudpss-hydrogen-4.0.0a7/test/test-plot.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-sdk.py` & `cloudpss-hydrogen-4.0.0a7/test/test-sdk.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-sdk1.py` & `cloudpss-hydrogen-4.0.0a7/test/test-sdk1.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-snapshot.py` & `cloudpss-hydrogen-4.0.0a7/test/test-snapshot.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test-topology.py` & `cloudpss-hydrogen-4.0.0a7/test/test-topology.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test.py` & `cloudpss-hydrogen-4.0.0a7/test/test.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test7950.py` & `cloudpss-hydrogen-4.0.0a7/test/test7950.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testAsync.py` & `cloudpss-hydrogen-4.0.0a7/test/testAsync.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testEvent.py` & `cloudpss-hydrogen-4.0.0a7/test/testEvent.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testRt-test.py` & `cloudpss-hydrogen-4.0.0a7/test/testRt-test.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testRt.py` & `cloudpss-hydrogen-4.0.0a7/test/testRt.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testRt2.py` & `cloudpss-hydrogen-4.0.0a7/test/testRt2.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/testSend.py` & `cloudpss-hydrogen-4.0.0a7/test/testSend.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test_in_new_web_1.py` & `cloudpss-hydrogen-4.0.0a7/test/test_in_new_web_1.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test_ws.py` & `cloudpss-hydrogen-4.0.0a7/test/test_ws.py`

 * *Files identical despite different names*

### Comparing `cloudpss-hydrogen-4.0.0a6/test/test_ws2.py` & `cloudpss-hydrogen-4.0.0a7/test/test_ws2.py`

 * *Files identical despite different names*

