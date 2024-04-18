# Comparing `tmp/robothub-2.5.8.tar.gz` & `tmp/robothub-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub-2.5.8.tar", last modified: Sun Apr 14 22:55:18 2024, max compression
+gzip compressed data, was "robothub-2.5.9.tar", last modified: Thu Apr 18 12:30:37 2024, max compression
```

## Comparing `robothub-2.5.8.tar` & `robothub-2.5.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-14 22:55:02.000000 robothub-2.5.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-14 22:55:02.000000 robothub-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 22:55:18.251026 robothub-2.5.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-14 22:55:02.000000 robothub-2.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:55:18.251026 robothub-2.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-14 22:55:02.000000 robothub-2.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.243026 robothub-2.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.247026 robothub-2.5.8/src/robothub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/frame_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/live_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/live_view_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.247026 robothub-2.5.8/src/robothub/replay/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/capture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/captures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/replay_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    33998 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/replay_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/src/robothub/robothub_core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_event_typechecks.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_stop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/src/robothub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.141693 robothub-2.5.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-18 12:30:20.000000 robothub-2.5.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-18 12:30:20.000000 robothub-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 12:30:37.141693 robothub-2.5.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-18 12:30:20.000000 robothub-2.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:30:37.141693 robothub-2.5.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-18 12:30:20.000000 robothub-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.133694 robothub-2.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.133694 robothub-2.5.9/src/robothub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/frame_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/live_view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/src/robothub/replay/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/capture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/captures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/replay_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33998 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/replay_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/src/robothub/robothub_core_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_event_typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_stop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.141693 robothub-2.5.9/src/robothub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_manager.py
```

### Comparing `robothub-2.5.8/LICENSE` & `robothub-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/PKG-INFO` & `robothub-2.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.8
+Version: 2.5.9
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.8/README.md` & `robothub-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/__init__.py` & `robothub-2.5.9/src/robothub/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 # Import symbols from robothub_core and make them available under the robothub namespace
 try:
     import robothub_core as robothub
 except ImportError:
     import robothub.robothub_core_wrapper as robothub
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 
 # Setup logging for the module
 # setup_logger(__name__)
```

### Comparing `robothub-2.5.8/src/robothub/application.py` & `robothub-2.5.9/src/robothub/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         """
         Connect to the device. This method is called in a separate thread.
         """
         give_up_time = time.monotonic() + 30
 
         self.__device_state = robothub_core.DeviceState.CONNECTING
         product_name = self._device_product_name
-        logger.info(f"Establishing connection with Device {product_name} and uploading the pipeline...")
+        logger.info(f"Establishing connection with Device {product_name}...")
         while self.running and time.monotonic() < give_up_time:
             logger.debug(
                 f"Device {product_name}: remaining time to connect - {give_up_time - time.monotonic()} seconds."
             )
             try:
                 self._device = self._acquire_device()
                                     
@@ -220,24 +220,25 @@
     def _acquire_device(self):
         pass
 
 
 class BaseDepthAIApplication(BaseApplication):
     def _manage_device_inner(self) -> None:
         self._device_stop_event.clear()
-        logger.info(f"Device {self._device_product_name}: creating Pipeline...")
-        self.pipeline = self.setup_pipeline()
-        assert self.pipeline is not None, f"setup_pipeline() must return a valid depthai.Pipeline object but returned {self.pipeline}."
-        logger.info(f"Device {self._device_product_name}: Pipeline created...")
         self._connect()
         if self._device is None:
             # Wait 30 seconds before trying to connect again
             self.wait(30)
             return
+        logger.info(f"Device {self._device_product_name}: creating Pipeline...")
+        self.pipeline = self.setup_pipeline()
+        assert self.pipeline is not None, f"setup_pipeline() must return a valid depthai.Pipeline object but returned {self.pipeline}."
+        logger.info(f"Device {self._device_product_name}: Pipeline created...")
 
+        self._device.startPipeline(self.pipeline)
         self._start_replay()
 
         if LOCAL_DEV is True:
             self.manage_device(self._device)
         else:
             # Start threads for user loop and reporting
             device_thread = Thread(
@@ -262,16 +263,15 @@
         self._close_device()
 
     def _start_replay(self):
         for replay in ReplayCamera.replay_camera_instances:
             replay.start_polling(self._device)
 
     def _acquire_device(self) -> depthai.Device:
-        return depthai.Device(self.pipeline, depthai.DeviceInfo(
-            self._device_ip or self._device_mxid))
+        return depthai.Device(depthai.DeviceInfo(self._device_ip or self._device_mxid))
 
     def __get_dai_device(self) -> depthai.Device:
         return self._device
 
     @abstractmethod
     def setup_pipeline(self) -> depthai.Pipeline:
         pass
```

### Comparing `robothub-2.5.8/src/robothub/decorators.py` & `robothub-2.5.9/src/robothub/decorators.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/events.py` & `robothub-2.5.9/src/robothub/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/frame_buffer.py` & `robothub-2.5.9/src/robothub/frame_buffer.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/live_view.py` & `robothub-2.5.9/src/robothub/live_view.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/live_view_utils.py` & `robothub-2.5.9/src/robothub/live_view_utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/replay/capture_manager.py` & `robothub-2.5.9/src/robothub/replay/capture_manager.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/replay/captures.py` & `robothub-2.5.9/src/robothub/replay/captures.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/replay/replay_builder.py` & `robothub-2.5.9/src/robothub/replay/replay_builder.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/replay/replay_camera.py` & `robothub-2.5.9/src/robothub/replay/replay_camera.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/replay/utils.py` & `robothub-2.5.9/src/robothub/replay/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/__init__.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/_event_typechecks.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/_event_typechecks.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/app.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/app.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/client.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/communicator.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/communicator.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/device.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/device.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/events.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/globals.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/globals.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/robothub_core_wrapper/streams.py` & `robothub-2.5.9/src/robothub/robothub_core_wrapper/streams.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub/utils.py` & `robothub-2.5.9/src/robothub/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.8/src/robothub.egg-info/PKG-INFO` & `robothub-2.5.9/src/robothub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.8
+Version: 2.5.9
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.8/src/robothub.egg-info/SOURCES.txt` & `robothub-2.5.9/src/robothub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

