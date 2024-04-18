# Comparing `tmp/omuchatprovider-0.2.4.tar.gz` & `tmp/omuchatprovider-0.2.5.tar.gz`

## Comparing `omuchatprovider-0.2.4.tar` & `omuchatprovider-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,35 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.python-version
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/run.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.vscode/launch.json
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/__main__.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/chatprovider.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/errors.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/helper.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/service.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/__init__.py
--rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/types/__init__.py
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/types/api.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/tasks/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/tasks/taskprofiler.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/__main__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/chatprovider.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/errors.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/helper.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/tasks.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/throttle.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/service.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/__init__.py
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/chat.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/const.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtube.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtubeapi.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/accessibility.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/chatactions.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/contents.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/continuations.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/frameworkupdates.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/image.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/live_chat.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/metadataactions.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/responsecontext.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/runs.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/simpletext.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/updated_metadata.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/urlendpoint.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/youtuberesponse.py
+-rw-r--r--   0        0        0    40286 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/ytcfg.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/PKG-INFO
```

### Comparing `omuchatprovider-0.2.4/src/omuchatprovider/chatprovider.py` & `omuchatprovider-0.2.5/src/omuchatprovider/chatprovider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import asyncio
 import time
+from typing import Dict
 
 from loguru import logger
 from omu.identifier import Identifier
 from omuchat import App, Channel, Client, Message, Room, events
 
 from omuchatprovider.errors import ProviderError
 
 from .services import ChatService, ProviderService, get_services
 
-IDENTIFIER = Identifier("cc.omuchat", "chatprovider")
+BASE_PROVIDER_IDENTIFIER = Identifier("cc.omuchat", "chatprovider")
 APP = App(
-    identifier=IDENTIFIER,
+    identifier=BASE_PROVIDER_IDENTIFIER,
     version="0.1.0",
 )
 
 
 client = Client(APP)
-services: dict[str, ProviderService] = {}
-chats: dict[str, ChatService] = {}
+
+services: Dict[str, ProviderService] = {}
+chat_services: Dict[Identifier, ChatService] = {}
 
 
 async def register_services():
     for service_class in get_services():
         service = service_class(client)
-        services[service.info.key()] = service
-        await client.chat.providers.add(service.info)
+        services[service.provider.key()] = service
+        await client.chat.providers.add(service.provider)
 
 
 async def update_channel(channel: Channel, service: ProviderService):
     try:
         if not channel.active:
             return
-        available_rooms = await service.fetch_rooms(channel)
-        for room, create_chat in available_rooms.items():
-            if room.key() in chats:
+        fetched_rooms = await service.fetch_rooms(channel)
+        for item in fetched_rooms:
+            if item.room.id in chat_services:
                 continue
-            chat = await create_chat()
-            chats[room.key()] = chat
+            chat = await item.create()
+            chat_services[item.room.id] = chat
             asyncio.create_task(chat.start())
-            logger.info(f"Started chat for {room.key()}")
+            logger.info(f"Started chat for {item.room.key()}")
     except ProviderError as e:
         logger.error(f"Failed to update channel {channel.id}: {e}")
 
 
 @client.on(events.channel.add)
 async def on_channel_create(channel: Channel):
     provider = get_provider(channel)
@@ -79,34 +81,34 @@
     while True:
         await recheck_channels()
         await recheck_rooms()
         await delay()
 
 
 async def recheck_rooms():
-    for chat in tuple(chats.values()):
+    for chat in tuple(chat_services.values()):
         if chat.closed:
-            del chats[chat.room.key()]
+            del chat_services[chat.room.id]
     rooms = await client.chat.rooms.fetch_items()
     for room in filter(lambda r: r.connected, rooms.values()):
         if room.provider_id not in services:
             continue
         if not await should_remove(room, services[room.provider_id]):
             continue
         await stop_room(room)
 
 
 async def stop_room(room: Room):
     room.status = "offline"
     room.connected = False
     await client.chat.rooms.update(room)
-    for key, chat in tuple(chats.items()):
+    for key, chat in tuple(chat_services.items()):
         if chat.room.key() == room.key():
             await chat.stop()
-            del chats[key]
+            del chat_services[key]
 
 
 async def should_remove(room: Room, provider_service: ProviderService):
     if room.channel_id is None:
         return False
     channel = await client.chat.channels.get(room.channel_id)
     if channel and not channel.active:
```

### Comparing `omuchatprovider-0.2.4/src/omuchatprovider/tasks/taskprofiler.py` & `omuchatprovider-0.2.5/src/omuchatprovider/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def create_task(self, coro: typing.Coroutine):
         name = coro.__name__
 
         async def wrapper():
             start_time = time.time()
             try:
                 await coro
-            except Exception as e:
+            except BaseException as e:
                 traceback.print_exc()
                 raise Exception(f"Task {name} failed") from e
             finally:
                 self.times[name] = time.time() - start_time
                 self.times_max[name] = max(
                     self.times_max.get(name, 0), self.times[name]
                 )
```

### Comparing `omuchatprovider-0.2.4/pyproject.toml` & `omuchatprovider-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuchatprovider"
-version = "0.2.4"
+version = "0.2.5"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "aiohttp>=3.9.1",
     "beautifulsoup4>=4.12.2",
```

