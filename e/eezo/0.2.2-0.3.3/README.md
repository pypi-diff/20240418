# Comparing `tmp/eezo-0.2.2.tar.gz` & `tmp/eezo-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.2.2.tar", last modified: Fri Apr 12 15:21:21 2024, max compression
+gzip compressed data, was "eezo-0.3.3.tar", last modified: Thu Apr 18 11:43:22 2024, max compression
```

## Comparing `eezo-0.2.2.tar` & `eezo-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 15:21:21.492862 eezo-0.2.2/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-12 15:21:21.492749 eezo-0.2.2/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.2.2/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 15:21:21.489191 eezo-0.2.2/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.2.2/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-04-10 16:05:56.000000 eezo-0.2.2/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    11786 2024-04-12 09:52:16.000000 eezo-0.2.2/eezo/connector.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 15:21:21.490692 eezo-0.2.2/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.2.2/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 15:21:21.492527 eezo-0.2.2/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     6068 2024-04-12 15:08:57.000000 eezo-0.2.2/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     6212 2024-04-12 15:08:54.000000 eezo-0.2.2/eezo/interface/interface_async.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.2.2/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 15:21:21.489894 eezo-0.2.2/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-12 15:21:21.000000 eezo-0.2.2/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      567 2024-04-12 15:21:21.000000 eezo-0.2.2/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-12 15:21:21.000000 eezo-0.2.2/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-12 15:21:21.000000 eezo-0.2.2/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-12 15:21:21.000000 eezo-0.2.2/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-12 15:21:21.492897 eezo-0.2.2/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1946 2024-04-12 15:21:01.000000 eezo-0.2.2/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.971730 eezo-0.3.3/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-04-18 11:43:22.971615 eezo-0.3.3/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.3.3/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.967498 eezo-0.3.3/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-04-18 09:35:35.000000 eezo-0.3.3/eezo/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.968806 eezo-0.3.3/eezo/agent/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       52 2024-04-17 18:38:28.000000 eezo-0.3.3/eezo/agent/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     8043 2024-04-18 07:45:30.000000 eezo-0.3.3/eezo/agent/agent.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     2948 2024-04-18 07:26:56.000000 eezo-0.3.3/eezo/agent/agents.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    12868 2024-04-18 11:28:06.000000 eezo-0.3.3/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    13835 2024-04-18 11:22:04.000000 eezo-0.3.3/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    12496 2024-04-18 11:26:20.000000 eezo-0.3.3/eezo/connector.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      355 2024-04-17 22:28:24.000000 eezo-0.3.3/eezo/errors.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.969769 eezo-0.3.3/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.3.3/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.971441 eezo-0.3.3/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.3.3/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4073 2024-04-18 09:09:39.000000 eezo-0.3.3/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     5276 2024-04-18 09:16:48.000000 eezo-0.3.3/eezo/interface/interface_async.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4502 2024-04-17 22:58:05.000000 eezo-0.3.3/eezo/interface/message.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3509 2024-04-18 09:46:52.000000 eezo-0.3.3/eezo/state.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3700 2024-04-18 09:40:44.000000 eezo-0.3.3/eezo/state_async.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 11:43:22.968179 eezo-0.3.3/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-04-18 11:43:22.000000 eezo-0.3.3/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      680 2024-04-18 11:43:22.000000 eezo-0.3.3/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-18 11:43:22.000000 eezo-0.3.3/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-18 11:43:22.000000 eezo-0.3.3/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-18 11:43:22.000000 eezo-0.3.3/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-18 11:43:22.971763 eezo-0.3.3/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1601 2024-04-18 11:42:57.000000 eezo-0.3.3/setup.py
```

### Comparing `eezo-0.2.2/README.md` & `eezo-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.2.2/eezo/async_client.py` & `eezo-0.3.3/eezo/interface/interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,101 @@
-from watchdog.events import FileSystemEventHandler
-from watchdog.observers import Observer
+from typing import Any, Dict, Callable, Optional
+from .message import Message
 
-from .interface.interface import Message
-from .connector import AsyncConnector
 
-import asyncio
-import aiohttp
-import sys
-import os
-
-SERVER = "https://api-service-bofkvbi4va-ey.a.run.app"
-if os.environ.get("EEZO_DEV_MODE") == "True":
-    print("Running in dev mode")
-    SERVER = "http://localhost:8082"
-
-CREATE_MESSAGE_ENDPOINT = SERVER + "/v1/create-message/"
-READ_MESSAGE_ENDPOINT = SERVER + "/v1/read-message/"
-DELETE_MESSAGE_ENDPOINT = SERVER + "/v1/delete-message/"
-
-
-class RestartHandler(FileSystemEventHandler):
-    def on_modified(self, event):
-        if event.src_path.endswith(".py"):
-            os.execl(sys.executable, sys.executable, *sys.argv)
-
-
-class AsyncClient:
-    def __init__(self, api_key=None, logger=False):
-        self.connector_functions = {}
-        self.tasks = []
-        self.observer = Observer()
-        self.api_key = os.environ["EEZO_API_KEY"] if api_key is None else api_key
-        self.logger = logger
-        if self.api_key is None:
-            raise ValueError("Eezo api_key is required")
-
-    def on(self, connector_id):
-        def decorator(func):
-            self.connector_functions[connector_id] = func
-            return func
-
-        return decorator
-
-    async def connect(self):
-        try:
-            self.observer.schedule(RestartHandler(), ".", recursive=False)
-            self.observer.start()
-
-            for connector_id, func in self.connector_functions.items():
-                c = AsyncConnector(self.api_key, connector_id, func, self.logger)
-                task = asyncio.create_task(c.connect())
-                self.tasks.append(task)
-
-            await asyncio.gather(*self.tasks)
-
-        except KeyboardInterrupt:
-            for task in self.tasks:
-                task.cancel()
-            self.observer.stop()
-
-    async def __request(self, method, endpoint, payload):
-        async with aiohttp.ClientSession() as session:
-            async with session.request(method, endpoint, json=payload) as response:
-                response_json = await response.json()
-                if response.status == 401:
-                    raise Exception(f"Unauthorized. Probably invalid api_key")
-                if response.status != 200:
-                    raise Exception(
-                        f"Error {response.status}: {response_json['detail']}"
-                    )
-                return response_json
-
-    async def new_message(self, eezo_id, thread_id, context="direct_message"):
-        new_message = Message()
-
-        async def notify():
-            nm = new_message.to_dict()
-            await self.__request(
-                "POST",
-                CREATE_MESSAGE_ENDPOINT,
-                {
-                    "api_key": self.api_key,
-                    "thread_id": thread_id,
-                    "eezo_id": eezo_id,
-                    "message_id": nm["id"],
-                    "interface": nm["interface"],
-                    "context": context,
-                },
-            )
-
-        new_message.notify = notify
-        return new_message
-
-    async def delete_message(self, message_id):
-        await self.__request(
-            "POST",
-            DELETE_MESSAGE_ENDPOINT,
-            {"api_key": self.api_key, "message_id": message_id},
+class Interface:
+    """
+    Interface class for managing communications and state for a specific job identified by a job ID.
+
+    Attributes:
+        job_id: Identifier for the specific job this interface is associated with.
+        user_id: User identifier for state and message association.
+        api_key: API key for authorization purposes.
+        send_message: Callback function to send messages.
+        _run: Private callback function to execute skills or agents.
+    """
+
+    def __init__(
+        self,
+        job_id: str,
+        user_id: str,
+        api_key: str,
+        cb_send_message: Callable[[Dict[str, Any]], Any],
+        cb_run: Callable[..., Any],
+    ):
+        """
+        Initialize the Interface with identifiers and callback functions.
+
+        Args:
+            job_id: A unique identifier for the job to which this interface pertains.
+            user_id: A unique identifier for the user who is associated with this job.
+            api_key: A string that represents the API key for authentication.
+            cb_send_message: A callback function that is used to send messages.
+            cb_run: A callback function that is used to execute agents or skills.
+
+        The Interface class acts as a facilitator between the client's job-specific operations and the server's
+        state management and messaging systems. It encapsulates methods for message creation, notification,
+        state retrieval, and invocation of external skills or agents.
+        """
+        self.job_id = job_id
+        self.message: Optional[Message] = None
+        self.user_id = user_id
+        self.api_key = api_key
+        self.send_message = cb_send_message
+        self._run = cb_run
+
+    def new_message(self) -> Message:
+        """
+        Creates and returns a new message object with a notification callback attached.
+
+        This method should be called when the client needs to create a new message to be sent.
+        It initializes a Message object and binds the `notify` method of the Interface as its
+        notification callback function.
+        """
+        self.message = Message(notify=self.notify)
+        return self.message
+
+    def notify(self) -> None:
+        """
+        Notifies that a message is ready to be sent, triggering the send_message callback.
+
+        If a message has been created using `new_message`, this method formats that message and
+        uses the `send_message` callback to send it. It raises an exception if called before a message
+        is created.
+        """
+        if self.message is None:
+            raise Exception("Please create a message first")
+
+        message_obj = self.message.to_dict()
+        self.send_message(
+            {
+                "message_id": message_obj["id"],
+                "interface": message_obj["interface"],
+            }
         )
 
-    async def update_message(self, message_id):
-        response_json = await self.__request(
-            "POST",
-            READ_MESSAGE_ENDPOINT,
-            {"api_key": self.api_key, "message_id": message_id},
+    def get_thread(self, nr: int = 5, to_string: bool = False) -> Any:
+        """
+        Retrieves and returns a thread of messages, with a limit on the number of messages.
+
+        Args:
+            nr: The number of messages to retrieve from the thread. Defaults to 5.
+            to_string: A boolean flag indicating whether to convert the messages to a string. Defaults to False.
+
+        The method delegates the operation to the `_run` callback, providing the required parameters.
+        """
+        return self._run(
+            skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string
         )
-        if "data" not in response_json:
-            raise Exception(f"Message not found for id {message_id}")
 
-        old_message = response_json["data"]
-        new_message = Message()  # Assuming Message is refactored for async
-
-        async def notify():
-            nm = new_message.to_dict()
-            await self.__request(
-                "POST",
-                CREATE_MESSAGE_ENDPOINT,
-                {
-                    "api_key": self.api_key,
-                    "thread_id": old_message["thread_id"],
-                    "eezo_id": old_message["eezo_id"],
-                    "message_id": nm["id"],
-                    "interface": nm["interface"],
-                    # Find a way to get context from old_message_obj
-                    "context": old_message["skill_id"],
-                },
-            )
-
-        new_message.notify = notify
-        new_message.id = old_message["id"]
-        return new_message
+    def invoke(self, agent_id: str, **kwargs: Any) -> Any:
+        """
+        Invokes an agent or skill and returns its result.
+
+        Args:
+            agent_id: A string identifier of the agent or skill to be invoked.
+            **kwargs: A variable number of keyword arguments that are passed to the agent or skill.
+
+        This method utilizes the `_run` callback to execute the agent or skill identified by `agent_id`
+        with the given keyword arguments.
+        """
+        return self._run(skill_id=agent_id, **kwargs)
```

### Comparing `eezo-0.2.2/eezo/connector.py` & `eezo-0.3.3/eezo/connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import traceback
 import logging
 import asyncio
 import socketio
 import aiohttp
 import requests
+import uuid
 import time
 import os
 
 SERVER = "https://api-service-bofkvbi4va-ey.a.run.app"
 if os.environ.get("EEZO_DEV_MODE") == "True":
     SERVER = "http://localhost:8082"
 
@@ -39,14 +40,15 @@
     def __init__(self, api_key, connector_id, connector_function, logger=False):
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
         self.job_responses = {}
         self.user_id = None
+        self.auth_token = None
         self.run_loop = True
 
         if logger:
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(asctime)s: %(message)s",
                 datefmt="%Y-%m-%d %H:%M:%S",
@@ -72,26 +74,28 @@
             )
             self.__log(f" ✔ Connector {self.connector_id} connected")
 
     def __log(self, message):
         if self.logger:
             logging.info(message)
 
-    async def __authenticate(self):
+    async def authenticate(self) -> str:
         async with aiohttp.ClientSession() as session:
             url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
             async with session.post(url, json={"api_key": self.api_key}) as response:
                 if response.status == 200:
                     resp_json = await response.json()
                     self.auth_token = resp_json.get("token")
                     self.user_id = resp_json.get("user_id")
                 else:
                     resp_json = await response.json()
                     raise Exception(f"{response.status}: {resp_json['detail']}")
 
+        return self.user_id, self.auth_token
+
     async def __get_job_result(self, job_id):
         while job_id not in self.job_responses:
             await asyncio.sleep(0.1)
         response = self.job_responses.pop(job_id)
         self.__log(f"<< Sub Job {job_id} completed")
         if not response.get("success", True):
             self.__log(f" ✖ Sub Job {response['id']} failed:\n{response['traceback']}.")
@@ -107,15 +111,15 @@
             job_obj["job_payload"],
         )
         self.__log(
             f"<< Job for connector {connector_id} received with payload: {payload}"
         )
         try:
             # Create an interface object that the connector function can use to interact with the Eezo server
-            i = AsyncInterface(
+            i: AsyncInterface = AsyncInterface(
                 job_id=job_id,
                 user_id=self.user_id,
                 api_key=self.api_key,
                 cb_send_message=lambda p: self.sio.emit("direct_message", p),
                 cb_invoke_connector=lambda p: self.sio.emit("invoke_skill", p),
                 cb_get_result=self.__get_job_result,
             )
@@ -129,30 +133,35 @@
                 error=str(e),
                 traceback=traceback.format_exc(),
                 error_tag="Connector error",
             )
             await self.sio.emit("job_completed", job_completed.to_dict())
 
     async def connect(self):
-        await self.__authenticate()
+        if not self.auth_token:
+            raise Exception("Not authenticated")
 
         self.sio.on(
             "disconnect",
             lambda: self.__log(f" ✖ Connector {self.connector_id} disconnected"),
         )
 
         def auth_error(message: str):
             self.__log(f" ✖ Authentication failed: {message}")
             self.run_loop = False
 
         async def on_token_expired():
-            await self.__authenticate()
+            await self.authenticate()
+
+        def job_response(response):
+            self.__log(f"<< Job response received: {response}")
+            self.job_responses[response["id"]] = response
 
         self.sio.on("job_request", lambda p: asyncio.create_task(self.__execute_job(p)))
-        self.sio.on("job_response", lambda p: self.job_responses.update({p["id"]: p}))
+        self.sio.on("job_response", job_response)
         self.sio.on("token_expired", on_token_expired)
         self.sio.on("auth_error", auth_error)
 
         while self.run_loop:
             try:
                 await self.sio.connect(SERVER)
                 await self.sio.wait()
@@ -180,21 +189,25 @@
                 else:
                     break
 
         await self.sio.disconnect()
 
 
 class Connector:
-    def __init__(self, api_key, connector_id, connector_function, logger=False):
+    def __init__(
+        self, api_key, connector_id, connector_function, job_responses, logger=False
+    ):
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
-        self.job_responses = {}
+        # needs to be in the main thread
+        self.job_responses = job_responses
         self.user_id = None
+        self.auth_token = None
         self.run_loop = True
 
         if logger:
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(asctime)s: %(message)s",
                 datefmt="%Y-%m-%d %H:%M:%S",
@@ -220,57 +233,72 @@
             )
             self.__log(f" ✔ Connector {self.connector_id} connected")
 
     def __log(self, message):
         if self.logger:
             logging.info(message)
 
-    def __authenticate(self):
+    def authenticate(self) -> str:
         url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
         response = requests.post(url, json={"api_key": self.api_key})
         if response.status_code == 200:
             self.auth_token = response.json().get("token")
             self.user_id = response.json().get("user_id")
         else:
             raise Exception(f"{response.status_code}: {response.json()['detail']}")
 
-    def __get_job_result(self, job_id):
+        return self.user_id, self.auth_token
+
+    def __run(self, skill_id, **kwargs):
+        """Invoke a skill and get the result."""
+        if not skill_id:
+            raise ValueError("skill_id is required")
+
+        job_id = str(uuid.uuid4())
+        self.sio.emit(
+            "invoke_skill",
+            {
+                "new_job_id": job_id,
+                "skill_id": skill_id,
+                "skill_payload": kwargs,
+            },
+        )
+
         while True:
             if job_id in self.job_responses:
                 response = self.job_responses.pop(job_id)
-                self.__log(f"<< Sub Job {job_id} completed.")
 
                 if not response.get("success", True):
                     self.__log(
-                        f" ✖ Sub Job {response['id']} failed:\n{response['traceback']}."
+                        f"<< Sub Job {response['id']} failed:\n{response['traceback']}."
                     )
                     raise Exception(response["error"])
 
+                self.__log(f"<< Sub Job {job_id} completed.")
                 return response["result"]
             else:
-                time.sleep(0.1)
+                time.sleep(1)
 
     def __execute_job(self, job_obj):
         job_id, connector_id, payload = (
             job_obj["job_id"],
             job_obj["connector_id"],
             job_obj["job_payload"],
         )
         self.__log(
             f"<< Job for connector {connector_id} received with payload: {payload}"
         )
         try:
             # Create an interface object that the connector function can use to interact with the Eezo server
-            i = Interface(
+            i: Interface = Interface(
                 job_id=job_id,
                 user_id=self.user_id,
                 api_key=self.api_key,
                 cb_send_message=lambda p: self.sio.emit("direct_message", p),
-                cb_invoke_connector=lambda p: self.sio.emit("invoke_skill", p),
-                cb_get_result=self.__get_job_result,
+                cb_run=self.__run,
             )
             # Call the connector function with the interface object and the job payload
             result = self.func(i, **payload)
             self.sio.emit("job_completed", JobCompleted(result, True).to_dict())
         except Exception as e:
             self.__log(f" ✖ Connector {connector_id} failed:\n{traceback.format_exc()}")
             job_completed = JobCompleted(
@@ -279,31 +307,29 @@
                 error=str(e),
                 traceback=str(traceback.format_exc()),
                 error_tag="Connector error",
             )
             self.sio.emit("job_completed", job_completed.to_dict())
 
     def connect(self):
-        self.__authenticate()
+        if not self.auth_token:
+            raise Exception("Not authenticated")
 
         self.sio.on(
             "disconnect",
             lambda: self.__log(f" ✖ Connector {self.connector_id} disconnected"),
         )
 
         def auth_error(message: str):
             self.__log(f" ✖ Authentication failed: {message}")
             self.run_loop = False
 
-        def job_response(response):
-            self.job_responses[response["id"]] = response
-
         self.sio.on("job_request", lambda p: self.__execute_job(p))
-        self.sio.on("job_response", job_response)
-        self.sio.on("token_expired", lambda: self.__authenticate())
+        self.sio.on("job_response", lambda p: self.job_responses.update({p["id"]: p}))
+        self.sio.on("token_expired", lambda: self.authenticate())
         self.sio.on("auth_error", auth_error)
 
         while self.run_loop:
             try:
                 self.sio.connect(SERVER)
                 self.sio.wait()
             except socketio.exceptions.ConnectionError as e:
```

### Comparing `eezo-0.2.2/eezo/interface/components/chart.py` & `eezo-0.3.3/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.2.2/setup.py` & `eezo-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.2.2",
-    description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
+    version="0.3.3",
+    description="Eezo enables you to build and supervise your AI agent workforces.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
         "async-timeout==4.0.3",
```

