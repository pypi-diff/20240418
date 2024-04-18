# Comparing `tmp/nonebot_plugin_zhichang-1.0.1.tar.gz` & `tmp/nonebot_plugin_zhichang-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zhichang-1.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_zhichang-1.0.2.tar", max compression
```

## Comparing `nonebot_plugin_zhichang-1.0.1.tar` & `nonebot_plugin_zhichang-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4652 2024-04-18 05:43:51.174735 nonebot_plugin_zhichang-1.0.1/nonebot_plugin_zhichang/__init__.py
--rw-r--r--   0        0        0      468 2024-04-18 08:36:41.167260 nonebot_plugin_zhichang-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.1/README.md
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4691 2024-04-18 08:49:50.428159 nonebot_plugin_zhichang-1.0.2/nonebot_plugin_zhichang/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-18 08:50:09.462946 nonebot_plugin_zhichang-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.2/README.md
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_zhichang-1.0.1/nonebot_plugin_zhichang/__init__.py` & `nonebot_plugin_zhichang-1.0.2/nonebot_plugin_zhichang/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     import ujson as json
 except ModuleNotFoundError:
     import json
 
 require("nonebot_plugin_apscheduler")
 
 from nonebot_plugin_apscheduler import scheduler
+from nonebot.plugin import PluginMeta
+
 
 subscribe = Path(__file__).parent / "subscribe.json"
 
 subscribe_list = json.loads(subscribe.read_text("utf-8")) if subscribe.is_file() else {}
 
 
 def save_subscribe():
```

### Comparing `nonebot_plugin_zhichang-1.0.1/README.md` & `nonebot_plugin_zhichang-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zhichang-1.0.1/PKG-INFO` & `nonebot_plugin_zhichang-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-zhichang
-Version: 1.0.1
+Version: 1.0.2
 Summary: 有趣的职场人专属日历
 Author: Priopus
 Author-email: 360048935@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.2 Summary:
 æè¶£çèåºäººä¸å±æ¥å Author: Priopus Author-email: 360048935@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0b1,<3.0.0) Requires-Dist: nonebot-plugin-
```

