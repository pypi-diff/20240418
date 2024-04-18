# Comparing `tmp/dm-aiomqtt-0.3.6.tar.gz` & `tmp/dm_aiomqtt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-aiomqtt-0.3.6.tar", last modified: Sun Mar 31 09:52:02 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.0.tar", last modified: Thu Apr 18 15:56:24 2024, max compression
```

## Comparing `dm-aiomqtt-0.3.6.tar` & `dm_aiomqtt-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:52:02.777067 dm-aiomqtt-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-03-31 09:52:02.777067 dm-aiomqtt-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-31 09:51:55.000000 dm-aiomqtt-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:52:02.777067 dm-aiomqtt-0.3.6/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-31 09:51:55.000000 dm-aiomqtt-0.3.6/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-03-31 09:51:55.000000 dm-aiomqtt-0.3.6/dm_aiomqtt/dm_aiomqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:52:02.777067 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:52:02.777067 dm-aiomqtt-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-31 09:52:02.000000 dm-aiomqtt-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:56:24.376509 dm_aiomqtt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 15:56:24.376509 dm_aiomqtt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-18 15:56:16.000000 dm_aiomqtt-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:56:24.372509 dm_aiomqtt-0.4.0/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 15:56:16.000000 dm_aiomqtt-0.4.0/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-04-18 15:56:16.000000 dm_aiomqtt-0.4.0/dm_aiomqtt/dm_aiomqtt_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:56:24.376509 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 15:56:24.000000 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 15:56:24.000000 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:56:24.000000 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 15:56:24.000000 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 15:56:24.000000 dm_aiomqtt-0.4.0/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:56:24.376509 dm_aiomqtt-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 15:56:23.000000 dm_aiomqtt-0.4.0/setup.py
```

### Comparing `dm-aiomqtt-0.3.6/README.md` & `dm_aiomqtt-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,79 +3,70 @@
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomqtt)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomqtt)
 
 ## Usage
 
-### Warning
-
-For correct operation of the client, **_readwrite_** access to `ping/#` topic is **REQUIRED**.
-Improved system for responding to loss of connection, will use this topic to send **ping** messages.
-
-(Format of ping messages - topic: `ping/[uuid4]`, payload: `1`)
-
-### Run in Windows
-
-_If you run async code in **Windows**, set correct selector_
-
-```python
-import asyncio
-import sys
-
-if sys.platform == "win32":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-```
-
 ### Example
 
 ```python
 from dm_aiomqtt import DMAioMqttClient
 import asyncio
 
 
 # create handler for 'test' topic
 async def test_topic_handler(publish: DMAioMqttClient.publish, topic: str, payload: str) -> None:
     print(f"Received message from {topic}: {payload}")
-    await publish("test/success", payload=True)
+    publish("test/success", payload=True)
 
 
 async def main():
     # create client
     mqtt_client = DMAioMqttClient("localhost", 1883, "username", "password")
 
     # add handler for 'test' topic
     mqtt_client.add_topic_handler("test", test_topic_handler)
 
     # start connection
     await mqtt_client.start()
 
     # publish
-    await mqtt_client.publish("test", payload="Hello World!", sent_logging=True)
+    mqtt_client.publish("test", payload="Hello World!", sent_logging=True)
 
     # other code (for example, endless waiting)
     await asyncio.Event().wait()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### TLS connection
 
 * NOT required client certificate
 
    ```python
-   mqtt_client = DMAioMqttClient("localhost", 8883, ca_file="ca.crt")
+   mqtt_client = DMAioMqttClient(
+       host="localhost",
+       port=8883,
+       ca_crt="ssl/ca.crt"
+   )
    ```
 
 * REQUIRED client certificate
 
    ```python
-   mqtt_client = DMAioMqttClient("localhost", 8883, ca_file="ca.crt", client_crt="client.crt", client_key="client.key")
+   mqtt_client = DMAioMqttClient(
+       host="localhost",
+       port=8883,
+       ca_crt="ssl/ca.crt",
+       client_crt="ssl/client.crt",
+       client_key="ssl/client.key"
+   )
    ```
 
 ### Set custom logger
 
 _If you want set up custom logger_
 
 ```python
@@ -106,8 +97,20 @@
 | Parameter         | Type               | Default Value | Description                               |
 |-------------------|--------------------|---------------|-------------------------------------------|
 | `topic`           | `str`              | (required)    | Topic name                                |
 | `payload`         | `str`              | `"DEBUG"`     | Content to send                           |
 | `qos`             | `0` \| `1` \| `2`  | `True`        | MQTT QoS                                  |
 | `payload_to_json` | `bool` \| `"auto"` | `True`        | Whether to convert content to JSON        |
 | `sent_logging`    | `bool`             | `False`       | Whether to print the sending notification |
-| `warn_logging`    | `bool`             | `False`       | Whether to print a send error warning     |
+| `error_logging`   | `bool`             | `False`       | Whether to print a send error warning     |
+
+### Run in Windows
+
+_If you run async code in **Windows**, set correct selector_
+
+```python
+import asyncio
+import sys
+
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+```
```

### Comparing `dm-aiomqtt-0.3.6/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.0/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,170 +27,127 @@
         host: str,
         port: int,
         username: str = "",
         password: str = "",
         ca_crt: str = "",
         client_crt: str = "",
         client_key: str = "",
-        ping_interval_s: int = 5,
-        clean_session: bool = True
+        identifier: str = None,
+        keepalive: int = 5,
+        clean_session: bool = False
     ) -> None:
         if self.__logger is None:
             self.__logger = DMLogger(f"DMAioMqttClient-{host}:{port}")
 
-        self.__ping_interval_s = ping_interval_s if ping_interval_s > 1 else 1
-
         self.__mqtt_config = {
             "hostname": host,
             "port": port,
-            "keepalive": self.__ping_interval_s * 3,
+            "keepalive": keepalive,
             "clean_session": clean_session,
-            "identifier": str(uuid.uuid4())
+            "identifier": identifier or str(uuid.uuid4())
         }
         if username or password:
             self.__mqtt_config["username"] = username
             self.__mqtt_config["password"] = password
         self.__mqtt_config["tls_context"] = self.__get_tls_context(ca_crt, client_crt, client_key)
 
-        self.__reconnect_timeout = self.__ping_interval_s * 2 + 1
-        self.__reconnect_timer_task = None
-        self.__is_reconnect = False
-        self.__reconnect_counter = 0
         self.__subscribes = {}
         self.__pattern_subscribes = {}
-        self.__ping_topic = f"ping/{self.__mqtt_config['identifier']}"
-        self.add_topic_handler(self.__ping_topic, self.__reset_reconnect_timer_task)
-        self.__client: aiomqtt.Client = None
+        self.__client: aiomqtt.Client = aiomqtt.Client(**self.__mqtt_config)
+        self.__connected_event = asyncio.Event()
 
     async def start(self) -> None:
-        await self.__connect_loop()
-        _ = asyncio.create_task(self.__ping_loop())
-
-    async def __connect(self) -> None:
-        self.__client = aiomqtt.Client(**self.__mqtt_config)
-        await self.__client.__aenter__()
-        self.__reconnect_counter = 0
-        self.__logger.info("Connected!")
+        _ = asyncio.create_task(self.__connect_loop())
+        await self.__connected_event.wait()
 
     async def __connect_loop(self) -> None:
         while True:
             try:
-                await self.__connect()
-                self.__is_reconnect = False
-                self.__reconnect_timer_task = asyncio.create_task(self.__reconnect_timer())
-                await self.__subscribe()
-                _ = asyncio.create_task(self.__listen())
-                return
+                async with aiomqtt.Client(**self.__mqtt_config) as self.__client:
+                    self.__logger.info("Connected!")
+                    self.__connected_event.set()
+                    await self.__listen()
             except Exception as e:
-                if self.__reconnect_counter < 1:
-                    self.__logger.error(f"Connection error: {e}.\nReconnecting...")
-                self.__reconnect_counter += 1
-                await asyncio.sleep(self.__ping_interval_s)
-
-    async def __disconnect(self) -> None:
-        try:
-            await self.__client.__aexit__(None, None, None)
-        except:
-            pass
-
-    async def __reconnect(self) -> None:
-        self.__reconnect_timer_task.cancel()
-        if self.__is_reconnect:
-            return
-        self.__is_reconnect = True
-        await self.__disconnect()
-        await self.__connect_loop()
-
-    async def __reset_reconnect_timer_task(self, *args, **kwargs) -> None:
-        self.__reconnect_timer_task.cancel()
-        self.__reconnect_timer_task = asyncio.create_task(self.__reconnect_timer())
-
-    async def __reconnect_timer(self) -> None:
-        await asyncio.sleep(self.__reconnect_timeout)
-        await self.__reconnect()
-
-    async def __ping_loop(self) -> None:
-        while True:
-            await self.publish(self.__ping_topic, 1)
-            await asyncio.sleep(self.__ping_interval_s)
+                if self.__connected_event.is_set():
+                    self.__logger.error(f"Error: {e}")
+                self.__connected_event.clear()
+                self.__connecting = False
 
     async def __listen(self) -> None:
-        try:
-            async for message in self.__client.messages:
-                topic = message.topic.value
-                payload = message.payload.decode('utf-8')
-
-                callbacks = self.__get_callbacks_from_pattern_subscribes(topic)
-                topic_params = self.__subscribes.get(topic)
-                if isinstance(topic_params, dict):
-                    callbacks.append(topic_params["cb"])
-
-                for callback in callbacks:
-                    if isinstance(callback, Callable):
-                        _ = asyncio.create_task(callback(self.publish, topic, payload))
-                    else:
-                        self.__logger.error(f"Callback is not a Callable object: {type(callback)}, {topic=}")
-        except Exception as e:
-            self.__logger.error(f"Connection error: {e}")
-            await self.__reconnect()
+        async for message in self.__client.messages:
+            topic = message.topic.value
+            payload = message.payload.decode('utf-8')
+
+            callbacks = self.__get_callbacks_from_pattern_subscribes(topic)
+            topic_params = self.__subscribes.get(topic)
+            if isinstance(topic_params, dict):
+                callbacks.append(topic_params["cb"])
+
+            for callback in callbacks:
+                if isinstance(callback, Callable):
+                    _ = asyncio.create_task(callback(self.publish, topic, payload))
+                else:
+                    self.__logger.error(f"Callback is not a Callable object: {type(callback)}, {topic=}")
 
-    def __get_callbacks_from_pattern_subscribes(self, current_topic: str) -> List[Callable]:
-        if current_topic == self.__ping_topic:
-            return []
+    def add_topic_handler(self, topic: str, callback: _SUBSCRIBE_CALLBACK_TYPE, qos: _QOS_TYPE = 0) -> None:
+        """
+        callback EXAMPLE:
+            async def test_topic_handler(publish: DMAioMqttClient.publish, topic: str, payload: str) -> None:
+               print(f"Received message from {topic}: {payload}")
+               publish("test/success", payload=True)
+        """
+        new_item = {"cb": callback, "qos": qos}
+        self.__subscribes[topic] = new_item
 
-        callbacks = []
-        for topic, params in self.__pattern_subscribes.items():
-            pattern = topic.replace("+", "[^/]+?")
-            pattern = pattern.replace("/#", "(/.+)*")
-            if re.search(pattern, current_topic):
-                callbacks.append(params["cb"])
-        return callbacks
+        if re.search(r"[+#]", topic):
+            self.__pattern_subscribes[topic] = new_item
 
-    async def publish(
+    def publish(
         self,
         topic: str,
         payload: Union[str, int, float, dict, list, bool, None],
         qos: _QOS_TYPE = 0,
         *,
         payload_to_json: Union[bool, Literal["auto"]] = "auto",
         sent_logging: bool = False,
-        warn_logging: bool = False,
+        error_logging: bool = False,
     ) -> None:
         """
         payload_to_json (bool, "auto"):
             - "auto":
                 will be converted all payload types expect: str, int, float
             - True:
                 will be converted all payload types
             - False:
                 will not be converted
         """
-        if payload_to_json is True or (payload_to_json == "auto" and type(payload) not in (str, int, float)):
-            payload = json.dumps(payload, ensure_ascii=False)
-        try:
-            await self.__client.publish(topic, payload, qos)
-        except Exception as e:
-            if warn_logging:
-                self.__logger.warning(f"Publish not sent: {e}")
-        else:
-            if sent_logging:
-                self.__logger.debug(f"Published message to '{topic}' topic ({qos=}): {payload}")
 
-    def add_topic_handler(self, topic: str, callback: _SUBSCRIBE_CALLBACK_TYPE, qos: _QOS_TYPE = 0) -> None:
-        """
-        callback EXAMPLE:
-            async def test_topic_handler(publish: DMAioMqttClient.publish, topic: str, payload: str) -> None:
-               print(f"Received message from {topic}: {payload}")
-               await publish("test/success", payload=True)
-        """
-        new_item = {"cb": callback, "qos": qos}
-        self.__subscribes[topic] = new_item
+        async def cb(payload):
+            if payload_to_json is True or (payload_to_json == "auto" and type(payload) not in (str, int, float)):
+                payload = json.dumps(payload, ensure_ascii=False)
+            try:
+                await self.__connected_event.wait()
+                await self.__client.publish(topic, payload, qos)
+            except Exception as e:
+                if error_logging:
+                    self.__logger.warning(f"Publish not sent: {e}")
+            else:
+                if sent_logging:
+                    self.__logger.debug(f"Published message to '{topic}' topic ({qos=}): {payload}")
 
-        if re.search(r"[+#]", topic):
-            self.__pattern_subscribes[topic] = new_item
+        _ = asyncio.create_task(cb(payload))
+
+    def __get_callbacks_from_pattern_subscribes(self, current_topic: str) -> List[Callable]:
+        callbacks = []
+        for topic, params in self.__pattern_subscribes.items():
+            pattern = topic.replace("+", "[^/]+?")
+            pattern = pattern.replace("/#", "(/.+)*")
+            if re.search(pattern, current_topic):
+                callbacks.append(params["cb"])
+        return callbacks
 
     async def __subscribe(self) -> None:
         for topic, params in self.__subscribes.items():
             _, qos = params.values()
             await self.__client.subscribe(topic, qos)
             self.__logger.debug(f"Subscribe to '{topic}' topic ({qos=})")
```

### Comparing `dm-aiomqtt-0.3.6/setup.py` & `dm_aiomqtt-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.3.6',
+    version='v0.4.0',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```

