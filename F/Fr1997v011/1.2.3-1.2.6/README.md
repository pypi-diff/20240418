# Comparing `tmp/Fr1997v011-1.2.3.tar.gz` & `tmp/Fr1997v011-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.2.3.tar", last modified: Thu Apr  4 11:14:16 2024, max compression
+gzip compressed data, was "Fr1997v011-1.2.6.tar", last modified: Thu Apr 18 02:38:06 2024, max compression
```

## Comparing `Fr1997v011-1.2.3.tar` & `Fr1997v011-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.007455 Fr1997v011-1.2.3/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.000945 Fr1997v011-1.2.3/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-04 11:14:16.006466 Fr1997v011-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-02 02:58:59.000000 Fr1997v011-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.001945 Fr1997v011-1.2.3/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.3/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.003945 Fr1997v011-1.2.3/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.3/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   125905 2024-04-04 11:13:38.000000 Fr1997v011-1.2.3/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.005449 Fr1997v011-1.2.3/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.3/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-04 11:14:16.007455 Fr1997v011-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.719171 Fr1997v011-1.2.6/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.712171 Fr1997v011-1.2.6/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-18 02:38:06.718171 Fr1997v011-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-17 10:09:41.000000 Fr1997v011-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.714170 Fr1997v011-1.2.6/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.6/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.716171 Fr1997v011-1.2.6/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.6/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   130107 2024-04-17 11:21:03.000000 Fr1997v011-1.2.6/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.717171 Fr1997v011-1.2.6/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.6/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:38:06.719171 Fr1997v011-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-17 10:09:41.000000 Fr1997v011-1.2.6/setup.py
```

### Comparing `Fr1997v011-1.2.3/LICENSE` & `Fr1997v011-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.2.3/README.md` & `Fr1997v011-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.2.2.tar.gz
+pip install dist/Fr1997v011-1.2.6.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.2.3/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.2.6/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,20 @@
             'http': ip
         }
         return proxies
 
 
 # 飞书
 class Feishu:
+    def __init__(self):
+        # 飞书
+        self.feishu_base_url = config_dict['feishu']['fs_base_url']
+        self.feishu_bot_url = config_dict['feishu']['fs_bot_url']  # 飞书机器人
+        self.feishu_token_url = config_dict['feishu']['fs_token_url']  # 飞书token
+
     # 飞书 机器人推送
     def feishu_send_message(self, text, WEBHOOK_URL=''):
         if WEBHOOK_URL == '':
             WEBHOOK_URL = config_dict['feishu']['fs_url']
 
         data = {
             "timestamp": int(time.time()),
@@ -522,28 +528,26 @@
         res = HttpJike.post(url=WEBHOOK_URL, data=data)
         if res.status_code == 200:
             print(res.json)
 
     # 飞书 应用token
     def feishu_get_token(self, app_id, app_secret):
         try:
-            url = "https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal"
             post_data = {"app_id": app_id,
                          "app_secret": app_secret}
-            res = HttpJike.post(url=url, data=post_data)
+            res = HttpJike.post(url=self.feishu_token_url, data=post_data)
             if res.status_code == 200:
                 tenant_access_token = res.json["tenant_access_token"]
                 return tenant_access_token
         except:
             pass
 
     # 飞书 批量新增
     def feishu_add_more_view(self, app_token, table_id, records, tenant_access_token):
-        url = f'https://open.feishu.cn/open-apis/bitable/v1/apps/{app_token}/tables/{table_id}/records/batch_create'
-
+        url = self.fs_url(app_token, 'add_more', table_id=table_id)
         headers = {
             'Authorization': f"Bearer {tenant_access_token}",
             'Content-Type': "application/json; charset=utf-8",
         }
         data = {
             "records": records
         }
@@ -552,14 +556,21 @@
             data_data = res.json
             code = data_data.get('code')
             msg = data_data.get('msg')
             data = data_data.get('data')
             if code == 0 and msg == "success" and data:
                 return 1
 
+    # 飞书各种url统一
+    def fs_url(self, app_token, mode, **kwargs):
+        base_url = f'{config_dict["feishu"]["fs_app_url"]}{app_token}/'
+        if mode == 'add_more':
+            table_id = kwargs['table_id']
+            return f'{base_url}tables/{table_id}/records/batch_create'
+
 
 # 时间
 class TimeJike:
     @staticmethod
     def zero_clock(day=0):
         t2 = time.time()
         a = time.localtime(t2)  # 时间戳 > 9元组
@@ -1433,14 +1444,65 @@
 
                 video_detail = data_data['aweme_detail']
                 data_json = mode_spider.douyin_video_response(video_detail, tp=res_tp)  # 数据获取
                 return data_json
         except Exception as E:
             return {'aweme_type': 1, 'is_alive': 0, 'err': E}
 
+    # 【api】 抖音合集列表
+    def api_douyin_mix_list(self, cursor=0, limit=6, use_proxies=1):
+        cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
+        headers = {
+            "authority": "www.douyin.com",
+            "pragma": "no-cache",
+            "cache-control": "no-cache",
+            "accept": "application/json, text/plain, */*",
+            "user-agent": config_dict['base_ua'],
+            "referer": "https://www.douy" + "in.com/user/MS4wLjABAAAAM5BxLLRhN2jrzttuOUI3LEmFClP8t6dp0bf67Oi3deE",
+            "accept-language": "zh-CN,zh;q=0.9",
+            'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;{random.choice(cookies)}'
+        }
+
+        url = f'https://www.douyin.com/aweme/v1/web/mix/list/?device_platform=webapp&aid=6383&channel=channel_pc_web&sec_user_id=MS4wLjABAAAAqfJDRsNO2778Ye6WecYtOl1qISyLAwUoG2rgsZFqzS9ZAKpN7tMuqr7O6P2Acwos&req_from=channel_pc_web&cursor={cursor}&count={limit}&pc_client_type=1&version_code=290100&version_name=29.1.0&cookie_enabled=true&screen_width=2048&screen_height=1280&browser_language=zh-CN&browser_platform=Win32&browser_name=Edge&browser_version=123.0.0.0&browser_online=true&engine_name=Blink&engine_version=123.0.0.0&os_name=Windows&os_version=10&cpu_core_num=32&device_memory=8&platform=PC&downlink=10&effective_type=4g&round_trip_time=50'
+        url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
+        try:
+            if use_proxies:
+                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
+            else:
+                response = HttpJike.get(url=url, headers=headers)
+            if response.status_code == 200:
+                data_data = response.json
+                print(data_data)
+                return data_data
+        except Exception as E:
+            pass
+
+    # 【api】 抖音合集详情
+    def api_douyin_mix_page(self, mix_id):
+        cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
+        headers = {
+            "authority": "www.douyin.com",
+            "pragma": "no-cache",
+            "cache-control": "no-cache",
+            "accept": "application/json, text/plain, */*",
+            "user-agent": config_dict['base_ua'],
+            "referer": "https://www.douy" + "in.com/user/MS4wLjABAAAAM5BxLLRhN2jrzttuOUI3LEmFClP8t6dp0bf67Oi3deE",
+            "accept-language": "zh-CN,zh;q=0.9",
+            'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;{random.choice(cookies)}'
+        }
+
+        url = f'https://www.douyin.com/aweme/v1/web/mix/aweme/?device_platform=webapp&aid=6383&channel=channel_pc_web&mix_id={mix_id}&cursor=0&count=20&pc_client_type=1&version_code=290100&version_name=29.1.0&cookie_enabled=true&screen_width=2048&screen_height=1280&browser_language=zh-CN&browser_platform=Win32&browser_name=Edge&browser_version=123.0.0.0&browser_online=true&engine_name=Blink&engine_version=123.0.0.0&os_name=Windows&os_version=10&cpu_core_num=32&device_memory=8&platform=PC&downlink=10&effective_type=4g&round_trip_time=50'
+        url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
+        response = requests.get(
+            url=url,
+            headers=headers,
+        )
+        print(response.status_code)
+        print(response.json())
+
     # 【api】 用户主页视频列表 amemv版本
     def user_video_list_mv(self, sec_uid, max_cursor='0', timeout=30):
         ret_data = {
             'list': []
         }
         headers = {
             'authority': 'www.douyin.com',
@@ -2036,14 +2098,17 @@
                             length = f.get('length', 255)
                             default = f.get('default', '')
                             fields_sql.append(f"{name} {field_type}({length}) DEFAULT '{default}' COMMENT '{comment}'")
                         elif field_type == 'INT' or field_type == 'TINYINT' or field_type == 'SMALLINT':
                             length = f.get('length', 11)
                             default = f.get('default', 0)
                             fields_sql.append(f"{name} {field_type}({length}) DEFAULT {default} COMMENT '{comment}'")
+                        elif field_type == 'TEXT':  # 新增条件处理 TEXT 类型
+                            default = f.get('default', '')
+                            fields_sql.append(f"{name} {field_type} DEFAULT '{default}' COMMENT '{comment}'")
                     if fields_sql:
                         this_time = time.strftime("%Y-%m-%d %X", time.localtime(int(time.time())))
                         table_notes = f'{this_time} 【高阳】创建此表'  # 表备注
                         sql_create_base = f"CREATE TABLE {table} ({field_cfg['id']} INT AUTO_INCREMENT PRIMARY KEY,{','.join(fields_sql)}) COMMENT='{table_notes}'"
                         cursor.execute(sql_create_base)
 
                         # 增加唯一索引
@@ -2249,23 +2314,27 @@
 
         # 获取查询结果
         results = [future.result() for future in futures]
 
         return results
 
     # ES 查询 分页
-    def es_search_page(self, table, query, sort, size=1, offset=0, is_ret_num=1, is_print=0):
+    def es_search_page(self, table, query, sort, size=1, offset=0, is_ret_num=1, is_print=0, **kwargs):
         body = {
             "query": query,
             "track_total_hits": True if is_ret_num == 1 else False,
             "size": size,
             "from": offset,
             "sort": sort,
         }
 
+        _source = kwargs.get("_source")
+        if _source is not None:
+            body['_source'] = _source
+
         # 排序方式
         es = self.db_es()
         response = es.search(
             index=table,
             body=body
         )
         _shards = response.get('_shards')
```

