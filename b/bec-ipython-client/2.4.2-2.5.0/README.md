# Comparing `tmp/bec_ipython_client-2.4.2.tar.gz` & `tmp/bec_ipython_client-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_ipython_client-2.4.2.tar", last modified: Tue Apr 16 15:05:13 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bec_ipython_client-2.4.2.tar` & `bec_ipython_client-2.5.0.tar`

### file list

```diff
@@ -1,57 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/
--rw-r--r--   0 root         (0) root         (0)      414 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.533278 bec_ipython_client-2.4.2/bec_ipython_client/
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/bec_magics.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.533278 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9941 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    11964 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4460 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5516 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54701 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4934 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.534278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    80400 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni.py
--rw-rw-rw-   0 root         (0) root         (0)     6399 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8918 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/x_ray_eye_align.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 15:05:02.000000 bec_ipython_client-2.4.2/bec_ipython_client/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7753 2024-04-16 14:21:24.000000 bec_ipython_client-2.4.2/bec_ipython_client/tests/end2end_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 15:05:13.535278 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      414 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1938 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-16 15:05:13.000000 bec_ipython_client-2.4.2/bec_ipython_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-16 15:05:13.536278 bec_ipython_client-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2254 2024-04-16 15:05:11.000000 bec_ipython_client-2.4.2/setup.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/demo.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/scan_progress.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0    49460 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/LamNI_logo.png
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/__init__.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py
+-rw-r--r--   0        0        0    54701 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/__init__.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/beamline_info.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/__init__.py
+-rw-r--r--   0        0        0    80400 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni.py
+-rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_test_config.yaml
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_scan_progress.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_x_ray_eye_align.py
+-rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/.gitignore
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/PKG-INFO
```

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/beamline_mixin.py` & `bec_ipython_client-2.5.0/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/bec_magics.py` & `bec_ipython_client-2.5.0/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/bec_startup.py` & `bec_ipython_client-2.5.0/bec_ipython_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/live_table.py` & `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/move_device.py` & `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/scan_progress.py` & `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/callbacks/utils.py` & `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/bec_hli.py` & `bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/high_level_interfaces/spec_hli.py` & `bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/main.py` & `bec_ipython_client-2.5.0/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/load_additional_correction.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/SLS/sls_info.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/beamline_info.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/plugins/flomni/x_ray_eye_align.py` & `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/prettytable.py` & `bec_ipython_client-2.5.0/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/progressbar.py` & `bec_ipython_client-2.5.0/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.4.2/bec_ipython_client/signals.py` & `bec_ipython_client-2.5.0/bec_ipython_client/signals.py`

 * *Files identical despite different names*

