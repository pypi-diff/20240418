# Comparing `tmp/kelvin_sdk_pubsub-3.0.3-py3-none-any.whl.zip` & `tmp/kelvin_sdk_pubsub-3.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16399 bytes, number of entries: 14
--rw-r--r--  2.0 unx      473 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/__init__.py
--rw-r--r--  2.0 unx     1946 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/client.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/config.py
--rw-r--r--  2.0 unx    20482 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/connection.py
--rw-r--r--  2.0 unx      149 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/error.py
--rw-r--r--  2.0 unx     1988 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/prometheus.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/py.typed
--rw-r--r--  2.0 unx     5438 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/types.py
--rw-r--r--  2.0 unx      740 b- defN 24-Feb-09 15:07 kelvin/sdk/pubsub/utils.py
--rw-r--r--  2.0 unx      411 b- defN 24-Feb-09 15:13 kelvin/sdk/pubsub/version.py
--rw-r--r--  2.0 unx     2976 b- defN 24-Feb-09 15:13 kelvin_sdk_pubsub-3.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-09 15:13 kelvin_sdk_pubsub-3.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-09 15:13 kelvin_sdk_pubsub-3.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1179 b- defN 24-Feb-09 15:13 kelvin_sdk_pubsub-3.0.3.dist-info/RECORD
-14 files, 55151 bytes uncompressed, 14423 bytes compressed:  73.8%
+Zip file size: 16569 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      473 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/__init__.py
+-rw-r--r--  2.0 unx     1946 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/client.py
+-rw-r--r--  2.0 unx    19399 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/config.py
+-rw-r--r--  2.0 unx    21039 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/connection.py
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/error.py
+-rw-r--r--  2.0 unx     1988 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/prometheus.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/py.typed
+-rw-r--r--  2.0 unx     5438 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/types.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Apr-18 20:41 kelvin/sdk/pubsub/utils.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-18 20:47 kelvin/sdk/pubsub/version.py
+-rw-r--r--  2.0 unx     3009 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1179 b- defN 24-Apr-18 20:47 kelvin_sdk_pubsub-3.0.4.dist-info/RECORD
+14 files, 55870 bytes uncompressed, 14593 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: kelvin/sdk/pubsub/utils.py
 Comment: 
 
 Filename: kelvin/sdk/pubsub/version.py
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.3.dist-info/METADATA
+Filename: kelvin_sdk_pubsub-3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.3.dist-info/WHEEL
+Filename: kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.3.dist-info/top_level.txt
+Filename: kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kelvin_sdk_pubsub-3.0.3.dist-info/RECORD
+Filename: kelvin_sdk_pubsub-3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kelvin/sdk/pubsub/config.py

```diff
@@ -260,15 +260,15 @@
     max_items: int = Field(
         1024,
         title="Max Items",
         description="Maximum number of items to hold in sync receive queue.",
         ge=0,
     )
     keepalive: int = Field(
-        60,
+        600,
         title="Keepalive",
         description="Maximum period in seconds between communications with the broker.",
         ge=0,
     )
 
     @root_validator(pre=True)
     def validate_app_config(cls, values: Dict[str, Any]) -> Any:
@@ -386,14 +386,18 @@
                 values["broker_url"] = broker_url
 
             credentials = deep_get(mqtt_config, "authentication.credentials", {})
             if credentials:
                 values["username"] = credentials.get("username")
                 values["password"] = credentials.get("password")
 
+            keepalive = mqtt_config.get("keepalive")
+            if keepalive:
+                values["keepalive"] = keepalive
+
         return values
 
     app_config: Optional[Dict[str, Any]] = Field(
         None,
         title="Application Configuration",
         description="Application configuration.",
     )
```

## kelvin/sdk/pubsub/connection.py

```diff
@@ -28,15 +28,15 @@
 from uuid import uuid4
 
 import orjson
 import structlog
 from asyncio_mqtt import Client as AsyncClient
 from asyncio_mqtt import MqttError
 from orjson import OPT_SORT_KEYS
-from paho.mqtt.client import Client, MQTTMessage
+from paho.mqtt.client import MQTT_ERR_SUCCESS, PINGREQ, Client, MQTTMessage
 
 from kelvin.sdk.datatype import Message
 from kelvin.sdk.datatype.base_messages import ParametersMsg, Recommendation
 from kelvin.sdk.datatype.krn import KRNAssetDataStream, KRNAssetMetric, KRNWorkload
 from kelvin.sdk.datatype.msg_type import KMessageTypeData
 
 from .config import PubSubClientConfig, Selector
@@ -324,14 +324,23 @@
 
         client.loop_start()
 
         if not self._connect_count:
             self._send_storage_config()
         self._connect_count += 1
 
+    def conn_check(self) -> None:
+        if self._client is None:
+            return
+
+        rc = self._client._send_simple_command(PINGREQ)  # noqa
+        if rc != MQTT_ERR_SUCCESS:
+            logger.info("Mqtt connection lost. Reconnecting")
+            self._client.reconnect()  # noqa
+
     def _send_storage_config(self) -> None:
         """Send storage configuration."""
 
         client = self._client
         if client is None:
             return
 
@@ -426,15 +435,19 @@
 
         qos = self.config.qos
 
         messages = message if isinstance(message, Sequence) else [message]
 
         for message in messages:
             for topic, payload, retain, asset, metric in self._make_payloads(message):
-                client.publish(topic, payload, qos=qos, retain=retain)
+                ret = client.publish(topic, payload, qos=qos, retain=retain)
+                if ret.rc != MQTT_ERR_SUCCESS:
+                    logger.info("Publish failed. Reconnecting Mqtt")
+                    client.reconnect()
+                    client.publish(topic, payload, qos=qos, retain=retain)
                 self.prometheus_client.set_asset_metric_timestamp(asset, metric)
                 self._output_count += 1
 
     def receive(self, timeout: Optional[float] = None) -> Optional[Message]:
         """Receive message."""
 
         if self._client is None:
```

## kelvin/sdk/pubsub/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '3.0.3'
-__version_tuple__ = version_tuple = (3, 0, 3)
+__version__ = version = '3.0.4'
+__version_tuple__ = version_tuple = (3, 0, 4)
```

## Comparing `kelvin_sdk_pubsub-3.0.3.dist-info/METADATA` & `kelvin_sdk_pubsub-3.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: kelvin-sdk-pubsub
-Version: 3.0.3
+Version: 3.0.4
 Summary: Kelvin Pub-Sub Client
 Home-page: https://kelvininc.com/
 Author: Kelvin Inc
 Author-email: engineering@kelvininc.com
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7.0
 Description-Content-Type: text/markdown
 Requires-Dist: asyncio-mqtt ==0.12.*
+Requires-Dist: paho-mqtt ==1.6.1
 Requires-Dist: kelvin-sdk-datatype ==8.0.3
 Requires-Dist: prometheus-client ==0.14.*
 Requires-Dist: pydantic ==1.10.*,>=1.10.2
 Requires-Dist: PyYAML ==6.0.*
 Requires-Dist: structlog ==23.1.*
 Requires-Dist: cached-property ; python_version < "3.8"
 Requires-Dist: typing-extensions ; python_version < "3.8"
```

## Comparing `kelvin_sdk_pubsub-3.0.3.dist-info/RECORD` & `kelvin_sdk_pubsub-3.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 kelvin/sdk/pubsub/__init__.py,sha256=bh0J3qAcQVxlaLBhlZX1SH1AQx0vAuu0klD0ehVSwOM,473
 kelvin/sdk/pubsub/client.py,sha256=NJX2ru0DdL8PSfFmY9pMbHhYRrbFg63ZZLDKnuBr9-Q,1946
-kelvin/sdk/pubsub/config.py,sha256=M8unZucBuHYB1OC66Mv9c1AVJgZfkO2-KuTT6px7RAg,19270
-kelvin/sdk/pubsub/connection.py,sha256=bK7uolsqBz6OgovpBldZGfITYWyLQUI7eRV4bgszWYA,20482
+kelvin/sdk/pubsub/config.py,sha256=PvXQ_3hUDny4bg9PkAI45IMY0J5W_pDP4MIYVkV32IU,19399
+kelvin/sdk/pubsub/connection.py,sha256=vfBJo606tMiyo4H8mVZUxvnEHW9nrMUlnR0_quDEOq8,21039
 kelvin/sdk/pubsub/error.py,sha256=muFeb6nK3hm8VBjv_ErFYvRJdmJ4uNeLSYmpgSSA-IU,149
 kelvin/sdk/pubsub/prometheus.py,sha256=LbJfB6YVOrry2YwXlo9IjO8pbzGcsK873xGrBp5Id00,1988
 kelvin/sdk/pubsub/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kelvin/sdk/pubsub/types.py,sha256=-vGsE8NX4FpFmkI7FDa4Oy3nbTH0qIfhAsOOQbMRWYk,5438
 kelvin/sdk/pubsub/utils.py,sha256=JqsTPzuAEqHZd7Y1FqUYSqMq6cvqKd67fOjlQWjTfKY,740
-kelvin/sdk/pubsub/version.py,sha256=tmsJrqMJ6jmtNKTruxlJdd_-BtOyY3AALPeqEhjqKi0,411
-kelvin_sdk_pubsub-3.0.3.dist-info/METADATA,sha256=XXfN0_JtWDFBb8G4sEtKKhTWhMzrje9jMCDVlRkxBrM,2976
-kelvin_sdk_pubsub-3.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-kelvin_sdk_pubsub-3.0.3.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
-kelvin_sdk_pubsub-3.0.3.dist-info/RECORD,,
+kelvin/sdk/pubsub/version.py,sha256=yyqcyuVbO5Bq7rMS_oAT4a92vlOM2Jk4fCNagNkWYJk,411
+kelvin_sdk_pubsub-3.0.4.dist-info/METADATA,sha256=KuwubBNfldCnYNHrwJOVIIcwpEPzYltJRjiPOF8pFsU,3009
+kelvin_sdk_pubsub-3.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kelvin_sdk_pubsub-3.0.4.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
+kelvin_sdk_pubsub-3.0.4.dist-info/RECORD,,
```

