# Comparing `tmp/tsugu-0.5.4.tar.gz` & `tmp/tsugu-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.5.4.tar", last modified: Wed Apr 17 07:43:22 2024, max compression
+gzip compressed data, was "tsugu-0.5.5.tar", last modified: Wed Apr 17 13:43:17 2024, max compression
```

## Comparing `tsugu-0.5.4.tar` & `tsugu-0.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 07:43:12.000000 tsugu-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:43:22.974630 tsugu-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 07:43:12.000000 tsugu-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:43:22.974630 tsugu-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 07:43:12.000000 tsugu-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 07:43:12.000000 tsugu-0.5.4/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    21682 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:43:17.280736 tsugu-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 13:43:08.000000 tsugu-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-17 13:43:17.280736 tsugu-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-17 13:43:08.000000 tsugu-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:43:17.280736 tsugu-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 13:43:08.000000 tsugu-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:43:17.276736 tsugu-0.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 13:43:08.000000 tsugu-0.5.5/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:43:17.280736 tsugu-0.5.5/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 13:43:08.000000 tsugu-0.5.5/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 13:43:08.000000 tsugu-0.5.5/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-17 13:43:08.000000 tsugu-0.5.5/tsugu/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 13:43:08.000000 tsugu-0.5.5/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21858 2024-04-17 13:43:08.000000 tsugu-0.5.5/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:43:17.280736 tsugu-0.5.5/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-17 13:43:17.000000 tsugu-0.5.5/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 13:43:17.000000 tsugu-0.5.5/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:43:17.000000 tsugu-0.5.5/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 13:43:17.000000 tsugu-0.5.5/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 13:43:17.000000 tsugu-0.5.5/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.5.4/LICENSE` & `tsugu-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.4/PKG-INFO` & `tsugu-0.5.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.4
+Version: 0.5.5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -31,15 +31,15 @@
         
         ***
         
         <h2 align="center"> 实现 </h2>
         
         
         - [x] 自然语言输入 -> 返回结果
-        - [ ] 独立路由输入 -> 返回结果 `目前仅基础路由`
+        - [ ] 独立路由输入 -> 返回结果 `部分支持`
         - [x] 本地数据库 (sqlite3)
         - [x] 远程数据库 (客户端)
         - [x] 配置项 (基础配置、代理、命令别名 等)
         
         
         <h2 align="center"> 安装与更新 </h2>
         
@@ -69,145 +69,155 @@
         
         
         <h2 align="center"> 测试与调用 </h2>
         
         
         
         
-        ## 调用 `tsugu.bot`
+        ## 调用 `tsugu.handler`
         
-        - `bot` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
+        - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
-        import base64
-        from PIL import Image
         import io
-        
         import tsugu
         
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
-        data = tsugu.bot('查卡 红 ksm 5x', '114514', 'red', '666808414')
-        
-        # 如果返回值为 None 代表bot不发送任何消息。
-        if not data:
-            print("[无反馈数据]")
-        
-        for item in data:
-            if item["type"] == "string":
-                print(f"[文字信息]\n{item['string']}")
-            elif item["type"] == "base64":
-                image_data = base64.b64decode(item["string"])
-                print(f"[图像大小: {len(image_data) / 1024:.2f}KB]")
-                Image.open(io.BytesIO(image_data)).show()
-            else:
-                print(item)
+        for i in tsugu.handler('查卡 ars 1x', '1528593481', 'red', '666808414'):
+            # 字符串
+            print(i) if isinstance(i, str) else None
+            # 图片
+            print(f"[图像大小: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes) else None
+            # from PIL import Image
+            # Image.open(io.BytesIO(i)).show() if isinstance(i, bytes) else None
         ```
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         
-        ## 调用 `tsugu.database`
+        - 异步框架下，可以使用 `run_in_executor` 方法:
         
+        > 以 lagrange-python 群聊为例，其他异步框架请自行查阅文档。
         ```python
+        loop = asyncio.get_running_loop()
+        args = (event.msg, str(event.uin), 'red', str(event.grp_id))
+        response = await loop.run_in_executor(None, tsugu.handler, *args)
+        
+        # 不发送消息
+        if not response:
+            return
+        
+        msg_list = []
+        for item in response:
+            # 处理文本类型的消息
+            msg_list.append(Text(item)) if isinstance(item, str) else None
+            msg_list.append(await client.upload_grp_image(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None
+        
+        await client.send_grp_msg(msg_list, event.grp_id)
+        ```
+        
+        ## 调用 `tsugu.database`
+        
+        ```py
         import tsugu
         
         tsugu.database(path="./data.db")
         
         # 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。
         # 远程数据库将不使用。
         # 更多功能可能在未来版本中添加。
         ```
+        > 注意，先进行此操作，后进行 `load_config_json` 操作，会覆盖数据库路径，导致数据库无法使用。
+        
         
         ## 查看与更改 `tsugu.config` 配置
         
-        - 查看默认配置文档: 
+        - 输出配置到 `config.json` 文件:
         ```py
         import tsugu
         
-        tsugu.config.show_docs()  # 输出默认配置文档到控制台
+        tsugu.config.output_config_json('./config.json')
         ```
-        - 你可以更改配置:   
+        
+        - 利用此文件，你可以更改配置项，然后重新加载配置:
+        ```py
+        import tsugu
+        
+        tsugu.config.load_config_json('./config.json')
+        ```
+        
+        
+        - 你也可以直接更改配置，但不推荐:   
         
         ```py
         import tsugu
         
         # 更改的后端地址。
         tsugu.config.backend = "http://127.0.0.0.1:3000"
         
-        # 设置代理。
-        tsugu.config.use_proxies = True
-        tsugu.config.proxies = {"http": "http://127.0.0.1:1145", "https": "http://127.0.0.1:1919"}
-        
         # 添加关闭抽卡模拟的群号。
         tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
-        
-        # 使用 `add_command_name` 和 `remove_command_name` 方法添加或删除命令名以添加别名或关闭命令。
-        tsugu.config.add_command_name(api="gacha", command_name="抽卡")
         ```
         > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         
-        ## 使用 `tsugu.router` 路由
+        
+        ## 使用 `tsugu.router` 路由与内部方法
         
         - 如果想自己进行自然语言处理，你可以使用单独的路由:
         ```py
         import tsugu
         
         # 获取用户数据
         reply = tsugu.router.get_user_data("red", "1234567890")
         
         # 查卡
         reply = tsugu.router.card("红 ksm", [0, 3], 5)
         
         # 设置玩家车牌转发
         reply = tsugu.router.set_car_forward("red", "1234567890", True)
+        
         ```
         
+        - 此外还暴露了一些内部方法，需要可以使用:
         
-        ***
+        ```py
+        import tsugu
+        
+        tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
+        tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0, '1000011232', True)
         
-        <h2 align="center"> 相对应登录端？ </h2>
+        tsugu.interior_local_method.submit_car_number_msg("123456 大分q1", "1234567890", "red")
+        ```
         
-        这不是一个好的时代， 但部署方式仍然是有不少的，如果有部署期望，可以看下面的 ▶️`客服ano酱指导` 进群聊聊天，我们会尽力帮助你。
         
-        基于 v2 api 的 `C#` + `Lagrange` 组合的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
-        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。   
+        ***
         
+        <h2 align="center"> 相对应登录端 </h2>
         
+        | 部署方式 | 传送门 |
+        | --- | --- |
+        | **lpt 登陆端部署** | [![release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
+        
+        基于 v2 api 的 `Go` + `Lagrange` 的登录端正由 [WindowsSov8](https://github.com/WindowsSov8forUs) 开发中，敬请期待。
+        基于 v2 api 的 `C#` + `Lagrange` 的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
+        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。
         
          <details>
         <summary><b>客服ano酱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
-        ***
-        
-        <h2 align="center"> 开发者的话 </h2>
-        
-        > kumo: 我草我要4了   
-        
-        > kumo: 未来还会继续完善以及同步更新喵，感谢大家的支持～  
-        &emsp;&emsp;&emsp;感谢提出建议的所有人～   
-        &emsp;&emsp;&emsp;也感谢山本和大家的付出与帮助!  
-        
-        > zhaomaoniu: 这周末不是很想写代码
-        
-        ***
-        
-        
-        
-        
-        
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,75 +1,83 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
 - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [ ] ç¬ç«è·¯ç±è¾å¥ -
-> è¿åç»æ `ç®åä»åºç¡è·¯ç±` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
+> è¿åç»æ `é¨åæ¯æ` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
 è¿ç¨æ°æ®åº (å®¢æ·ç«¯) - [x] éç½®é¡¹
 (åºç¡éç½®ãä»£çãå½ä»¤å«å ç­)
                           ********** ?å?®??è?£??ä?¸??æ??´?æ??° **********
 ## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## æ´æ° ```shell pip
 install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip install tsugu
 --index-url https://pypi.org/simple/ ``` ## åç«¯éæ± -
 åºå¾ï¼éè¦æ¯æ `v2 API` (2024.2.28æ¥ä»¥åçåç«¯çæ¬) -
 utilsï¼éè¦æ¯æ `v2 API` -
 ç¨æ·æ°æ®ï¼éè¦ä¸ä¸ªå¯ç¨äº**æ°æ®åº**çåç«¯ï¼éè¦æ¯æ `v2
 API` >
 ä¸ä¸ªåç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
                           ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
-## è°ç¨ `tsugu.bot` - `bot` æ¯ `tsugu`
+## è°ç¨ `tsugu.handler` - `handler` æ¯ `tsugu`
 çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import base64 from PIL import Image import io import tsugu #
-åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å° é¢éid data =
-tsugu.bot('æ¥å¡ çº¢ ksm 5x', '114514', 'red', '666808414') #
-å¦æè¿åå¼ä¸º None ä»£è¡¨botä¸åéä»»ä½æ¶æ¯ã if not data: print("
-[æ åé¦æ°æ®]") for item in data: if item["type"] == "string": print(f"
-[æå­ä¿¡æ¯]\n{item['string']}") elif item["type"] == "base64": image_data =
-base64.b64decode(item["string"]) print(f"[å¾åå¤§å°: {len(image_data) /
-1024:.2f}KB]") Image.open(io.BytesIO(image_data)).show() else: print(item) ```
-> å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
-`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## è°ç¨ `tsugu.database`
-```python import tsugu tsugu.database(path="./data.db") #
+```python import io import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹
+ç¨æ·id å¹³å° é¢éid for i in tsugu.handler('æ¥å¡ ars 1x', '1528593481',
+'red', '666808414'): # å­ç¬¦ä¸² print(i) if isinstance(i, str) else None #
+å¾ç print(f"[å¾åå¤§å°: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes)
+else None # from PIL import Image # Image.open(io.BytesIO(i)).show() if
+isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
+`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
+å¯ä»¥å¡«å `red`ã - å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor`
+æ¹æ³: > ä»¥ lagrange-python
+ç¾¤èä¸ºä¾ï¼å¶ä»å¼æ­¥æ¡æ¶è¯·èªè¡æ¥éææ¡£ã ```python loop =
+asyncio.get_running_loop() args = (event.msg, str(event.uin), 'red', str
+(event.grp_id)) response = await loop.run_in_executor(None, tsugu.handler,
+*args) # ä¸åéæ¶æ¯ if not response: return msg_list = [] for item in
+response: # å¤çææ¬ç±»åçæ¶æ¯ msg_list.append(Text(item)) if
+isinstance(item, str) else None msg_list.append(await client.upload_grp_image
+(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None await
+client.send_grp_msg(msg_list, event.grp_id) ``` ## è°ç¨ `tsugu.database`
+```py import tsugu tsugu.database(path="./data.db") #
 æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
 æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã #
-æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` ## æ¥çä¸æ´æ¹
-`tsugu.config` éç½® - æ¥çé»è®¤éç½®ææ¡£: ```py import tsugu
-tsugu.config.show_docs() # è¾åºé»è®¤éç½®ææ¡£å°æ§å¶å° ``` -
-ä½ å¯ä»¥æ´æ¹éç½®: ```py import tsugu # æ´æ¹çåç«¯å°åã
-tsugu.config.backend = "http://127.0.0.0.1:3000" # è®¾ç½®ä»£çã
-tsugu.config.use_proxies = True tsugu.config.proxies = {"http": "http://
-127.0.0.1:1145", "https": "http://127.0.0.1:1919"} #
+æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` >
+æ³¨æï¼åè¿è¡æ­¤æä½ï¼åè¿è¡ `load_config_json`
+æä½ï¼ä¼è¦çæ°æ®åºè·¯å¾ï¼å¯¼è´æ°æ®åºæ æ³ä½¿ç¨ã ##
+æ¥çä¸æ´æ¹ `tsugu.config` éç½® - è¾åºéç½®å° `config.json` æä»¶:
+```py import tsugu tsugu.config.output_config_json('./config.json') ``` -
+å©ç¨æ­¤æä»¶ï¼ä½ å¯ä»¥æ´æ¹éç½®é¡¹ï¼ç¶åéæ°å è½½éç½®: ```py
+import tsugu tsugu.config.load_config_json('./config.json') ``` -
+ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
+æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
 æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] # ä½¿ç¨ `add_command_name` å `remove_command_name`
-æ¹æ³æ·»å æå é¤å½ä»¤åä»¥æ·»å å«åæå³é­å½ä»¤ã
-tsugu.config.add_command_name(api="gacha", command_name="æ½å¡") ``` >
+= ["114514", "1919810"] ``` >
 æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-## ä½¿ç¨ `tsugu.router` è·¯ç± -
+## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
 å¦ææ³èªå·±è¿è¡èªç¶è¯­è¨å¤çï¼ä½ å¯ä»¥ä½¿ç¨åç¬çè·¯ç±: ```py
 import tsugu # è·åç¨æ·æ°æ® reply = tsugu.router.get_user_data("red",
 "1234567890") # æ¥å¡ reply = tsugu.router.card("çº¢ ksm", [0, 3], 5) #
 è®¾ç½®ç©å®¶è½¦çè½¬å reply = tsugu.router.set_car_forward("red",
-"1234567890", True) ``` ***
-                       ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯?ï?¼? **********
-è¿ä¸æ¯ä¸ä¸ªå¥½çæ¶ä»£ï¼
-ä½é¨ç½²æ¹å¼ä»ç¶æ¯æä¸å°çï¼å¦ææé¨ç½²ææï¼å¯ä»¥çä¸é¢ç
-â¶ï¸`å®¢æanoé±æå¯¼` è¿ç¾¤èèå¤©ï¼æä»¬ä¼å°½åå¸®å©ä½ ã åºäº
-v2 api ç `C#` + `Lagrange` ç»åçç»å½ç«¯æ­£ç± [æ£±é](https://
-github.com/DreamPrism) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç
-`NoneBot2` æä»¶ä¹ç± [zhaomaoniu](https://github.com/zhaomaoniu)
-å¼åä¸­ï¼æ¬è¯·æå¾ã ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+"1234567890", True) ``` -
+æ­¤å¤è¿æ´é²äºä¸äºåé¨æ¹æ³ï¼éè¦å¯ä»¥ä½¿ç¨: ```py import tsugu
+tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
+tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0,
+'1000011232', True) tsugu.interior_local_method.submit_car_number_msg("123456
+å¤§åq1", "1234567890", "red") ``` ***
+                        ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯ **********
+| é¨ç½²æ¹å¼ | ä¼ éé¨ | | --- | --- | | **lpt ç»éç«¯é¨ç½²** | [!
+[release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-
+py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) | åºäº
+v2 api ç `Go` + `Lagrange` çç»å½ç«¯æ­£ç± [WindowsSov8](https://
+github.com/WindowsSov8forUs) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäº v2 api ç `C#`
++ `Lagrange` çç»å½ç«¯æ­£ç± [æ£±é](https://github.com/DreamPrism)
+å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç `NoneBot2` æä»¶ä¹ç±
+[zhaomaoniu](https://github.com/zhaomaoniu) å¼åä¸­ï¼æ¬è¯·æå¾ã
+?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ***
-                          ********** ?å?¼??å???è???ç???è?¯? **********
-> kumo: æèæè¦4äº > kumo:
-æªæ¥è¿ä¼ç»§ç»­å®åä»¥ååæ­¥æ´æ°åµï¼æè°¢å¤§å®¶çæ¯æï½
-   æè°¢æåºå»ºè®®çææäººï½
-   ä¹æè°¢å±±æ¬åå¤§å®¶çä»åºä¸å¸®å©! > zhaomaoniu:
-è¿å¨æ«ä¸æ¯å¾æ³åä»£ç  *** Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-0.5.4/setup.py` & `tsugu-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.5.4',
+    version='0.5.5',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.5.4/test/test_main.py` & `tsugu-0.5.5/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.4/tsugu/config.py` & `tsugu-0.5.5/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.4/tsugu/handler.py` & `tsugu-0.5.5/tsugu/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         if message.startswith('主服务器'):
             return set_server_mode(platform, user_id, message[4:].strip())
 
     # 设置默认服务器列表
     if config.features.get('change_server_list', True):
         if message.startswith('设置默认服务器'):
-            return set_default_server(platform, user_id, message[6:].strip())
+            return set_default_server(platform, user_id, message[7:].strip())
 
     return None
 
 
 def bot_extra_remote_server(message, user_id, platform):
     # 玩家状态
     if config.features.get('player_status', True):
@@ -200,26 +200,33 @@
         if message in ['关闭车牌转发', '关闭个人车牌转发']:
             r = Remote.set_car_forward(platform, user_id, False)
             return text_response('已关闭车牌转发') if r.get('status') == 'success' else None
 
     # 切换服务器模式
     if config.features.get('change_main_server', True):
         if message.endswith('服模式'):
+            if server_exists(r_ := query_server_info(message[:-2])) is False:
+                return text_response('未找到服务器') if len(message) <= 5 else None
             if r := Remote.set_server_mode(platform, user_id, message[:-2]).get('status') == 'success':
                 return text_response('已切换为' + message[:-2] + '模式')
             return text_response(r.get('data')) if len(message) <= 5 else None
 
         if message.startswith('主服务器'):
+            if server_exists(r_ := query_server_info(message[4:].strip())) is False:
+                return text_response('未找到服务器') if len(message) <= 7 else None
             if r := Remote.set_server_mode(platform, user_id, message[4:].strip()).get('status') == 'success':
                 return text_response('主服务器已切换为' + message[4:].strip())
             return text_response(r.get('data')) if ' ' in message else None
 
     # 设置默认服务器列表
     if config.features.get('change_server_list', True):
         if message.startswith('设置默认服务器'):
+            for i in message[7:].strip().split(' '):
+                if server_exists(r_ := query_server_info(i)) is False:
+                    return text_response(f'未找到服务器 {i}')
             if r := Remote.set_default_server(platform, user_id, message[6:].strip()).get('status') == 'success':
                 return text_response('默认服务器已设置为' + message[6:].strip())
             return text_response(r.get('data')) if ' ' in message else None
 
     return None
```

### Comparing `tsugu-0.5.4/tsugu/router.py` & `tsugu-0.5.5/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.4/tsugu/utils.py` & `tsugu-0.5.5/tsugu/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,18 @@
     cursor = db_manager.conn.cursor()
     cursor.execute("UPDATE users SET car = ? WHERE user_id = ? AND platform = ?", (status, user_id, platform))
     db_manager.conn.commit()
     return text_response('车牌转发设置成功')
 
 
 def set_default_server(platform, user_id, text):
-
+    print(text)
+    for i in text.strip().split(' '):
+        if server_exists(r_ := query_server_info(i)) is False:
+            return text_response(f'未找到服务器 {i}')
     default_server = convert_server_names_to_indices(text)
     get_user_data(platform, user_id)
     cursor = db_manager.conn.cursor()
     cursor.execute("UPDATE users SET default_server = ? WHERE user_id = ? AND platform = ?",
                    (json.dumps(default_server), user_id, platform))
     db_manager.conn.commit()
     return text_response(f'默认服务器设置为 {text}')
```

### Comparing `tsugu-0.5.4/tsugu.egg-info/PKG-INFO` & `tsugu-0.5.5/tsugu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.4
+Version: 0.5.5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -31,15 +31,15 @@
         
         ***
         
         <h2 align="center"> 实现 </h2>
         
         
         - [x] 自然语言输入 -> 返回结果
-        - [ ] 独立路由输入 -> 返回结果 `目前仅基础路由`
+        - [ ] 独立路由输入 -> 返回结果 `部分支持`
         - [x] 本地数据库 (sqlite3)
         - [x] 远程数据库 (客户端)
         - [x] 配置项 (基础配置、代理、命令别名 等)
         
         
         <h2 align="center"> 安装与更新 </h2>
         
@@ -69,145 +69,155 @@
         
         
         <h2 align="center"> 测试与调用 </h2>
         
         
         
         
-        ## 调用 `tsugu.bot`
+        ## 调用 `tsugu.handler`
         
-        - `bot` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
+        - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
-        import base64
-        from PIL import Image
         import io
-        
         import tsugu
         
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
-        data = tsugu.bot('查卡 红 ksm 5x', '114514', 'red', '666808414')
-        
-        # 如果返回值为 None 代表bot不发送任何消息。
-        if not data:
-            print("[无反馈数据]")
-        
-        for item in data:
-            if item["type"] == "string":
-                print(f"[文字信息]\n{item['string']}")
-            elif item["type"] == "base64":
-                image_data = base64.b64decode(item["string"])
-                print(f"[图像大小: {len(image_data) / 1024:.2f}KB]")
-                Image.open(io.BytesIO(image_data)).show()
-            else:
-                print(item)
+        for i in tsugu.handler('查卡 ars 1x', '1528593481', 'red', '666808414'):
+            # 字符串
+            print(i) if isinstance(i, str) else None
+            # 图片
+            print(f"[图像大小: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes) else None
+            # from PIL import Image
+            # Image.open(io.BytesIO(i)).show() if isinstance(i, bytes) else None
         ```
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         
-        ## 调用 `tsugu.database`
+        - 异步框架下，可以使用 `run_in_executor` 方法:
         
+        > 以 lagrange-python 群聊为例，其他异步框架请自行查阅文档。
         ```python
+        loop = asyncio.get_running_loop()
+        args = (event.msg, str(event.uin), 'red', str(event.grp_id))
+        response = await loop.run_in_executor(None, tsugu.handler, *args)
+        
+        # 不发送消息
+        if not response:
+            return
+        
+        msg_list = []
+        for item in response:
+            # 处理文本类型的消息
+            msg_list.append(Text(item)) if isinstance(item, str) else None
+            msg_list.append(await client.upload_grp_image(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None
+        
+        await client.send_grp_msg(msg_list, event.grp_id)
+        ```
+        
+        ## 调用 `tsugu.database`
+        
+        ```py
         import tsugu
         
         tsugu.database(path="./data.db")
         
         # 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。
         # 远程数据库将不使用。
         # 更多功能可能在未来版本中添加。
         ```
+        > 注意，先进行此操作，后进行 `load_config_json` 操作，会覆盖数据库路径，导致数据库无法使用。
+        
         
         ## 查看与更改 `tsugu.config` 配置
         
-        - 查看默认配置文档: 
+        - 输出配置到 `config.json` 文件:
         ```py
         import tsugu
         
-        tsugu.config.show_docs()  # 输出默认配置文档到控制台
+        tsugu.config.output_config_json('./config.json')
         ```
-        - 你可以更改配置:   
+        
+        - 利用此文件，你可以更改配置项，然后重新加载配置:
+        ```py
+        import tsugu
+        
+        tsugu.config.load_config_json('./config.json')
+        ```
+        
+        
+        - 你也可以直接更改配置，但不推荐:   
         
         ```py
         import tsugu
         
         # 更改的后端地址。
         tsugu.config.backend = "http://127.0.0.0.1:3000"
         
-        # 设置代理。
-        tsugu.config.use_proxies = True
-        tsugu.config.proxies = {"http": "http://127.0.0.1:1145", "https": "http://127.0.0.1:1919"}
-        
         # 添加关闭抽卡模拟的群号。
         tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
-        
-        # 使用 `add_command_name` 和 `remove_command_name` 方法添加或删除命令名以添加别名或关闭命令。
-        tsugu.config.add_command_name(api="gacha", command_name="抽卡")
         ```
         > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         
-        ## 使用 `tsugu.router` 路由
+        
+        ## 使用 `tsugu.router` 路由与内部方法
         
         - 如果想自己进行自然语言处理，你可以使用单独的路由:
         ```py
         import tsugu
         
         # 获取用户数据
         reply = tsugu.router.get_user_data("red", "1234567890")
         
         # 查卡
         reply = tsugu.router.card("红 ksm", [0, 3], 5)
         
         # 设置玩家车牌转发
         reply = tsugu.router.set_car_forward("red", "1234567890", True)
+        
         ```
         
+        - 此外还暴露了一些内部方法，需要可以使用:
         
-        ***
+        ```py
+        import tsugu
+        
+        tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
+        tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0, '1000011232', True)
         
-        <h2 align="center"> 相对应登录端？ </h2>
+        tsugu.interior_local_method.submit_car_number_msg("123456 大分q1", "1234567890", "red")
+        ```
         
-        这不是一个好的时代， 但部署方式仍然是有不少的，如果有部署期望，可以看下面的 ▶️`客服ano酱指导` 进群聊聊天，我们会尽力帮助你。
         
-        基于 v2 api 的 `C#` + `Lagrange` 组合的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
-        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。   
+        ***
         
+        <h2 align="center"> 相对应登录端 </h2>
         
+        | 部署方式 | 传送门 |
+        | --- | --- |
+        | **lpt 登陆端部署** | [![release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
+        
+        基于 v2 api 的 `Go` + `Lagrange` 的登录端正由 [WindowsSov8](https://github.com/WindowsSov8forUs) 开发中，敬请期待。
+        基于 v2 api 的 `C#` + `Lagrange` 的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
+        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。
         
          <details>
         <summary><b>客服ano酱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
-        ***
-        
-        <h2 align="center"> 开发者的话 </h2>
-        
-        > kumo: 我草我要4了   
-        
-        > kumo: 未来还会继续完善以及同步更新喵，感谢大家的支持～  
-        &emsp;&emsp;&emsp;感谢提出建议的所有人～   
-        &emsp;&emsp;&emsp;也感谢山本和大家的付出与帮助!  
-        
-        > zhaomaoniu: 这周末不是很想写代码
-        
-        ***
-        
-        
-        
-        
-        
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,75 +1,83 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
 - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [ ] ç¬ç«è·¯ç±è¾å¥ -
-> è¿åç»æ `ç®åä»åºç¡è·¯ç±` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
+> è¿åç»æ `é¨åæ¯æ` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
 è¿ç¨æ°æ®åº (å®¢æ·ç«¯) - [x] éç½®é¡¹
 (åºç¡éç½®ãä»£çãå½ä»¤å«å ç­)
                           ********** ?å?®??è?£??ä?¸??æ??´?æ??° **********
 ## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## æ´æ° ```shell pip
 install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip install tsugu
 --index-url https://pypi.org/simple/ ``` ## åç«¯éæ± -
 åºå¾ï¼éè¦æ¯æ `v2 API` (2024.2.28æ¥ä»¥åçåç«¯çæ¬) -
 utilsï¼éè¦æ¯æ `v2 API` -
 ç¨æ·æ°æ®ï¼éè¦ä¸ä¸ªå¯ç¨äº**æ°æ®åº**çåç«¯ï¼éè¦æ¯æ `v2
 API` >
 ä¸ä¸ªåç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
                           ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
-## è°ç¨ `tsugu.bot` - `bot` æ¯ `tsugu`
+## è°ç¨ `tsugu.handler` - `handler` æ¯ `tsugu`
 çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import base64 from PIL import Image import io import tsugu #
-åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å° é¢éid data =
-tsugu.bot('æ¥å¡ çº¢ ksm 5x', '114514', 'red', '666808414') #
-å¦æè¿åå¼ä¸º None ä»£è¡¨botä¸åéä»»ä½æ¶æ¯ã if not data: print("
-[æ åé¦æ°æ®]") for item in data: if item["type"] == "string": print(f"
-[æå­ä¿¡æ¯]\n{item['string']}") elif item["type"] == "base64": image_data =
-base64.b64decode(item["string"]) print(f"[å¾åå¤§å°: {len(image_data) /
-1024:.2f}KB]") Image.open(io.BytesIO(image_data)).show() else: print(item) ```
-> å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
-`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## è°ç¨ `tsugu.database`
-```python import tsugu tsugu.database(path="./data.db") #
+```python import io import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹
+ç¨æ·id å¹³å° é¢éid for i in tsugu.handler('æ¥å¡ ars 1x', '1528593481',
+'red', '666808414'): # å­ç¬¦ä¸² print(i) if isinstance(i, str) else None #
+å¾ç print(f"[å¾åå¤§å°: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes)
+else None # from PIL import Image # Image.open(io.BytesIO(i)).show() if
+isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
+`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
+å¯ä»¥å¡«å `red`ã - å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor`
+æ¹æ³: > ä»¥ lagrange-python
+ç¾¤èä¸ºä¾ï¼å¶ä»å¼æ­¥æ¡æ¶è¯·èªè¡æ¥éææ¡£ã ```python loop =
+asyncio.get_running_loop() args = (event.msg, str(event.uin), 'red', str
+(event.grp_id)) response = await loop.run_in_executor(None, tsugu.handler,
+*args) # ä¸åéæ¶æ¯ if not response: return msg_list = [] for item in
+response: # å¤çææ¬ç±»åçæ¶æ¯ msg_list.append(Text(item)) if
+isinstance(item, str) else None msg_list.append(await client.upload_grp_image
+(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None await
+client.send_grp_msg(msg_list, event.grp_id) ``` ## è°ç¨ `tsugu.database`
+```py import tsugu tsugu.database(path="./data.db") #
 æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
 æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã #
-æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` ## æ¥çä¸æ´æ¹
-`tsugu.config` éç½® - æ¥çé»è®¤éç½®ææ¡£: ```py import tsugu
-tsugu.config.show_docs() # è¾åºé»è®¤éç½®ææ¡£å°æ§å¶å° ``` -
-ä½ å¯ä»¥æ´æ¹éç½®: ```py import tsugu # æ´æ¹çåç«¯å°åã
-tsugu.config.backend = "http://127.0.0.0.1:3000" # è®¾ç½®ä»£çã
-tsugu.config.use_proxies = True tsugu.config.proxies = {"http": "http://
-127.0.0.1:1145", "https": "http://127.0.0.1:1919"} #
+æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` >
+æ³¨æï¼åè¿è¡æ­¤æä½ï¼åè¿è¡ `load_config_json`
+æä½ï¼ä¼è¦çæ°æ®åºè·¯å¾ï¼å¯¼è´æ°æ®åºæ æ³ä½¿ç¨ã ##
+æ¥çä¸æ´æ¹ `tsugu.config` éç½® - è¾åºéç½®å° `config.json` æä»¶:
+```py import tsugu tsugu.config.output_config_json('./config.json') ``` -
+å©ç¨æ­¤æä»¶ï¼ä½ å¯ä»¥æ´æ¹éç½®é¡¹ï¼ç¶åéæ°å è½½éç½®: ```py
+import tsugu tsugu.config.load_config_json('./config.json') ``` -
+ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
+æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
 æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] # ä½¿ç¨ `add_command_name` å `remove_command_name`
-æ¹æ³æ·»å æå é¤å½ä»¤åä»¥æ·»å å«åæå³é­å½ä»¤ã
-tsugu.config.add_command_name(api="gacha", command_name="æ½å¡") ``` >
+= ["114514", "1919810"] ``` >
 æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-## ä½¿ç¨ `tsugu.router` è·¯ç± -
+## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
 å¦ææ³èªå·±è¿è¡èªç¶è¯­è¨å¤çï¼ä½ å¯ä»¥ä½¿ç¨åç¬çè·¯ç±: ```py
 import tsugu # è·åç¨æ·æ°æ® reply = tsugu.router.get_user_data("red",
 "1234567890") # æ¥å¡ reply = tsugu.router.card("çº¢ ksm", [0, 3], 5) #
 è®¾ç½®ç©å®¶è½¦çè½¬å reply = tsugu.router.set_car_forward("red",
-"1234567890", True) ``` ***
-                       ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯?ï?¼? **********
-è¿ä¸æ¯ä¸ä¸ªå¥½çæ¶ä»£ï¼
-ä½é¨ç½²æ¹å¼ä»ç¶æ¯æä¸å°çï¼å¦ææé¨ç½²ææï¼å¯ä»¥çä¸é¢ç
-â¶ï¸`å®¢æanoé±æå¯¼` è¿ç¾¤èèå¤©ï¼æä»¬ä¼å°½åå¸®å©ä½ ã åºäº
-v2 api ç `C#` + `Lagrange` ç»åçç»å½ç«¯æ­£ç± [æ£±é](https://
-github.com/DreamPrism) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç
-`NoneBot2` æä»¶ä¹ç± [zhaomaoniu](https://github.com/zhaomaoniu)
-å¼åä¸­ï¼æ¬è¯·æå¾ã ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+"1234567890", True) ``` -
+æ­¤å¤è¿æ´é²äºä¸äºåé¨æ¹æ³ï¼éè¦å¯ä»¥ä½¿ç¨: ```py import tsugu
+tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
+tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0,
+'1000011232', True) tsugu.interior_local_method.submit_car_number_msg("123456
+å¤§åq1", "1234567890", "red") ``` ***
+                        ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯ **********
+| é¨ç½²æ¹å¼ | ä¼ éé¨ | | --- | --- | | **lpt ç»éç«¯é¨ç½²** | [!
+[release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-
+py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) | åºäº
+v2 api ç `Go` + `Lagrange` çç»å½ç«¯æ­£ç± [WindowsSov8](https://
+github.com/WindowsSov8forUs) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäº v2 api ç `C#`
++ `Lagrange` çç»å½ç«¯æ­£ç± [æ£±é](https://github.com/DreamPrism)
+å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç `NoneBot2` æä»¶ä¹ç±
+[zhaomaoniu](https://github.com/zhaomaoniu) å¼åä¸­ï¼æ¬è¯·æå¾ã
+?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ***
-                          ********** ?å?¼??å???è???ç???è?¯? **********
-> kumo: æèæè¦4äº > kumo:
-æªæ¥è¿ä¼ç»§ç»­å®åä»¥ååæ­¥æ´æ°åµï¼æè°¢å¤§å®¶çæ¯æï½
-   æè°¢æåºå»ºè®®çææäººï½
-   ä¹æè°¢å±±æ¬åå¤§å®¶çä»åºä¸å¸®å©! > zhaomaoniu:
-è¿å¨æ«ä¸æ¯å¾æ³åä»£ç  *** Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown
```

