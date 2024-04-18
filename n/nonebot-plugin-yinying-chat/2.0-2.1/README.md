# Comparing `tmp/nonebot-plugin-yinying-chat-2.0.tar.gz` & `tmp/nonebot-plugin-yinying-chat-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-yinying-chat-2.0.tar", last modified: Thu Apr 18 08:48:57 2024, max compression
+gzip compressed data, was "nonebot-plugin-yinying-chat-2.1.tar", last modified: Thu Apr 18 14:31:27 2024, max compression
```

## Comparing `nonebot-plugin-yinying-chat-2.0.tar` & `nonebot-plugin-yinying-chat-2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 08:48:57.941996 nonebot-plugin-yinying-chat-2.0/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-18 08:48:57.941996 nonebot-plugin-yinying-chat-2.0/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      968 2024-04-16 04:48:34.000000 nonebot-plugin-yinying-chat-2.0/README.md
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 08:48:57.941996 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/
--rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/ChatSession.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)     4440 2024-04-17 15:27:29.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/__init__.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)      588 2024-04-18 08:46:46.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/config.py
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 08:48:57.941996 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-18 08:48:57.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 08:48:57.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 08:48:57.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 08:48:57.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/requires.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 08:48:57.000000 nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat.egg-info/top_level.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)      529 2024-04-18 08:48:39.000000 nonebot-plugin-yinying-chat-2.0/pyproject.toml
--rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 08:48:57.941996 nonebot-plugin-yinying-chat-2.0/setup.cfg
--rw-r--r--   0 stafx     (1000) stafx     (1000)      397 2024-04-18 08:48:10.000000 nonebot-plugin-yinying-chat-2.0/setup.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 14:31:27.787864 nonebot-plugin-yinying-chat-2.1/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-18 14:31:27.787864 nonebot-plugin-yinying-chat-2.1/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      968 2024-04-16 04:48:34.000000 nonebot-plugin-yinying-chat-2.1/README.md
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 14:31:27.787864 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/ChatSession.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     4834 2024-04-18 14:29:21.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/__init__.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      588 2024-04-18 08:46:46.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/config.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 14:31:27.787864 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      235 2024-04-18 14:31:27.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 14:31:27.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 14:31:27.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 14:31:27.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/requires.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 14:31:27.000000 nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat.egg-info/top_level.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      548 2024-04-18 14:31:15.000000 nonebot-plugin-yinying-chat-2.1/pyproject.toml
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 14:31:27.787864 nonebot-plugin-yinying-chat-2.1/setup.cfg
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      397 2024-04-18 14:31:08.000000 nonebot-plugin-yinying-chat-2.1/setup.py
```

### Comparing `nonebot-plugin-yinying-chat-2.0/README.md` & `nonebot-plugin-yinying-chat-2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/ChatSession.py` & `nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/ChatSession.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/__init__.py` & `nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,27 @@
 
 from nonebot import on_command, on_message
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, Bot
 from nonebot.adapters.onebot.v11.event import Event, MessageEvent, PrivateMessageEvent,GroupMessageEvent
 from .config import Config, ConfigError
 from .ChatSession import ChatSession
+from nonebot.plugin import PluginMetadata
 
 
+# 定义插件元数据
+plugin_metadata = PluginMetadata(
+    name="Yuanluo", 
+    description="这是一个通过调用银影API来和银影聊天的插件",  
+    type="application",
+    usage="快来和银影聊天吧~", 
+    homepage="https://github.com/YuxiCN/nonebot_plugin_yinying_chat",
+    supported_adapters={"~onebot.v11"}
+    
+)
 
 # 配置导入
 plugin_config = Config.parse_obj(nonebot.get_driver().config.dict())
 
 # 导入设置内的API，模型名称，AppID
 yinying_api_key = plugin_config.yinying_api_key
 yinying_model_name = plugin_config.yinying_model_name
```

### Comparing `nonebot-plugin-yinying-chat-2.0/nonebot_plugin_yinying_chat/config.py` & `nonebot-plugin-yinying-chat-2.1/nonebot_plugin_yinying_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-2.0/pyproject.toml` & `nonebot-plugin-yinying-chat-2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-yinying-chat"
-version = "2.0"
+version = "2.1"
 description = "A nonebot plugin for yinying-chat"
 authors = ["Yuanluo <3313512421@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
+openai = "^0.27.0"
 aiohttp = "^3.8.4"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

