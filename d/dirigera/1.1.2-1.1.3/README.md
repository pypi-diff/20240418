# Comparing `tmp/dirigera-1.1.2.tar.gz` & `tmp/dirigera-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.1.2.tar", last modified: Tue Apr 16 06:56:45 2024, max compression
+gzip compressed data, was "dirigera-1.1.3.tar", last modified: Thu Apr 18 18:13:01 2024, max compression
```

## Comparing `dirigera-1.1.2.tar` & `dirigera-1.1.3.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 06:56:38.000000 dirigera-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-16 06:56:45.672232 dirigera-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-16 06:56:38.000000 dirigera-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-16 06:56:38.000000 dirigera-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:56:45.672232 dirigera-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 06:56:38.000000 dirigera-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.668232 dirigera-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.668232 dirigera-1.1.2/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.969124 dirigera-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 18:12:53.000000 dirigera-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-18 18:13:01.969124 dirigera-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-18 18:12:53.000000 dirigera-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 18:12:53.000000 dirigera-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:13:01.969124 dirigera-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 18:12:53.000000 dirigera-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.961124 dirigera-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.961124 dirigera-1.1.3/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.965124 dirigera-1.1.3/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/devices/water_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.965124 dirigera-1.1.3/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 18:12:53.000000 dirigera-1.1.3/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.969124 dirigera-1.1.3/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 18:13:01.000000 dirigera-1.1.3/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:13:01.969124 dirigera-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-18 18:12:53.000000 dirigera-1.1.3/tests/test_water_sensor.py
```

### Comparing `dirigera-1.1.2/LICENSE` & `dirigera-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/PKG-INFO` & `dirigera-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.2
+Version: 1.1.3
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.2/README.md` & `dirigera-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/pyproject.toml` & `dirigera-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.1.2"
+version = "1.1.3"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.1.2/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.3/src/dirigera/devices/air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/blinds.py` & `dirigera-1.1.3/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/controller.py` & `dirigera-1.1.3/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/device.py` & `dirigera-1.1.3/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.3/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/light.py` & `dirigera-1.1.3/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.3/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.3/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/outlet.py` & `dirigera-1.1.3/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/devices/scene.py` & `dirigera-1.1.3/src/dirigera/devices/scene.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.3/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/hub/auth.py` & `dirigera-1.1.3/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/src/dirigera/hub/hub.py` & `dirigera-1.1.3/src/dirigera/hub/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ..devices.blinds import Blind, dict_to_blind
 from ..devices.controller import Controller, dict_to_controller
 from ..devices.outlet import Outlet, dict_to_outlet
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
 from ..devices.motion_sensor import MotionSensor, dict_to_motion_sensor
 from ..devices.open_close_sensor import OpenCloseSensor, dict_to_open_close_sensor
 from ..devices.scene import Action, Info, Scene, SceneType, Trigger, dict_to_scene
+from ..devices.water_sensor import WaterSensor, dict_to_water_sensor
 
 urllib3.disable_warnings(category=InsecureRequestWarning)
 
 
 class Hub(AbstractSmartHomeHub):
     def __init__(
         self,
@@ -338,14 +339,32 @@
     def get_scene_by_id(self, scene_id: str) -> Scene:
         """
         Fetches a specific scene by a given id
         """
         data = self.get(f"/scenes/{scene_id}")
         return dict_to_scene(data, self)
 
+    def get_water_sensors(self) -> List[WaterSensor]:
+        """
+        Fetches all water sensors registered in the Hub
+        """
+        devices = self.get("/devices")
+        water_sensors = list(filter(lambda x: x["type"] == "waterSensor", devices))
+        return [dict_to_water_sensor(water_sensor, self) for water_sensor in water_sensors]
+
+    def get_water_sensor_by_id(self, id_: str) -> WaterSensor:
+        """
+        Fetches a water sensor by its id
+        if that water sensors does not exist or is a device of another type raises ValueError
+        """
+        water_sensor = self._get_device_data_by_id(id_)
+        if water_sensor["type"] != "waterSensor":
+            raise ValueError("Device is not a WaterSensor")
+        return dict_to_water_sensor(water_sensor, self)
+
     def get_all_devices(self) -> List[Device]:
         """
         Fetches all devices registered in the Hub
         """
         devices: List[Device] = []
         devices.extend(self.get_air_purifiers())
         devices.extend(self.get_blinds())
```

### Comparing `dirigera-1.1.2/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.3/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.2
+Version: 1.1.3
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.2/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.3/src/dirigera.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
 src/dirigera/devices/motion_sensor.py
 src/dirigera/devices/open_close_sensor.py
 src/dirigera/devices/outlet.py
 src/dirigera/devices/scene.py
+src/dirigera/devices/water_sensor.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
 src/dirigera/hub/utils.py
 tests/test_air_purifier.py
 tests/test_blinds.py
 tests/test_controller.py
 tests/test_environment_sensor.py
 tests/test_light.py
 tests/test_motion_sensor.py
 tests/test_open_close_sensor.py
 tests/test_outlet.py
 tests/test_scenes.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_water_sensor.py
```

### Comparing `dirigera-1.1.2/tests/test_air_purifier.py` & `dirigera-1.1.3/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_blinds.py` & `dirigera-1.1.3/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_controller.py` & `dirigera-1.1.3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_environment_sensor.py` & `dirigera-1.1.3/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_light.py` & `dirigera-1.1.3/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_motion_sensor.py` & `dirigera-1.1.3/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_open_close_sensor.py` & `dirigera-1.1.3/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_outlet.py` & `dirigera-1.1.3/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_scenes.py` & `dirigera-1.1.3/tests/test_scenes.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.2/tests/test_utils.py` & `dirigera-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

