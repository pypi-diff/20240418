# Comparing `tmp/THISDLChatBot-2.0.8.tar.gz` & `tmp/THISDLChatBot-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.8.tar", last modified: Sun Apr 14 13:29:31 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.9.tar", last modified: Wed Apr 17 06:00:37 2024, max compression
```

## Comparing `THISDLChatBot-2.0.8.tar` & `THISDLChatBot-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 13:29:31.642817 THISDLChatBot-2.0.8/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 13:29:31.642586 THISDLChatBot-2.0.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 13:29:31.641245 THISDLChatBot-2.0.8/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    31040 2024-04-14 11:10:21.000000 THISDLChatBot-2.0.8/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.8/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2675 2024-04-14 13:29:19.000000 THISDLChatBot-2.0.8/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.8/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 13:29:31.642292 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 13:29:31.000000 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 13:29:31.000000 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 13:29:31.000000 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 13:29:31.000000 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 13:29:31.000000 THISDLChatBot-2.0.8/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 13:29:31.642867 THISDLChatBot-2.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 13:21:55.000000 THISDLChatBot-2.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 06:00:37.993636 THISDLChatBot-2.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-17 06:00:37.993359 THISDLChatBot-2.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 06:00:37.991935 THISDLChatBot-2.0.9/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    31071 2024-04-17 05:58:14.000000 THISDLChatBot-2.0.9/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.9/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-04-14 13:29:19.000000 THISDLChatBot-2.0.9/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      861 2024-04-17 05:58:40.000000 THISDLChatBot-2.0.9/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.9/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 06:00:37.993069 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-17 06:00:37.000000 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-17 06:00:37.000000 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-17 06:00:37.000000 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-17 06:00:37.000000 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-17 06:00:37.000000 THISDLChatBot-2.0.9/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-17 06:00:37.993684 THISDLChatBot-2.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-17 06:00:33.000000 THISDLChatBot-2.0.9/setup.py
```

### Comparing `THISDLChatBot-2.0.8/LICENSE` & `THISDLChatBot-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/README.md` & `THISDLChatBot-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,30 +28,31 @@
             messages = await self._GetMessages()
             for RawMessage in messages:
                 message = Message(RawMessage, self)
                 await self._UpdatePointer(message)
                 if (await message.GetFromUser()).GetUserId() == self.userid:
                     continue
                 if message.IsCommand():
-                    await self._CommandProcessor(message)
+                    self._CommandProcessor(message)
                 if message.GetType() == 'MessageEventFriendRequest' and self.config['auto_accept']:
                     await self.Accept(True, (await message.GetFromUser()).GetUserId())
-                await self._MessageProcessor(message)
+                self._MessageProcessor(message)
             await asyncio.sleep(self.config['wait_time'] / 1000)
 
-    async def _CommandProcessor(self, message: Message):
+    def _CommandProcessor(self, message: Message):
         for plugin in self.plugins:
             for commandProcessor in plugin.CommandProcessors:
                 if (message.GetData() + ' ').startswith(f'/{commandProcessor.command} '):
-                    await commandProcessor.Process((message.GetData() + ' ').split(' ')[1:], message, self)
+                    asyncio.create_task(
+                        commandProcessor.Process((message.GetData() + ' ').split(' ')[1:], message, self))
 
-    async def _MessageProcessor(self, message: Message):
+    def _MessageProcessor(self, message: Message):
         for plugin in self.plugins:
             for messageProcessor in plugin.MessageProcessors:
-                await messageProcessor.Process(message, self)
+                asyncio.create_task(messageProcessor.Process(message, self))
 
     async def _UpdatePointer(self, message: Message):
         if message.GetRoomType() == 'Private':
             await self._httpclient.post(
                 url="http://chat.thisit.cc/index.php?action=im.cts.updatePointer&body_format=json&lang=1",
                 json={
                     "action": "im.cts.updatePointer",
```

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Message.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.8/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.9/THISDLChatBot/Plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from .CommandProcessor import CommandProcessor
 from .MessageProcessor import MessageProcessor
 
+
 class Plugin:
     def __init__(self, name: str) -> None:
         self.name = name
         self.CommandProcessors = []
         self.MessageProcessors = []
         self.bot = None
 
     async def OnLoad(self):
         pass
 
     def OnCommand(self, command: str):
         def commandProcessor(func):
             def wrapper():
                 self.CommandProcessors.append(CommandProcessor(command, func))
+
             return wrapper()
+
         return commandProcessor
 
     def OnMessage(self):
         def messageProcessor(func):
             def wrapper():
                 self.MessageProcessors.append(MessageProcessor(func))
+
             return wrapper()
+
         return messageProcessor
 
 
 def LoadPlugin(plugin: str) -> Plugin:
     return __import__(plugin).plugin
```

