# Comparing `tmp/assemblyline-core-4.5.1.dev93.tar.gz` & `tmp/assemblyline-core-4.5.1.dev94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.5.1.dev93.tar", last modified: Thu Apr 18 15:20:02 2024, max compression
+gzip compressed data, was "assemblyline-core-4.5.1.dev94.tar", last modified: Thu Apr 18 15:57:29 2024, max compression
```

## Comparing `assemblyline-core-4.5.1.dev93.tar` & `assemblyline-core-4.5.1.dev94.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.042145 assemblyline-core-4.5.1.dev93/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-18 15:20:02.042145 assemblyline-core-4.5.1.dev93/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.990144 assemblyline-core-4.5.1.dev93/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-18 15:19:58.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.994144 assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.994144 assemblyline-core-4.5.1.dev93/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9179 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/archiver/run_archiver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/badlist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.998144 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.998144 assemblyline-core-4.5.1.dev93/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.002144 assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.010144 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16277 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20026 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.010144 assemblyline-core-4.5.1.dev93/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.014144 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.014144 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.014144 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.018144 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.030145 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24747 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65957 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23635 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.030145 assemblyline-core-4.5.1.dev93/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9906 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34206 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.034144 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.038144 assemblyline-core-4.5.1.dev93/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:01.994144 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-18 15:20:01.000000 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-18 15:20:01.000000 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 15:20:01.000000 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-18 15:20:01.000000 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-18 15:20:01.000000 assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-18 15:20:02.046145 assemblyline-core-4.5.1.dev93/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:20:02.042145 assemblyline-core-4.5.1.dev93/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_badlist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_safelist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-18 15:19:45.000000 assemblyline-core-4.5.1.dev93/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-18 15:19:46.000000 assemblyline-core-4.5.1.dev93/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.503708 assemblyline-core-4.5.1.dev94/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-18 15:57:29.503708 assemblyline-core-4.5.1.dev94/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.483708 assemblyline-core-4.5.1.dev94/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-18 15:57:26.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.483708 assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.483708 assemblyline-core-4.5.1.dev94/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9179 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/archiver/run_archiver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/badlist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.487708 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.487708 assemblyline-core-4.5.1.dev94/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.487708 assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.491708 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16277 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20026 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.491708 assemblyline-core-4.5.1.dev94/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.491708 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.491708 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.491708 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.495708 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.495708 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24747 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65957 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.495708 assemblyline-core-4.5.1.dev94/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34206 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.495708 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.499708 assemblyline-core-4.5.1.dev94/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.483708 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-18 15:57:29.000000 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-18 15:57:29.000000 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 15:57:29.000000 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-18 15:57:29.000000 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-18 15:57:29.000000 assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-18 15:57:29.503708 assemblyline-core-4.5.1.dev94/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 15:57:29.499708 assemblyline-core-4.5.1.dev94/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_badlist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_safelist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-18 15:57:11.000000 assemblyline-core-4.5.1.dev94/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-18 15:57:12.000000 assemblyline-core-4.5.1.dev94/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.5.1.dev93/LICENCE.md` & `assemblyline-core-4.5.1.dev94/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/PKG-INFO` & `assemblyline-core-4.5.1.dev94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev93
+Version: 4.5.1.dev94
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev93/README.md` & `assemblyline-core-4.5.1.dev94/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/archiver/run_archiver.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/badlist_client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/es_metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/metrics/metrics_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/replay/replay.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/safelist_client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/scaler/scaler_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/server_base.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/signature_client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/submission_client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/tasking_client.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/tasking_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             # Update the datastore with the uploaded file
             self.datastore.save_or_freshen_file(file_info['sha256'], file_info, file_info['expiry_ts'],
                                                 file_info['classification'], is_section_image=is_section_image)
 
             # Upload file to the filestore (upload already checks if the file exists)
             self.filestore.upload(file_path, file_info['sha256'])
         else:
-            raise TaskingClientException(f"Uploaded file '{file_path}' does not match expected file hash. "
+            raise TaskingClientException("Uploaded file does not match expected file hash. "
                                          f"[{file_info['sha256']} != {expected_sha256}]")
 
     # Service
     @elasticapm.capture_span(span_type='tasking_client')
     def register_service(self, service_data, log_prefix=""):
         keep_alive = True
```

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/updater/helper.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/updater/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,20 +209,23 @@
 
     return image_name, tag_name, auth_config
 
 
 # Default for obtaining tags from DockerHub
 def _get_dockerhub_tags(image_name, update_channel, proxies=None):
     # Find latest tag for each types
+    rv = []
     url = f"https://{DEFAULT_DOCKER_REGISTRY}/v2/repositories/{image_name}/tags" \
-        f"?page_size=5&page=1&name={update_channel}"
+          f"?page_size=50&page=1&name={update_channel}"
+    while True:
+        resp = requests.get(url, proxies=proxies)
+        if resp.ok:
+            resp_data = resp.json()
+            rv.extend([x['name'] for x in resp_data['results']])
+            # Page until there are no results left
+            url = resp_data.get('next', None)
+            if url is None:
+                break
+        else:
+            break
 
-    # Get tag list
-    resp = requests.get(url, proxies=proxies)
-
-    # Test for valid response
-    if resp.ok:
-        # Test for positive list of tags
-        resp_data = resp.json()
-        return [x['name'] for x in resp_data['results']]
-
-    return []
+    return rv
```

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/updater/run_updater.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/vacuum/worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.5.1.dev94/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev93
+Version: 4.5.1.dev94
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev93/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.5.1.dev94/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/setup.py` & `assemblyline-core-4.5.1.dev94/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_alerter.py` & `assemblyline-core-4.5.1.dev94/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_badlist_client.py` & `assemblyline-core-4.5.1.dev94/test/test_badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_dispatcher.py` & `assemblyline-core-4.5.1.dev94/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_expiry.py` & `assemblyline-core-4.5.1.dev94/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_plumber.py` & `assemblyline-core-4.5.1.dev94/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_replay.py` & `assemblyline-core-4.5.1.dev94/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_safelist_client.py` & `assemblyline-core-4.5.1.dev94/test/test_safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_scaler.py` & `assemblyline-core-4.5.1.dev94/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_scheduler.py` & `assemblyline-core-4.5.1.dev94/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_signature_client.py` & `assemblyline-core-4.5.1.dev94/test/test_signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_simulation.py` & `assemblyline-core-4.5.1.dev94/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_vacuum.py` & `assemblyline-core-4.5.1.dev94/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_worker_ingest.py` & `assemblyline-core-4.5.1.dev94/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev93/test/test_worker_submit.py` & `assemblyline-core-4.5.1.dev94/test/test_worker_submit.py`

 * *Files identical despite different names*
