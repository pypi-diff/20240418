# Comparing `tmp/anedya_dev_sdk-0.1.3.tar.gz` & `tmp/anedya_dev_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya_dev_sdk-0.1.3.tar", last modified: Tue Apr 16 11:14:57 2024, max compression
+gzip compressed data, was "anedya_dev_sdk-0.1.4.tar", last modified: Thu Apr 18 07:44:29 2024, max compression
```

## Comparing `anedya_dev_sdk-0.1.3.tar` & `anedya_dev_sdk-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.3/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.3/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.3/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.3/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya_dev_sdk-0.1.3/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-16 11:12:11.000000 anedya_dev_sdk-0.1.3/src/anedya/anedya.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/anedya/client/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.3/src/anedya/client/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2888 2024-04-16 10:38:21.000000 anedya_dev_sdk-0.1.3/src/anedya/client/bindDevice.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      731 2024-04-09 10:17:45.000000 anedya_dev_sdk-0.1.3/src/anedya/client/callbacks.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.3/src/anedya/client/certs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2127 2024-04-09 09:46:47.000000 anedya_dev_sdk-0.1.3/src/anedya/client/mqttHandlers.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3237 2024-04-16 10:36:25.000000 anedya_dev_sdk-0.1.3/src/anedya/client/submitData.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2595 2024-04-16 10:48:17.000000 anedya_dev_sdk-0.1.3/src/anedya/client/submitLogs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2796 2024-04-16 10:48:15.000000 anedya_dev_sdk-0.1.3/src/anedya/client/timeSync.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2736 2024-04-16 10:58:02.000000 anedya_dev_sdk-0.1.3/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya_dev_sdk-0.1.3/src/anedya/errors.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2354 2024-04-16 11:09:16.000000 anedya_dev_sdk-0.1.3/src/anedya/models.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.3/src/anedya/transaction.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      678 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/requires.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.3/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.3/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.818052 anedya_dev_sdk-0.1.4/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.4/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.4/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-18 07:44:29.818052 anedya_dev_sdk-0.1.4/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.4/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-18 07:44:29.818052 anedya_dev_sdk-0.1.4/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.4/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.814052 anedya_dev_sdk-0.1.4/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.814052 anedya_dev_sdk-0.1.4/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-04-18 07:34:23.000000 anedya_dev_sdk-0.1.4/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4218 2024-04-18 07:36:51.000000 anedya_dev_sdk-0.1.4/src/anedya/anedya.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.814052 anedya_dev_sdk-0.1.4/src/anedya/client/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.4/src/anedya/client/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3435 2024-04-18 07:09:53.000000 anedya_dev_sdk-0.1.4/src/anedya/client/bindDevice.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      731 2024-04-09 10:17:45.000000 anedya_dev_sdk-0.1.4/src/anedya/client/callbacks.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.4/src/anedya/client/certs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2134 2024-04-18 07:36:31.000000 anedya_dev_sdk-0.1.4/src/anedya/client/mqttHandlers.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3417 2024-04-18 07:17:54.000000 anedya_dev_sdk-0.1.4/src/anedya/client/submitData.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2975 2024-04-18 07:12:59.000000 anedya_dev_sdk-0.1.4/src/anedya/client/submitLogs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3167 2024-04-18 07:17:21.000000 anedya_dev_sdk-0.1.4/src/anedya/client/timeSync.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3618 2024-04-18 06:58:49.000000 anedya_dev_sdk-0.1.4/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya_dev_sdk-0.1.4/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3383 2024-04-18 07:24:16.000000 anedya_dev_sdk-0.1.4/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.4/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.818052 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-18 07:44:29.000000 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      678 2024-04-18 07:44:29.000000 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-18 07:44:29.000000 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-18 07:44:29.000000 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/requires.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-18 07:44:29.000000 anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-18 07:44:29.818052 anedya_dev_sdk-0.1.4/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.4/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.4/tests/test_core.py
```

### Comparing `anedya_dev_sdk-0.1.3/LICENSE` & `anedya_dev_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/PKG-INFO` & `anedya_dev_sdk-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
```

### Comparing `anedya_dev_sdk-0.1.3/README.md` & `anedya_dev_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/setup.cfg` & `anedya_dev_sdk-0.1.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.1.3
+version = 0.1.4
 url = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 author = Anedya Systems
 author_email = support@anedya.io
 description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
 requires_python = ">=3.7"
 dependencies = ["requests","paho-mqtt>=2.0.0"]
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/anedya.py` & `anedya_dev_sdk-0.1.4/src/anedya/anedya.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
                 protocol=MQTTv5)
             self._mqttclient.username_pw_set(
                 username=str(self._config._deviceID),
                 password=self._config.connection_key)
             self.on_connect = config.on_connect
             self.on_disconnect = config.on_disconnect
             self.on_message = config.on_message
-            self._mqttclient.on_connect = self.onconnect_handler
-            self._mqttclient.on_disconnect = self.ondisconnect_handler
+            self._mqttclient.on_connect = self._onconnect_handler
+            self._mqttclient.on_disconnect = self._ondisconnect_handler
             # self._mqttclient.on_message = self.onmessage_handler
             self._mqttclient._connect_timeout = 1.0
             self._transactions = Transactions()
             # Set TLS Context
             context = SSLContext(ssl.PROTOCOL_TLS_CLIENT)
             context.load_verify_locations(cadata=ANEDYA_CA_CERTS)
             # self._mqttclient.tls_set()
@@ -99,10 +99,11 @@
 
     def disconnect(self):
         self._mqttclient.disconnect()
         return
 
     from .client.bindDevice import bind_device
     from .client.submitData import submit_data
+    from .client.submitLogs import submit_logs
     from .client.timeSync import get_time
-    from .client.mqttHandlers import onconnect_handler, ondisconnect_handler
+    from .client.mqttHandlers import _onconnect_handler, _ondisconnect_handler
     from .client.callbacks import _error_callback, _response_callback
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/bindDevice.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/bindDevice.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 import json
 from ..config import ConnectionMode
 from ..errors import AnedyaInvalidConfig, AnedyaTxFailure
 
 
-def bind_device(self, binding_secret: str, timeout: float | None = None):
+def bind_device(self, binding_secret: str, timeout: float | None = None) -> bool:
     """
-    :param binding_secret: Binding secret to be used for binding the device
-    :raises AnedyaInvalidConfig: If the configuration is not provided
-    :raises AnedyaTxFailure: If the transaction fails
+    Call this function to bind a device with the Anedya platform
 
-    This function provides a way to bind a device to the Anedya platform.
+    Args:
+        binding_secret (str): A one time Binding secret obtained from the platform. This secret is usually passed to device during provisioning process through
+        mobile app or any other process.
+        timeout (float | None, optional): Time out in seconds for the request. In production setup it is advisable to use a timeout or else your program can get stuck indefinitely. Defaults to None.
+
+    Raises:
+        AnedyaInvalidConfig: Method can raise this method if either configuration is not provided or if the connection mode is invalid.
+        AnedyaTxFailure: Method can raise this method if the transaction fails.
+
+    Returns:
+        bool: Returns true if the device is successfully bound with the platform.
     """
     if self._config is None:
         raise AnedyaInvalidConfig('Configuration not provided')
     if self._config.connection_mode == ConnectionMode.MQTT:
         return _bind_device_mqtt(self, binding_secret=binding_secret, timeout=timeout)
     elif self._config.connection_mode == ConnectionMode.HTTP:
         return _bind_device_http(self, binding_secret=binding_secret, timeout=timeout)
     else:
         raise AnedyaInvalidConfig('Invalid connection mode')
 
 
-def _bind_device_http(self, binding_secret: str, timeout: float | None = None):
+def _bind_device_http(self, binding_secret: str, timeout: float | None = None) -> bool:
     if self._config._testmode:
         url = "https://device.stageapi.anedya.io/v1/submitData"
     else:
         url = self._baseurl + "v1/bindDevice"
     requestPayload = {"bindingsecret": binding_secret,
                       "deviceid": str(self._config._deviceID)}
     r = self._httpsession.post(url, data=json.dumps(requestPayload), timeout=timeout)
     try:
         jsonResponse = r.json()
         payload = json.loads(jsonResponse)
         if payload['success'] is not True:
             raise AnedyaTxFailure(payload['error'], payload['errCode'])
     except ValueError:
         raise AnedyaTxFailure(message="Invalid JSON response")
-    return
+    return True
 
 
 def _bind_device_mqtt(self, binding_secret: str, timeout: float | None = None):
     # Create and register a transaction
     tr = self._transactions.create_transaction()
     # Encode the payload
     requestPayload = {
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/callbacks.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/callbacks.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/certs.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/certs.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/mqttHandlers.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/mqttHandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..errors import AnedyaInvalidCredentials, AnedyaRateLimitExceeded
 from ..errors import AnedyaException
 
 
-def onconnect_handler(self, client, userdata, flags, reason_code, properties):
+def _onconnect_handler(self, client, userdata, flags, reason_code, properties):
     rc = reason_code.value
     if rc == 135:
         raise AnedyaInvalidCredentials("Invalid credentials")
     elif rc == 134:
         raise AnedyaInvalidCredentials("Invalid Credentials")
     elif rc == 159:
         raise AnedyaRateLimitExceeded("Connection rate exceeded")
@@ -32,20 +32,20 @@
 
         # Call the on_connect callback if it is not None
         if self.on_connect is not None:
             self.on_connect()
     return
 
 
-def ondisconnect_handler(self,
-                         client,
-                         userdata,
-                         disconnect_flags,
-                         reason_code,
-                         properties):
+def _ondisconnect_handler(self,
+                          client,
+                          userdata,
+                          disconnect_flags,
+                          reason_code,
+                          properties):
     # First call the disconnect handler callback
     if self.on_disconnect is not None:
         self.on_disconnect(client,
                            userdata,
                            disconnect_flags,
                            reason_code,
                            properties)
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/submitData.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/submitData.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from ..config import ConnectionMode
 from ..models import DataPoints, AnedyaEncoder
 import json
 
 
 def submit_data(self, data: DataPoints, timeout: float | None = None):
     """
-    :param data: Data to send as a :class: DataPoints object
-    :param timeout: Timeout in seconds, default is None
+    Submit data to Anedya Platform.
 
-    :raises AnedyaTxFailure: If data could not be submitted due to an error
+    Args:
+        data (DataPoints): Datapoints object, you can submit multiple types of variable in single request.
+        timeout (float | None, optional): Time out in seconds for the request. In production setup it is advisable to use a timeout or else your program can get stuck indefinitely. Defaults to None.
 
-    This function sends data to the Anedya Cloud platform. It determines the connection mode from the SDK configuration and calls the appropriate submit data method (_submit_data_http or _submit_data_mqtt).
+    Raises:
+        AnedyaInvalidConfig: Method can raise this method if either configuration is not provided or if the connection mode is invalid.
+        AnedyaTxFailure: Method can raise this method if the transaction fails.
     """
 
     if self._config is None:
         raise AnedyaInvalidConfig('Configuration not provided')
     if self._config.connection_mode == ConnectionMode.HTTP:
         return _submit_data_http(self, data=data, timeout=timeout)
     elif self._config.connection_mode == ConnectionMode.MQTT:
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/submitLogs.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/submitLogs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 from ..errors import AnedyaInvalidConfig, AnedyaTxFailure
 from ..config import ConnectionMode
 import json
 
 
 def submit_logs(self, logs: LogsCache, timeout: float | None = None):
     """
-    :param logs: Logs to be send. :class: LogCache format.
-    :param timeout: Timeout in seconds, default is None.
+    Submit logs to Anedya
+
+    Args:
+        logs (LogsCache): Logs
+        timeout (float | None, optional): Time out in seconds for the request. In production setup it is advisable to use a timeout or else your program can get stuck indefinitely. Defaults to None.
+
+    Raises:
+        AnedyaInvalidConfig: Method can raise this method if either configuration is not provided or if the connection mode is invalid.
+        AnedyaTxFailure: Method can raise this method if the transaction fails.
     """
     if self._config is None:
         raise AnedyaInvalidConfig('Configuration not provided')
     if self._config.connection_mode == ConnectionMode.HTTP:
         return _submit_log_http(self, logs=logs, timeout=timeout)
     elif self._config.connection_mode == ConnectionMode.MQTT:
         return _submit_data_mqtt(self, logs=logs, timeout=timeout)
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/client/timeSync.py` & `anedya_dev_sdk-0.1.4/src/anedya/client/timeSync.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from ..errors import AnedyaInvalidConfig, AnedyaTxFailure
 from ..config import ConnectionMode
 import json
 import time
 
 
-def get_time(self, timeout: float | None = None):
+def get_time(self, timeout: float | None = None) -> int:
     """
-    Get current time from Anedya Time Service using HTTP request - 
-    Gets current time using HTTP requests.
-    Accuracy is generally within few tens of millisecond. For greater accuracy 
-    consider using NTP time service from Anedya
+    Fetch the time information from Anedya.
+
+    Args:
+        timeout (float | None, optional): Time out in seconds for the request. In production setup it is advisable to use a timeout or else your program can get stuck indefinitely. Defaults to None.
+
+    Raises:
+        AnedyaInvalidConfig: Method can raise this method if either configuration is not provided or if the connection mode is invalid.
+        AnedyaTxFailure: Method can raise this method if the transaction fails.
+
+    Returns:
+        int: The method returns the current time in Unix millisecond epoch in UTC timezone
     """
     if self._config is None:
         raise AnedyaInvalidConfig('Configuration not provided')
     if self._config.connection_mode == ConnectionMode.HTTP:
         return _time_sync_http(self, timeout=timeout)
     elif self._config.connection_mode == ConnectionMode.MQTT:
         return _time_sync_mqtt(self, timeout=timeout)
@@ -32,17 +39,17 @@
     r = self._httpsession.post(url, data=json.dumps(requestPayload), timeout=timeout)
     try:
         jsonResponse = r.json()
         payload = json.loads(jsonResponse)
         if payload['success'] is not True:
             raise AnedyaTxFailure(payload['error'], payload['errCode'])
         deviceRecTime = int(time.time_ns() / 1000000)
-        ServerReceiveTime = jsonResponse["serverReceiveTime"]
-        ServerSendTime = jsonResponse["serverSendTime"]
-        currentTime = (ServerReceiveTime + ServerSendTime + deviceRecTime - deviceSendTime) / 2
+        ServerReceiveTime = int(jsonResponse["serverReceiveTime"])
+        ServerSendTime = int(jsonResponse["serverSendTime"])
+        currentTime = int((ServerReceiveTime + ServerSendTime + deviceRecTime - deviceSendTime) / 2)
     except ValueError:
         raise AnedyaTxFailure(message="Invalid JSON response")
     return currentTime
 
 
 def _time_sync_mqtt(self, timeout: float | None = None):
     # Create and register a transaction
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/errors.py` & `anedya_dev_sdk-0.1.4/src/anedya/errors.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/src/anedya/transaction.py` & `anedya_dev_sdk-0.1.4/src/anedya/transaction.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
```

### Comparing `anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/SOURCES.txt` & `anedya_dev_sdk-0.1.4/src/anedya_dev_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.3/tests/test_config.py` & `anedya_dev_sdk-0.1.4/tests/test_config.py`

 * *Files identical despite different names*

