# Comparing `tmp/duckietown-messages-0.0.7.tar.gz` & `tmp/duckietown-messages-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-messages-0.0.7.tar", last modified: Tue Mar 19 03:58:20 2024, max compression
+gzip compressed data, was "duckietown-messages-0.0.8.tar", last modified: Wed Mar 20 06:19:09 2024, max compression
```

## Comparing `duckietown-messages-0.0.7.tar` & `duckietown-messages-0.0.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      491 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2188 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.857300 duckietown-messages-0.0.7/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.861300 duckietown-messages-0.0.7/src/duckietown_messages/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-19 03:58:14.000000 duckietown-messages-0.0.7/src/duckietown_messages/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.861300 duckietown-messages-0.0.7/src/duckietown_messages/actuators/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/actuators/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      274 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/actuators/car_lights.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      312 2024-03-06 22:25:40.000000 duckietown-messages-0.0.7/src/duckietown_messages/actuators/differential_pwm.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1039 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/actuators/display_fragment.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      334 2024-03-06 22:27:23.000000 duckietown-messages-0.0.7/src/duckietown_messages/actuators/display_fragments.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      691 2024-03-19 03:57:52.000000 duckietown-messages-0.0.7/src/duckietown_messages/base.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.861300 duckietown-messages-0.0.7/src/duckietown_messages/colors/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/colors/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      842 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/colors/rgb.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      946 2024-03-19 03:57:52.000000 duckietown-messages-0.0.7/src/duckietown_messages/colors/rgba.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.861300 duckietown-messages-0.0.7/src/duckietown_messages/geometry_2d/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_2d/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      155 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_2d/point.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      405 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_2d/roi.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.861300 duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      432 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/position.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      476 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/quaternion.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      814 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/transformation.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/sensors/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      237 2024-03-06 22:27:23.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/angular_velocities.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      326 2024-03-06 22:27:37.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/button_event.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      297 2024-03-17 16:34:10.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/camera.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1190 2024-03-06 22:29:07.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/compressed_image.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5647 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/image.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      238 2024-03-06 22:32:42.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/linear_accelerations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      252 2024-03-18 03:54:34.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/range.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      394 2024-03-06 22:33:40.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/range_finder.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      209 2024-03-06 22:33:55.000000 duckietown-messages-0.0.7/src/duckietown_messages/sensors/temperature.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/simulation/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/simulation/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/simulation/hil/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/simulation/hil/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      361 2024-03-18 03:54:39.000000 duckietown-messages-0.0.7/src/duckietown_messages/simulation/hil/connection_configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/standard/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      182 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/boolean.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      185 2024-03-17 23:04:47.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/dictionary.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      421 2024-03-06 22:24:28.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/header.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      181 2024-03-09 06:11:22.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/integer.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2024-03-17 23:05:05.000000 duckietown-messages-0.0.7/src/duckietown_messages/standard/list.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      224 2024-03-19 03:57:52.000000 duckietown-messages-0.0.7/src/duckietown_messages/utils/exceptions.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages/utils/image/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/utils/image/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2455 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/utils/image/jpeg.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      202 2024-03-06 20:49:36.000000 duckietown-messages-0.0.7/src/duckietown_messages/utils/image/pil.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-19 03:58:20.865301 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      491 2024-03-19 03:58:20.000000 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2146 2024-03-19 03:58:20.000000 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-19 03:58:20.000000 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       48 2024-03-19 03:58:20.000000 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       46 2024-03-19 03:58:20.000000 duckietown-messages-0.0.7/src/duckietown_messages.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      491 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2188 2024-03-07 05:01:51.000000 duckietown-messages-0.0.8/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.479725 duckietown-messages-0.0.8/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.479725 duckietown-messages-0.0.8/src/duckietown_messages/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-20 06:19:04.000000 duckietown-messages-0.0.8/src/duckietown_messages/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.483725 duckietown-messages-0.0.8/src/duckietown_messages/actuators/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/actuators/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      274 2024-03-06 23:40:02.000000 duckietown-messages-0.0.8/src/duckietown_messages/actuators/car_lights.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      312 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/actuators/differential_pwm.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1039 2024-03-07 00:14:09.000000 duckietown-messages-0.0.8/src/duckietown_messages/actuators/display_fragment.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      334 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/actuators/display_fragments.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      691 2024-03-19 03:49:56.000000 duckietown-messages-0.0.8/src/duckietown_messages/base.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.483725 duckietown-messages-0.0.8/src/duckietown_messages/colors/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 23:34:41.000000 duckietown-messages-0.0.8/src/duckietown_messages/colors/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      842 2024-03-06 23:57:56.000000 duckietown-messages-0.0.8/src/duckietown_messages/colors/rgb.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      946 2024-03-18 21:56:45.000000 duckietown-messages-0.0.8/src/duckietown_messages/colors/rgba.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.483725 duckietown-messages-0.0.8/src/duckietown_messages/geometry_2d/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:56:45.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_2d/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      155 2024-03-06 23:11:47.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_2d/point.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      405 2024-03-06 23:11:46.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_2d/roi.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.483725 duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:57:02.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      432 2024-03-06 23:11:59.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/position.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      476 2024-03-06 23:11:59.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/quaternion.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      814 2024-03-06 23:31:05.000000 duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/transformation.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.483725 duckietown-messages-0.0.8/src/duckietown_messages/sensors/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      237 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/angular_velocities.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      326 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/button_event.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      297 2024-03-13 22:17:31.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/camera.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1190 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/compressed_image.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5775 2024-03-20 04:38:02.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/image.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      238 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/linear_accelerations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      252 2024-03-18 19:19:31.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/range.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      394 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/range_finder.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      209 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/sensors/temperature.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages/simulation/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/simulation/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages/simulation/hil/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/simulation/hil/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      361 2024-03-18 19:19:31.000000 duckietown-messages-0.0.8/src/duckietown_messages/simulation/hil/connection_configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages/standard/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      182 2024-03-06 23:26:24.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/boolean.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      185 2024-03-17 23:05:54.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/dictionary.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      421 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/header.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      181 2024-03-06 23:29:16.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/integer.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2024-03-17 23:05:54.000000 duckietown-messages-0.0.8/src/duckietown_messages/standard/list.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      224 2024-03-19 03:50:19.000000 duckietown-messages-0.0.8/src/duckietown_messages/utils/exceptions.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages/utils/image/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/utils/image/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2455 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/utils/image/jpeg.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      202 2024-03-06 22:39:51.000000 duckietown-messages-0.0.8/src/duckietown_messages/utils/image/pil.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 06:19:09.487725 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      491 2024-03-20 06:19:09.000000 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2146 2024-03-20 06:19:09.000000 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-20 06:19:09.000000 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       48 2024-03-20 06:19:09.000000 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       46 2024-03-20 06:19:09.000000 duckietown-messages-0.0.8/src/duckietown_messages.egg-info/top_level.txt
```

### Comparing `duckietown-messages-0.0.7/setup.py` & `duckietown-messages-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/actuators/display_fragment.py` & `duckietown-messages-0.0.8/src/duckietown_messages/actuators/display_fragment.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/base.py` & `duckietown-messages-0.0.8/src/duckietown_messages/base.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/colors/rgb.py` & `duckietown-messages-0.0.8/src/duckietown_messages/colors/rgb.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/colors/rgba.py` & `duckietown-messages-0.0.8/src/duckietown_messages/colors/rgba.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/geometry_3d/transformation.py` & `duckietown-messages-0.0.8/src/duckietown_messages/geometry_3d/transformation.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/sensors/compressed_image.py` & `duckietown-messages-0.0.8/src/duckietown_messages/sensors/compressed_image.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/sensors/image.py` & `duckietown-messages-0.0.8/src/duckietown_messages/sensors/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         encoder: ImageEncoding = SUPPORTED_ENCODINGS[encoding]
         h, w, c, *_ = im.shape + (1,)
         msg = Image(
             header=header or Header(),
             width=w,
             height=h,
             encoding=encoding,
-            step=w * c * encoder.channel_size_bits,
+            step=w * c * int(encoder.channel_size_bits / 8),
             data=encoder.pack(im).tobytes(),
             # TODO: this always True?
             is_bigendian=False
         )
         # ---
         return msg
 
@@ -125,17 +125,18 @@
         if self.encoding not in SUPPORTED_ENCODINGS:
             raise ValueError(f"Image encoding '{self.encoding}' not supported.")
         encoder: ImageEncoding = SUPPORTED_ENCODINGS[self.encoding]
         # get image shape
         if self.encoding == "mono1":
             w, h, c = (self.width, self.height, 1)
         else:
-            w, h, c = (self.width, self.height, int(self.step / (self.width * encoder.channel_size_bits)))
+            w, h, c = (self.width, self.height, int(self.step / (self.width * (encoder.channel_size_bits / 8))))
         # validate number of channel
-        assert c == encoder.num_channels
+        assert c == encoder.num_channels, "Number of channels does not match the encoding. Expected %d, got %d." % (
+            encoder.num_channels, c)
         # turn bytes into array
         im = np.frombuffer(self.data, dtype=np.uint8)
         # unpack data
         im = encoder.unpack(im)
         # shape array
         im = im.reshape((h, w, c)) if c > 1 else im.reshape((h, w))
         # reorder channels
```

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages/utils/image/jpeg.py` & `duckietown-messages-0.0.8/src/duckietown_messages/utils/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `duckietown-messages-0.0.7/src/duckietown_messages.egg-info/SOURCES.txt` & `duckietown-messages-0.0.8/src/duckietown_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

