# Comparing `tmp/bec-server-2.4.2.tar.gz` & `tmp/bec_server-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-2.4.2.tar", last modified: Tue Apr 16 15:05:14 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bec-server-2.4.2.tar` & `bec_server-2.5.0.tar`

### file list

```diff
@@ -1,100 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.386354 bec-server-2.4.2/
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-16 15:05:14.386354 bec-server-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.381353 bec-server-2.4.2/bec_server/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.382353 bec-server-2.4.2/bec_server/bec_server_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/bec_server_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/bec_server_utils/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/bec_server_utils/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/bec_server_utils/subprocess_launch.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/bec_server_utils/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.382353 bec-server-2.4.2/bec_server/data_processing/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.382353 bec-server-2.4.2/bec_server/data_processing/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/data_processing/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/dap_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4891 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/dap_service.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/dap_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    12174 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/data_processing/lmfit1d_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.382353 bec-server-2.4.2/bec_server/device_server/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.382353 bec-server-2.4.2/bec_server/device_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/device_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/device_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.383354 bec-server-2.4.2/bec_server/device_server/devices/
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/devices/config_update_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     5026 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/devices/device_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    23444 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/devices/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)     7707 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/device_server/rpc_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.383354 bec-server-2.4.2/bec_server/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.383354 bec-server-2.4.2/bec_server/file_writer/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/file_writer/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    11717 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer/file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer/file_writer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer/merged_dicts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.383354 bec-server-2.4.2/bec_server/file_writer_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22190 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer_plugins/cSAXS.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/file_writer_plugins/default_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.384353 bec-server-2.4.2/bec_server/scan_bundler/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/bec_emitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/bluesky_emitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.384353 bec-server-2.4.2/bec_server/scan_bundler/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/scan_bundler/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/emitter.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_bundler/scan_bundler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.385354 bec-server-2.4.2/bec_server/scan_server/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.385354 bec-server-2.4.2/bec_server/scan_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/scan_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     6531 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/device_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/path_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_assembler.py
--rw-rw-rw-   0 root         (0) root         (0)     6354 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_guard.py
--rw-rw-rw-   0 root         (0) root         (0)     4114 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.385354 bec-server-2.4.2/bec_server/scan_server/scan_plugins/
--rw-rw-rw-   0 root         (0) root         (0)    21424 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13216 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     6379 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-rw-rw-   0 root         (0) root         (0)    13056 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/owis_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     9086 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_plugins/sgalil_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    34791 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     4173 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_server.py
--rw-rw-rw-   0 root         (0) root         (0)    18416 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_stubs.py
--rw-rw-rw-   0 root         (0) root         (0)    35666 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scan_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    52578 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scan_server/scans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.385354 bec-server-2.4.2/bec_server/scihub/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.385354 bec-server-2.4.2/bec_server/scihub/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec-server-2.4.2/bec_server/scihub/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/repeated_timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.386354 bec-server-2.4.2/bec_server/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scibec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8519 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scibec/config_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7549 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scibec/scibec_connector.py
--rw-rw-rw-   0 root         (0) root         (0)    10557 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.386354 bec-server-2.4.2/bec_server/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scilog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2698 2024-04-16 14:21:24.000000 bec-server-2.4.2/bec_server/scihub/scilog/scilog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:14.386354 bec-server-2.4.2/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3204 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      201 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-16 15:05:14.000000 bec-server-2.4.2/bec_server.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-16 15:05:14.387354 bec-server-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-16 15:05:11.000000 bec-server-2.4.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/README.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    23444 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/default_writer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34791 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/owis_grid.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/sgalil_grid.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_flomni_fermat_scan.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11570 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    26372 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53971 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0   108162 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scilog_connector.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 bec_server-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bec_server-2.5.0/PKG-INFO
```

### Comparing `bec-server-2.4.2/bec_server/bec_server_utils/launch.py` & `bec_server-2.5.0/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/bec_server_utils/service_handler.py` & `bec_server-2.5.0/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/bec_server_utils/subprocess_launch.py` & `bec_server-2.5.0/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/bec_server_utils/tmux_launch.py` & `bec_server-2.5.0/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/data_processing/cli/launch.py` & `bec_server-2.5.0/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/data_processing/dap_server.py` & `bec_server-2.5.0/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/data_processing/dap_service.py` & `bec_server-2.5.0/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/data_processing/dap_service_manager.py` & `bec_server-2.5.0/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/data_processing/lmfit1d_service.py` & `bec_server-2.5.0/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/cli/launch.py` & `bec_server-2.5.0/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/device_server.py` & `bec_server-2.5.0/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/devices/config_update_handler.py` & `bec_server-2.5.0/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/devices/device_serializer.py` & `bec_server-2.5.0/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/devices/devicemanager.py` & `bec_server-2.5.0/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/device_server/rpc_mixin.py` & `bec_server-2.5.0/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer/cli/launch.py` & `bec_server-2.5.0/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer/file_writer.py` & `bec_server-2.5.0/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer/file_writer_manager.py` & `bec_server-2.5.0/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer/merged_dicts.py` & `bec_server-2.5.0/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer_plugins/cSAXS.py` & `bec_server-2.5.0/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/file_writer_plugins/default_writer.py` & `bec_server-2.5.0/bec_server/file_writer_plugins/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_bundler/bec_emitter.py` & `bec_server-2.5.0/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_bundler/bluesky_emitter.py` & `bec_server-2.5.0/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_bundler/cli/launch.py` & `bec_server-2.5.0/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_bundler/emitter.py` & `bec_server-2.5.0/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_bundler/scan_bundler.py` & `bec_server-2.5.0/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/cli/launch.py` & `bec_server-2.5.0/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/device_validation.py` & `bec_server-2.5.0/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/path_optimization.py` & `bec_server-2.5.0/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_assembler.py` & `bec_server-2.5.0/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_guard.py` & `bec_server-2.5.0/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_manager.py` & `bec_server-2.5.0/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_plugins/LamNIFermatScan.py` & `bec_server-2.5.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py` & `bec_server-2.5.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec_server-2.5.0/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_plugins/owis_grid.py` & `bec_server-2.5.0/bec_server/scan_server/scan_plugins/owis_grid.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_plugins/sgalil_grid.py` & `bec_server-2.5.0/bec_server/scan_server/scan_plugins/sgalil_grid.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_queue.py` & `bec_server-2.5.0/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_server.py` & `bec_server-2.5.0/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_stubs.py` & `bec_server-2.5.0/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scan_worker.py` & `bec_server-2.5.0/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scan_server/scans.py` & `bec_server-2.5.0/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/cli/launch.py` & `bec_server-2.5.0/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/repeated_timer.py` & `bec_server-2.5.0/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/scibec/config_handler.py` & `bec_server-2.5.0/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/scibec/scibec_connector.py` & `bec_server-2.5.0/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec_server-2.5.0/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/scihub.py` & `bec_server-2.5.0/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.4.2/bec_server/scihub/scilog/scilog.py` & `bec_server-2.5.0/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

