# Comparing `tmp/nonebot-plugin-sendmsg-by-bots-0.1.3.tar.gz` & `tmp/nonebot-plugin-sendmsg-by-bots-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.1.3.tar", last modified: Fri Mar 22 03:14:15 2024, max compression
+gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.1.4.tar", last modified: Thu Apr 18 11:17:53 2024, max compression
```

## Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3.tar` & `nonebot-plugin-sendmsg-by-bots-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2800 2024-03-22 03:14:12.232877 nonebot-plugin-sendmsg-by-bots-0.1.3/README.md
--rw-r--r--   0        0        0     1976 2024-03-22 03:14:12.232877 nonebot-plugin-sendmsg-by-bots-0.1.3/nonebot_plugin_sendmsg_by_bots/__init__.py
--rw-r--r--   0        0        0      336 2024-03-22 03:14:12.232877 nonebot-plugin-sendmsg-by-bots-0.1.3/nonebot_plugin_sendmsg_by_bots/config.py
--rw-r--r--   0        0        0     8999 2024-03-22 03:14:12.232877 nonebot-plugin-sendmsg-by-bots-0.1.3/nonebot_plugin_sendmsg_by_bots/tools.py
--rw-r--r--   0        0        0      575 2024-03-22 03:14:12.232877 nonebot-plugin-sendmsg-by-bots-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2800 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/README.md
+-rw-r--r--   0        0        0     1976 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/__init__.py
+-rw-r--r--   0        0        0      336 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/config.py
+-rw-r--r--   0        0        0     9007 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/tools.py
+-rw-r--r--   0        0        0      575 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.1.4/PKG-INFO
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3/README.md` & `nonebot-plugin-sendmsg-by-bots-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3/nonebot_plugin_sendmsg_by_bots/__init__.py` & `nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3/nonebot_plugin_sendmsg_by_bots/tools.py` & `nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,25 +195,24 @@
     '''转为拉格兰markdown消息发生'''
     md_text = {
              "type": "markdown",
              "data": {
                "content": '{"content":"' + repr(text)[1:-1].replace('\"','\\"').replace("\'","\\'") + '"}'
              }
            }
-    md_node = MessageSegment.node_custom(user_id=10000,nickname="测试",content=[md_text])
-    md = MessageSegment.node_custom_lgr(md_node)
-    bot = current_bot.get()
-    res_id = await bot.call_api("send_forward_msg", messages=md)
-    lmsg = {
-            "type": "longmsg",
-            "data": {
-                "id": res_id
-            }
-        }
-   #  return lmsg
+    # md_node = MessageSegment.node_custom(user_id=10000,nickname="测试",content=[md_text])
+    # md = MessageSegment.node_custom_lgr(md_node)
+    # bot = current_bot.get()
+    # res_id = await bot.call_api("send_forward_msg", messages=md)
+    # lmsg = {
+    #         "type": "longmsg",
+    #         "data": {
+    #             "id": res_id
+    #         }
+    #     }
     event = current_event.get()
     if isinstance(event,GroupMessageEvent):
-        await send_group_msg_by_bots_once(group_id=event.group_id,msg=[lmsg],self_id=bot_id)
+        await send_group_msg_by_bots_once(group_id=event.group_id,msg=[md_text],self_id=bot_id)
         # await bot.call_api("send_group_msg",group_id=event.group_id,message=[lmsg])
     else:
-        await send_private_msg_by_bots_once(user_id=event.user_id,msg=[lmsg],self_id=bot_id)
+        await send_private_msg_by_bots_once(user_id=event.user_id,msg=[md_text],self_id=bot_id)
         # await bot.call_api("send_private_msg",user_id=event.user_id,message=[lmsg])
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3/pyproject.toml` & `nonebot-plugin-sendmsg-by-bots-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sendmsg-by-bots"
-version = "0.1.3"
+version = "0.1.4"
 description = "a send msg tools"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.3/PKG-INFO` & `nonebot-plugin-sendmsg-by-bots-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sendmsg-by-bots
-Version: 0.1.3
+Version: 0.1.4
 Summary: a send msg tools
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.1.4
 Summary: a send msg tools License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-sendmsg-by-bots Project-URL: Repository, https://
 github.com/nek0us/nonebot-plugin-sendmsg-by-bots Description-Content-Type:
 text/markdown
                              x_[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
```

