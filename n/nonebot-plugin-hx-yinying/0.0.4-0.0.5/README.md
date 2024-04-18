# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.4.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.4.tar", last modified: Wed Apr 17 16:02:55 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.5.tar", last modified: Wed Apr 17 18:40:05 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.4.tar` & `nonebot-plugin-hx-yinying-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.579310 nonebot-plugin-hx-yinying-0.0.4/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3353 2024-04-17 16:02:55.580311 nonebot-plugin-hx-yinying-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2913 2024-04-17 15:39:35.000000 nonebot-plugin-hx-yinying-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.474057 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1330 2024-04-17 07:14:59.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0     7633 2024-04-17 15:38:59.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      597 2024-04-17 15:33:44.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.571306 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3353 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-17 16:02:55.590216 nonebot-plugin-hx-yinying-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-17 16:02:50.000000 nonebot-plugin-hx-yinying-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:40:05.414411 nonebot-plugin-hx-yinying-0.0.5/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3355 2024-04-17 18:40:05.419298 nonebot-plugin-hx-yinying-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2915 2024-04-17 16:31:33.000000 nonebot-plugin-hx-yinying-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 18:40:05.331616 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     1246 2024-04-17 18:38:55.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0     7633 2024-04-17 15:38:59.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      597 2024-04-17 15:33:44.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:40:05.414411 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3355 2024-04-17 18:40:04.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-17 18:40:05.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 18:40:04.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-17 18:40:04.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 18:40:04.000000 nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-17 18:40:05.428653 nonebot-plugin-hx-yinying-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-17 18:40:01.000000 nonebot-plugin-hx-yinying-0.0.5/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.4/LICENSE` & `nonebot-plugin-hx-yinying-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.4/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
+
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
  * @LastEditors    : huanxin
- * @LastEditTime   : 2024-4-17 00:04:25
+ * @LastEditTime   : 2024-4-18 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.5 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
-img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
+img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
-@LastEditors : huanxin * @LastEditTime : 2024-4-17 00:04:25 * @Description :
+@LastEditors : huanxin * @LastEditTime : 2024-4-18 00:04:25 * @Description :
 None * @GitHub : https://github.com/huanxin -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
```

### Comparing `nonebot-plugin-hx-yinying-0.0.4/README.md` & `nonebot-plugin-hx-yinying-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
+
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
  * @LastEditors    : huanxin
- * @LastEditTime   : 2024-4-17 00:04:25
+ * @LastEditTime   : 2024-4-18 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-[![All Contributors](https://img.shields.io/badge/all_contributors-0-
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-
 orange.svg?style=flat-square)](#contributors-) * @Author : huanxin * @Date :
-2024-4-17 00:04:25 * @LastEditors : huanxin * @LastEditTime : 2024-4-17 00:04:
+2024-4-17 00:04:25 * @LastEditors : huanxin * @LastEditTime : 2024-4-18 00:04:
 25 * @Description : None * @GitHub : https://github.com/huanxin -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
```

### Comparing `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,15 @@
     MessageEvent,
     PrivateMessageEvent,
 )
 from nonebot.log import default_filter, logger, logger_id, sys
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me
 from nonebot.adapters.onebot.v11.event import PrivateMessageEvent, GroupMessageEvent
-from .chat import (
-    gen_chat_text,
-    get_id,
-    send_with_at,
-    finish_with_at,
-    get_answer,
-)
+from .chat import get_answer
 import json,datetime
 hx_config = get_plugin_config(Config)
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
```

### Comparing `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/chat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
+
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
  * @LastEditors    : huanxin
- * @LastEditTime   : 2024-4-17 00:04:25
+ * @LastEditTime   : 2024-4-18 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.5 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
-img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
+img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
-@LastEditors : huanxin * @LastEditTime : 2024-4-17 00:04:25 * @Description :
+@LastEditors : huanxin * @LastEditTime : 2024-4-18 00:04:25 * @Description :
 None * @GitHub : https://github.com/huanxin -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
```

### Comparing `nonebot-plugin-hx-yinying-0.0.4/setup.py` & `nonebot-plugin-hx-yinying-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.4",
+    version="0.0.5",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

