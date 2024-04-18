# Comparing `tmp/xtnkk-tools-1.0.1.2.tar.gz` & `tmp/xtnkk-tools-1.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.1.2.tar", last modified: Thu Apr 18 02:32:32 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.1.3.tar", last modified: Thu Apr 18 04:34:58 2024, max compression
```

## Comparing `xtnkk-tools-1.0.1.2.tar` & `xtnkk-tools-1.0.1.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.2/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-18 02:32:27.000000 xtnkk-tools-1.0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools/
--rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.1.2/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      460 2024-04-18 02:29:04.000000 xtnkk-tools-1.0.1.2/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     5586 2024-04-17 16:35:57.000000 xtnkk-tools-1.0.1.2/xtnkk_tools/tools.py
--rw-rw-rw-   0        0        0      911 2024-04-18 02:32:27.000000 xtnkk-tools-1.0.1.2/xtnkk_tools/update.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 02:32:32.000000 xtnkk-tools-1.0.1.2/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-18 04:34:50.000000 xtnkk-tools-1.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/
+-rw-rw-rw-   0        0        0     5489 2024-04-18 04:22:33.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-18 04:15:31.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     6241 2024-04-18 04:34:37.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.1.2/setup.py` & `xtnkk-tools-1.0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.1.2",  # 版本
+    version="1.0.1.3",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.1.2/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.1.3/xtnkk_tools/MongoDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             data: 单条数据
             insert_ignore: 索引冲突是否忽略 默认False
             is_add_create_time: 是否在数据中添加一个创建数据10时间戳字段 默认False不创建
             is_add_create_time_field_name: 自定义创建数据时间戳字段名：默认：create_dt
         Returns: 插入成功的行数
         """
         if is_add_create_time:
-            data[is_add_create_time_field_name] = get_now_time_int(is_time_10=True)
+            data[is_add_create_time_field_name] = get_now_timestamp_int(is_time_10=True)
         collection = self.get_collection(coll_name)
         try:
             collection.insert_one(data)
         except DuplicateKeyError as e:
             if not insert_ignore:
                 raise e
             return 0
```

### Comparing `xtnkk-tools-1.0.1.2/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.1.3/xtnkk_tools/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,69 +55,121 @@
     :param file_path: 文件路径
     :return: 
     """
     result = get_file_md5_32(file_path)
     return result[8:24]
 
 
-def get_now_time_int(is_time_10=False, is_time_13=False, is_time_day0=False, is_time_day59=False):
+def get_now_timestamp_int(is_time_10=False, is_time_13=False):
     """
         获取当前时间戳
     :param is_time_10: 是否需要处理为10位的时间戳，默认不处理
     :param is_time_13: 是否需要处理为13位的时间戳，默认不处理
-    :param is_time_day0: 是否需要处理为当天00:00:00点时间戳，默认不处理
-    :param is_time_day59: 是否需要处理为当天23:59:59点时间戳，默认不处理
     :return:
     """
 
     if is_time_10:
         val = int(time.time())
     elif is_time_13:
         val = int(time.time() * 1000)
     else:
         val = time.time()
-    if is_time_day0:
-        val = get_now_day0_time_int(is_time_13)
-    elif is_time_day59:
-        val = get_now_day59_time_int(is_time_13)
     return val
 
 
-def get_now_day0_time_int(is_time_13=False):
+def get_now_day0_timestamp_int(is_time_13=False):
     """
         获取当天0点时间戳
     :param is_time_13: 是否需要处理为13位的时间戳，默认不处理并且返回10位时间戳
     :return:
     """
     val = time.mktime(datetime.date.today().timetuple())
     if is_time_13:
         return int(val * 1000)
     else:
         return int(val)
 
 
-def get_now_day59_time_int(is_time_13=False):
+def get_now_day59_timestamp_int(is_time_13=False):
     """
         获取当天23:59:59点时间戳
     :param is_time_13: 是否需要处理为13位的时间戳，默认不处理并且返回10位时间戳
     :return:
     """
     # 获取当前日期时间
     now = datetime.datetime.now()
     # 设置小时、分钟、秒为 23:59:59
     last_second = now.replace(hour=23, minute=59, second=59)
     # 转换为时间戳
     timestamp = time.mktime(last_second.timetuple())
     # 转换为整数类型
     if is_time_13:
-        return int(timestamp * 1000)
+        return get_10_to_13_timestamp(timestamp)
     else:
         return int(timestamp)
 
 
+def get_x_day_timestamp(x, is_time_13=False):
+    """
+        获取x天的0点的时间戳
+    :param x: 0:当天; 1:1天后; -1:一天前
+    :param is_time_13: 是否需要处理为13位的时间戳，默认不处理并且返回10位时间戳
+    :return:
+    """
+    if x == 0:
+        date_string = datetime.datetime.now().strftime("%Y-%m-%d")  # 当天日期
+    elif x > 0:
+        future_date = datetime.datetime.now() + datetime.timedelta(days=x)
+        date_string = future_date.strftime("%Y-%m-%d")  # x天后的日期
+    else:
+        past_date = datetime.datetime.now() - datetime.timedelta(days=abs(x))
+        date_string = past_date.strftime("%Y-%m-%d")  # x天前的日期
+
+    timestamp = get_date_s_to_timestamp(date_string=date_string)
+    if is_time_13:
+        return get_10_to_13_timestamp(timestamp)
+    else:
+        return int(timestamp)
+
+
+def get_date_s_to_timestamp(date_string, date_format="%Y-%m-%d", is_time_13=False):
+    """
+        根据日期格式转换为时间戳，date_string和date_format需要配合，自行传参修改，这里是以%Y-%m-%d为格式也就是2024-04-18
+    :param date_string: 字符串类型的日期格式 例如：2024-04-18
+    :param date_format: 时间格式
+    :param is_time_13: 是否需要处理为13位的时间戳，默认不处理并且返回10位时间戳
+    :return:
+    """
+    date_obj = datetime.datetime.strptime(date_string, date_format)
+    timestamp = date_obj.timestamp()
+    return timestamp
+
+
+def get_10_to_13_timestamp(timestamp):
+    """
+        10位时间戳转13位时间戳
+    :param timestamp:
+    :return:
+    """
+    if len(str(int(timestamp))) == 10:
+        return int(timestamp * 1000)
+    return 0
+
+
+def get_13_to_10_timestamp(timestamp):
+    """
+        13位时间戳转10位时间戳
+    :param timestamp:
+    :return:
+    """
+    if len(str(int(timestamp))) == 13:
+        return int(timestamp // 1000)
+    return 0
+
+
 def get_str_to_json(str_json):
     """
         字符串类型的json格式 转 json
     :param str_json: 字符串json
     :return:
     """
     try:
@@ -153,20 +205,11 @@
     # 根据总条数和limit计算总页数
     total_pages = math.ceil(total / limit)
     return total_pages
 
 
 if __name__ == '__main__':
     pass
-    # print(get_md5_16("1", True))  # 获取16位md5结果
-    # print(get_md5_32("1", True))  # 获取32位md5结果
-    # print(get_now_time_int())  # 获取当前时间戳
-    # print(get_now_time_int(True, False))  # 获取当前10位时间戳
-    # print(get_now_time_int(False, True))  # 获取当前13位时间戳
-    # print(get_now_time_int(True, False, True, False))  # 获取当天0点10位时间戳
-    # print(get_now_time_int(False, True, True, False))  # 获取当天0点13位时间戳
-    # print(get_now_time_int(True, False, False, True))  # 获取当天23:59:59 10位时间戳
-    # print(get_now_time_int(False, True, False, True))  # 获取当天23:59:59 13位时间戳
-    # print("获取当天0点时间戳", get_now_day0_time_int(False))  # 获取当天0点时间戳
-    # print("获取当天0点时间戳", get_now_day0_time_int(True))  # 获取当天0点时间戳
-    # print("获取当天23:59:59点时间戳", get_now_day59_time_int(False))  # 获取当天23:59:59点时间戳
-    # print("获取当天23:59:59点时间戳", get_now_day59_time_int(True))  # 获取当天23:59:59点时间戳
+    print(get_x_day_timestamp(0))
+    print(get_x_day_timestamp(0, True))
+    print(get_x_day_timestamp(1))
+    print(get_x_day_timestamp(-1))
```

