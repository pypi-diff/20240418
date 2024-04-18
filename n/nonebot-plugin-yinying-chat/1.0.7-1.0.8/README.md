# Comparing `tmp/nonebot-plugin-yinying-chat-1.0.7.tar.gz` & `tmp/nonebot-plugin-yinying-chat-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-yinying-chat-1.0.7.tar", last modified: Thu Apr 18 07:06:38 2024, max compression
+gzip compressed data, was "nonebot-plugin-yinying-chat-1.0.8.tar", last modified: Thu Apr 18 07:11:59 2024, max compression
```

## Comparing `nonebot-plugin-yinying-chat-1.0.7.tar` & `nonebot-plugin-yinying-chat-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:06:38.265509 nonebot-plugin-yinying-chat-1.0.7/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:06:38.265509 nonebot-plugin-yinying-chat-1.0.7/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)     1296 2024-04-17 22:04:25.000000 nonebot-plugin-yinying-chat-1.0.7/README.md
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:06:38.265509 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/
--rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/ChatSession.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)     4832 2024-04-18 07:05:50.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/__init__.py
--rw-r--r--   0 stafx     (1000) stafx     (1000)      527 2024-04-17 21:45:11.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/config.py
-drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:06:38.265509 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/
--rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:06:38.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
--rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 07:06:38.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 07:06:38.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 07:06:38.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/requires.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 07:06:38.000000 nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat.egg-info/top_level.txt
--rw-r--r--   0 stafx     (1000) stafx     (1000)      531 2024-04-18 07:06:23.000000 nonebot-plugin-yinying-chat-1.0.7/pyproject.toml
--rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 07:06:38.265509 nonebot-plugin-yinying-chat-1.0.7/setup.cfg
--rw-r--r--   0 stafx     (1000) stafx     (1000)      399 2024-04-18 07:06:29.000000 nonebot-plugin-yinying-chat-1.0.7/setup.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:11:59.105508 nonebot-plugin-yinying-chat-1.0.8/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:11:59.105508 nonebot-plugin-yinying-chat-1.0.8/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     1296 2024-04-17 22:04:25.000000 nonebot-plugin-yinying-chat-1.0.8/README.md
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:11:59.105508 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     2413 2024-04-17 15:23:28.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/ChatSession.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)     4832 2024-04-18 07:05:50.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/__init__.py
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      572 2024-04-18 07:10:54.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/config.py
+drwxr-xr-x   0 stafx     (1000) stafx     (1000)        0 2024-04-18 07:11:59.105508 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      237 2024-04-18 07:11:59.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/PKG-INFO
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      408 2024-04-18 07:11:59.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)        1 2024-04-18 07:11:59.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       64 2024-04-18 07:11:59.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/requires.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       28 2024-04-18 07:11:59.000000 nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat.egg-info/top_level.txt
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      531 2024-04-18 07:11:30.000000 nonebot-plugin-yinying-chat-1.0.8/pyproject.toml
+-rw-r--r--   0 stafx     (1000) stafx     (1000)       38 2024-04-18 07:11:59.105508 nonebot-plugin-yinying-chat-1.0.8/setup.cfg
+-rw-r--r--   0 stafx     (1000) stafx     (1000)      399 2024-04-18 07:11:25.000000 nonebot-plugin-yinying-chat-1.0.8/setup.py
```

### Comparing `nonebot-plugin-yinying-chat-1.0.7/README.md` & `nonebot-plugin-yinying-chat-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/ChatSession.py` & `nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/ChatSession.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/__init__.py` & `nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-yinying-chat-1.0.7/nonebot_plugin_yinying_chat/config.py` & `nonebot-plugin-yinying-chat-1.0.8/nonebot_plugin_yinying_chat/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,7 +9,9 @@
     yinying_app_id: Optional[str] = ""    #在这里输入AppID
     enable_private_chat: bool = True    #是否开启私聊
     yinying_chat_public: bool = False  # 群聊是否开启公共会话
 
 
 class ConfigError(Exception):
     pass
+
+global_config = nonebot.get_driver().config
```

### Comparing `nonebot-plugin-yinying-chat-1.0.7/pyproject.toml` & `nonebot-plugin-yinying-chat-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-yinying-chat"
-version = "1.0.7"
+version = "1.0.8"
 description = "A nonebot plugin for yinying-chat"
 authors = ["Yuanluo <3313512421@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

