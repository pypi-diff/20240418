# Comparing `tmp/nonebot_plugin_yinyu-0.0.3.tar.gz` & `tmp/nonebot_plugin_yinyu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_yinyu-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_yinyu-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_yinyu-0.0.3.tar` & `nonebot_plugin_yinyu-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.3/LICENSE
--rw-r--r--   0        0        0      935 2024-04-18 01:24:51.003306 nonebot_plugin_yinyu-0.0.3/nonebot_plugin_yinyu/__init__.py
--rw-r--r--   0        0        0      619 2024-04-18 01:39:31.047968 nonebot_plugin_yinyu-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.3/README.md
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 nonebot_plugin_yinyu-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.4/LICENSE
+-rw-r--r--   0        0        0      879 2024-04-18 02:23:34.772118 nonebot_plugin_yinyu-0.0.4/nonebot_plugin_yinyu/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-18 02:24:42.869854 nonebot_plugin_yinyu-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.4/README.md
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 nonebot_plugin_yinyu-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_yinyu-0.0.3/LICENSE` & `nonebot_plugin_yinyu-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yinyu-0.0.3/nonebot_plugin_yinyu/__init__.py` & `nonebot_plugin_yinyu-0.0.4/nonebot_plugin_yinyu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 __plugin_meta__ = PluginMetadata(
     name="淫语",
     description="把语句变成淫语",
     usage="淫语",
     type="application",
     homepage="https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu",
-    supported_adapters={"nonebot.adapters.onebot.v11"},
 )
 
 body = on_command("淫语")
 
 
 @body.handle()
 async def handle_first_receive(arg: Message = CommandArg()):
```

### Comparing `nonebot_plugin_yinyu-0.0.3/pyproject.toml` & `nonebot_plugin_yinyu-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-yinyu"
-version = "0.0.3"
+version = "0.0.4"
 description = "一个语句瑟瑟化插件"
 authors = ["shiyingyingjiang <2798134864@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_yinyu"}]
 homepage = "https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu"
 repository = "https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu"
```

### Comparing `nonebot_plugin_yinyu-0.0.3/README.md` & `nonebot_plugin_yinyu-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yinyu-0.0.3/PKG-INFO` & `nonebot_plugin_yinyu-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-yinyu
-Version: 0.0.3
+Version: 0.0.4
 Summary: 一个语句瑟瑟化插件
 Home-page: https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu
 License: MIT
 Author: shiyingyingjiang
 Author-email: 2798134864@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-yinyu Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-yinyu Version: 0.0.4 Summary:
 ä¸ä¸ªè¯­å¥ççåæä»¶ Home-page: https://github.com/shi-yingyingjiang/
 nonebot-plugin-yinyu License: MIT Author: shiyingyingjiang Author-email:
 2798134864@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```
