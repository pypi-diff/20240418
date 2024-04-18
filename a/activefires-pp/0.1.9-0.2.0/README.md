# Comparing `tmp/activefires-pp-0.1.9.tar.gz` & `tmp/activefires_pp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activefires-pp-0.1.9.tar", last modified: Mon Jul 17 09:46:18 2023, max compression
+gzip compressed data, was "activefires_pp-0.2.0.tar", last modified: Thu Apr 18 09:20:52 2024, max compression
```

## Comparing `activefires-pp-0.1.9.tar` & `activefires_pp-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/workflows/deploy-sdist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/activefires_pp/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/api_posting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/fire_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/geojson_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/geometries_from_shapefiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/spatiotemporal_alarm_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/activefires_pp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_api_posting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fire_detection_id_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fire_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    21920 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fires_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_geojson_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_shapefile_geometries.py
--rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/activefires_pp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_spatiotemporal_alarm_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/continuous_integration/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/auth_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fire_notifier.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fire_notifier_regional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fires_pp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/log_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/spatio_temporal_alarm_filtering.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.904070 activefires_pp-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.904070 activefires_pp-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.github/workflows/deploy-sdist.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.904070 activefires_pp-0.2.0/activefires_pp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/api_posting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/fire_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/geojson_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/geometries_from_shapefiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/sanity_check_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/spatiotemporal_alarm_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/activefires_pp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18594 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_api_posting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_fire_detection_id_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_fire_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31099 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_fires_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22380 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_geojson_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_messaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_shapefile_geometries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30802 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/activefires_pp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.904070 activefires_pp-0.2.0/activefires_pp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 09:20:52.000000 activefires_pp-0.2.0/activefires_pp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/bin/active_fires_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/bin/active_fires_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/bin/active_fires_spatiotemporal_alarm_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/continuous_integration/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/auth_tokens.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/fire_notifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/fire_notifier_regional.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/fires_pp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/log_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/examples/spatio_temporal_alarm_filtering.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 09:20:52.908070 activefires_pp-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-18 09:20:50.000000 activefires_pp-0.2.0/setup.py
```

### Comparing `activefires-pp-0.1.9/.github/PULL_REQUEST_TEMPLATE.md` & `activefires_pp-0.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/.github/workflows/ci.yaml` & `activefires_pp-0.2.0/.github/workflows/ci.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
   test:
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
       fail-fast: true
       matrix:
         os: ["ubuntu-latest", "macos-latest"]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
         experimental: [false]
         include:
-          - python-version: "3.11"
+          - python-version: "3.12"
             os: "ubuntu-latest"
             experimental: true
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
       OS: ${{ matrix.os }}
       UNSTABLE: ${{ matrix.experimental }}
```

### Comparing `activefires-pp-0.1.9/.gitignore` & `activefires_pp-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/CHANGELOG.md` & `activefires_pp-0.2.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+## Version <v0.2.0> (2024/04/18)
+
+### Pull Requests Merged
+
+#### Features added
+
+* [PR 22](https://github.com/adybbroe/activefires-pp/pull/22) - Add filter to discard spurious detections with very low FRP and high TB(I-Band 4)
+* [PR 21](https://github.com/adybbroe/activefires-pp/pull/21) - Filter incoming messages on product name
+
+In this release 2 pull requests were closed.
+
+
+## Version <v0.1.10> (2023/12/14)
+
+### Pull Requests Merged
+
+#### Bugs fixed
+
+* [PR 20](https://github.com/adybbroe/activefires-pp/pull/20) - Fixing bug updating the detection id while running more than one day
+
+#### Features added
+
+* [PR 19](https://github.com/adybbroe/activefires-pp/pull/19) - Allow specify products to notify
+* [PR 18](https://github.com/adybbroe/activefires-pp/pull/18) - Leave out ssh and hostname from the URI in the output message
+* [PR 17](https://github.com/adybbroe/activefires-pp/pull/17) - Refactor and add sweref99 output
+* [PR 15](https://github.com/adybbroe/activefires-pp/pull/15) - Add unit conversion support
+
+In this release 5 pull requests were closed.
+
+
 ## Version <v0.1.9> (2023/07/17)
 
 ## Version <v0.1.8> (2023/07/14)
 
 
 ### Pull Requests Merged
```

### Comparing `activefires-pp-0.1.9/LICENSE` & `activefires_pp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/PKG-INFO` & `activefires_pp-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: activefires-pp
-Version: 0.1.9
+Name: activefires_pp
+Version: 0.2.0
 Summary: Post-processing of and notifications on Satellite active fire detections
 Home-page: https://github.com/adybbroe/activefires-pp
 Author: Adam Dybroe
 Author-email: adam.dybroe@smhi.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `activefires-pp-0.1.9/README.md` & `activefires_pp-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/RELEASING.md` & `activefires_pp-0.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/__init__.py` & `activefires_pp-0.2.0/activefires_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/api_posting.py` & `activefires_pp-0.2.0/activefires_pp/api_posting.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/config.py` & `activefires_pp-0.2.0/activefires_pp/config.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/fire_notifications.py` & `activefires_pp-0.2.0/activefires_pp/fire_notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam Dybbroe
+# Copyright (c) 2021 - 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -16,16 +16,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Creating and sending notifications for detected forest fires.
-"""
+"""Creating and sending notifications for detected forest fires."""
 
 import socket
 from netrc import netrc
 from datetime import datetime
 import os
 import logging
 import signal
@@ -52,16 +51,18 @@
 else:
     NETRCFILE = None
 
 LOG = logging.getLogger(__name__)
 
 
 class RecipientDataStruct(object):
-    def __init__(self):
+    """A data structure to control the list of configured recipients."""
 
+    def __init__(self):
+        """Initialize the recipient data structure."""
         self.recipients_with_attachment = []
         self.recipients_without_attachment = []
         self.recipients_all = []
         self.region_name = None
         self.region_code = None
         self.subject = None
 
@@ -136,15 +137,14 @@
         self.publisher = NoisyPublisher("end_user_notifier")
         self.publisher.start()
         self.loop = True
         signal.signal(signal.SIGTERM, self.signal_shutdown)
 
     def _set_options_from_config(self, config):
         """From the configuration on disk set the option dictionary, holding all metadata for processing."""
-
         for item in config:
             self.options[item] = config[item]
 
         if isinstance(self.options.get('subscribe_topics'), str):
             subscribe_topics = self.options.get('subscribe_topics').split(',')
             for item in subscribe_topics:
                 if len(item) == 0:
@@ -180,21 +180,34 @@
                     # No fires detected - no notification to send:
                     LOG.info("Message type info: No fires detected - no notification to send.")
                     continue
                 elif msg.type not in ['file', 'collection', 'dataset']:
                     LOG.debug("Message type not supported: %s", str(msg.type))
                     continue
 
+                if not self._product_name_supported(msg):
+                    continue
+
                 output_msg = self.notify_end_users(msg)
                 if output_msg:
                     LOG.debug("Sending message: %s", str(output_msg))
                     self.publisher.send(str(output_msg))
                 else:
                     LOG.debug("No message to send")
 
+    def _product_name_supported(self, incoming_msg):
+        """Check that the product name is supported via the configuration."""
+        product_name = incoming_msg.data.get('product')
+        product_list = self.options.get('products')
+        if product_list and product_name and product_name not in product_list:
+            LOG.info('Product %s will not generate a notification!', product_name)
+            return False
+
+        return True
+
     def notify_end_users(self, msg):
         """Send notifications to configured end users (mail and text messages)."""
         LOG.debug("Start sending notifications to configured end users.")
 
         filename = get_filename_from_posttroll_message(msg)
         ffdata = read_geojson_data(filename)
         if not ffdata:
@@ -214,15 +227,14 @@
         self._send_notifications_without_attachments(server, self.recipients, sub_messages, platform_name)
         self._send_notifications_with_attachments(server, self.recipients, full_message, filename, platform_name)
 
         return _create_output_message(msg, self.output_topic, self.recipients.recipients_all)
 
     def _send_notifications_with_attachments(self, server, recipients, full_message, filename, platform_name):
         """Send notifications with attachments."""
-
         notification = MIMEMultipart()
         notification['From'] = self.sender
         if platform_name:
             notification['Subject'] = recipients.subject + ' Satellit = %s' % platform_name
         else:
             notification['Subject'] = recipients.subject
 
@@ -248,15 +260,14 @@
             server.sendmail(self.sender, recip, txt)
             LOG.debug("Text sent: %s", txt)
 
         server.quit()
 
     def _send_notifications_without_attachments(self, server, recipients, sub_messages, platform_name):
         """Send notifications without attachments."""
-
         for submsg in sub_messages:
             notification = MIMEMultipart()
             notification['From'] = self.sender
             if platform_name:
                 notification['Subject'] = recipients.subject + ' Satellit = %s' % platform_name
             else:
                 notification['Subject'] = recipients.subject
```

### Comparing `activefires-pp-0.1.9/activefires_pp/geojson_utils.py` & `activefires_pp-0.2.0/activefires_pp/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2022 Adam Dybbroe
+# Copyright (c) 2021-2023 Adam Dybbroe
 
 # Author(s):
 
-#   Adam Dybbroe <Firstname.Lastname@smhi.se>
+#   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Geojson utilities."""
+"""Utility functions for the Active Fires postprocessing."""
 
-import geojson
-import json
+import cartopy.io.shapereader as shpreader
+from datetime import date, datetime, timezone
+from urllib.parse import urlparse
+import pathlib
 import logging
-from trollsift import Parser, globify
-import pytz
-from datetime import datetime
-import numpy as np
+import zoneinfo
+from pint import UnitRegistry
 
 LOG = logging.getLogger(__name__)
 
 
-def read_geojson_data(filename):
-    """Read Geo json data from file."""
-    if str(filename).endswith('.geojson') and filename.exists():
-        # Read the file:
-        try:
-            with open(filename, "r") as fpt:
-                return geojson.load(fpt)
-        except json.decoder.JSONDecodeError:
-            LOG.exception("Geojson file invalid and cannot be read: %s", str(filename))
-    else:
-        LOG.error("No valid filename to read: %s", str(filename))
-
-
-def get_geojson_files_in_observation_time_order(path, pattern, time_interval):
-    """Get all geojson files with filtered active fire detections (=triggered alarms) since *dtime*."""
-    dtime_start = time_interval[0]
-    dtime_end = time_interval[1]
-    if not dtime_end:
-        dtime_end = datetime.utcnow()
-
-    p__ = Parser(pattern)
-    files = path.glob(globify(pattern))
-    dtimes = []
-    fnames = []
-    for gjson_file in files:
-        fname = gjson_file.name
-        res = p__.parse(fname)
-        if res['start_time'] > dtime_start and res['start_time'] < dtime_end:
-            dtimes.append(res['start_time'])
-            fnames.append(fname)
-
-    dtimes = np.array(dtimes)
-    fnames = np.array(fnames)
-
-    idx = dtimes.argsort()
-    files = np.take(fnames, idx)
-    return files.tolist()
-
-
-def store_geojson_alarm(fires_alarms_dir, file_parser, idx, alarm):
-    """Store the fire alarm to a geojson file."""
-    utc = pytz.timezone('utc')
-    start_time = datetime.fromisoformat(alarm["features"]["properties"]["observation_time"])
-    platform_name = alarm["features"]["properties"]["platform_name"]
-    start_time = start_time.astimezone(utc).replace(tzinfo=None)
-    fname = file_parser.compose({'start_time': start_time, 'id': idx,
-                                 'platform_name': platform_name})
-    output_filename = fires_alarms_dir / fname
-    with open(output_filename, 'w') as fpt:
-        geojson.dump(alarm, fpt)
+def datetime_utc2local(utc_dtime, tzone_str, is_dst=True):
+    """Convert a UTC datetime to local time, using DST on default."""
+    tzone = zoneinfo.ZoneInfo(tzone_str)
+    utc_dtime = utc_dtime.replace(tzinfo=timezone.utc)
+    return utc_dtime.astimezone(tzone)
 
-    return output_filename
+
+def get_local_timezone_offset(timezone_str):
+    """Get the local time zone offset as a timedelta object."""
+    utcnow = datetime.utcnow()
+    utcnow = utcnow.replace(tzinfo=timezone.utc)
+    tzone = zoneinfo.ZoneInfo(timezone_str)
+    return utcnow.astimezone(tzone).replace(tzinfo=timezone.utc) - utcnow
+
+
+def get_geometry_from_shapefile(shapefile):
+    """Read shapefile and return geometry as a multipolygon."""
+    records = shpreader.Reader(shapefile).records()
+    geometries = [c.geometry for c in records]
+
+    return geometries
+
+
+def json_serial(obj):
+    """JSON serializer for objects not serializable by default json code."""
+    if isinstance(obj, (datetime, date)):
+        return obj.isoformat()
+    raise TypeError("Type %s not serializable" % type(obj))
+
+
+def get_filename_from_posttroll_message(pytroll_message):
+    """Get the filename from the Posttroll message."""
+    url = urlparse(pytroll_message.data.get('uri'))
+    filepath = pathlib.Path(url.path)
+    LOG.info('File path: %s', str(filepath))
+    return filepath
+
+
+class UnitConverter:
+    """A converter for physical units using Pint."""
+
+    def __init__(self, units):
+        """Initialize the unit converter."""
+        self.units = units
+        self.ureg = UnitRegistry()
+
+        self.orig_units = {'power': self.ureg.watt * 1e6,
+                           'temperature': self.ureg.kelvin}
+
+    def convert(self, varname, variable):
+        """Convert a unit."""
+        variable = variable * self.orig_units[varname]
+        variable.ito(self.units[varname])
+        return variable
```

### Comparing `activefires-pp-0.1.9/activefires_pp/geometries_from_shapefiles.py` & `activefires_pp-0.2.0/activefires_pp/geometries_from_shapefiles.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/logger.py` & `activefires_pp-0.2.0/activefires_pp/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021 Adam.Dybbroe
+# Copyright (c) 2021, 2023 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam.Dybbroe <a000680@c21856.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -16,16 +16,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""The log handling.
-"""
+"""The log handling."""
 
 import logging
 import logging.config
 import logging.handlers
 import yaml
 
 LOG_FORMAT = "[%(asctime)s %(levelname)-8s] %(message)s"
```

### Comparing `activefires-pp-0.1.9/activefires_pp/post_processing.py` & `activefires_pp-0.2.0/activefires_pp/post_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021 - 2023 Adam.Dybbro
+# Copyright (c) 2021 - 2024 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -26,32 +26,37 @@
 from trollsift import Parser, globify
 import time
 import pandas as pd
 from datetime import datetime, timedelta
 import numpy as np
 import os
 from six.moves.urllib.parse import urlparse
-from geojson import Feature, Point, FeatureCollection, dump
+
 import logging
 import signal
 from queue import Empty
 from threading import Thread
 from posttroll.listener import ListenerContainer
 from posttroll.message import Message
 from posttroll.publisher import NoisyPublisher
 import pyproj
 from matplotlib.path import Path
 import shapely
 
 from activefires_pp.utils import datetime_utc2local
+from activefires_pp.utils import UnitConverter
 from activefires_pp.utils import get_local_timezone_offset
-from activefires_pp.utils import json_serial
 from activefires_pp.config import read_config
 from activefires_pp.geometries_from_shapefiles import ShapeGeometry
 
+from activefires_pp.geojson_utils import store_geojson
+from activefires_pp.geojson_utils import geojson_feature_collection_from_detections
+from activefires_pp.geojson_utils import map_coordinates_in_feature_collection
+from activefires_pp.sanity_check_detections import remove_spurious_detections
+
 # M-band output:
 # column 1: latitude of fire pixel (degrees)
 # column 2: longitude of fire pixel (degrees)
 # column 3: M13 brightness temperature of fire pixel (K)
 # column 4: Along-scan fire pixel resolution (km)
 # column 5: Along-track fire pixel resolution (km)
 # column 6: detection confidence (%)
@@ -83,42 +88,42 @@
     Filtering for static and false alarms, and/or simply on geographical regions.
     Data is stored in geojson format.
     """
 
     def __init__(self, filepath=None, afdata=None, platform_name=None, timezone='GMT'):
         """Initialize the ActiveFiresShapefileFiltering class."""
         self.input_filepath = filepath
-        self._afdata = afdata
+        self.afdata = afdata
         if afdata is None:
             self.metadata = {}
         else:
             self.metadata = afdata.attrs
 
         self.timezone = timezone
         self.platform_name = platform_name
 
     def get_af_data(self, filepattern=None, localtime=True):
         """Read the Active Fire results from file - ascii formatted output from CSPP VIIRS-AF."""
-        if self._afdata is not None:
+        if self.afdata is not None:
             # Make sure the attrs are populated with metadata instance attribute
-            self._afdata.attrs.update(self.metadata)
-            return self._afdata
+            self.afdata.attrs.update(self.metadata)
+            return self.afdata
 
         if not self.input_filepath or not os.path.exists(self.input_filepath):
             # FIXME! Better to raise an exception!?
-            return self._afdata
+            return self.afdata
 
         if not filepattern:
             raise AttributeError("file pattern must be provided in order to be able to read from file!")
 
         self.metadata = self._get_metadata_from_filename(filepattern)
-        self._afdata = _read_data(self.input_filepath)
+        self.afdata = _read_data(self.input_filepath)
         self._add_start_and_end_time_to_active_fires_data(localtime)
 
-        return self._afdata
+        return self.afdata
 
     def _get_metadata_from_filename(self, infile_pattern):
         """From the filename retrieve the metadata such as satellite and sensing time."""
         return get_metadata_from_filename(infile_pattern, self.input_filepath)
 
     def _add_start_and_end_time_to_active_fires_data(self, localtime):
         """Add start and end time to active fires data."""
@@ -129,52 +134,52 @@
         else:
             starttime = datetime_utc2local(self.metadata['start_time'], 'GMT')
             endtime = datetime_utc2local(self.metadata['end_time'], 'GMT')
 
         starttime = starttime.replace(tzinfo=None)
         endtime = endtime.replace(tzinfo=None)
 
-        self._afdata['starttime'] = np.repeat(starttime, len(self._afdata)).astype(np.datetime64)
-        self._afdata['endtime'] = np.repeat(endtime, len(self._afdata)).astype(np.datetime64)
+        self.afdata['starttime'] = np.repeat(starttime, len(self.afdata)).astype(np.datetime64)
+        self.afdata['endtime'] = np.repeat(endtime, len(self.afdata)).astype(np.datetime64)
 
         logger.info('Start and end times: %s %s',
-                    str(self._afdata['starttime'][0]),
-                    str(self._afdata['endtime'][0]))
+                    str(self.afdata['starttime'][0]),
+                    str(self.afdata['endtime'][0]))
 
     def _apply_timezone_offset(self, obstime):
         """Apply the time zone offset to the datetime objects."""
         obstime_offset = get_local_timezone_offset(self.timezone)
         return np.repeat(obstime.replace(tzinfo=None) + obstime_offset,
-                         len(self._afdata)).astype(np.datetime64)
+                         len(self.afdata)).astype(np.datetime64)
 
-    def fires_filtering(self, shapefile, start_geometries_index=1, inside=True):
+    def fires_shapefile_filtering(self, shapefile, start_geometries_index=1, inside=True):
         """Remove fires outside National borders or filter out potential false detections.
 
         If *inside* is True the filtering will keep those detections that are inside the polygon.
         If *inside* is False the filtering will disregard the detections that are inside the polygon.
         """
-        detections = self._afdata
+        detections = self.afdata
 
         lons = detections.longitude.values
         lats = detections.latitude.values
 
         toc = time.time()
         points_inside = get_global_mask_from_shapefile(shapefile, (lons, lats), start_geometries_index)
         logger.debug("Time used checking inside polygon - mpl path method: %f", time.time() - toc)
 
-        self._afdata = detections[points_inside == inside]
+        self.afdata = detections[points_inside == inside]
 
-        if len(self._afdata) == 0:
+        if len(self.afdata) == 0:
             logger.debug("No fires after filtering on Polygon...")
         else:
-            logger.debug("Number of detections after filtering on Polygon: %d", len(self._afdata))
+            logger.debug("Number of detections after filtering on Polygon: %d", len(self.afdata))
 
     def get_regional_filtermasks(self, shapefile, globstr):
         """Get the regional filter masks from the shapefile."""
-        detections = self._afdata
+        detections = self.afdata
 
         lons = detections.longitude.values
         lats = detections.latitude.values
 
         logger.debug("Before ShapeGeometry instance - shapefile name = %s" % str(shapefile))
         logger.debug("Shape file glob-string = %s" % str(globstr))
         shape_geom = ShapeGeometry(shapefile, globstr)
@@ -249,58 +254,14 @@
         detections.to_csv(output_filename, index=False)
         return output_filename
     else:
         logger.debug("No detections to save!")
         return None
 
 
-def geojson_feature_collection_from_detections(detections, platform_name=None):
-    """Create the Geojson feature collection from fire detection data."""
-    if len(detections) == 0:
-        logger.debug("No detections to save!")
-        return None
-
-    # Convert points to GeoJSON
-    features = []
-    for idx in range(len(detections)):
-        starttime = detections.iloc[idx].starttime
-        endtime = detections.iloc[idx].endtime
-        mean_granule_time = starttime.to_pydatetime() + (endtime.to_pydatetime() -
-                                                         starttime.to_pydatetime()) / 2.
-
-        prop = {'power': detections.iloc[idx].power,
-                'tb': detections.iloc[idx].tb,
-                'confidence': int(detections.iloc[idx].conf),
-                'id': detections.iloc[idx].detection_id,
-                'observation_time': json_serial(mean_granule_time)
-                }
-        if platform_name:
-            prop['platform_name'] = platform_name
-        else:
-            logger.debug("No platform name specified for output")
-
-        feat = Feature(
-            geometry=Point(map(float, [detections.iloc[idx].longitude, detections.iloc[idx].latitude])),
-            properties=prop)
-        features.append(feat)
-
-    return FeatureCollection(features)
-
-
-def store_geojson(output_filename, feature_collection):
-    """Store the Geojson feature collection of fire detections on disk."""
-    path = os.path.dirname(output_filename)
-    if not os.path.exists(path):
-        logger.info("Create directory: %s", path)
-        os.makedirs(path)
-
-    with open(output_filename, 'w') as fpt:
-        dump(feature_collection, fpt)
-
-
 def get_mask_from_multipolygon(points, geometry, start_idx=1):
     """Get mask for points from a shapely Multipolygon."""
     shape = geometry.geoms[0]
     pth = Path(shape.exterior.coords)
     mask = pth.contains_points(points)
 
     if sum(mask) == len(points):
@@ -352,17 +313,20 @@
 
         self.host = socket.gethostname()
         self.timezone = self.options.get('timezone', 'GMT')
 
         self.input_topic = self.options['subscribe_topics'][0]
         self.output_topic = self.options['publish_topic']
         self.infile_pattern = self.options.get('af_pattern_ibands')
-        self.outfile_pattern_national = self.options.get('geojson_file_pattern_national')
-        self.outfile_pattern_regional = self.options.get('geojson_file_pattern_regional')
+
+        self.outfile_patterns_national = config.get('output').get('national')
+        self.outfile_patterns_regional = config.get('output').get('regional')
+
         self.output_dir = self.options.get('output_dir', '/tmp')
+
         self.filepath_detection_id_cache = self.options.get('filepath_detection_id_cache')
 
         frmt = self.options['regional_shapefiles_format']
         self.regional_shapefiles_globstr = globify(frmt)
 
         self._fire_detection_id = None
         self._initialize_fire_detection_id()
@@ -374,14 +338,19 @@
 
     def _setup_and_start_communication(self):
         """Set up the Posttroll communication and start the publisher."""
         logger.debug("Starting up... Input topic: %s", self.input_topic)
         now = datetime_utc2local(datetime.now(), self.timezone)
         logger.debug("Output times for timezone: {zone} Now = {time}".format(zone=str(self.timezone), time=now))
 
+        tic = time.time()
+        units = {'temperature': 'degC'}
+        self.unit_converter = UnitConverter(units)
+        logger.debug("Unit conversion initialization with Pint took %f seconds.", time.time() - tic)
+
         self._check_borders_shapes_exists()
 
         self.listener = ListenerContainer(topics=[self.input_topic])
         self.publisher = NoisyPublisher("active_fires_postprocessing")
         self.publisher.start()
         self.loop = True
         signal.signal(signal.SIGTERM, self.signal_shutdown)
@@ -427,14 +396,42 @@
             for output_msg in output_messages:
                 logger.debug("Sending message: %s", str(output_msg))
                 self.publisher.send(str(output_msg))
             return None
 
         return filename
 
+    def get_output_filepath_from_projname(self, projname, metadata):
+        """From the projection-name (given in the config file) retrieve the output file path."""
+        try:
+            pout = Parser(self.outfile_patterns_national[projname]['geojson_file_pattern'])
+        except KeyError:
+            raise KeyError('Projection name %s not supported in configuration!' % projname)
+
+        return os.path.join(self.output_dir, pout.compose(metadata))
+
+    def _national_save_and_publish(self, feature_collection, ndata, af_shapeff, msg, projname='default'):
+        """Take the fearure collection and store the results in a Geojson file and publish."""
+        if feature_collection is None:
+            logger.info("No geojson file created, number of fires after filtering = %d", ndata)
+            output_messages = self._generate_no_fires_messages(msg,
+                                                               'No true fire detections inside National borders')  # noqa
+            return
+
+        out_filepath = self.get_output_filepath_from_projname(projname, af_shapeff.metadata)
+        logger.debug("Output file path = %s", out_filepath)
+
+        store_geojson(out_filepath, feature_collection)
+        output_messages = self.get_output_messages(out_filepath, msg, ndata, proj_name=projname)
+
+        for output_msg in output_messages:
+            if output_msg:
+                logger.debug("Sending message: %s", str(output_msg))
+                self.publisher.send(str(output_msg))
+
     def do_postprocessing_on_message(self, msg, filename):
         """Do the fires post processing on a message."""
         platform_name = msg.data.get('platform_name')
         af_shapeff = ActiveFiresShapefileFiltering(filename, platform_name=platform_name,
                                                    timezone=self.timezone)
         afdata = af_shapeff.get_af_data(self.infile_pattern)
         if len(afdata) == 0:
@@ -446,40 +443,31 @@
 
         afdata = self.fires_filtering(msg, af_shapeff)
         logger.debug("After fires_filtering...: Number of fire detections = %d", len(afdata))
         if len(afdata) == 0:
             logger.debug("No fires - so no regional filtering to be done!")
             return
 
-        # It is here that we should add a uniue day-ID to each of the detections!
         afdata = self.add_unique_day_id(afdata)
         self.save_id_to_file()
+        afdata = self.add_tb_celcius(afdata)
 
         # 1) Create geojson feature collection
         # 2) Dump geojson data to disk
+
         feature_collection = geojson_feature_collection_from_detections(afdata,
                                                                         platform_name=af_shapeff.platform_name)
 
-        fmda = af_shapeff.metadata
-        pout = Parser(self.outfile_pattern_national)
-        out_filepath = os.path.join(self.output_dir, pout.compose(fmda))
-        logger.debug("Output file path = %s", out_filepath)
-
-        if feature_collection is None:
-            logger.info("No geojson file created, number of fires after filtering = %d", len(afdata))
-            output_messages = self._generate_no_fires_messages(msg,
-                                                               'No true fire detections inside National borders')  # noqa
-        else:
-            store_geojson(out_filepath, feature_collection)
-            output_messages = self.get_output_messages(out_filepath, msg, len(afdata))
-
-        for output_msg in output_messages:
-            if output_msg:
-                logger.debug("Sending message: %s", str(output_msg))
-                self.publisher.send(str(output_msg))
+        for proj_name in self.outfile_patterns_national:
+            if proj_name == "default":
+                self._national_save_and_publish(feature_collection, len(afdata), af_shapeff, msg)
+            else:
+                epsg_str = self.outfile_patterns_national[proj_name].get('projection')
+                other_fc = map_coordinates_in_feature_collection(feature_collection, epsg_str)
+                self._national_save_and_publish(other_fc, len(afdata), af_shapeff, msg, proj_name)
 
         # Do the regional filtering now:
         if not self.regional_filtermask:
             logger.info("No regional filtering is attempted.")
             return
 
         # FIXME! If afdata is empty (len=0) then it seems all data are inside all regions!
@@ -512,40 +500,41 @@
         logger.debug("Perform regional masking on VIIRS AF detections and publish accordingly.")
 
         afdata = afsff_obj.get_af_data()
         fmda = afsff_obj.metadata
 
         fmda['platform'] = afsff_obj.platform_name
 
-        pout = Parser(self.outfile_pattern_regional)
+        pout = Parser(self.outfile_patterns_regional['default']['geojson_file_pattern'])
 
         output_messages = []
         regions_with_detections = 0
         for region_name in regional_fmask:
             if not regional_fmask[region_name]['some_inside_test_area']:
                 continue
 
             regions_with_detections = regions_with_detections + 1
             fmda['region_name'] = regional_fmask[region_name]['attributes']['Kod_omr']
 
             out_filepath = os.path.join(self.output_dir, pout.compose(fmda))
             logger.debug("Output file path = %s", out_filepath)
             data_in_region = afdata[regional_fmask[region_name]['mask']]
 
-            # filepath = store_geojson(out_filepath, data_in_region, platform_name=fmda['platform'])
-            feature_collection = geojson_feature_collection_from_detections(data_in_region,
-                                                                            platform_name=fmda['platform'])
-            if feature_collection is None:
+            try:
+                feature_collection = geojson_feature_collection_from_detections(data_in_region,
+                                                                                platform_name=fmda['platform'])
+            except ValueError:
                 logger.warning("Something wrong happended storing regional " +
                                "data to Geojson - area: {name}".format(name=str(region_name)))
                 continue
 
             store_geojson(out_filepath, feature_collection)
 
-            outmsg = self._generate_output_message(out_filepath, msg, regional_fmask[region_name])
+            outmsg = self._generate_output_message(out_filepath, msg, 'default',
+                                                   regional_fmask[region_name])
             output_messages.append(outmsg)
             logger.info("Geojson file created! Number of fires in region = %d", len(data_in_region))
 
         logger.debug("Regional masking done. Number of regions with fire " +
                      "detections on this granule: %s" % str(regions_with_detections))
         return output_messages
 
@@ -557,46 +546,54 @@
 
         """
         logger.debug("Read VIIRS AF detections and perform quality control and spatial filtering")
 
         fmda = af_shapeff.metadata
         # metdata contains time and everything but it is not being transfered to the dataframe.attrs
 
-        pout = Parser(self.outfile_pattern_national)
+        pout = Parser(self.outfile_patterns_national['default']['geojson_file_pattern'])
         out_filepath = os.path.join(self.output_dir, pout.compose(fmda))
         logger.debug("Output file path = %s", out_filepath)
 
         # National filtering:
-        af_shapeff.fires_filtering(self.shp_borders)
+        af_shapeff.fires_shapefile_filtering(self.shp_borders)
 
         # Metadata should be transfered here!
         afdata_ff = af_shapeff.get_af_data()
 
+        # Remove spurious detections if any:
+        afdata_ff = remove_spurious_detections(afdata_ff)
+        af_shapeff.afdata = afdata_ff
+
         if len(afdata_ff) > 0:
             logger.debug("Doing the fires filtering: shapefile-mask = %s", str(self.shp_filtermask))
-            af_shapeff.fires_filtering(self.shp_filtermask, start_geometries_index=0, inside=False)
+            af_shapeff.fires_shapefile_filtering(self.shp_filtermask, start_geometries_index=0, inside=False)
             afdata_ff = af_shapeff.get_af_data()
-            logger.debug("After fires_filtering: Number of fire detections left: %d", len(afdata_ff))
+            logger.debug("After fires_shapefile_filtering: Number of fire detections left: %d", len(afdata_ff))
 
         return afdata_ff
 
-    def get_output_messages(self, filepath, msg, number_of_data):
+    def get_output_messages(self, filepath, msg, number_of_data, proj_name='default'):
         """Generate the adequate output message(s) depending on if an output file was created or not."""
         logger.info("Geojson file created! Number of fires = %d", number_of_data)
-        return [self._generate_output_message(filepath, msg)]
+        return [self._generate_output_message(filepath, msg, proj_name)]
 
-    def _generate_output_message(self, filepath, input_msg, region=None):
+    def _generate_output_message(self, filepath, input_msg, proj_name, region=None):
         """Create the output message to publish."""
         output_topic = generate_posttroll_topic(self.output_topic, region)
         to_send = prepare_posttroll_message(input_msg, region)
-        to_send['uri'] = ('ssh://%s/%s' % (self.host, filepath))
+        to_send['uri'] = str(filepath)
         to_send['uid'] = os.path.basename(filepath)
         to_send['type'] = 'GEOJSON-filtered'
         to_send['format'] = 'geojson'
-        to_send['product'] = 'afimg'
+        if proj_name == 'default':
+            to_send['product'] = 'afimg'
+        else:
+            to_send['product'] = 'afimg_{proj_name}'.format(proj_name=proj_name)
+
         pubmsg = Message(output_topic, 'file', to_send)
         return pubmsg
 
     def _generate_no_fires_messages(self, input_msg, msg_string):
         """Create the output messages to publish."""
         to_send = prepare_posttroll_message(input_msg)
         to_send['info'] = msg_string
@@ -618,19 +615,16 @@
             self._fire_detection_id = self.get_id_from_file()
         else:
             self._fire_detection_id = {'date': datetime.utcnow(), 'counter': 0}
 
     def update_fire_detection_id(self):
         """Update the fire detection ID registry."""
         now = datetime.utcnow()
-        tdelta = now - self._fire_detection_id['date']
-        if tdelta.total_seconds() > 24*3600:
-            self._initialize_fire_detection_id()
-        elif tdelta.total_seconds() > 0 and self._fire_detection_id['date'].day != now.day:
-            self._initialize_fire_detection_id()
+        if self._fire_detection_id['date'].date() < now.date():
+            self._fire_detection_id = {'date': datetime.utcnow(), 'counter': 0}
 
         self._fire_detection_id['counter'] = self._fire_detection_id['counter'] + 1
 
     def save_id_to_file(self):
         """Save the (current) detection id on disk.
 
         It is assumed that the user permissions are so that a file can actually
@@ -654,25 +648,36 @@
                 'counter': int(counter)}
 
     def _create_id_string(self):
         """From the internal fire detection id create the id string to be exposed to the user."""
         return (self._fire_detection_id['date'].strftime('%Y%m%d') +
                 '-' + str(self._fire_detection_id['counter']))
 
-    def add_unique_day_id(self, afdata):
+    def add_unique_day_id(self, data_frame):
         """Add a unique detection id - date + a running number for the day."""
         # Add id's to the detections:
         id_list = []
-        for _i in range(len(afdata)):
+        for _i in range(len(data_frame)):
             self.update_fire_detection_id()
             id_ = self._create_id_string()
             id_list.append(id_)
 
-        afdata['detection_id'] = id_list
-        return afdata
+        col = len(data_frame.columns)
+        data_frame.insert(col, 'detection_id', id_list)
+        return data_frame
+
+    def add_tb_celcius(self, data_frame):
+        """Add a column with TB in Celcius to the fire detection data frame."""
+        def kelvin2celcius(x):
+            tb_c = self.unit_converter.convert('temperature', x)
+            return tb_c.magnitude
+
+        col = data_frame.columns.get_loc('tb')
+        data_frame.insert(2, "tb_celcius", data_frame.iloc[:, col].apply(kelvin2celcius))
+        return data_frame
 
     def close(self):
         """Shutdown the Active Fires postprocessing."""
         logger.info('Terminating Active Fires post processing.')
         self.loop = False
         logger.info('Dumping the latest detection id to disk: %s', str(self.filepath_detection_id_cache))
         self.save_id_to_file()
```

### Comparing `activefires-pp-0.1.9/activefires_pp/spatiotemporal_alarm_filtering.py` & `activefires_pp-0.2.0/activefires_pp/spatiotemporal_alarm_filtering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2022 Adam Dybbroe
+# Copyright (c) 2022, 2023, 2024 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -47,15 +47,15 @@
 from posttroll.message import Message
 from posttroll.publisher import NoisyPublisher
 
 import pytz
 from datetime import datetime, timedelta
 
 from geopy import distance
-from geojson import FeatureCollection, dump
+from geojson import FeatureCollection
 from itertools import combinations
 from pathlib import Path
 
 from activefires_pp.utils import get_filename_from_posttroll_message
 from activefires_pp.config import read_config
 from activefires_pp.config import get_xauthentication_token
 
@@ -117,15 +117,15 @@
     def _check_and_set_thresholds_from_config(self, config):
         """Check that adequate thresholds are provided in config file."""
         if 'time_and_space_thresholds' not in config:
             raise OSError('Missing time and space thresholds from configuration!')
 
         self._log_message_per_threshold = {
             'hour_threshold': ("Threshold defining when a new detection should trigger an " +
-                               "alarm on the same spot (in hours): ",
+                               "alarm on the same spot (in hours): %3.1f",
                                "Threshold in time is missing!"),
             'long_fires_threshold_km': ("Threshold defining the maximum extention of a fire before " +
                                         "dividing it in smaller pieces (in km): %3.1f",
                                         "Threshold for splitting long fires is missing!"),
             "spatial_threshold_km": ("Threshold defining the maximum distance between two detections " +
                                      "beyond which they must trigger more than one alarm (km): %3.1f",
                                      "A spatial threshold is missing!")
@@ -162,28 +162,32 @@
 
     def signal_shutdown(self, *args, **kwargs):
         """Shutdown the Notifier process."""
         self.close()
 
     def run(self):
         """Run the spatiotemporal alarm filtering."""
+        product_list = self.options.get('products')
         while self.loop:
             try:
                 msg = self.listener.output_queue.get(timeout=1)
                 LOG.debug("Message: %s", str(msg.data))
             except Empty:
                 continue
             else:
                 if msg.type in ['info', ]:
                     # No fires detected - no notification to send:
                     LOG.info("Message type info: No fires detected - no alarm to generate.")
                     continue
                 elif msg.type not in ['file', 'collection', 'dataset']:
                     LOG.debug("Message type not supported: %s", str(msg.type))
                     continue
+                elif product_list and msg.data.get('product', 'unknown') not in product_list:
+                    LOG.debug("Product %s not supported/requested. Ignore.", str(msg.data.get('product')))
+                    continue
 
                 generated_alarms = self.spatio_temporal_alarm_filtering(msg)
                 if generated_alarms:
                     LOG.debug("Number of generated alarms: %d", len(generated_alarms))
                 else:
                     LOG.debug("No alarms generated!")
 
@@ -252,24 +256,14 @@
     xauth_filepath = os.environ.get('FIREALARMS_XAUTH_FILEPATH')
     if xauth_filepath is None:
         raise OSError("Environment variable FIREALARMS_XAUTH_FILEPATH not set!")
 
     return xauth_filepath
 
 
-def dump_collection(idx, features):
-    """Dump the list of features as a Geojson Feature Collection."""
-    tmpdir = Path(DIR_SPATIAL_FILTER)
-    fname = 'sos_alarm_{index}.geojson'.format(index=idx)
-    output_filename = tmpdir / fname
-    feature_collection = FeatureCollection(features)
-    with open(output_filename, 'w') as fpt:
-        dump(feature_collection, fpt)
-
-
 def create_alarms_from_fire_detections(fire_data, past_detections_dir, sos_alarms_file_pattern,
                                        time_space_thresholds):
     """Create alarm(s) from a set of detections."""
     long_fires_threshold = time_space_thresholds.get('long_fires_threshold_km', 1.2)
     gathered_fires = join_fire_detections(fire_data)
 
     # Now go through the gathered fires and split long/large clusters of
@@ -483,27 +477,32 @@
             break
 
     return shall_trigger_alarm
 
 
 def distance_and_time_from_geojson_position(position, filepath):
     """Read the geojson data and get the observation time and the distance to a position given as input."""
-    lon0, lat0 = position
     gjdata = read_geojson_data(filepath)
-    lon, lat = gjdata["geometry"]["coordinates"]
     # Get distance to this fire point:
-    dist = distance.distance((lat0, lon0), (lat, lon)).kilometers
+    dist = get_distance_between_two_points(position, gjdata["geometry"]["coordinates"])
 
     obstime = datetime.fromisoformat(gjdata["properties"]["observation_time"])
     utc = pytz.timezone('utc')
     obstime = obstime.astimezone(utc).replace(tzinfo=None)
 
     return obstime, dist
 
 
+def get_distance_between_two_points(geo_point1, geo_point2):
+    """Get the distance in km on the earth between two (lon,lat) points."""
+    lon0, lat0 = geo_point1
+    lon, lat = geo_point2
+    return distance.distance((lat0, lon0), (lat, lon)).kilometers
+
+
 def _create_output_message(msg, topic, geojson, filename):
     """Create the output message from the input message and the geojson payload."""
     to_send = msg.data.copy()
     to_send.pop('type', None)
     to_send['related_detection'] = geojson['features']['properties']['related_detection']
     to_send['power'] = geojson['features']['properties']['power']
     to_send['tb'] = geojson['features']['properties']['tb']
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_api_posting.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_api_posting.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_config.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2022 Adam.Dybbroe
+# Copyright (c) 2022, 2023 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam.Dybbroe <a000680@c21856.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -22,21 +22,44 @@
 
 """Test getting the yaml configurations from file."""
 
 from activefires_pp.config import read_config
 from activefires_pp.config import get_xauthentication_token
 
 
-def test_get_yaml_configuration(fake_yamlconfig_file):
-    """Test read and get the yaml configuration from file."""
+def test_get_yaml_configuration_for_alarm_filtering(fake_yamlconfig_file):
+    """Test read and get the yaml configuration from file for alarm filtering."""
     config = read_config(fake_yamlconfig_file)
+    assert config['products'] == ['afimg']
     assert config['subscribe_topics'] == '/VIIRS/L2/Fires/PP/National'
     assert config['publish_topic'] == '/VIIRS/L2/Fires/PP/SOSAlarm'
     assert config['geojson_file_pattern_alarms'] == 'sos_{start_time:%Y%m%d_%H%M%S}_{id:d}.geojson'
     assert config['fire_alarms_dir'] == '/path/where/the/filtered/alarms/will/be/stored'
     assert config['restapi_url'] == 'https://xxx.smhi.se:xxxx'
 
 
 def test_get_xauthentication_token(fake_token_file):
     """Test getting the xauthentication token from a file."""
     fake_token = get_xauthentication_token(fake_token_file)
     assert fake_token == 'my-token'
+
+
+def test_read_yaml_configuration_for_postprocessing(fake_yamlconfig_file_post_processing):
+    """Test read in the yaml configuration for fires post processing."""
+    config = read_config(fake_yamlconfig_file_post_processing)
+
+    assert config['subscribe_topics'] == 'VIIRS/L2/AFI'
+    assert config['publish_topic'] == '/VIIRS/L2/Fires/PP'
+    assert config['timezone'] == 'Europe/Stockholm'
+    assert config['af_pattern_ibands'] == 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}_b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt'  # noqa
+    assert config['regional_shapefiles_format'] == 'omr_{region_code:s}_Buffer.{ext:s}'
+    assert config['output_dir'] == '/path/where/the/filtered/results/will/be/stored'
+
+    assert len(config['output']['national']['default']) == 1
+    assert config['output']['national']['default'] == {'geojson_file_pattern':
+                                              'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}.geojson'}  # noqa
+    assert config['output']['national']['sweref99'] == {'geojson_file_pattern':
+                                                        'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_sweref99.geojson',  # noqa
+                                                        'projection': "EPSG:3006"}
+
+    assert config['output']['regional']['default'] == {'geojson_file_pattern':
+                                              'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_{region_name:s}.geojson'}  # noqa
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_fire_detection_id_handling.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_messaging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,323 +1,268 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2023 Adam.Dybbroe
+# Copyright (c) 2021-2024 Adam.Dybbroe
 
 # Author(s):
 
-#   Adam.Dybbroe <a000680@c21856.ad.smhi.se>
+#   Adam Dybbroe <Firstname.Lastname@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Test operations on the fire detection id."""
+"""Unit testing the message handling part of the post-processing."""
 
+import pytest
 from unittest.mock import patch
-from unittest import TestCase
-import pandas as pd
-
-import io
 from datetime import datetime
-from freezegun import freeze_time
-
-from activefires_pp.post_processing import ActiveFiresShapefileFiltering
-from activefires_pp.post_processing import ActiveFiresPostprocessing
-from activefires_pp.post_processing import COL_NAMES
-
-
-TEST_ACTIVE_FIRES_FILEPATH2 = "./AFIMG_npp_d20230616_t1110054_e1111296_b60284_c20230616112418557033_cspp_dev.txt"
-TEST_ACTIVE_FIRES_FILEPATH3 = "./AFIMG_j01_d20230617_t1140564_e1142209_b28903_c20230617115513873196_cspp_dev.txt"
-TEST_ACTIVE_FIRES_FILEPATH4 = "./AFIMG_j01_d20230618_t0942269_e0943514_b28916_c20230618095604331171_cspp_dev.txt"
-
-
-# Here we have sorted out all detections not passing the filter mask!
-# So, 4 fire detections are left corresponding to what would end up in the geojson files:
-TEST_ACTIVE_FIRES_FILE_DATA2 = """
-# Active Fires I-band EDR
-#
-# source: AFIMG_npp_d20230616_t1110054_e1111296_b60284_c20230616112418557033_cspp_dev.nc
-# version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
-#
-# column 1: latitude of fire pixel (degrees)
-# column 2: longitude of fire pixel (degrees)
-# column 3: I04 brightness temperature of fire pixel (K)
-# column 4: Along-scan fire pixel resolution (km)
-# column 5: Along-track fire pixel resolution (km)
-# column 6: detection confidence ([7,8,9]->[lo,med,hi])
-# column 7: fire radiative power (MW)
-#
-# number of fire pixels: 14
-#
-  62.65801239,   17.25905228,  339.66326904,  0.375,  0.375,    8,    2.51202917
-  64.21694183,   17.42074966,  329.65161133,  0.375,  0.375,    8,    3.39806151
-  64.56904602,   16.60095215,  346.52050781,  0.375,  0.375,    8,   20.59289360
-  64.57222748,   16.59840012,  348.72860718,  0.375,  0.375,    8,   20.59289360
-"""
-
-# Here we have sorted out all detections not passing the filter mask!
-# So, 1 fire detection is left corresponding to what would end up in the geojson files:
-TEST_ACTIVE_FIRES_FILE_DATA3 = """
-# Active Fires I-band EDR
-#
-# source: AFIMG_j01_d20230617_t1140564_e1142209_b28903_c20230617115513873196_cspp_dev.nc
-# version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
-#
-# column 1: latitude of fire pixel (degrees)
-# column 2: longitude of fire pixel (degrees)
-# column 3: I04 brightness temperature of fire pixel (K)
-# column 4: Along-scan fire pixel resolution (km)
-# column 5: Along-track fire pixel resolution (km)
-# column 6: detection confidence ([7,8,9]->[lo,med,hi])
-# column 7: fire radiative power (MW)
-#
-# number of fire pixels: 9
-#
-  64.46707153,   17.65028381,  330.15390015,  0.375,  0.375,    8,    3.75669074
-"""
-
-
-# Here we have sorted out all detections not passing the filter mask!
-# So, 2 fire detections are left corresponding to what would end up in the geojson files:
-TEST_ACTIVE_FIRES_FILE_DATA4 = """
-# Active Fires I-band EDR
-#
-# source: AFIMG_j01_d20230618_t0942269_e0943514_b28916_c20230618095604331171_cspp_dev.nc
-# version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
-#
-# column 1: latitude of fire pixel (degrees)
-# column 2: longitude of fire pixel (degrees)
-# column 3: I04 brightness temperature of fire pixel (K)
-# column 4: Along-scan fire pixel resolution (km)
-# column 5: Along-track fire pixel resolution (km)
-# column 6: detection confidence ([7,8,9]->[lo,med,hi])
-# column 7: fire radiative power (MW)
-#
-# number of fire pixels: 10
-#
-  65.55922699,   17.62709618,  335.81488037,  0.375,  0.375,    8,    4.66374302
-  67.27209473,   20.14731216,  348.89843750,  0.375,  0.375,    8,   11.79477501
-"""
-
-CONFIG_EXAMPLE = {'publish_topic': '/VIIRS/L2/Fires/PP',
-                  'subscribe_topics': 'VIIRS/L2/AFI',
-                  'af_pattern_ibands':
-                  'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}' +
-                  '_b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt',
-                  'geojson_file_pattern_national': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}.geojson',
-                  'geojson_file_pattern_regional': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_' +
-                  '{region_name:s}.geojson',
-                  'regional_shapefiles_format': 'omr_{region_code:s}_Buffer.{ext:s}',
-                  'output_dir': '/path/where/the/filtered/results/will/be/stored',
-                  'filepath_detection_id_cache': '/path/to/the/detection_id/cache',
-                  'timezone': 'Europe/Stockholm'}
-
-MY_FILE_PATTERN = ("AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}_" +
-                   "b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt")
-
+import logging
 
-@freeze_time('2023-06-16 11:24:00')
-@patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
-@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_add_unique_day_id_to_detections_sameday(readdata, setup_comm, get_config, gethostname):
-    """Test adding unique id's to the fire detection data."""
-    get_config.return_value = CONFIG_EXAMPLE
-    gethostname.return_value = "my.host.name"
-
-    myconfigfile = "/my/config/file/path"
-    myborders_file = "/my/shape/file/with/country/borders"
-    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+from posttroll.message import Message
+from posttroll.testing import patched_publisher
+from posttroll.publisher import create_publisher_from_dict_config
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+from activefires_pp.post_processing import ActiveFiresPostprocessing
+from activefires_pp.spatiotemporal_alarm_filtering import _create_output_message
 
-    myfilepath = TEST_ACTIVE_FIRES_FILEPATH2
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA2)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
-    readdata.return_value = afdata
+TEST_MSG = """pytroll://VIIRS/L2/AFI/edr/2/nrk/test/polar/direct_readout file safusr.t@lxserv2313.smhi.se 2021-04-07T00:41:41.568370 v1.01 application/json {"start_time": "2021-04-07T00:28:17", "end_time": "2021-04-07T00:29:40", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "format": "edr", "type": "netcdf", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17530, "origin": "172.29.4.164:9099", "uri": "ssh://lxserv2313.smhi.se/san1/polar_out/direct_readout/viirs_active_fires/unfiltered/AFIMG_j01_d20210407_t0028179_e0029407_b17531_c20210407004133375592_cspp_dev.nc", "uid": "AFIMG_j01_d20210407_t0028179_e0029407_b17531_c20210407004133375592_cspp_dev.nc"}"""  # noqa
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
-    with patch('os.path.exists') as mypatch:
-        mypatch.return_value = True
-        afdata = this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
+TEST_MSG_TXT = """pytroll://VIIRS/L2/AFI/edr/2/nrk/test/polar/direct_readout file safusr.t@lxserv2313.smhi.se 2023-07-05T10:27:28.821803 v1.01 application/json {"start_time": "2023-07-05T10:07:50", "end_time": "2023-07-05T10:09:15", "orbit_number": 1, "platform_name": "Suomi-NPP", "sensor": "viirs", "format": "edr", "type": "txt", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 60553, "origin": "172.29.4.164:9099", "uri": "/san1/polar_out/direct_readout/viirs_active_fires/unfiltered/AFIMG_npp_d20230705_t1007509_e1009151_b60553_c20230705102721942345_cspp_dev.txt", "uid": "AFIMG_npp_d20230705_t1007509_e1009151_b60553_c20230705102721942345_cspp_dev.txt"}"""  # noqa
 
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime.utcnow(),
-                                                         'counter': 0})
 
-    # 4 fire detections, so (current) ID should be raised by 4
-    afdata = afpp.add_unique_day_id(afdata)
-    assert 'detection_id' in afdata
-    assert afdata['detection_id'].values.tolist() == ['20230616-1', '20230616-2',
-                                                      '20230616-3', '20230616-4']
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime.utcnow(),
-                                                         'counter': 4})
+def get_fake_publisher(portnumber=1979):
+    """Return a fake publisher."""
+    return create_publisher_from_dict_config(dict(port=portnumber, nameservers=False))
 
 
-@freeze_time('2023-06-17 11:55:00')
+@patch('os.path.exists')
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_add_unique_day_id_to_detections_24hours_plus(readdata, setup_comm,
-                                                      get_config, gethostname):
-    """Test adding unique id's to the fire detection data."""
-    get_config.return_value = CONFIG_EXAMPLE
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing.get_id_from_file')
+def test_check_incoming_message_nc_file_exists(setup_comm, gethostname, path_exists,
+                                               get_id_from_file,
+                                               fake_yamlconfig_file_post_processing):
+    """Test the check of incoming message content and getting the file path from the message.
+
+    Here we test the case when a netCDF file is provided in the message and we
+    test the behaviour when the file also actually exist on the file system.
+    """
     gethostname.return_value = "my.host.name"
+    path_exists.return_value = True
+    get_id_from_file.return_value = {'date': datetime.utcnow(), 'counter': 0}
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
-    afpp._fire_detection_id = {'date': datetime(2023, 6, 16, 11, 24, 0), 'counter': 4}
-
-    myfilepath = TEST_ACTIVE_FIRES_FILEPATH3
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
+    afpp.filepath_detection_id_cache = False
+
+    input_msg = Message.decode(rawstr=TEST_MSG)
+    with patched_publisher() as published_messages:
+        afpp.publisher = get_fake_publisher()
+        afpp.publisher.start()
+        result = afpp.check_incoming_message_and_get_filename(input_msg)
+        afpp.publisher.stop()
+
+    assert result is None
+    assert len(published_messages) == 2
+    assert 'No fire detections for this granule' in published_messages[0]
+    assert 'No fire detections for this granule' in published_messages[1]
+    assert 'VIIRS/L2/Fires/PP/National' in published_messages[0]
+    assert 'VIIRS/L2/Fires/PP/Regional' in published_messages[1]
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA3)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
-    readdata.return_value = afdata
-
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
-    with patch('os.path.exists') as mypatch:
-        mypatch.return_value = True
-        afdata = this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
-
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime(2023, 6, 16, 11, 24, 0),
-                                                         'counter': 4})
-    # 1 new fire detection, so (current) ID should be raised - a new day, so id
-    # starting over from 0, and a new date!
-    afdata = afpp.add_unique_day_id(afdata)
-    assert 'detection_id' in afdata
-    assert afdata['detection_id'].values.tolist() == ['20230617-1']
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime(2023, 6, 17, 11, 55, 0),
-                                                         'counter': 1})
 
-
-@freeze_time('2023-06-18 09:56:00')
+@patch('os.path.exists')
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_add_unique_day_id_to_detections_newday(readdata, setup_comm, get_config, gethostname):
-    """Test adding unique id's to the fire detection data."""
-    get_config.return_value = CONFIG_EXAMPLE
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing.get_id_from_file')
+def test_check_incoming_message_txt_file_exists(setup_comm, gethostname, path_exists,
+                                                get_id_from_file,
+                                                fake_yamlconfig_file_post_processing):
+    """Test the check of incoming message content and getting the file path from the message.
+
+    Here we test the case when a txt file is provided in the message and we
+    test the behaviour when the file also actually exist on the file system.
+    """
     gethostname.return_value = "my.host.name"
+    path_exists.return_value = True
+    get_id_from_file.return_value = {'date': datetime.utcnow(), 'counter': 0}
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
-    afpp._fire_detection_id = {'date': datetime(2023, 6, 17, 11, 55, 0), 'counter': 1}
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
 
-    myfilepath = TEST_ACTIVE_FIRES_FILEPATH4
+    input_msg = Message.decode(rawstr=TEST_MSG_TXT)
+    with patched_publisher() as published_messages:
+        afpp.publisher = get_fake_publisher(1980)
+        afpp.publisher.start()
+        result = afpp.check_incoming_message_and_get_filename(input_msg)
+        afpp.publisher.stop()
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA4)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
-    readdata.return_value = afdata
-
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
-    with patch('os.path.exists') as mypatch:
-        mypatch.return_value = True
-        afdata = this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
-
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime(2023, 6, 17, 11, 55, 0),
-                                                         'counter': 1})
-    # 2 new fire detections, so (current) ID should be raised - a new day, so id
-    # starting over from 0, and a new date!
-    afdata = afpp.add_unique_day_id(afdata)
-    assert 'detection_id' in afdata
-    assert afdata['detection_id'].values.tolist() == ['20230618-1', '20230618-2']
-    TestCase().assertDictEqual(afpp._fire_detection_id, {'date': datetime(2023, 6, 18, 9, 56, 0),
-                                                         'counter': 2})
+    assert len(published_messages) == 0
+    assert result == '/san1/polar_out/direct_readout/viirs_active_fires/unfiltered/AFIMG_npp_d20230705_t1007509_e1009151_b60553_c20230705102721942345_cspp_dev.txt'  # noqa
 
 
+@patch('os.path.exists')
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_store_fire_detection_id_on_disk(readdata, setup_comm,
-                                         get_config, gethostname, tmp_path):
-    """Test store the latest/current detection id to a file."""
-    get_config.return_value = CONFIG_EXAMPLE
+def test_check_incoming_message_txt_file_does_not_exist(setup_comm, gethostname, path_exists,
+                                                        fake_yamlconfig_file_post_processing):
+    """Test the check of incoming message content and getting the file path from the message.
+
+    Here we test the case when a txt file is provided in the message and we
+    test the behaviour when the file does not exist on the file system.
+    """
     gethostname.return_value = "my.host.name"
+    path_exists.return_value = False
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
-    afpp._fire_detection_id = {'date': datetime(2023, 6, 17, 11, 55, 0), 'counter': 1}
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
 
-    detection_id_cache = tmp_path / 'detection_id_cache.txt'
-    afpp.filepath_detection_id_cache = str(detection_id_cache)
-    afpp.save_id_to_file()
+    input_msg = Message.decode(rawstr=TEST_MSG_TXT)
+    with patched_publisher() as published_messages:
+        afpp.publisher = get_fake_publisher(1981)
+        afpp.publisher.start()
+        result = afpp.check_incoming_message_and_get_filename(input_msg)
+        afpp.publisher.stop()
+
+    assert len(published_messages) == 0
+    assert result is None
+
+
+@pytest.mark.parametrize("projname, expected",
+                         [("sweref99", 'afimg_sweref99'),
+                          ("default", 'afimg')]
+                         )
+def test_prepare_posttroll_message_national(caplog, projname, expected,
+                                            fake_yamlconfig_file_post_processing):
+    """Test prepare the posttroll message for detections on a National level."""
+    myboarders_file = "/my/shape/file/with/country/boarders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    with open(afpp.filepath_detection_id_cache) as fpt:
-        result = fpt.read()
+    with patch('socket.gethostname') as gethostname:
+        with patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication'):
+            gethostname.return_value = "my.host.name"
 
-    assert result == '20230617-1'
+            afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                             myboarders_file, mymask_file)
 
+    test_filepath = "/my/geojson/file/path"
 
-@freeze_time('2023-06-18 12:00:00')
-@patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
-@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_initialize_fire_detection_id_nofile(readdata, setup_comm,
-                                             get_config, gethostname, tmp_path):
-    """Test initialize the fire detection id with no cache on disk."""
-    get_config.return_value = CONFIG_EXAMPLE
-    gethostname.return_value = "my.host.name"
+    input_msg = Message.decode(rawstr=TEST_MSG)
+    with caplog.at_level(logging.INFO):
+        result_messages = afpp.get_output_messages(test_filepath, input_msg, 1, proj_name=projname)
 
-    myconfigfile = "/my/config/file/path"
-    myborders_file = "/my/shape/file/with/country/borders"
-    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+    log_expected = "Geojson file created! Number of fires = 1"
+    assert log_expected in caplog.text
+
+    res_msg = result_messages[0]
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    assert res_msg.data['platform_name'] == 'NOAA-20'
+    assert res_msg.data['type'] == 'GEOJSON-filtered'
+    assert res_msg.data['format'] == 'geojson'
+    assert res_msg.data['product'] == expected
+    assert res_msg.subject == '/VIIRS/L2/Fires/PP/National'
+    assert res_msg.data['uri'] == '/my/geojson/file/path'
 
-    assert afpp.filepath_detection_id_cache == '/path/to/the/detection_id/cache'
 
-    expected = {'date': datetime(2023, 6, 18, 12, 0, 0), 'counter': 0}
+def test_prepare_posttroll_message_regional(caplog, fake_yamlconfig_file_post_processing):
+    """Test setup the posttroll message."""
+    myboarders_file = "/my/shape/file/with/country/boarders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp._initialize_fire_detection_id()
-    TestCase().assertDictEqual(afpp._fire_detection_id, expected)
+    with patch('socket.gethostname') as gethostname:
+        with patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication'):
+            gethostname.return_value = "my.host.name"
+            afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                             myboarders_file, mymask_file)
+
+    test_filepath = "/my/geojson/file/path"
+    input_msg = Message.decode(rawstr=TEST_MSG)
+
+    fake_region_mask = {'attributes': {'Kod_omr': '9999',
+                                       'Testomr': 'Some area description'}}
+    with caplog.at_level(logging.INFO):
+        res_msg = afpp._generate_output_message(test_filepath, input_msg, 'default',
+                                                region=fake_region_mask)
+
+    assert res_msg.data['uri'] == test_filepath
+    assert caplog.text == ''
+    assert res_msg.subject == '/VIIRS/L2/Fires/PP/Regional/9999'
 
 
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-@patch('activefires_pp.post_processing._read_data')
-def test_get_fire_detection_id_from_file(readdata, setup_comm,
-                                         get_config, gethostname, tmp_path):
-    """Test rtrieve the detection id from file."""
-    get_config.return_value = CONFIG_EXAMPLE
+def test_prepare_posttroll_message_no_fires(setup_comm, gethostname,
+                                            fake_yamlconfig_file_post_processing):
+    """Test setup the posttroll message."""
     gethostname.return_value = "my.host.name"
 
-    myconfigfile = "/my/config/file/path"
-    myborders_file = "/my/shape/file/with/country/borders"
+    myboarders_file = "/my/shape/file/with/country/boarders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
-    afpp._fire_detection_id = {'date': datetime(2023, 6, 17, 11, 55, 0), 'counter': 1}
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myboarders_file, mymask_file)
+
+    input_msg = Message.decode(rawstr=TEST_MSG)
+    msg_str = 'No fire detections for this granule'
 
-    detection_id_cache = tmp_path / 'detection_id_cache.txt'
-    afpp.filepath_detection_id_cache = str(detection_id_cache)
-    afpp.save_id_to_file()
-    result = afpp.get_id_from_file()
-    expected = {'date': datetime(2023, 6, 17), 'counter': 1}
-    TestCase().assertDictEqual(result, expected)
+    result_messages = afpp._generate_no_fires_messages(input_msg, msg_str)
 
-    afpp._initialize_fire_detection_id()
-    TestCase().assertDictEqual(afpp._fire_detection_id, expected)
+    for (nat_or_reg, res_msg) in zip(['National', 'Regional'], result_messages):
+        assert res_msg.data['info'] == msg_str
+        assert res_msg.subject == '/VIIRS/L2/Fires/PP/' + nat_or_reg
+        assert 'type' not in res_msg.data
+        assert 'format' not in res_msg.data
+        assert 'product' not in res_msg.data
+        assert 'uri' not in res_msg.data
+
+
+def test_create_output_message(tmp_path):
+    """Test create output message from geojson payload."""
+    input_msg = Message.decode(rawstr=TEST_MSG)
+    filename = tmp_path / 'test_geojson_alarm_file.geojson'
+    output_topic = '/VIIRS/L2/Fires/PP/SOSAlarm'
+    geojson_alarm = {"features": {"geometry": {"coordinates": [16.249069, 57.156235], "type": "Point"},
+                                  "properties": {"confidence": 8,
+                                                 "observation_time": "2021-06-19T02:58:45.700000+02:00",
+                                                 "platform_name": "NOAA-20",
+                                                 "power": 2.23312426,
+                                                 "related_detection": False,
+                                                 "tb": 310.37322998}, "type": "Feature"},
+                     "type": "FeatureCollection"}
+
+    output_msg = _create_output_message(input_msg, output_topic, geojson_alarm, filename)
+
+    assert output_msg.data == {'start_time': datetime(2021, 4, 7, 0, 28, 17),
+                               'end_time': datetime(2021, 4, 7, 0, 29, 40),
+                               'orbit_number': 1,
+                               'platform_name': 'NOAA-20',
+                               'sensor': 'viirs',
+                               'data_processing_level': '2',
+                               'format': 'geojson',
+                               'variant': 'DR',
+                               'orig_orbit_number': 17530,
+                               'origin': '172.29.4.164:9099',
+                               'related_detection': False,
+                               'power': 2.23312426,
+                               'tb': 310.37322998,
+                               'coordinates': [16.249069, 57.156235],
+                               'file': 'test_geojson_alarm_file.geojson',
+                               'uri': str(filename)}
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_fire_notifications.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_fire_notifications.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,28 +22,32 @@
 
 """Unit testing the fire notifications."""
 
 import unittest
 from unittest.mock import patch
 import yaml
 import io
-# from posttroll.message import Message
+from posttroll.message import Message
 
 from activefires_pp.fire_notifications import EndUserNotifier
 from activefires_pp.fire_notifications import EndUserNotifierRegional
 from activefires_pp.fire_notifications import get_recipients_for_region
 
 TEST_CONFIG_FILE = "/home/a000680/usr/src/forks/activefires-pp/examples/fire_notifier.yaml"
 TEST_CONFIG_FILE_REGIONAL = "/home/a000680/usr/src/forks/activefires-pp/examples/fire_notifier_regional.yaml"
 
 NAT_CONFIG = """
 # Publish/subscribe
 publish_topic: VIIRS/L2/MSB/National
 subscribe_topics: VIIRS/L2/Fires/PP/National
 
+products:
+  - afimg
+  - afimg_some_other_geoid
+
 smtp_server: smtp.mydomain.se
 
 domain: mydomain.se
 
 sender: active-fires@mydomain.se
 
 recipients: ["recipient1@recipients.se", "recipient2@recipients.se", "recipient3@recipients.se"]
@@ -98,14 +102,16 @@
   text: 'Stop being bothered: Send a note to unsubscribe@mydomain.xx'
 """
 
 REGIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/Regional/0114 file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.542021 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "region_name": "Storstockholms brandf\u00f6rsvar", "region_code": "0114", "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "uid": "AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
 NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
+NATIONAL_TEST_MESSAGE2 = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953_somegeoid.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg_somegeoid"}"""  # noqa
+
 
 class MyNetrcMock(object):
     """Mocking the handling of secrets via the .netrc file."""
 
     def __init__(self):
         """Initialize the netrc mock class."""
         self.hosts = {'default': ('my_user', None, 'my_passwd')}
@@ -118,14 +124,60 @@
 class TestNotifyEndUsers(unittest.TestCase):
     """Test notifications on National fires."""
 
     @patch('activefires_pp.fire_notifications.netrc')
     @patch('activefires_pp.fire_notifications.socket.gethostname')
     @patch('activefires_pp.fire_notifications.read_config')
     @patch('activefires_pp.fire_notifications.EndUserNotifier._setup_and_start_communication')
+    def test_check_incoming_message_product_name_ok(self, setup_comm, read_config, gethostname, netrc):
+        """Test the incoming message for the 'right' product (name)."""
+        secrets = MyNetrcMock()
+        netrc.return_value = secrets
+        gethostname.return_value = 'default'
+
+        myconfigfile = "/my/config/file/path"
+        natstream = io.StringIO(NAT_CONFIG)
+
+        read_config.return_value = yaml.load(natstream, Loader=yaml.UnsafeLoader)
+
+        this = EndUserNotifier(myconfigfile)
+
+        input_msg = Message.decode(rawstr=NATIONAL_TEST_MESSAGE)
+
+        result = this._product_name_supported(input_msg)
+
+        assert result is True
+
+    @patch('activefires_pp.fire_notifications.netrc')
+    @patch('activefires_pp.fire_notifications.socket.gethostname')
+    @patch('activefires_pp.fire_notifications.read_config')
+    @patch('activefires_pp.fire_notifications.EndUserNotifier._setup_and_start_communication')
+    def test_check_incoming_message_product_name_not_ok(self, setup_comm, read_config, gethostname, netrc):
+        """Test the incoming message for the 'right' product (name)."""
+        secrets = MyNetrcMock()
+        netrc.return_value = secrets
+        gethostname.return_value = 'default'
+
+        myconfigfile = "/my/config/file/path"
+        natstream = io.StringIO(NAT_CONFIG)
+
+        read_config.return_value = yaml.load(natstream, Loader=yaml.UnsafeLoader)
+
+        this = EndUserNotifier(myconfigfile)
+
+        input_msg = Message.decode(rawstr=NATIONAL_TEST_MESSAGE2)
+
+        result = this._product_name_supported(input_msg)
+
+        assert result is False
+
+    @patch('activefires_pp.fire_notifications.netrc')
+    @patch('activefires_pp.fire_notifications.socket.gethostname')
+    @patch('activefires_pp.fire_notifications.read_config')
+    @patch('activefires_pp.fire_notifications.EndUserNotifier._setup_and_start_communication')
     def test_get_options_national_filtering(self, setup_comm, read_config, gethostname, netrc):
         """Test get the config options for National fires filtering."""
         secrets = MyNetrcMock()
         netrc.return_value = secrets
         gethostname.return_value = 'default'
 
         myconfigfile = "/my/config/file/path"
@@ -133,15 +185,17 @@
 
         read_config.return_value = yaml.load(natstream, Loader=yaml.UnsafeLoader)
 
         this = EndUserNotifier(myconfigfile)
 
         expected = {'publish_topic': 'VIIRS/L2/MSB/National',
                     'subscribe_topics': ['VIIRS/L2/Fires/PP/National'],
-                    'smtp_server': 'smtp.mydomain.se', 'domain': 'mydomain.se', 'sender': 'active-fires@mydomain.se',
+                    'products': ['afimg', 'afimg_some_other_geoid'],
+                    'smtp_server': 'smtp.mydomain.se',
+                    'domain': 'mydomain.se', 'sender': 'active-fires@mydomain.se',
                     'recipients': ['recipient1@recipients.se', 'recipient2@recipients.se', 'recipient3@recipients.se'],
                     'recipients_attachment': ['recipient1@recipients.se', 'recipient2@recipients.se'],
                     'subject': 'My subject', 'max_number_of_fires_in_sms': 3,
                     'fire_data': ['power', 'observation_time'],
                     'unsubscribe': {'address': 'unsubscribe@mydomain.xx',
                                     'text': 'Stop being bothered: Send a note to unsubscribe@mydomain.xx'},
                     'unsubscribe_address': 'unsubscribe@mydomain.xx',
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_fires_filtering.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_fires_filtering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021 - 2023 Adam Dybbroe
+# Copyright (c) 2021 - 2024 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -14,37 +14,41 @@
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# along with this 2program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Test the Fires filtering functionality."""
 
 import pytest
 from unittest.mock import patch
 from unittest import TestCase
-from freezegun import freeze_time
 
 import pandas as pd
 from geojson import FeatureCollection
 import numpy as np
 import io
+import logging
 from datetime import datetime
+from freezegun import freeze_time
 
 from activefires_pp.post_processing import ActiveFiresShapefileFiltering
 from activefires_pp.post_processing import ActiveFiresPostprocessing
 from activefires_pp.post_processing import COL_NAMES
-
+from activefires_pp.tests.test_utils import AF_FILE_PATTERN
+from activefires_pp.utils import UnitConverter
 from activefires_pp.post_processing import geojson_feature_collection_from_detections
 
+
 TEST_ACTIVE_FIRES_FILEPATH = "./AFIMG_j01_d20210414_t1126439_e1128084_b17637_c20210414114130392094_cspp_dev.txt"
 TEST_ACTIVE_FIRES_FILEPATH2 = "./AFIMG_npp_d20230616_t1110054_e1111296_b60284_c20230616112418557033_cspp_dev.txt"
+TEST_ACTIVE_FIRES_FILEPATH3 = "./AFIMG_j01_d20230617_t1140564_e1142209_b28903_c20230617115513873196_cspp_dev.txt"
 
 
 TEST_ACTIVE_FIRES_FILE_DATA = """
 # Active Fires I-band EDR
 #
 # source: AFIMG_j01_d20210414_t1126439_e1128084_b17637_c20210414114130392094_cspp_dev.nc
 # version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
@@ -93,38 +97,43 @@
 # column 4: Along-scan fire pixel resolution (km)
 # column 5: Along-track fire pixel resolution (km)
 # column 6: detection confidence ([7,8,9]->[lo,med,hi])
 # column 7: fire radiative power (MW)
 #
 # number of fire pixels: 14
 #
+  58.74638367,    8.54766846,  340.68481445,  0.375,  0.375,    8,   10.83046722
+  55.34669113,   -4.51371527,  325.72799683,  0.375,  0.375,    8,    6.21815872
   62.65801239,   17.25905228,  339.66326904,  0.375,  0.375,    8,    2.51202917
   64.21694183,   17.42074966,  329.65161133,  0.375,  0.375,    8,    3.39806151
   64.56904602,   16.60095215,  346.52050781,  0.375,  0.375,    8,   20.59289360
   64.57222748,   16.59840012,  348.72860718,  0.375,  0.375,    8,   20.59289360
 """
 
-CONFIG_EXAMPLE = {'publish_topic': '/VIIRS/L2/Fires/PP',
-                  'subscribe_topics': 'VIIRS/L2/AFI',
-                  'af_pattern_ibands':
-                  'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}' +
-                  '_b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt',
-                  'geojson_file_pattern_national': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}.geojson',
-                  'geojson_file_pattern_regional': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_' +
-                  '{region_name:s}.geojson',
-                  'regional_shapefiles_format': 'omr_{region_code:s}_Buffer.{ext:s}',
-                  'output_dir': '/path/where/the/filtered/results/will/be/stored',
-                  'filepath_detection_id_cache': '/path/to/the/detection_id/cache',
-                  'timezone': 'Europe/Stockholm'}
-
-OPEN_FSTREAM = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-
+# Here we have sorted out all detections not passing the filter mask!
+# So, 1 fire detection is left corresponding to what would end up in the geojson files:
+TEST_ACTIVE_FIRES_FILE_DATA3 = """
+# Active Fires I-band EDR
+#
+# source: AFIMG_j01_d20230617_t1140564_e1142209_b28903_c20230617115513873196_cspp_dev.nc
+# version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
+#
+# column 1: latitude of fire pixel (degrees)
+# column 2: longitude of fire pixel (degrees)
+# column 3: I04 brightness temperature of fire pixel (K)
+# column 4: Along-scan fire pixel resolution (km)
+# column 5: Along-track fire pixel resolution (km)
+# column 6: detection confidence ([7,8,9]->[lo,med,hi])
+# column 7: fire radiative power (MW)
+#
+# number of fire pixels: 9
+#
+  64.46707153,   17.65028381,  330.15390015,  0.375,  0.375,    8,    3.75669074
+"""
 
-MY_FILE_PATTERN = ("AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}_" +
-                   "b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt")
 
 TEST_REGIONAL_MASK = {}
 TEST_REGIONAL_MASK['Bergslagen (RRB)'] = {'mask': np.array([False, False, False, False, False,
                                                             False, False, False, False,
                                                             False, False, False, False,  True,
                                                             False, False, False, False]),
                                           'attributes': {'Join_Count': 2, 'TARGET_FID': 142,
@@ -147,110 +156,143 @@
                                                           'Shape_Area': 2040770168.02},
                                            'all_inside_test_area': False, 'some_inside_test_area': False}
 
 FAKE_MASK1 = np.array([False, False, False, False, False, False, False, False,  True,
                        False, False,  True, False,  True, False, False, False, False])
 FAKE_MASK2 = np.array([True, False,  True])
 
+FAKE_MASK11 = np.array([True, True])
+FAKE_MASK12 = np.array([False])
+
 
 @patch('activefires_pp.post_processing._read_data')
-def test_add_start_and_end_time_to_active_fires_data_utc(readdata):
+def test_add_start_and_end_time_to_active_fires_data_utc(readdata, fake_active_fires_file_data):
     """Test adding start and end times to the active fires data."""
-    myfilepath = TEST_ACTIVE_FIRES_FILEPATH
+    open_fstream, myfilepath = fake_active_fires_file_data
+    afdata = pd.read_csv(open_fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
 
-    # fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-    afdata = pd.read_csv(OPEN_FSTREAM, index_col=None, header=None, comment='#', names=COL_NAMES)
     readdata.return_value = afdata
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
+        af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=False)
 
-    assert 'starttime' in this._afdata
-    assert 'endtime' in this._afdata
-    assert this._afdata['starttime'].shape == (18,)
+    assert 'starttime' in af_shpfile_filter.afdata
+    assert 'endtime' in af_shpfile_filter.afdata
+    assert af_shpfile_filter.afdata['starttime'].shape == (18,)
 
-    assert str(this._afdata['starttime'][0]) == '2021-04-14 11:26:43.900000'
-    assert str(this._afdata['endtime'][0]) == '2021-04-14 11:28:08'
+    assert str(af_shpfile_filter.afdata['starttime'][0]) == '2021-04-14 11:26:43.900000'
+    assert str(af_shpfile_filter.afdata['endtime'][0]) == '2021-04-14 11:28:08'
 
 
 @patch('activefires_pp.post_processing._read_data')
-def test_add_start_and_end_time_to_active_fires_data_localtime(readdata):
+def test_add_start_and_end_time_to_active_fires_data_localtime(readdata, fake_active_fires_file_data):
     """Test adding start and end times to the active fires data."""
-    myfilepath = TEST_ACTIVE_FIRES_FILEPATH
+    open_fstream, myfilepath = fake_active_fires_file_data
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    afdata = pd.read_csv(open_fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
     readdata.return_value = afdata
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Stockholm')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Stockholm')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=True)
+        af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=True)
 
-    assert 'starttime' in this._afdata
-    assert 'endtime' in this._afdata
+    assert 'starttime' in af_shpfile_filter.afdata
+    assert 'endtime' in af_shpfile_filter.afdata
 
-    assert str(this._afdata['starttime'][0]) == '2021-04-14 13:26:43.900000'
-    assert str(this._afdata['endtime'][0]) == '2021-04-14 13:28:08'
+    assert str(af_shpfile_filter.afdata['starttime'][0]) == '2021-04-14 13:26:43.900000'
+    assert str(af_shpfile_filter.afdata['endtime'][0]) == '2021-04-14 13:28:08'
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Iceland')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Iceland')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=True)
+        af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=True)
 
-    assert 'starttime' in this._afdata
-    assert 'endtime' in this._afdata
+    assert 'starttime' in af_shpfile_filter.afdata
+    assert 'endtime' in af_shpfile_filter.afdata
 
-    assert str(this._afdata['starttime'][0]) == '2021-04-14 11:26:43.900000'
-    assert str(this._afdata['endtime'][0]) == '2021-04-14 11:28:08'
+    assert str(af_shpfile_filter.afdata['starttime'][0]) == '2021-04-14 11:26:43.900000'
+    assert str(af_shpfile_filter.afdata['endtime'][0]) == '2021-04-14 11:28:08'
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Helsinki')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Helsinki')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=True)
+        af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=True)
 
-    assert 'starttime' in this._afdata
-    assert 'endtime' in this._afdata
+    assert 'starttime' in af_shpfile_filter.afdata
+    assert 'endtime' in af_shpfile_filter.afdata
 
-    assert str(this._afdata['starttime'][0]) == '2021-04-14 14:26:43.900000'
-    assert str(this._afdata['endtime'][0]) == '2021-04-14 14:28:08'
+    assert str(af_shpfile_filter.afdata['starttime'][0]) == '2021-04-14 14:26:43.900000'
+    assert str(af_shpfile_filter.afdata['endtime'][0]) == '2021-04-14 14:28:08'
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Lisbon')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='Europe/Lisbon')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=True)
+        af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=True)
+
+    assert 'starttime' in af_shpfile_filter.afdata
+    assert 'endtime' in af_shpfile_filter.afdata
+
+    assert str(af_shpfile_filter.afdata['starttime'][0]) == '2021-04-14 12:26:43.900000'
+    assert str(af_shpfile_filter.afdata['endtime'][0]) == '2021-04-14 12:28:08'
+
+
+@patch('socket.gethostname')
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
+def test_get_output_filepath_from_projname(setup_comm, gethostname,
+                                           fake_yamlconfig_file_post_processing):
+    """Test getting the correct output file path from the projection name."""
+    gethostname.return_value = "my.host.name"
+
+    myborders_file = "/my/shape/file/with/country/borders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
+
+    fake_metadata = {'platform': 'j01',
+                     'start_time': datetime(2021, 4, 14, 11, 26, 43, 900000),
+                     'end_hour': datetime(1900, 1, 1, 11, 28, 8, 400000),
+                     'orbit': '17637',
+                     'processing_time': datetime(2021, 4, 14, 11, 41, 30, 392094),
+                     'end_time': datetime(2021, 4, 14, 11, 28, 8)}
+
+    outpath = afpp.get_output_filepath_from_projname('default', fake_metadata)
+    assert outpath == '/path/where/the/filtered/results/will/be/stored/AFIMG_j01_d20210414_t112643.geojson'
+    outpath = afpp.get_output_filepath_from_projname('sweref99', fake_metadata)
+    assert outpath == '/path/where/the/filtered/results/will/be/stored/AFIMG_j01_d20210414_t112643_sweref99.geojson'
 
-    assert 'starttime' in this._afdata
-    assert 'endtime' in this._afdata
+    with pytest.raises(KeyError) as exec_info:
+        outpath = afpp.get_output_filepath_from_projname('some_other_projection_name', fake_metadata)
 
-    assert str(this._afdata['starttime'][0]) == '2021-04-14 12:26:43.900000'
-    assert str(this._afdata['endtime'][0]) == '2021-04-14 12:28:08'
+    expected = "'Projection name some_other_projection_name not supported in configuration!'"
+    assert str(exec_info.value) == expected
 
 
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-def test_regional_fires_filtering(setup_comm, get_config, gethostname):
+def test_regional_fires_filtering(setup_comm, gethostname,
+                                  fake_active_fires_file_data,
+                                  fake_yamlconfig_file_post_processing):
     """Test the regional fires filtering."""
-    # FIXME! This test is to big/broad. Need for refactoring!
+    # FIXME! This test is too big/broad. Need for refactoring!
+    open_fstream, _ = fake_active_fires_file_data
 
-    get_config.return_value = CONFIG_EXAMPLE
     gethostname.return_value = "my.host.name"
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
     afpp._initialize_fire_detection_id()
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    afdata = pd.read_csv(open_fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
 
     starttime = datetime.fromisoformat('2021-04-14 11:26:43.900')
     endtime = datetime.fromisoformat('2021-04-14 11:28:08')
 
     afdata['starttime'] = np.repeat(starttime, len(afdata)).astype(np.datetime64)
     afdata['endtime'] = np.repeat(endtime, len(afdata)).astype(np.datetime64)
 
@@ -272,60 +314,103 @@
     with patch('activefires_pp.post_processing.store_geojson') as store_geojson:
         with patch('activefires_pp.post_processing.ActiveFiresPostprocessing._generate_output_message') as generate_msg:
             generate_msg.return_value = "my fake output message"
             result = afpp.regional_fires_filtering_and_publishing(mymsg, regional_fmask, af_shapeff)
 
     store_geojson.assert_called_once()
     generate_msg.assert_called_once()
-
     assert len(result) == 1
     assert result[0] == "my fake output message"
 
 
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
 @patch('activefires_pp.post_processing.get_global_mask_from_shapefile', side_effect=[FAKE_MASK1, FAKE_MASK2])
-def test_general_national_fires_filtering(get_global_mask, setup_comm, get_config, gethostname):
+def test_general_national_fires_filtering(get_global_mask, setup_comm,
+                                          gethostname, fake_active_fires_file_data,
+                                          fake_yamlconfig_file_post_processing):
     """Test the general/basic national fires filtering."""
-    get_config.return_value = CONFIG_EXAMPLE
+    open_fstream, _ = fake_active_fires_file_data
     gethostname.return_value = "my.host.name"
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
-
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
+    afdata = pd.read_csv(open_fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
 
     # Add metadata to the pandas dataframe:
     fake_metadata = {'platform': 'j01',
                      'start_time': datetime(2021, 4, 14, 11, 26, 43, 900000),
                      'end_hour': datetime(1900, 1, 1, 11, 28, 8, 400000),
                      'orbit': '17637',
                      'processing_time': datetime(2021, 4, 14, 11, 41, 30, 392094),
                      'end_time': datetime(2021, 4, 14, 11, 28, 8)}
     afdata.attrs = fake_metadata
 
     af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name='NOAA-20')
-    afdata = af_shapeff.get_af_data(MY_FILE_PATTERN)
+    afdata = af_shapeff.get_af_data(AF_FILE_PATTERN)
 
     mymsg = "Fake message"
     result = afpp.fires_filtering(mymsg, af_shapeff)
 
     assert get_global_mask.call_count == 2
 
     assert isinstance(result, pd.core.frame.DataFrame)
     assert len(result) == 1
     np.testing.assert_almost_equal(result.iloc[0]['latitude'], 59.52483368)
     np.testing.assert_almost_equal(result.iloc[0]['longitude'], 17.1681633)
 
 
+@patch('socket.gethostname')
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
+@patch('activefires_pp.post_processing.get_global_mask_from_shapefile', side_effect=[FAKE_MASK11, FAKE_MASK12])
+def test_general_national_fires_filtering_spurious_detections(get_global_mask, setup_comm,
+                                                              gethostname, fake_active_fires_ascii_file5,
+                                                              fake_yamlconfig_file_post_processing,
+                                                              caplog):
+    """Test the general/basic national fires filtering - here with one spurious detection (caused by SEU onboard)."""
+    gethostname.return_value = "my.host.name"
+
+    myborders_file = "/my/shape/file/with/country/borders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=fake_active_fires_ascii_file5, timezone='GMT')
+    afdata = af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=False)
+    # Add metadata to the pandas dataframe:
+    fake_metadata = {'platform': 'j02',
+                     'start_time': datetime(2023, 12, 11, 1, 52, 44, 500000),
+                     'end_hour': datetime(1900, 1, 1, 1, 54, 7, 400000),
+                     'orbit': '5616',
+                     'processing_time': datetime(2023, 12, 11, 2, 7, 10, 860273),
+                     'end_time': datetime(2023, 12, 11, 1, 54, 7)}
+    afdata.attrs = fake_metadata
+
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
+
+    af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name='NOAA-21')
+    afdata = af_shapeff.get_af_data(AF_FILE_PATTERN)
+
+    mymsg = "Fake message"
+    with caplog.at_level(logging.INFO):
+        result = afpp.fires_filtering(mymsg, af_shapeff)
+
+    log_output1 = "Number of spurious detections filtered out = 1"
+    assert log_output1 in caplog.text
+
+    log_output2 = '(13.09044647,57.90747833): Tb4 = 324.07070923 FRP = 0.1102294'
+    assert log_output2 in caplog.text
+
+    assert len(result) == 1
+    np.testing.assert_almost_equal(result.iloc[0]['latitude'], 60.17847443)
+    np.testing.assert_almost_equal(result.iloc[0]['longitude'], -3.87098718)
+
+
 @pytest.mark.usefixtures("fake_national_borders_shapefile")
 @pytest.mark.usefixtures("fake_yamlconfig_file_post_processing")
 @patch('socket.gethostname')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
 def test_checking_national_borders_shapefile_file_exists(setup_comm, gethostname,
                                                          fake_yamlconfig_file_post_processing,
                                                          fake_national_borders_shapefile):
@@ -338,64 +423,60 @@
     afpp._check_borders_shapes_exists()
 
     assert afpp.shp_borders.name == 'some_national_borders_shape.yaml'
     assert afpp.shp_borders.is_file()
 
 
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
-def test_checking_national_borders_shapefile_file_nonexisting(setup_comm, get_config, gethostname):
+def test_checking_national_borders_shapefile_file_nonexisting(setup_comm, gethostname,
+                                                              fake_yamlconfig_file_post_processing):
     """Test the checking of the national borders shapefile - borders shapefile does not exist."""
-    get_config.return_value = CONFIG_EXAMPLE
     gethostname.return_value = "my.host.name"
 
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
     with pytest.raises(OSError) as exec_info:
         afpp._check_borders_shapes_exists()
 
     expected = "Shape file does not exist! Filename = /my/shape/file/with/country/borders"
     assert str(exec_info.value) == expected
 
 
 @freeze_time('2023-06-16 11:24:00')
 @patch('socket.gethostname')
-@patch('activefires_pp.post_processing.read_config')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
 @patch('activefires_pp.post_processing._read_data')
-def test_get_feature_collection_from_firedata(readdata, setup_comm,
-                                              get_config, gethostname):
+def test_get_feature_collection_from_firedata_with_detection_id(readdata, setup_comm, gethostname,
+                                                                fake_yamlconfig_file_post_processing):
     """Test get the Geojson Feature Collection from fire detection."""
-    get_config.return_value = CONFIG_EXAMPLE
     gethostname.return_value = "my.host.name"
-
-    myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
-    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
     afpp._initialize_fire_detection_id()
 
     myfilepath = TEST_ACTIVE_FIRES_FILEPATH2
 
     fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA2)
     afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
     readdata.return_value = afdata
 
-    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
-        afdata = this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
+        afdata = af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=False)
 
+    afdata = afdata[2::]  # Reduce to only contain the last detections!
     afdata = afpp.add_unique_day_id(afdata)
-
     result = geojson_feature_collection_from_detections(afdata, platform_name='Suomi-NPP')
 
     # NB! The time of the afdata is here still in UTC!
     expected = FeatureCollection([{"geometry": {"coordinates": [17.259052, 62.658012],
                                                 "type": "Point"},
                                    "properties": {"confidence": 8,
                                                   "observation_time": "2023-06-16T11:10:47.200000",
@@ -428,7 +509,84 @@
                                                   "platform_name": "Suomi-NPP",
                                                   "id": '20230616-4',
                                                   "power": 20.5928936,
                                                   "tb": 348.72860718},
                                    "type": "Feature"}])
 
     TestCase().assertDictEqual(result, expected)
+
+
+@patch('socket.gethostname')
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
+@patch('activefires_pp.post_processing._read_data')
+def test_get_feature_collection_from_firedata_tb_celcius(readdata, setup_comm, gethostname,
+                                                         fake_yamlconfig_file_post_processing):
+    """Test get the Geojson Feature Collection from fire detection."""
+    gethostname.return_value = "my.host.name"
+    myborders_file = "/my/shape/file/with/country/borders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+
+    afpp = ActiveFiresPostprocessing(fake_yamlconfig_file_post_processing,
+                                     myborders_file, mymask_file)
+    afpp._initialize_fire_detection_id()
+
+    units = {'temperature': 'degC'}
+    afpp.unit_converter = UnitConverter(units)
+
+    myfilepath = TEST_ACTIVE_FIRES_FILEPATH2
+    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA2)
+
+    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    readdata.return_value = afdata
+
+    af_shpfile_filter = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
+    with patch('os.path.exists') as mypatch:
+        mypatch.return_value = True
+        afdata = af_shpfile_filter.get_af_data(filepattern=AF_FILE_PATTERN, localtime=False)
+
+    afdata = afdata[2::]  # Reduce to only contain the last detections!
+
+    afdata = afpp.add_tb_celcius(afdata)
+    result = geojson_feature_collection_from_detections(afdata, platform_name='Suomi-NPP')
+
+    # NB! The time of the afdata is here still in UTC!
+    expected = FeatureCollection([{"geometry": {"coordinates": [17.259052, 62.658012],
+                                                "type": "Point"},
+                                   "properties": {
+                                       "confidence": 8,
+                                       "observation_time": "2023-06-16T11:10:47.200000",
+                                       "platform_name": "Suomi-NPP",
+                                       "power": 2.51202917,
+                                       "tb": 339.66326904,
+                                       "tb_celcius": 66.51326904000001},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [17.42075, 64.216942],
+                                                "type": "Point"},
+                                   "properties": {
+                                       "confidence": 8,
+                                       "observation_time": "2023-06-16T11:10:47.200000",
+                                       "platform_name": "Suomi-NPP",
+                                       "power": 3.39806151,
+                                       "tb": 329.65161133,
+                                       "tb_celcius": 56.50161133},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [16.600952, 64.569046],
+                                                "type": "Point"},
+                                   "properties": {
+                                       "confidence": 8,
+                                       "observation_time": "2023-06-16T11:10:47.200000",
+                                       "platform_name": "Suomi-NPP",
+                                       "power": 20.5928936,
+                                       "tb": 346.52050781,
+                                       "tb_celcius": 73.37050781000005},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [16.5984, 64.572227],
+                                                "type": "Point"},
+                                   "properties": {"confidence": 8,
+                                                  "observation_time": "2023-06-16T11:10:47.200000",
+                                                  "platform_name": "Suomi-NPP",
+                                                  "power": 20.5928936,
+                                                  "tb": 348.72860718,
+                                                  "tb_celcius": 75.57860718},
+                                   "type": "Feature"}])
+
+    TestCase().assertDictEqual(result, expected)
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_shapefile_geometries.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_shapefile_geometries.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2022 Adam Dybbroe
+# Copyright (c) 2022, 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -26,14 +26,15 @@
 from unittest.mock import patch
 import pathlib
 import json
 import logging
 
 from activefires_pp.geojson_utils import read_geojson_data
 from activefires_pp.spatiotemporal_alarm_filtering import create_alarms_from_fire_detections
+from activefires_pp.spatiotemporal_alarm_filtering import get_distance_between_two_points
 from activefires_pp.spatiotemporal_alarm_filtering import join_fire_detections
 from activefires_pp.spatiotemporal_alarm_filtering import split_large_fire_clusters
 from activefires_pp.spatiotemporal_alarm_filtering import create_one_detection_from_collection
 from activefires_pp.spatiotemporal_alarm_filtering import create_single_point_alarms_from_collections
 from activefires_pp.spatiotemporal_alarm_filtering import AlarmFilterRunner
 from activefires_pp.spatiotemporal_alarm_filtering import get_xauthentication_filepath_from_environment
 
@@ -148,21 +149,14 @@
 # AFIMG_NOAA-20_20210618_124819_sweden.geojson
 TEST_MONSTERAS_PREVIOUS2_COLLECTION = """{"type": "FeatureCollection", "features":
 [{"type": "Feature", "geometry": {"type": "Point", "coordinates": [16.252192, 57.15242]},
 "properties": {"power": 2.87395763, "tb": 330.10293579, "confidence": 8,
 "observation_time": "2021-06-18T14:49:01.750000+02:00", "platform_name": "NOAA-20"}}]}"""
 
 
-CONFIG_EXAMPLE = {'subscribe_topics': '/VIIRS/L2/Fires/PP/National',
-                  'publish_topic': '/VIIRS/L2/Fires/PP/SOSAlarm',
-                  'geojson_file_pattern_alarms': 'sos_{start_time:%Y%m%d_%H%M%S}_{id:d}.geojson',
-                  'fire_alarms_dir': '/path/where/the/filtered/alarms/will/be/stored',
-                  'restapi_url': 'https://xxx.smhi.se:xxxx'}
-
-
 def test_join_fire_detections_large_fire(fake_geojson_file_many_detections):
     """Test create alarm from set of fire detections."""
     ffdata = read_geojson_data(fake_geojson_file_many_detections)
 
     joined_detections = join_fire_detections(ffdata)
 
     for key in joined_detections.keys():
@@ -379,14 +373,15 @@
     assert alarm_runner.listener is None
     assert alarm_runner.publisher is None
     assert alarm_runner.loop is False
     assert alarm_runner.sos_alarms_file_pattern == 'sos_{start_time:%Y%m%d_%H%M%S}_{id:d}.geojson'
     assert alarm_runner.restapi_url == 'https://xxx.smhi.se:xxxx'
     assert alarm_runner.options == {'subscribe_topics': ['/VIIRS/L2/Fires/PP/National'],
                                     'publish_topic': '/VIIRS/L2/Fires/PP/SOSAlarm',
+                                    'products': ['afimg'],
                                     'geojson_file_pattern_alarms': 'sos_{start_time:%Y%m%d_%H%M%S}_{id:d}.geojson',
                                     'fire_alarms_dir': '/path/where/the/filtered/alarms/will/be/stored',
                                     'restapi_url': 'https://xxx.smhi.se:xxxx',
                                     'time_and_space_thresholds': {'hour_threshold': 6,
                                                                   'long_fires_threshold_km': 1.2,
                                                                   'spatial_threshold_km': 0.8}}
 
@@ -510,7 +505,37 @@
     alarm_runner._log_message_per_threshold = {thr_type:
                                                ('okay message - hours: %3.1f', 'error message - hours'), }
     with pytest.raises(OSError) as exec_info:
         alarm_runner._check_and_set_threshold(thr_type, config)
 
     expected = alarm_runner._log_message_per_threshold[thr_type][1]
     assert str(exec_info.value) == expected
+
+# @pytest.mark.parametrize()
+
+
+@pytest.mark.parametrize("lonlats, expected",
+                         [((12.5, 62.5),
+                           135.02288790715303),
+                          ((13.5, 68.5),
+                           542.596822830585),
+                          ]
+                         )
+def test_get_distance_between_two_points_input_okay(lonlats, expected):
+    """Test the derivation of distance between two lon,lat points."""
+    point1 = (13.438972, 63.634071)
+    point2 = lonlats[0], lonlats[1]
+
+    dist_km = get_distance_between_two_points(point1, point2)
+    assert dist_km == pytest.approx(expected)
+
+
+def test_get_distance_between_two_points_input_invalid():
+    """Test the derivation of distance between two lon,lat points."""
+    point1 = (13.438972, 63.634071)
+    point2 = (386845.899472, 6420007.169359)
+
+    with pytest.raises(ValueError) as exec_info:
+        _ = get_distance_between_two_points(point1, point2)
+
+    expected = "Latitude must be in the [-90; 90] range."
+    assert str(exec_info.value) in expected
```

### Comparing `activefires-pp-0.1.9/activefires_pp/tests/test_utils.py` & `activefires_pp-0.2.0/activefires_pp/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022, 2023 Adam.Dybbroe
+# Copyright (c) 2021, 2022, 2023, 2024 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam.Dybbroe <a000680@c21856.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -30,14 +30,18 @@
 from activefires_pp.utils import get_filename_from_posttroll_message
 from activefires_pp.utils import datetime_utc2local
 from activefires_pp.utils import json_serial
 
 NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
 
+AF_FILE_PATTERN = ("AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}_" +
+                   "b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt")
+
+
 def test_json_serial():
     """Test the json_serial function."""
     dtime_obj = datetime(2021, 4, 7, 11, 58, 53, 200000)
     res = json_serial(dtime_obj)
 
     assert res == "2021-04-07T11:58:53.200000"
```

### Comparing `activefires-pp-0.1.9/activefires_pp.egg-info/PKG-INFO` & `activefires_pp-0.2.0/activefires_pp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activefires-pp
-Version: 0.1.9
+Version: 0.2.0
 Summary: Post-processing of and notifications on Satellite active fire detections
 Home-page: https://github.com/adybbroe/activefires-pp
 Author: Adam Dybroe
 Author-email: adam.dybroe@smhi.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `activefires-pp-0.1.9/activefires_pp.egg-info/SOURCES.txt` & `activefires_pp-0.2.0/activefires_pp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 activefires_pp/api_posting.py
 activefires_pp/config.py
 activefires_pp/fire_notifications.py
 activefires_pp/geojson_utils.py
 activefires_pp/geometries_from_shapefiles.py
 activefires_pp/logger.py
 activefires_pp/post_processing.py
+activefires_pp/sanity_check_detections.py
 activefires_pp/spatiotemporal_alarm_filtering.py
 activefires_pp/utils.py
 activefires_pp.egg-info/PKG-INFO
 activefires_pp.egg-info/SOURCES.txt
 activefires_pp.egg-info/dependency_links.txt
 activefires_pp.egg-info/not-zip-safe
 activefires_pp.egg-info/requires.txt
```

### Comparing `activefires-pp-0.1.9/bin/active_fires_notifier.py` & `activefires_pp-0.2.0/bin/active_fires_notifier.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/bin/active_fires_postprocessing.py` & `activefires_pp-0.2.0/bin/active_fires_postprocessing.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/bin/active_fires_spatiotemporal_alarm_filtering.py` & `activefires_pp-0.2.0/bin/active_fires_spatiotemporal_alarm_filtering.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/examples/fire_notifier.yaml` & `activefires_pp-0.2.0/examples/fire_notifier.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Publish/subscribe
 publish_topic: VIIRS/L2/MSB/National
 subscribe_topics: VIIRS/L2/Fires/PP/National
 
+products:
+  - afimg
+  - afimg_some_other_geoid
+
 smtp_server: smtp.mydomain.se
 
 domain: mydomain.se
 
 sender: active-fires@mydomain.se
 
 recipients: ["recipient1@recipients.se", "recipient2@recipients.se", "recipient3@recipients.se"]
```

### Comparing `activefires-pp-0.1.9/examples/fire_notifier_regional.yaml` & `activefires_pp-0.2.0/examples/fire_notifier_regional.yaml`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/examples/log_config.yaml` & `activefires_pp-0.2.0/examples/log_config.yaml`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.9/setup.py` & `activefires_pp-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam Dybbroe
+# Copyright (c) 2021, 2022, 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -36,20 +36,20 @@
 with open('./README.md', 'r') as fd:
     long_description = fd.read()
 
 description = 'Post-processing of and notifications on Satellite active fire detections'
 
 requires = ['posttroll', 'netifaces', 'trollsift', 'setuptools_scm', 'pycrs',
             'shapely', 'cartopy', 'pandas', 'geojson', 'fiona', 'geopy', 'matplotlib',
-            'requests']
+            'requests', 'pint']
 test_requires = ['mock', 'posttroll', 'trollsift', 'pycrs',
                  'shapely', 'cartopy', 'pandas', 'geojson', 'fiona',
                  'freezegun', 'responses']
 
-setup(name="activefires-pp",
+setup(name="activefires_pp",
       description=description,
       author='Adam Dybroe',
       author_email='adam.dybroe@smhi.se',
       classifiers=["Development Status :: 3 - Alpha",
                    "Intended Audience :: Science/Research",
                    "License :: OSI Approved :: GNU General Public License v3 " +
                    "or later (GPLv3+)",
```

