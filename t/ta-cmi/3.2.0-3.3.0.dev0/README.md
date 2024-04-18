# Comparing `tmp/ta-cmi-3.2.0.tar.gz` & `tmp/ta_cmi-3.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-3.2.0.tar", last modified: Mon Jan 15 17:55:26 2024, max compression
+gzip compressed data, was "ta_cmi-3.3.0.dev0.tar", last modified: Wed Apr 17 19:10:38 2024, max compression
```

## Comparing `ta-cmi-3.2.0.tar` & `ta_cmi-3.3.0.dev0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.981505 ta-cmi-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8133 2024-01-15 17:55:26.980505 ta-cmi-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6562 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 17:55:26.981505 ta-cmi-3.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.979505 ta-cmi-3.2.0/ta_cmi/
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/channel.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi_api.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/cmi_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe_api.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/coe_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3567 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/const.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2024-01-15 17:55:13.000000 ta-cmi-3.2.0/ta_cmi/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 17:55:26.980505 ta-cmi-3.2.0/ta_cmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8133 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-15 17:55:26.000000 ta-cmi-3.2.0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-17 19:10:38.071427 ta_cmi-3.3.0.dev0/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1067 2023-04-18 18:49:16.000000 ta_cmi-3.3.0.dev0/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     8199 2024-04-17 19:10:38.064427 ta_cmi-3.3.0.dev0/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     6681 2024-01-15 17:46:52.000000 ta_cmi-3.3.0.dev0/README.md
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2024-04-17 19:10:38.072426 ta_cmi-3.3.0.dev0/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      658 2024-04-17 18:31:36.000000 ta_cmi-3.3.0.dev0/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-17 19:10:37.872427 ta_cmi-3.3.0.dev0/ta_cmi/
+-rwxrwxrwx   0 user      (1000) user      (1000)      423 2024-01-15 17:51:33.000000 ta_cmi-3.3.0.dev0/ta_cmi/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2918 2024-03-28 14:09:07.000000 ta_cmi-3.3.0.dev0/ta_cmi/api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1228 2024-03-28 14:09:07.000000 ta_cmi-3.3.0.dev0/ta_cmi/channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      885 2024-04-15 20:07:58.000000 ta_cmi-3.3.0.dev0/ta_cmi/cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2700 2023-07-28 19:34:46.000000 ta_cmi-3.3.0.dev0/ta_cmi/cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      543 2024-03-28 14:09:07.000000 ta_cmi-3.3.0.dev0/ta_cmi/cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3559 2023-12-02 09:25:43.000000 ta_cmi-3.3.0.dev0/ta_cmi/coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     6728 2024-04-17 18:00:09.000000 ta_cmi-3.3.0.dev0/ta_cmi/coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      403 2023-04-21 23:42:39.000000 ta_cmi-3.3.0.dev0/ta_cmi/coe_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3684 2024-04-15 20:06:19.000000 ta_cmi-3.3.0.dev0/ta_cmi/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     4642 2024-04-15 20:07:12.000000 ta_cmi-3.3.0.dev0/ta_cmi/device.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-17 19:10:38.057428 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     8199 2024-04-17 19:10:37.000000 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      512 2024-04-17 19:10:37.000000 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2024-04-17 19:10:37.000000 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       31 2024-04-17 19:10:37.000000 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2024-04-17 19:10:37.000000 ta_cmi-3.3.0.dev0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2024-04-17 19:10:38.042427 ta_cmi-3.3.0.dev0/tests/
+-rwxrwxrwx   0 user      (1000) user      (1000)     3792 2023-07-28 19:34:46.000000 ta_cmi-3.3.0.dev0/tests/test_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      624 2023-04-18 18:49:17.000000 ta_cmi-3.3.0.dev0/tests/test_cmi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     5148 2023-07-28 19:34:46.000000 ta_cmi-3.3.0.dev0/tests/test_cmi_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      967 2023-04-18 18:49:17.000000 ta_cmi-3.3.0.dev0/tests/test_cmi_channel.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     6522 2023-12-02 09:24:54.000000 ta_cmi-3.3.0.dev0/tests/test_coe.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     7164 2024-04-17 18:24:21.000000 ta_cmi-3.3.0.dev0/tests/test_coe_api.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    11627 2024-04-17 14:51:16.000000 ta_cmi-3.3.0.dev0/tests/test_device.py
```

### Comparing `ta-cmi-3.2.0/LICENSE` & `ta_cmi-3.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ta-cmi-3.2.0/PKG-INFO` & `ta_cmi-3.3.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 3.2.0
+Version: 3.3.0.dev0
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
@@ -24,14 +24,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.9.3
+Requires-Dist: packaging>=24.0
 
 # TA-CMI
 A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 
 ## How to use package
 
 ### Json API
```

### Comparing `ta-cmi-3.2.0/README.md` & `ta_cmi-3.3.0.dev0/ta_cmi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: ta-cmi
+Version: 3.3.0.dev0
+Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+Home-page: https://gitlab.com/DeerMaximum/ta-cmi
+Author: DeerMaximum
+Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
+License: MIT License
+        
+        Copyright (c) 2021 DeerMaximum
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.9.3
+Requires-Dist: packaging>=24.0
+
 # TA-CMI
 A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 
 ## How to use package
 
 ### Json API
 
@@ -113,8 +146,8 @@
     except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
         print(f"Error: {error}")
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 loop.close()
-```
+```
```

### Comparing `ta-cmi-3.2.0/setup.py` & `ta_cmi-3.3.0.dev0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     readme = f.read()
 
 with open("LICENSE", "r", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="ta-cmi",
-    version="3.2.0",
+    version="3.3.0dev0",
     description="A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/ta-cmi",
     author="DeerMaximum",
     author_email="2629822-DeerMaximum@users.noreply.gitlab.com",
     license=license,
     packages=["ta_cmi"],
-    install_requires=["aiohttp>=3.7.4"],
+    install_requires=["aiohttp>=3.9.3", "packaging>=24.0"],
 )
```

### Comparing `ta-cmi-3.2.0/ta_cmi/coe.py` & `ta_cmi-3.3.0.dev0/ta_cmi/coe.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-3.2.0/ta_cmi/coe_api.py` & `ta_cmi-3.3.0.dev0/ta_cmi/coe_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+from dataclasses import dataclass
 from typing import Any, Dict
 
 from aiohttp import ClientSession
 
 from .api import API
 from .coe_channel import CoEChannel
 from .const import _LOGGER, ChannelMode
 
 
+@dataclass
+class CoEServerConfig:
+    coe_version: int
+
+
 class CoEAPI(API):
     """Class to perform API requests to the CoE Addon."""
 
     COE_VERSION = "/version"
+    COE_CONFIG = "/config"
     COE_DATA = "/receive/{id}"
     COE_SEND_ANALOG = "/send/analog"
     COE_SEND_DIGITAL = "/send/digital"
+    COE_SEND_ANALOG_V2 = "/send/v2/analog"
+    COE_SEND_DIGITAL_V2 = "/send/v2/digital"
 
     DIGITAL_VALUES_PER_PAGE = 16
     ANALOG_VALUES_PER_PAGE = 4
 
     def __init__(self, host: str, session: ClientSession = None) -> None:
         """Initialize."""
         super().__init__(session)
@@ -50,23 +59,35 @@
         _LOGGER.debug("Received version from CoE server: %s", data)
 
         if len(data) == 0:
             return None
 
         return data.get("version", None)
 
+    async def get_coe_server_config(self) -> CoEServerConfig:
+        """Get the CoE config from the server."""
+        url = f"{self.host}{self.COE_VERSION}"
+
+        _LOGGER.debug("Receive current config from CoE server: %s", url)
+
+        data = await self._make_request_get(url)
+
+        _LOGGER.debug("Received version from CoE server: %s", data)
+
+        return CoEServerConfig(coe_version=data.get("coe_version", 0))
+
     @staticmethod
-    def _check_channel_type(
+    def _check_channel_mode(
         target_mode: ChannelMode, channel_to_check: list[CoEChannel]
     ) -> bool:
         """Check if the channel type equals the target."""
         for channel in channel_to_check:
-            if channel.type != target_mode:
+            if channel.mode != target_mode:
                 _LOGGER.warning(
-                    f"Channel has wrong type. Expected type: {target_mode}, actual type: {channel.type}"
+                    f"Channel has wrong mode. Expected mode: {target_mode}, actual mode: {channel.mode}"
                 )
                 return False
 
         return True
 
     @staticmethod
     def _check_array_length(array: list, target_size: int) -> bool:
@@ -96,15 +117,15 @@
         return {"value": channel.value, "unit": int(channel.unit)}
 
     async def send_analog_values(self, channels: list[CoEChannel], page: int):
         """Send analog values to the CoE server."""
         _LOGGER.debug("Send analog values to CoE server")
 
         if (
-            not self._check_channel_type(ChannelMode.ANALOG, channels)
+            not self._check_channel_mode(ChannelMode.ANALOG, channels)
             or not self._check_array_length(channels, self.ANALOG_VALUES_PER_PAGE)
             or not self._check_analog_page_size(page)
         ):
             _LOGGER.error("Could not send analog values. Please see logs for details.")
             return
 
         data = {
@@ -120,17 +141,60 @@
 
     async def send_digital_values(
         self, channels: list[CoEChannel], second_page: bool = False
     ) -> None:
         """Send digital values to the CoE server."""
         _LOGGER.debug("Send digital values to CoE server")
 
-        if not self._check_channel_type(
+        if not self._check_channel_mode(
             ChannelMode.DIGITAL, channels
         ) or not self._check_array_length(channels, self.DIGITAL_VALUES_PER_PAGE):
             _LOGGER.error("Could not send digital values. Please see logs for details.")
             return
 
         data = {"values": [bool(x.value) for x in channels], "page": int(second_page)}
 
         url = f"{self.host}{self.COE_SEND_DIGITAL}"
         await self._make_request_post(url, data)
+
+    @staticmethod
+    def _map_channel_to_v2_body(channel: CoEChannel) -> dict[str, Any]:
+        """Map a channel to a v2 request body."""
+        return {"channel": channel.index, "value": channel.value, "unit": channel.unit}
+
+    async def send_analog_value_v2(self, channel: CoEChannel) -> None:
+        """Send analog values to the CoE server (Version 2)."""
+        _LOGGER.debug("Send analog value to CoE server (V2)")
+
+        if not self._check_channel_mode(ChannelMode.ANALOG, [channel]):
+            _LOGGER.error("Could not send analog values. Please see logs for details.")
+            return
+
+        data = self._map_channel_to_v2_body(channel)
+
+        if data.get("channel", 0) <= 0:
+            _LOGGER.error(
+                "Could not send analog values. Channel must be greater than zero."
+            )
+            return
+
+        url = f"{self.host}{self.COE_SEND_ANALOG_V2}"
+        await self._make_request_post(url, data)
+
+    async def send_digital_value_v2(self, channel: CoEChannel) -> None:
+        """Send digital values to the CoE server (Version 2)."""
+        _LOGGER.debug("Send digital value to CoE server (V2)")
+
+        if not self._check_channel_mode(ChannelMode.DIGITAL, [channel]):
+            _LOGGER.error("Could not send digital values. Please see logs for details.")
+            return
+
+        data = self._map_channel_to_v2_body(channel)
+
+        if data.get("channel", 0) <= 0:
+            _LOGGER.error(
+                "Could not send digital values. Channel must be greater than zero."
+            )
+            return
+
+        url = f"{self.host}{self.COE_SEND_DIGITAL_V2}"
+        await self._make_request_post(url, data)
```

### Comparing `ta-cmi-3.2.0/ta_cmi/const.py` & `ta_cmi-3.3.0.dev0/ta_cmi/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import enum
 from logging import Logger, NullHandler, getLogger
-from typing import Dict
+from typing import Awaitable, Callable, Dict
 
 HTTP_OK: int = 200
 HTTP_UNAUTHORIZED: int = 401
 
 _LOGGER: Logger = getLogger(__package__)
 _LOGGER.addHandler(NullHandler())
 
+SLEEP_FUNCTION_TYPE = Callable[[int], Awaitable[None]]
+
 
 class ChannelType(enum.Enum):
     INPUT = "Inputs"
     OUTPUT = "Outputs"
     DL_BUS = "DL-Bus"
     SYSTEM_VALUES_GENERAL = "General"
     SYSTEM_VALUES_DATE = "Date"
@@ -123,14 +125,15 @@
     "69": "W",
     "70": "t",
     "71": "kg",
     "72": "g",
     "73": "cm",
     "74": "K",
     "75": "lx",
+    "76": "Bg/m³",
 }
 
 UNITS_DE: Dict[str, str] = {
     "1": "°C",
     "2": "W/m²",
     "3": "l/h",
     "4": "Sek",
@@ -183,14 +186,15 @@
     "69": "W",
     "70": "t",
     "71": "kg",
     "72": "g",
     "73": "cm",
     "74": "K",
     "75": "lx",
+    "76": "Bg/m³",
 }
 
 RAS_STATE: Dict[int, str] = {
     0: "Time/auto",
     1: "Standard",
     2: "Setback",
     3: "Standby/frost pr",
```

### Comparing `ta-cmi-3.2.0/ta_cmi/device.py` & `ta_cmi-3.3.0.dev0/ta_cmi/device.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,138 @@
-import asyncio
-from typing import Any, Dict, List
-
-from .channel import Channel
-from .cmi_api import CMIAPI
-from .cmi_channel import CMIChannel
-from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
-
-
-class Device:
-    """Class to interact with a device."""
-
-    def __init__(self, node_id: str, api: CMIAPI) -> None:
-        """Initialize."""
-        super().__init__()
-
-        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
-
-        self.id = node_id
-        self._api = api
-
-        self.api_version: int = 0
-        self.device_id: str = "00"
-
-    def _extract_device_info(self, json: Dict[str, Any]) -> None:
-        """Extract device info from request response."""
-        self.api_version: int = json["Header"]["Version"]
-        self.device_id: str = json["Header"]["Device"]
-
-        if self.device_id not in DEVICES.keys():
-            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
-
-    @staticmethod
-    def _extract_channels(
-        mode: ChannelType, raw_channels: List[Dict[str, Any]]
-    ) -> Dict[int, CMIChannel]:
-        """Extract channel info from data array from request."""
-        list_of_channels: Dict[int, CMIChannel] = {}
-        for channel_raw in raw_channels:
-            ch: CMIChannel = CMIChannel(mode, channel_raw)
-            list_of_channels[ch.index] = ch
-
-        return list_of_channels
-
-    def _get_json_params(self) -> str:
-        """Compose json params based on the device type."""
-        default_params = "I,O"
-        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
-
-    async def _make_request_to_device(self) -> Dict[str, Any]:
-        """Make a request to the device."""
-        params = self._get_json_params()
-
-        data: dict[str, Any] = {}
-
-        if len(params.split(",")) > 7:
-            first_params = ",".join(params.split(",")[:7])
-            params = ",".join(params.split(",")[7:])
-
-            data = await self._api.get_device_data(self.id, first_params)
-
-            await asyncio.sleep(61)
-
-        if len(data.keys()) == 0:
-            return await self._api.get_device_data(self.id, params)
-
-        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
-
-        return data
-
-    async def fetch_type(self) -> None:
-        """Fetch the device type without parsing the data from the device."""
-        self._extract_device_info(await self._make_request_to_device())
-
-    async def update(self) -> None:
-        """Update data."""
-        _LOGGER.debug("Update device: %s", self.id)
-        res: Dict[str, Any] = await self._make_request_to_device()
-
-        if self.device_id == "00":
-            self._extract_device_info(res)
-            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
-
-        for channel_type_text in res["Data"]:
-            channel_type = ChannelType(channel_type_text)
-            self._channels[channel_type] = self._extract_channels(
-                channel_type, res["Data"][channel_type_text]
-            )
-
-    def set_device_type(self, device_name: str) -> None:
-        """Set the type of the device manually."""
-        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
-
-        if len(type_id) != 1:
-            raise InvalidDeviceError(f"Invalid device name: {device_name}")
-
-        self.device_id = type_id[0]
-
-    def get_device_type(self) -> str:
-        """Get the type of the device."""
-        return DEVICES.get(self.device_id, "Unknown")
-
-    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
-        """Get all the fetched channels from a type."""
-        return self._channels.get(channel_type, {})
-
-    def has_channel_type(self, channel_type: ChannelType) -> bool:
-        """Check if a channel type was fetched."""
-        return self._channels.get(channel_type, None) is not None
-
-    def __repr__(self) -> str:
-        text = f"Node {self.id}: Type: {self.get_device_type()}"
-
-        for channel_type in self._channels:
-            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
-
-        return text
-
-
-class InvalidDeviceError(Exception):
-    """Triggered when an invalid device type is set."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
+import asyncio
+from typing import Any, Dict, List
+
+from .cmi_api import CMIAPI
+from .cmi_channel import CMIChannel
+from .const import (
+    _LOGGER,
+    DEVICES,
+    SLEEP_FUNCTION_TYPE,
+    SUPPORTED_PARAMS_FOR_DEVICE,
+    ChannelType,
+)
+
+
+class Device:
+    """Class to interact with a device."""
+
+    def __init__(
+        self,
+        node_id: str,
+        api: CMIAPI,
+        sleep_function: SLEEP_FUNCTION_TYPE = asyncio.sleep,
+    ) -> None:
+        """Initialize."""
+        super().__init__()
+
+        self._sleep_function = sleep_function
+
+        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
+
+        self.id = node_id
+        self._api = api
+
+        self.api_version: int = 0
+        self.device_id: str = "00"
+
+    def _extract_device_info(self, json: Dict[str, Any]) -> None:
+        """Extract device info from request response."""
+        self.api_version: int = json["Header"]["Version"]
+        self.device_id: str = json["Header"]["Device"]
+
+        if self.device_id not in DEVICES.keys():
+            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
+
+    @staticmethod
+    def _extract_channels(
+        mode: ChannelType, raw_channels: List[Dict[str, Any]]
+    ) -> Dict[int, CMIChannel]:
+        """Extract channel info from data array from request."""
+        list_of_channels: Dict[int, CMIChannel] = {}
+        for channel_raw in raw_channels:
+            ch: CMIChannel = CMIChannel(mode, channel_raw)
+            list_of_channels[ch.index] = ch
+
+        return list_of_channels
+
+    def _get_json_params(self) -> str:
+        """Compose json params based on the device type."""
+        default_params = "I,O"
+        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
+
+    async def _make_request_to_device(self) -> Dict[str, Any]:
+        """Make a request to the device."""
+        params = self._get_json_params()
+
+        data: dict[str, Any] = {}
+
+        if len(params.split(",")) > 7:
+            first_params = ",".join(params.split(",")[:7])
+            params = ",".join(params.split(",")[7:])
+
+            data = await self._api.get_device_data(self.id, first_params)
+
+            await self._sleep_function(61)
+
+        if len(data.keys()) == 0:
+            return await self._api.get_device_data(self.id, params)
+
+        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
+
+        return data
+
+    async def fetch_type(self) -> None:
+        """Fetch the device type without parsing the data from the device."""
+        self._extract_device_info(await self._make_request_to_device())
+
+    async def update(self) -> None:
+        """Update data."""
+        _LOGGER.debug("Update device: %s", self.id)
+        res: Dict[str, Any] = await self._make_request_to_device()
+
+        if self.device_id == "00":
+            self._extract_device_info(res)
+            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
+
+        for channel_type_text in res["Data"]:
+            channel_type = ChannelType(channel_type_text)
+            self._channels[channel_type] = self._extract_channels(
+                channel_type, res["Data"][channel_type_text]
+            )
+
+    def set_device_type(self, device_name: str) -> None:
+        """Set the type of the device manually."""
+        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
+
+        if len(type_id) != 1:
+            raise InvalidDeviceError(f"Invalid device name: {device_name}")
+
+        self.device_id = type_id[0]
+
+    def get_device_type(self) -> str:
+        """Get the type of the device."""
+        return DEVICES.get(self.device_id, "Unknown")
+
+    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
+        """Get all the fetched channels from a type."""
+        return self._channels.get(channel_type, {})
+
+    def has_channel_type(self, channel_type: ChannelType) -> bool:
+        """Check if a channel type was fetched."""
+        return self._channels.get(channel_type, None) is not None
+
+    def __repr__(self) -> str:
+        text = f"Node {self.id}: Type: {self.get_device_type()}"
+
+        for channel_type in self._channels:
+            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
+
+        return text
+
+
+class InvalidDeviceError(Exception):
+    """Triggered when an invalid device type is set."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
```

