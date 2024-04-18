# Comparing `tmp/bec_lib-2.4.2.tar.gz` & `tmp/bec_lib-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-2.4.2.tar", last modified: Tue Apr 16 15:05:13 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bec_lib-2.4.2.tar` & `bec_lib-2.5.0.tar`

### file list

```diff
@@ -1,62 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.962316 bec_lib-2.4.2/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-16 15:05:13.962316 bec_lib-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-16 14:21:24.000000 bec_lib-2.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.961316 bec_lib-2.4.2/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/alarm_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5994 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.961316 bec_lib-2.4.2/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_lib-2.4.2/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/logbook_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     7455 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/observer.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/queue_items.py
--rw-rw-rw-   0 root         (0) root         (0)    39020 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/request_items.py
--rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.962316 bec_lib-2.4.2/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_lib-2.4.2/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/tests/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    22469 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5549 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2024-04-16 14:21:24.000000 bec_lib-2.4.2/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.962316 bec_lib-2.4.2/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1470 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      245 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 15:05:13.000000 bec_lib-2.4.2/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-16 15:05:13.963316 bec_lib-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-04-16 15:05:11.000000 bec_lib-2.4.2/setup.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.5.0/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/client.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/connector.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/device.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/logger.py
+-rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    39020 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    38908 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_file_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/init_config.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/setup.cfg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/setup.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 bec_lib-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 bec_lib-2.5.0/PKG-INFO
```

### Comparing `bec_lib-2.4.2/PKG-INFO` & `bec_lib-2.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: bec_lib
-Version: 2.4.2
-Summary: BEC library
-Home-page: https://gitlab.psi.ch/bec/bec
-Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # BEC Lib
 
 bec-lib is a Python library communicating with the [Beamline and Experiment Control (BEC)](https://gitlab.psi.ch/bec/bec) server. It is primarily used to build new BEC clients such as graphical user interfaces (GUIs) or command line interfaces (CLIs).
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bec-lib.
```

### Comparing `bec_lib-2.4.2/bec_lib/__init__.py` & `bec_lib-2.5.0/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/alarm_handler.py` & `bec_lib-2.5.0/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/async_data.py` & `bec_lib-2.5.0/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/bec_service.py` & `bec_lib-2.5.0/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/bl_checks.py` & `bec_lib-2.5.0/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/bl_conditions.py` & `bec_lib-2.5.0/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/callback_handler.py` & `bec_lib-2.5.0/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/channel_monitor.py` & `bec_lib-2.5.0/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/client.py` & `bec_lib-2.5.0/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/config_helper.py` & `bec_lib-2.5.0/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/configs/demo_config.yaml` & `bec_lib-2.5.0/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/configs/openapi_schema.json` & `bec_lib-2.5.0/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/connector.py` & `bec_lib-2.5.0/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/dap_plugin_objects.py` & `bec_lib-2.5.0/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/dap_plugins.py` & `bec_lib-2.5.0/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/device.py` & `bec_lib-2.5.0/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/devicemanager.py` & `bec_lib-2.5.0/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/endpoints.py` & `bec_lib-2.5.0/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/file_utils.py` & `bec_lib-2.5.0/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/lmfit_serializer.py` & `bec_lib-2.5.0/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/logbook_connector.py` & `bec_lib-2.5.0/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/logger.py` & `bec_lib-2.5.0/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/messages.py` & `bec_lib-2.5.0/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/numpy_encoder.py` & `bec_lib-2.5.0/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/observer.py` & `bec_lib-2.5.0/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/pdf_writer.py` & `bec_lib-2.5.0/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/queue_items.py` & `bec_lib-2.5.0/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/redis_connector.py` & `bec_lib-2.5.0/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/request_items.py` & `bec_lib-2.5.0/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scan_data.py` & `bec_lib-2.5.0/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scan_items.py` & `bec_lib-2.5.0/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scan_manager.py` & `bec_lib-2.5.0/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scan_report.py` & `bec_lib-2.5.0/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scans.py` & `bec_lib-2.5.0/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/scibec_validator.py` & `bec_lib-2.5.0/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/serialization.py` & `bec_lib-2.5.0/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/service_config.py` & `bec_lib-2.5.0/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/signature_serializer.py` & `bec_lib-2.5.0/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/tests/fixtures.py` & `bec_lib-2.5.0/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/tests/test_config.yaml` & `bec_lib-2.5.0/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/tests/utils.py` & `bec_lib-2.5.0/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/user_scripts_mixin.py` & `bec_lib-2.5.0/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.2/bec_lib/utils.py` & `bec_lib-2.5.0/bec_lib/utils.py`

 * *Files identical despite different names*

