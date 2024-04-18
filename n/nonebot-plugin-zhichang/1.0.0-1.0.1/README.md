# Comparing `tmp/nonebot_plugin_zhichang-1.0.0.tar.gz` & `tmp/nonebot_plugin_zhichang-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zhichang-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_zhichang-1.0.1.tar", max compression
```

## Comparing `nonebot_plugin_zhichang-1.0.0.tar` & `nonebot_plugin_zhichang-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4652 2024-04-18 05:43:51.174735 nonebot_plugin_zhichang-1.0.0/nonebot_plugin_zhichang/__init__.py
--rw-r--r--   0        0        0      468 2024-04-18 05:43:51.058129 nonebot_plugin_zhichang-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.0/README.md
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4652 2024-04-18 05:43:51.174735 nonebot_plugin_zhichang-1.0.1/nonebot_plugin_zhichang/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-18 08:36:41.167260 nonebot_plugin_zhichang-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1913 2024-04-18 05:43:51.029151 nonebot_plugin_zhichang-1.0.1/README.md
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 nonebot_plugin_zhichang-1.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_zhichang-1.0.0/nonebot_plugin_zhichang/__init__.py` & `nonebot_plugin_zhichang-1.0.1/nonebot_plugin_zhichang/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zhichang-1.0.0/README.md` & `nonebot_plugin_zhichang-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zhichang-1.0.0/PKG-INFO` & `nonebot_plugin_zhichang-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-zhichang
-Version: 1.0.0
+Version: 1.0.1
 Summary: 有趣的职场人专属日历
 Author: Priopus
 Author-email: 360048935@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0b1,<3.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0)
 Requires-Dist: nonebot2 (>=2.0.0b2,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-zhichang Version: 1.0.1 Summary:
 æè¶£çèåºäººä¸å±æ¥å Author: Priopus Author-email: 360048935@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0b1,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0b2,<3.0.0)
+apscheduler (>=0.4.0,<0.5.0) Requires-Dist: nonebot2 (>=2.0.0b2,<3.0.0)
 Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-zhichang _â¨ æè¶£çèåºäººä¸å±æ¥å â¨__[_l_i_c_e_n_s_e_]
                                 _[_p_y_p_i_][python]
 ## ð ä»ç» ææå¾ ![example](https://github.com/Priopus/
 nonebot_plugin_zhichang/blob/main/images/8af5b7c09ab1dbd5a9edf66cb6d92d9d.png)
```

