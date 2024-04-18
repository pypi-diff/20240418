# Comparing `tmp/zbx_wxwork_assistant-1.1.0-py3-none-any.whl.zip` & `tmp/zbx_wxwork_assistant-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7609 bytes, number of entries: 9
--rw-r--r--  2.0 unx     6504 b- defN 24-Apr-17 10:35 ZbxAssistant/ZbxApis.py
+Zip file size: 7737 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     7191 b- defN 24-Apr-18 03:01 ZbxAssistant/ZbxApis.py
 -rw-r--r--  2.0 unx      605 b- defN 24-Apr-17 10:35 ZbxAssistant/ZbxConfigs.py
 -rw-r--r--  2.0 unx     1078 b- defN 24-Apr-17 09:59 ZbxAssistant/ZbxWxworkHots.py
 -rw-r--r--  2.0 unx     6149 b- defN 24-Apr-17 10:45 ZbxAssistant/ZbxWxworkProblems.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 ZbxAssistant/__init__.py
--rw-r--r--  2.0 unx     1337 b- defN 24-Apr-17 10:45 zbx_wxwork_assistant-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 10:45 zbx_wxwork_assistant-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-17 10:45 zbx_wxwork_assistant-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      766 b- defN 24-Apr-17 10:45 zbx_wxwork_assistant-1.1.0.dist-info/RECORD
-9 files, 16544 bytes uncompressed, 6273 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx     1337 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      766 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/RECORD
+9 files, 17231 bytes uncompressed, 6401 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: ZbxAssistant/ZbxWxworkProblems.py
 Comment: 
 
 Filename: ZbxAssistant/__init__.py
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.0.dist-info/METADATA
+Filename: zbx_wxwork_assistant-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.0.dist-info/WHEEL
+Filename: zbx_wxwork_assistant-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.0.dist-info/top_level.txt
+Filename: zbx_wxwork_assistant-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.0.dist-info/RECORD
+Filename: zbx_wxwork_assistant-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ZbxAssistant/ZbxApis.py

```diff
@@ -83,76 +83,94 @@
                     if self.login_user in media.get("sendto", ""):
                         matched_user = (user.get("userid"), user.get("username"))
                         cache.set(cached_user_key, matched_user)
                         return cache.get(cached_user_key)
         except ZabbixAPIException as err:
             logging.error(msg=str(err))
 
-    def create_zbx_user_token(self, token_name: str):
+    @property
+    def token_name(self):
+        """Zabbix 用户的默认 Token 规范名称"""
+        return f"WxZbxAssistant_{self.zbx_user[1]}"
+
+    @property
+    def user_token_page(self):
+        """获取 Zabbix 用户页面上的 token"""
+        try:
+            tokens = self.zbxapi.token.get(
+                {
+                    "filter": {
+                        "name": self.token_name
+                    }
+                }
+            )
+            return tokens
+        except ZabbixAPIException as err:
+            logging.error(str(err))
+
+    def create_zbx_user_token(self):
         """
             创建 Zabbix 用户 Token：
-        :param token_name:
         :return:
         """
         tokenids = self.zbxapi.token.create(
             {
-                "name": token_name,
+                "name": self.token_name,
                 "userid": self.zbx_user[0]
             }
         )
         tokens = self.zbxapi.token.generate(
             [tokenids.get("tokenids")[0]]
         )
         if tokens[0].get("token"):
-            cache.set(token_name, tokens[0].get("token"))
-        return cache.get(token_name)
+            cache.set(
+                self.token_name,
+                {
+                    "tokenid": tokens[0].get("tokenid"),
+                    "token": tokens[0].get("token")
+                }
+            )
+        return cache.get(self.token_name).get("token")
 
     @property
     def user_token(self):
         """
             创建企业微信登录用户对应的 Zabbix 用户的 token：
                 1. API Tokens 信息存在于 Zabbix 用户的个人设置项中，可以手动创建，
                    也可以通过 API 创建，通过 API 创建则需要管理员权限；
                 2. token 一旦被创建则不再改变，但是用户个人页面上必须存在相应的 token 记录，
                    如果被删除则会失效。
         :return:
         """
-        token_name = f"WxZbxAssistant_{self.zbx_user[1]}"
-        try:
-            tokens = self.zbxapi.token.get(
-                {
-                    "filter": {
-                        "name": token_name
-                    }
-                }
-            )
-            if tokens and cache.get(token_name):
-                return cache.get(token_name)
-            if self.zbx_user and not tokens:
-                return self.create_zbx_user_token(token_name=token_name)
-            if tokens and not cache.get(token_name):
-                self.zbxapi.token.delete([tokens[0].get("tokenid")])
-                return self.create_zbx_user_token(token_name=token_name)
-            if not tokens and cache.get(token_name):
-                cache.delete(token_name)
-                return self.create_zbx_user_token(token_name=token_name)
-        except ZabbixAPIException as err:
-            logging.error(msg=str(err))
+        if self.user_token_page and cache.get(self.token_name):
+            return cache.get(self.token_name).get("token")
+        if self.zbx_user and not self.user_token_page:
+            return self.create_zbx_user_token()
+        if self.user_token_page and not cache.get(self.token_name):
+            self.zbxapi.token.delete([self.user_token_page[0].get("tokenid")])
+            return self.create_zbx_user_token()
+        if not self.user_token_page and cache.get(self.token_name):
+            cache.delete(self.token_name)
+            return self.create_zbx_user_token()
 
     @property
     def user_zbxapi(self):
         """
             封装【登录用户(即普通用户)】的 Zabbix Json RPC 调用：
                 1. 企业微信用户登录之后，后台获取到其对应的 Zabbix User ID，通过管理员用户生成其 Token，
                    然后使用 Zabbix User 用户名及其 Token 重新封装 API，基于此进行后续的操作。
         :return:
         """
         if self._user_zbx_api:
             return self._user_zbx_api
         try:
+            # Zabbix 页面上的用户 Token 须和缓存中的 Token 是同一个，否则认证失败
+            if (self.user_token_page and cache.get(self.token_name) and
+                    self.user_token_page[0].get("tokenid") != cache.get(self.token_name).get("tokenid")):
+                cache.delete(self.token_name)
             user_id = self.zbx_user[0]
             token = self.user_token
             if user_id and token:
                 zbx_api = ZabbixAPI(server=self.url, timeout=ZABBIX_TIMEOUT)
                 # 与 Zabbix API 进行 HTTPS 通信时，【不验证 SSL 证书的有效性】
                 # 在连接的 Zabbix API 服务器使用【自签名证书】或者希望【忽略由于某些原因引起的证书验证问题】时有用
                 zbx_api.validate_certs = False
```

## Comparing `zbx_wxwork_assistant-1.1.0.dist-info/METADATA` & `zbx_wxwork_assistant-1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zbx-wxwork-assistant
-Version: 1.1.0
+Version: 1.1.2
 Summary: A simple package for zabbix-wxwork assistant tool.
 Author: gary
 Author-email: mepmb@sina.com
 Requires-Dist: zabbix-api >=0.5.4
 Requires-Dist: diskcache ~=5.4.0
 
 zbx-wxwork-assistant
```

