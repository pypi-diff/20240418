# Comparing `tmp/meili-sdk-0.6.7.tar.gz` & `tmp/meili-sdk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.6.7.tar", last modified: Fri Mar 22 14:13:40 2024, max compression
+gzip compressed data, was "meili-sdk-0.6.8.tar", last modified: Thu Apr 18 10:46:49 2024, max compression
```

## Comparing `meili-sdk-0.6.7.tar` & `meili-sdk-0.6.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.771772 meili-sdk-0.6.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5025 2024-03-22 14:13:40.771772 meili-sdk-0.6.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.758772 meili-sdk-0.6.7/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.760773 meili-sdk-0.6.7/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.761772 meili-sdk-0.6.7/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.763773 meili-sdk-0.6.7/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.764773 meili-sdk-0.6.7/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8603 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.764773 meili-sdk-0.6.7/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.767773 meili-sdk-0.6.7/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/maps.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.767773 meili-sdk-0.6.7/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.768772 meili-sdk-0.6.7/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18314 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.771772 meili-sdk-0.6.7/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/action_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/cancel_task_message.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7135 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/path.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/preset.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/station.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/task_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/traffic_control_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/update_map_message.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/meili_sdk/websockets/models/vehicle_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 14:13:40.759773 meili-sdk-0.6.7/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5025 2024-03-22 14:13:40.000000 meili-sdk-0.6.7/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2285 2024-03-22 14:13:40.000000 meili-sdk-0.6.7/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 14:13:40.000000 meili-sdk-0.6.7/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-22 14:13:40.000000 meili-sdk-0.6.7/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-22 14:13:40.000000 meili-sdk-0.6.7/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-03-22 14:13:40.771772 meili-sdk-0.6.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-22 14:13:31.000000 meili-sdk-0.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.169485 meili-sdk-0.6.8/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.171485 meili-sdk-0.6.8/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.171485 meili-sdk-0.6.8/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.173485 meili-sdk-0.6.8/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.174485 meili-sdk-0.6.8/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.174485 meili-sdk-0.6.8/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.176484 meili-sdk-0.6.8/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.177485 meili-sdk-0.6.8/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.177485 meili-sdk-0.6.8/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19393 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/action_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/preset.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/station.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/update_map_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/vehicle_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.170485 meili-sdk-0.6.8/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-18 10:46:49.181484 meili-sdk-0.6.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/setup.py
```

### Comparing `meili-sdk-0.6.7/LICENSE.txt` & `meili-sdk-0.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/PKG-INFO` & `meili-sdk-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.7
+Version: 0.6.8
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.7/README.md` & `meili-sdk-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/clients/__init__.py` & `meili-sdk-0.6.8/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.6.8/meili_sdk/clients/apitoken_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/clients/base.py` & `meili-sdk-0.6.8/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.6.8/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/exceptions.py` & `meili-sdk-0.6.8/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/base.py` & `meili-sdk-0.6.8/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/form.py` & `meili-sdk-0.6.8/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/task.py` & `meili-sdk-0.6.8/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/team.py` & `meili-sdk-0.6.8/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/trigger.py` & `meili-sdk-0.6.8/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/models/vehicle.py` & `meili-sdk-0.6.8/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/client.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         resource = client.get_ros_resources()
         token = resource.get_token(setup_uuid)
         _, setup, _, _ = resource.get_ros_setup(setup_uuid)
         return cls(
             client_id=setup.mqtt_id, token=token, setup_uuid=setup_uuid, *args, *kwargs
         )
 
-    def subscribe_default_topics(self, vehicle_serial_number, manufacturer="meili"):
+    def subscribe_default_topics(self, vehicle_serial_number, manufacturer = "meili"):
         self.subscribe_to_orders(vehicle_serial_number, manufacturer=manufacturer)
         self.subscribe_to_actions(vehicle_serial_number, manufacturer=manufacturer)
 
     def run(self, block=False):
         try:
             self.connection_state = MqttConnectionStatus.CONNECTING
             self.client.connect(
@@ -135,21 +135,15 @@
             try:
                 message = json.dumps(message)
             except (TypeError, ValueError):
                 message = str(message)
 
         self.client.publish(topic=topic, payload=message, qos=qos)
 
-    def publish_to_state_topic(
-        self,
-        vehicle_serial_number: str,
-        message: any,
-        manufacturer: str = "meili",
-        qos=0,
-    ):
+    def publish_to_state_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/state"
         return self.publish(topic, message, qos)
 
     def wait_for_connection(self, timeout=10):
         """
         Block execution until connection is established
 
@@ -169,23 +163,19 @@
             and (datetime.now() - start_time).seconds < timeout
         ):
             continue
 
         if self.connection_state != MqttConnectionStatus.CONNECTED:
             raise TimeoutError("Timed out")
 
-    def subscribe_to_actions(
-        self, vehicle_serial_number: str, manufacturer: str = "meili"
-    ):
-        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/instantactions"
+    def subscribe_to_actions(self, vehicle_serial_number: str, manufacturer: str = "meili"):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/instantActions"
         return self.subscribe(topic)
 
-    def subscribe_to_orders(
-        self, vehicle_serial_number: str, manufacturer: str = "meili"
-    ):
+    def subscribe_to_orders(self, vehicle_serial_number: str, manufacturer: str = "meili"):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/order"
         return self.subscribe(topic)
 
     def __check_connection(self, custom_message=None):
         if not self.client.is_connected():
             raise ConnectionError(custom_message or "Connection is closed")
```

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/models/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
     def validate_theta(self):
         if self.theta < 0 or self.theta > 360:
             raise ValidationError("Theta must be between 0 and 360 degrees")
 
 
 class VDA5050NodePosition(BaseModel):
-    X: float
-    Y: float
-    Theta: float
+    x: float
+    y: float
+    theta: float
 
     def validate_theta(self):
         if self.theta < 0 or self.theta > 360:
             raise ValidationError("Theta must be between 0 and 360 degrees")
 
 
 class VDA5050VehicleBatteryState(BaseModel):
@@ -64,14 +64,53 @@
         kwargs.setdefault("released", False)
         node_position = kwargs.pop("nodePosition")
         if not isinstance(node_position, VDA5050NodePosition):
             node_position = VDA5050NodePosition(**node_position)
         kwargs["nodePosition"] = node_position
         super().__init__(**kwargs)
 
+class VDA5050ActionState(BaseModel):
+    actionId: str
+    actionStatus: str
+    actionDescription: t.Optional[str] = None
+    resultDescription: t.Optional[str] = None
+
+    def validate_actionStatus(self):
+        if self.actionID not in ["WAITING", "INITIALIZING", 
+                                 "RUNNING", "FINISHED", "FAILED"
+                                 ]:
+            raise ValidationError("""actionStatus must be one of the following: [
+                            "WAITING",
+                            "INITIALIZING",
+                            "RUNNING",
+                            "FINISHED",
+                            "FAILED"
+                        ]""")
+        
+class VDA5050ErrorReference(BaseModel):
+    referenceKey: str
+    referenceValue: str
+
+
+class VDA5050Error(BaseModel):
+    errorType: str
+    errorLevel: str
+    errorReferences: t.Optional[t.List[VDA5050ErrorReference]] = None
+    errorDescription: t.Optional[str] = None
+
+    def validatea_errorLevel(self):
+        if self.errorLevel not in ["WARNING", "FATAL"]:
+            raise ValidationError("""errorLevel must be one of "WARNING" or "FATAL" """)
+        
+class VDA5050Velocity(BaseModel):
+    vx: float
+    vy: float
+    omega: float
+
+
 
 class VDA5050StateMessage(BaseModel):
     """
     Message to be sent to FMS MQTT Broker
 
     When initializing the message, headerId and timestamp will be automatically generated
     """
@@ -79,21 +118,25 @@
     headerId: int
     timestamp: datetime
     version: str
     manufacturer: str
     serialNumber: str
     orderId: t.Optional[str] = None
     lastNodeId: t.Optional[str] = None
+    lastNodeSequenceId: t.Optional[int] = None
     driving: bool
     paused: bool
     newBaseRequested: bool
     nodeStates: t.Optional[t.List[VDA5050NodeState]] = None
     agvPosition: t.Optional[VDA5050VehiclePosition] = None
     batteryState: t.Optional[VDA5050VehicleBatteryState] = None
     operatingMode: str
+    velocity: t.Optional[VDA5050Velocity] = None
+    actionStates: t.Optional[t.List[VDA5050ActionState]] = None
+    errors: t.Optional[t.List[VDA5050Error]] = None
 
     def __init__(self, **kwargs):
         global CURRENT_HEADER_ID
         CURRENT_HEADER_ID += 1
 
         kwargs.setdefault("headerId", CURRENT_HEADER_ID)
         kwargs.setdefault("timestamp", datetime.now())
```

### Comparing `meili-sdk-0.6.7/meili_sdk/mqtt/site.py` & `meili-sdk-0.6.8/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/base.py` & `meili-sdk-0.6.8/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/forms.py` & `meili-sdk-0.6.8/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/organizations.py` & `meili-sdk-0.6.8/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/tasks.py` & `meili-sdk-0.6.8/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/teams.py` & `meili-sdk-0.6.8/meili_sdk/resources/teams.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/triggers.py` & `meili-sdk-0.6.8/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/resources/vehicles.py` & `meili-sdk-0.6.8/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/schedules/loader.py` & `meili-sdk-0.6.8/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/schedules/models.py` & `meili-sdk-0.6.8/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/site.py` & `meili-sdk-0.6.8/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/client.py` & `meili-sdk-0.6.8/meili_sdk/websockets/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 from meili_sdk.websockets.models.update_map_message import (
     ConfirmMapMessage,
     UpdateMapMessage,
 )
 from meili_sdk.websockets.models.vehicle_settings import VehicleSettingsMessage
 
+
 logger = logging.getLogger("meili_sdk")
 
 __all__ = ("MeiliWebsocketClient",)
 
 
 class MeiliWebsocketClient:
     """
@@ -80,14 +81,15 @@
             fake_opened_connection: t.Optional[bool] = False,
             message_error_handler: t.Optional[t.Callable] = None,
             update_map_handler: t.Optional[t.Callable] = None,
             vehicle_initial_position_handler: t.Optional[t.Callable] = None,
             update_vehicle_settings: t.Optional[t.Callable] = None,
             pause_task_handler: t.Optional[t.Callable] = None,
             resume_task_handler: t.Optional[t.Callable] = None,
+            remove_vehicle_from_fleet_handler: t.Optional[t.Callable] = None,
     ) -> None:
         self.token = token
         self.__connection_is_open = fake_opened_connection
         self.__fleet = fleet
 
         host = override_host or get_host()
         self.url = BaseResource.build_url(
@@ -112,14 +114,15 @@
         self.__message_error_handler = message_error_handler
         self.__update_map_handler = update_map_handler
         self.__update_vehicle_settings = update_vehicle_settings
         self.__pause_task_handler = pause_task_handler
         self.__resume_task_handler = resume_task_handler
         self.__connection = None
         self.__vehicle_initial_position_handler = vehicle_initial_position_handler
+        self.__remove_vehicle_from_fleet_handler = remove_vehicle_from_fleet_handler
 
     def get_headers(self) -> dict:
         return {
             "x-meili-app-name": "sdk",
             "x-meili-app-version": VERSION,
             "x-meili-fleet-token": self.token,
         }
@@ -388,20 +391,37 @@
 
         if self.__topic_list_initializer_handler and callable(
             self.__topic_list_initializer_handler
         ):
             self.__topic_list_initializer_handler(topics, message, vehicle)
 
     def process_message_error(self, message: dict):
+        
+        # Handle vehicle removal from fleet
+        if message["errors"] and message["errors"]["vehicle"][0]:
+            pattern = r"^Vehicle with UUID ([0-9a-fA-F]{32}) does not exist, or was removed from the fleet setup$"
+            match = re.search(pattern, message["errors"]["vehicle"][0])
+            logger.warning(f"{message['errors']['vehicle'][0]}")
+            if match:
+                logger.warning("Vehicle removal from fleet detected.")
+                vehicle_to_remove_uuid = match.group(1) # Get the UUID from the error message 
+                self.process_remove_vehicle_from_fleet(vehicle_to_remove_uuid)
+                return
+        
         logger.warning(
             f"Validation failed for message with the following errors: {message}"
         )
+
         if self.__message_error_handler:
             self.__message_error_handler(message["errors"])
 
+    def process_remove_vehicle_from_fleet(self, vehicle_uuid: str):
+        if self.__remove_vehicle_from_fleet_handler and callable(self.__remove_vehicle_from_fleet_handler):
+            self.__remove_vehicle_from_fleet_handler(vehicle_uuid)
+
     def _get_registration_message(self):
         return Message(
             event=constants.EVENT_REGISTER,
             vehicles=self._get_registration_vehicles(),
         )
 
     def _get_registration_vehicles(self):
```

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/constants.py` & `meili-sdk-0.6.8/meili_sdk/websockets/constants.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/__init__.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/message.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/task.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/task_v2.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/task_v2.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk/websockets/models/update_map_message.py` & `meili-sdk-0.6.8/meili_sdk/websockets/models/update_map_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.6.8/meili_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.7
+Version: 0.6.8
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.7/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.6.8/meili_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.7/setup.cfg` & `meili-sdk-0.6.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.6.7
+version = 0.6.8
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Meili Robots
 author_email = info@meilirobots.com
```
