# Comparing `tmp/nonebot_plugin_yinyu-0.0.2.tar.gz` & `tmp/nonebot_plugin_yinyu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_yinyu-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_yinyu-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_yinyu-0.0.2.tar` & `nonebot_plugin_yinyu-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-17 14:31:44.000000 nonebot_plugin_yinyu-0.0.2/LICENSE
--rw-r--r--   0        0        0      982 2024-04-17 14:31:44.000000 nonebot_plugin_yinyu-0.0.2/nonebot_plugin_yinyu/_init_.py
--rw-r--r--   0        0        0      619 2024-04-17 14:31:44.000000 nonebot_plugin_yinyu-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-17 14:31:44.000000 nonebot_plugin_yinyu-0.0.2/README.md
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 nonebot_plugin_yinyu-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.3/LICENSE
+-rw-r--r--   0        0        0      935 2024-04-18 01:24:51.003306 nonebot_plugin_yinyu-0.0.3/nonebot_plugin_yinyu/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-18 01:39:31.047968 nonebot_plugin_yinyu-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-17 11:43:42.000000 nonebot_plugin_yinyu-0.0.3/README.md
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 nonebot_plugin_yinyu-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_yinyu-0.0.2/LICENSE` & `nonebot_plugin_yinyu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yinyu-0.0.2/pyproject.toml` & `nonebot_plugin_yinyu-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-yinyu"
-version = "0.0.2"
+version = "0.0.3"
 description = "一个语句瑟瑟化插件"
 authors = ["shiyingyingjiang <2798134864@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_yinyu"}]
 homepage = "https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu"
 repository = "https://github.com/shi-yingyingjiang/nonebot-plugin-yinyu"
```

### Comparing `nonebot_plugin_yinyu-0.0.2/README.md` & `nonebot_plugin_yinyu-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yinyu-0.0.2/PKG-INFO` & `nonebot_plugin_yinyu-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-yinyu
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: nonebot-plugin-yinyu Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-yinyu Version: 0.0.3 Summary:
 ä¸ä¸ªè¯­å¥ççåæä»¶ Home-page: https://github.com/shi-yingyingjiang/
 nonebot-plugin-yinyu License: MIT Author: shiyingyingjiang Author-email:
 2798134864@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

