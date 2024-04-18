# Comparing `tmp/nonebot_plugin_zhichang-1.0.2.tar.gz` & `tmp/nonebot_plugin_zhichang-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zhichang-1.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_zhichang-1.0.3.tar", max compression
```

## Comparing `nonebot_plugin_zhichang-1.0.2.tar` & `nonebot_plugin_zhichang-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4691 2024-04-18 08:49:50.428159 nonebot_plugin_zhichang-1.0.2/nonebot_plugin_zhichang/__init__.py
--rw-r--r--   0        0        0      468 2024-04-18 08:50:09.462946 nonebot_plugin_zhichang-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.2/README.md
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4915 2024-04-18 09:03:39.261540 nonebot_plugin_zhichang-1.0.3/nonebot_plugin_zhichang/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-18 09:03:56.298913 nonebot_plugin_zhichang-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.3/README.md
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_zhichang-1.0.2/nonebot_plugin_zhichang/__init__.py` & `nonebot_plugin_zhichang-1.0.3/nonebot_plugin_zhichang/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,22 @@
     import json
 
 require("nonebot_plugin_apscheduler")
 
 from nonebot_plugin_apscheduler import scheduler
 from nonebot.plugin import PluginMeta
 
+__plugin_meta__ = PluginMeta(
+    name="职场日历",
+    description="有趣的职场人专属日历",
+    usage="职场日历",
+    type="application",
+    homepage="https://github.com/Priopus/nonebot-plugin-zhichang"
+)
+
 
 subscribe = Path(__file__).parent / "subscribe.json"
 
 subscribe_list = json.loads(subscribe.read_text("utf-8")) if subscribe.is_file() else {}
 
 
 def save_subscribe():
```

### Comparing `nonebot_plugin_zhichang-1.0.2/README.md` & `nonebot_plugin_zhichang-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zhichang-1.0.2/PKG-INFO` & `nonebot_plugin_zhichang-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-zhichang
-Version: 1.0.2
+Version: 1.0.3
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
-Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.3 Summary:
 æè¶£çèåºäººä¸å±æ¥å Author: Priopus Author-email: 360048935@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0b1,<3.0.0) Requires-Dist: nonebot-plugin-
```

