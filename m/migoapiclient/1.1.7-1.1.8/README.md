# Comparing `tmp/migoapiclient-1.1.7.tar.gz` & `tmp/migoapiclient-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.7.tar", last modified: Mon Apr 15 10:22:24 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.8.tar", last modified: Thu Apr 18 11:00:18 2024, max compression
```

## Comparing `migoapiclient-1.1.7.tar` & `migoapiclient-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:22:24.904130 migoapiclient-1.1.7/
--rw-rw-rw-   0        0        0     3900 2024-04-15 10:22:24.903614 migoapiclient-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 10:22:24.899611 migoapiclient-1.1.7/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.7/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    12302 2024-04-15 10:22:15.000000 migoapiclient-1.1.7/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.7/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:22:24.902614 migoapiclient-1.1.7/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-15 10:22:24.000000 migoapiclient-1.1.7/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-15 10:22:24.000000 migoapiclient-1.1.7/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:22:24.000000 migoapiclient-1.1.7/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 10:22:24.000000 migoapiclient-1.1.7/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 10:22:24.904130 migoapiclient-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-15 10:22:15.000000 migoapiclient-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:22:24.902614 migoapiclient-1.1.7/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/
+-rw-rw-rw-   0        0        0     3900 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.133909 migoapiclient-1.1.8/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.8/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    12320 2024-04-18 10:59:25.000000 migoapiclient-1.1.8/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.8/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.140919 migoapiclient-1.1.8/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-18 10:59:25.000000 migoapiclient-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.140919 migoapiclient-1.1.8/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.8/src/__init__.py
```

### Comparing `migoapiclient-1.1.7/PKG-INFO` & `migoapiclient-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.7/README.md` & `migoapiclient-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.7/migoapiclient/api_client.py` & `migoapiclient-1.1.8/migoapiclient/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,43 +38,43 @@
     def res_callback(self, res_data: Response):
         """
         响应回调
         :param res_data 响应数据
         """
         return res_data
 
-    def try_get(self, url, error_count: int = 0, **kwargs):
+    def try_get(self, url, error_count: int = 0, e='', **kwargs):
         """
         尝试重发get请求
         """
         while error_count <= self.retry_count:
             try:
                 res_data = self.get(url, timeout=self.timeout, **kwargs)
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
-                return self.try_get(url, error_count, **kwargs)
+                return self.try_get(url, error_count, e, **kwargs)
         raise Exception('已经尝试请求：{}次，服务器依然没有响应，错误信息是：{}'.format(self.retry_count, str(e)))
 
-    def try_post(self, url: str, error_count: int = 0, **kwargs):
+    def try_post(self, url: str, error_count: int = 0, e='', **kwargs):
         """
         尝试重发post请求
         """
         while error_count <= self.retry_count:
             try:
                 res_data = self.post(url, timeout=self.timeout, **kwargs)
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
                 time.sleep(error_count)
-                return self.try_post(url, error_count, **kwargs)
+                return self.try_post(url, error_count, e, **kwargs)
         raise Exception('已经尝试请求：{}次，服务器依然没有响应，错误信息是：{}'.format(self.retry_count, str(e)))
 
     @staticmethod
     def get_log_time():
         """
         生成日志时间
         """
```

### Comparing `migoapiclient-1.1.7/migoapiclient/file_manager.py` & `migoapiclient-1.1.8/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.7/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.8/migoapiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.7/setup.py` & `migoapiclient-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.1.7'
+VERSION = '1.1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

