# Comparing `tmp/nonebot-plugin-yinying-chat-1.0.5.tar.gz` & `tmp/nonebot-plugin-yinying-chat-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-yinying-chat-1.0.5.tar", last modified: Thu Apr 18 06:59:03 2024, max compression
+gzip compressed data, was "nonebot-plugin-yinying-chat-1.0.6.tar", last modified: Thu Apr 18 07:03:21 2024, max compression
```

## Comparing `nonebot-plugin-yinying-chat-1.0.5.tar` & `nonebot-plugin-yinying-chat-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 06:59:03.615512 nonebot-plugin-yinying-chat-1.0.5/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 06:59:03.615512 nonebot-plugin-yinying-chat-1.0.5/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)     1296 2024-04-17 22:04:25.000000 nonebot-plugin-yinying-chat-1.0.5/README.md
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 06:59:03.615512 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/
--rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/ChatSession.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)     4954 2024-04-18 06:58:40.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/__init__.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)      527 2024-04-17 21:45:11.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/config.py
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 06:59:03.615512 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 06:59:03.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 06:59:03.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 06:59:03.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 06:59:03.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/requires.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 06:59:03.000000 nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat.egg-info/top_level.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)      531 2024-04-18 06:58:03.000000 nonebot-plugin-yinying-chat-1.0.5/pyproject.toml
--rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 06:59:03.615512 nonebot-plugin-yinying-chat-1.0.5/setup.cfg
--rw-r--r--   0 stafx     (1000) stafx     (1000)      399 2024-04-18 06:58:08.000000 nonebot-plugin-yinying-chat-1.0.5/setup.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:03:21.405510 nonebot-plugin-yinying-chat-1.0.6/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:03:21.405510 nonebot-plugin-yinying-chat-1.0.6/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     1296 2024-04-17 22:04:25.000000 nonebot-plugin-yinying-chat-1.0.6/README.md
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:03:21.405510 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/ChatSession.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     4930 2024-04-18 07:02:38.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/__init__.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      527 2024-04-17 21:45:11.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/config.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:03:21.405510 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:03:21.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 07:03:21.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 07:03:21.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 07:03:21.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/requires.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 07:03:21.000000 nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat.egg-info/top_level.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      531 2024-04-18 07:02:59.000000 nonebot-plugin-yinying-chat-1.0.6/pyproject.toml
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 07:03:21.405510 nonebot-plugin-yinying-chat-1.0.6/setup.cfg
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      399 2024-04-18 07:02:53.000000 nonebot-plugin-yinying-chat-1.0.6/setup.py
```

### Comparing `nonebot-plugin-yinying-chat-1.0.5/README.md` & `nonebot-plugin-yinying-chat-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/ChatSession.py` & `nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/ChatSession.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/__init__.py` & `nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from nonebot.adapters.onebot.v11.event import Event, MessageEvent, PrivateMessageEvent,GroupMessageEvent
 from .config import Config, ConfigError
 from .ChatSession import ChatSession
 from nonebot.plugin import PluginMetadata
 
 # 定义插件元数据
 plugin_metadata = PluginMetadata(
-    name="MyPlugin", 
+    name="Yuanluo", 
     description="这是一个通过调用银影API来和银影聊天的插件",  
-    version="1.0.5", 
     type="application",
     usage="快来和银影聊天吧~", 
     homepage="https://github.com/YuxiCN/nonebot_plugin_yinying_chat",
     supported_adapters={"~onebot.v11"}
     
 )
```

### Comparing `nonebot-plugin-yinying-chat-1.0.5/nonebot_plugin_yinying_chat/config.py` & `nonebot-plugin-yinying-chat-1.0.6/nonebot_plugin_yinying_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.5/pyproject.toml` & `nonebot-plugin-yinying-chat-1.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-yinying-chat"
-version = "1.0.5"
+version = "1.0.6"
 description = "A nonebot plugin for yinying-chat"
 authors = ["Yuanluo <3313512421@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

