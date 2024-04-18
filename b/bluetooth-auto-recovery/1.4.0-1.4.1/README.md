# Comparing `tmp/bluetooth_auto_recovery-1.4.0.tar.gz` & `tmp/bluetooth_auto_recovery-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.4.0.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.4.1.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.4.0.tar` & `bluetooth_auto_recovery-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-03-13 23:42:43.734142 bluetooth_auto_recovery-1.4.0/LICENSE
--rw-r--r--   0        0        0     3840 2024-03-13 23:42:43.734142 bluetooth_auto_recovery-1.4.0/README.md
--rw-r--r--   0        0        0     2618 2024-03-13 23:42:44.446149 bluetooth_auto_recovery-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1063 2024-03-13 23:42:44.418149 bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 23:42:43.738143 bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    23611 2024-03-13 23:42:43.738143 bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0      225 2024-03-13 23:42:43.738143 bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/util.py
--rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3840 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/README.md
+-rw-r--r--   0        0        0     2618 2024-04-18 00:14:28.842423 bluetooth_auto_recovery-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1063 2024-04-18 00:14:28.794422 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    24748 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0      225 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/util.py
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.4.1/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.4.0/LICENSE` & `bluetooth_auto_recovery-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.4.0/README.md` & `bluetooth_auto_recovery-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.4.0/pyproject.toml` & `bluetooth_auto_recovery-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.4.0"
+version = "1.4.1"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/__init__.py` & `bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 import asyncio
 import importlib
 import sys
 from types import ModuleType
 
 _MODULE_CACHE: dict[str, ModuleType] = {}
```

### Comparing `bluetooth_auto_recovery-1.4.0/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/recover.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,22 +118,27 @@
         rfkill_hci_state["soft"], rfkill_hci_state["hard"], rfkill_hci_state["idx"]
     )
 
 
 class BluetoothMGMTProtocol(asyncio.Protocol):
     """Bluetooth MGMT protocol."""
 
-    def __init__(self, timeout: float) -> None:
+    def __init__(
+        self, timeout: float, connection_mode_future: asyncio.Future[None]
+    ) -> None:
         """Initialize the protocol."""
         self.future: asyncio.Future[btmgmt_protocol.Response] | None = None
         self.transport: asyncio.Transport | None = None
         self.timeout = timeout
+        self.connection_mode_future = connection_mode_future
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         """Handle connection made."""
+        if not self.connection_mode_future.done():
+            self.connection_mode_future.set_result(None)
         self.transport = cast(asyncio.Transport, transport)
 
     def data_received(self, data: bytes) -> None:
         """Handle data received."""
         try:
             if (
                 self.future
@@ -187,24 +192,26 @@
             self.protocol = None
         btmgmt_socket.close(self.sock)
 
     async def setup(self) -> None:
         """Set up management interface."""
         self.sock = btmgmt_socket.open()
         loop = asyncio.get_running_loop()
+        connection_made_future: asyncio.Future[None] = loop.create_future()
         try:
             async with asyncio_timeout(5):
                 # _create_connection_transport accessed directly to avoid SOCK_STREAM check
                 # see https://bugs.python.org/issue38285
                 _, protocol = await loop._create_connection_transport(  # type: ignore[attr-defined]
                     self.sock,
-                    lambda: BluetoothMGMTProtocol(self.timeout),
+                    lambda: BluetoothMGMTProtocol(self.timeout, connection_made_future),
                     None,
                     None,
                 )
+                await connection_made_future
         except asyncio.TimeoutError:
             btmgmt_socket.close(self.sock)
             raise
         assert isinstance(protocol, BluetoothMGMTProtocol)  # nosec
         self.protocol = protocol
         await self._find_controller()
 
@@ -568,34 +575,56 @@
     except asyncio.TimeoutError:
         _LOGGER.warning(
             "Could not determine the power state of the Bluetooth adapter %s due to timeout after %s seconds",
             name,
             adapter.timeout,
         )
         timed_out_getting_powered = True
+    except Exception:  # pylint: disable=broad-except
+        _LOGGER.exception(
+            "Could not determine the power state of the Bluetooth adapter %s: %s",
+            name,
+        )
 
     # Do not attempt to power off if it timed out getting the power state
     # as it likely means the adapter interface is frozen and will not respond to
     # power off commands so we need to proceed to bounce the interface
     if not timed_out_getting_powered:
         try:
             await _execute_power_off(adapter, name, power_state_before_reset)
         except asyncio.TimeoutError:
             _LOGGER.warning(
                 "Could not reset the power state of the Bluetooth adapter %s due to timeout after %s seconds",
                 name,
                 adapter.timeout,
             )
+        except Exception:
+            _LOGGER.exception(
+                "Could not reset the power state of the Bluetooth adapter %s", name
+            )
 
     try:
         await _bounce_adapter_interface(adapter)
     except Exception as ex:  # pylint: disable=broad-except
         _LOGGER.warning("Could not cycle the Bluetooth adapter %s: %s", name, ex)
 
-    return await _execute_power_on(adapter, name, power_state_before_reset)
+    try:
+        return await _execute_power_on(adapter, name, power_state_before_reset)
+    except asyncio.TimeoutError:
+        _LOGGER.warning(
+            "Could not reset the power state of the Bluetooth adapter %s due to timeout after %s seconds",
+            name,
+            adapter.timeout,
+        )
+        return False
+    except Exception:
+        _LOGGER.exception(
+            "Could not reset the power state of the Bluetooth adapter %s", name
+        )
+        return False
 
 
 async def _execute_power_on(
     adapter: MGMTBluetoothCtl, name: str, power_state_before_reset: bool | None
 ) -> bool:
     """Execute the power off."""
     try:
```

### Comparing `bluetooth_auto_recovery-1.4.0/PKG-INFO` & `bluetooth_auto_recovery-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-auto-recovery
-Version: 1.4.0
+Version: 1.4.1
 Summary: Recover bluetooth adapters that are in an stuck state
 Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.4.0 Summary:
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.4.1 Summary:
 Recover bluetooth adapters that are in an stuck state Home-page: https://
 github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

