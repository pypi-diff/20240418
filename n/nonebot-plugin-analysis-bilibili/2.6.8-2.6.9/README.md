# Comparing `tmp/nonebot_plugin_analysis_bilibili-2.6.8.tar.gz` & `tmp/nonebot_plugin_analysis_bilibili-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.6.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.6.9.tar", max compression
```

## Comparing `nonebot_plugin_analysis_bilibili-2.6.8.tar` & `nonebot_plugin_analysis_bilibili-2.6.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2738 2024-01-16 10:41:03.782715 nonebot_plugin_analysis_bilibili-2.6.8/README.md
--rw-r--r--   0        0        0     4471 2024-01-16 10:41:03.782715 nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/__init__.py
--rw-r--r--   0        0        0    16850 2024-01-16 10:41:03.782715 nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
--rw-r--r--   0        0        0     2284 2024-01-16 10:41:03.782715 nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/wbi.py
--rw-r--r--   0        0        0      594 2024-01-16 10:41:03.782715 nonebot_plugin_analysis_bilibili-2.6.8/pyproject.toml
--rw-r--r--   0        0        0     3644 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.6.8/PKG-INFO
+-rw-r--r--   0        0        0     2738 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/README.md
+-rw-r--r--   0        0        0     4932 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/__init__.py
+-rw-r--r--   0        0        0    16850 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
+-rw-r--r--   0        0        0     2284 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/wbi.py
+-rw-r--r--   0        0        0      575 2024-04-09 08:50:02.120943 nonebot_plugin_analysis_bilibili-2.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.6.9/PKG-INFO
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/README.md` & `nonebot_plugin_analysis_bilibili-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/__init__.py` & `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import re
 from typing import List, Union
 from aiohttp import ClientSession
-from nonebot import on_regex, logger
+from nonebot import on_regex, logger, require
 from nonebot.adapters import Event
 from nonebot.rule import Rule
+from nonebot.plugin import PluginMetadata
 from .analysis_bilibili import config, b23_extract, bili_keyword, search_bili_by_title
-from nonebot_plugin_saa import MessageFactory, MessageSegmentFactory, Text, Image
+
+require("nonebot_plugin_saa")
+from nonebot_plugin_saa import MessageFactory, MessageSegmentFactory, Text, Image  # noqa: E402
+
+__plugin_meta__ = PluginMetadata(
+    name="analysis_bilibili",
+    description="自动解析bilibili链接内容",
+    usage="https://github.com/mengshouer/nonebot_plugin_analysis_bilibili?tab=readme-ov-file#%E4%BD%BF%E7%94%A8%E6%96%B9%E5%BC%8F",
+    type="application",
+    homepage="https://github.com/mengshouer/nonebot_plugin_analysis_bilibili",
+)
 
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36 Edg/116.0.1938.69"
 }
 
 blacklist = [str(i) for i in getattr(config, "analysis_blacklist", [])]
 group_blacklist = [str(i) for i in getattr(config, "analysis_group_blacklist", [])]
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/analysis_bilibili.py` & `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/nonebot_plugin_analysis_bilibili/wbi.py` & `nonebot_plugin_analysis_bilibili-2.6.9/nonebot_plugin_analysis_bilibili/wbi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/pyproject.toml` & `nonebot_plugin_analysis_bilibili-2.6.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-analysis-bilibili"
-version = "2.6.8"
+version = "2.6.9"
 description = "nonebot2解析bilibili插件"
 authors = ["mengshouer"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/mengshouer/nonebot_plugin_analysis_bilibili"
 keywords = ["nonebot", "nonebot2", "bilibili"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.7"
 nonebot2 = "^2.1.1"
-nonebot-plugin-send-anything-anywhere = [{ version = ">=0.3.2" }]
+nonebot-plugin-send-anything-anywhere = "^0.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_analysis_bilibili-2.6.8/PKG-INFO` & `nonebot_plugin_analysis_bilibili-2.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-analysis-bilibili
-Version: 2.6.8
+Version: 2.6.9
 Summary: nonebot2解析bilibili插件
 Home-page: https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
 License: MIT
 Keywords: nonebot,nonebot2,bilibili
 Author: mengshouer
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.7,<4.0)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3.2)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3,<0.4)
 Requires-Dist: nonebot2 (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
 Description-Content-Type: text/markdown
 
 <!--
  * @Author         : mengshouer
  * @Date           : 2021-03-16 00:00:00
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.6.8
+Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.6.9
 Summary: nonebot2è§£æbilibiliæä»¶ Home-page: https://github.com/mengshouer/
 nonebot_plugin_analysis_bilibili License: MIT Keywords:
 nonebot,nonebot2,bilibili Author: mengshouer Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: aiohttp
-(>=3.7,<4.0) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3.2)
+(>=3.7,<4.0) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.3,<0.4)
 Requires-Dist: nonebot2 (>=2.1.1,<3.0.0) Project-URL: Repository, https://
 github.com/mengshouer/nonebot_plugin_analysis_bilibili Description-Content-
 Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
            # nonebot_plugin_analysis_bilibili _â¨ NoneBot bilibili
                        è§é¢ãçªå§è§£ææä»¶ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
```

