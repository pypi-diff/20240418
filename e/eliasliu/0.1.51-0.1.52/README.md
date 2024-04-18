# Comparing `tmp/eliasliu-0.1.51.tar.gz` & `tmp/eliasliu-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.51.tar", last modified: Thu Jan 25 16:33:49 2024, max compression
+gzip compressed data, was "eliasliu-0.1.52.tar", last modified: Wed Apr 17 23:25:08 2024, max compression
```

## Comparing `eliasliu-0.1.51.tar` & `eliasliu-0.1.52.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 16:33:49.517813 eliasliu-0.1.51/
--rw-rw-rw-   0        0        0     7039 2024-01-25 16:33:49.514335 eliasliu-0.1.51/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2023-08-17 12:07:05.000000 eliasliu-0.1.51/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 16:33:49.476283 eliasliu-0.1.51/elias/
-drwxrwxrwx   0        0        0        0 2024-01-25 16:33:49.489793 eliasliu-0.1.51/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/__init__.py
--rw-rw-rw-   0        0        0    30771 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/check.py
--rw-rw-rw-   0        0        0     1376 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-01-25 16:33:49.500822 eliasliu-0.1.51/elias/datax/
--rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92979 2023-12-21 09:13:21.000000 eliasliu-0.1.51/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-01-25 16:31:22.000000 eliasliu-0.1.51/elias/picture.py
--rw-rw-rw-   0        0        0    76919 2024-01-25 16:06:05.000000 eliasliu-0.1.51/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2023-12-06 03:39:07.000000 eliasliu-0.1.51/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-01-25 16:33:49.512309 eliasliu-0.1.51/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7039 2024-01-25 16:33:49.000000 eliasliu-0.1.51/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-01-25 16:33:49.000000 eliasliu-0.1.51/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 16:33:49.000000 eliasliu-0.1.51/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-01-25 16:33:49.000000 eliasliu-0.1.51/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-25 16:33:49.000000 eliasliu-0.1.51/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 16:33:49.517813 eliasliu-0.1.51/setup.cfg
--rw-rw-rw-   0        0        0     1924 2024-01-25 16:33:38.000000 eliasliu-0.1.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.330547 eliasliu-0.1.52/
+-rw-rw-rw-   0        0        0     7039 2024-04-17 23:25:08.328566 eliasliu-0.1.52/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2023-08-17 12:07:05.000000 eliasliu-0.1.52/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.275508 eliasliu-0.1.52/elias/
+drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.293520 eliasliu-0.1.52/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/__init__.py
+-rw-rw-rw-   0        0        0    30771 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.310532 eliasliu-0.1.52/elias/datax/
+-rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-04-17 23:23:15.000000 eliasliu-0.1.52/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-01-25 16:31:22.000000 eliasliu-0.1.52/elias/picture.py
+-rw-rw-rw-   0        0        0    76919 2024-01-25 16:06:05.000000 eliasliu-0.1.52/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.326572 eliasliu-0.1.52/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7039 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 23:25:08.330547 eliasliu-0.1.52/setup.cfg
+-rw-rw-rw-   0        0        0     1924 2024-04-17 23:24:35.000000 eliasliu-0.1.52/setup.py
```

### Comparing `eliasliu-0.1.51/PKG-INFO` & `eliasliu-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.51
+Version: 0.1.52
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.51/README.md` & `eliasliu-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.52/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/douyin.py` & `eliasliu-0.1.52/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/jd.py` & `eliasliu-0.1.52/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/name_in_db.py` & `eliasliu-0.1.52/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.52/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.52/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/Scripts/youdao.py` & `eliasliu-0.1.52/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/check.py` & `eliasliu-0.1.52/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/config_env_variable.py` & `eliasliu-0.1.52/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datamove.py` & `eliasliu-0.1.52/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/auto_create_table.py` & `eliasliu-0.1.52/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/job.py` & `eliasliu-0.1.52/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/main.py` & `eliasliu-0.1.52/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/reader.py` & `eliasliu-0.1.52/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/run.py` & `eliasliu-0.1.52/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/datax/writer.py` & `eliasliu-0.1.52/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/etl.py` & `eliasliu-0.1.52/elias/etl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2447,15 +2447,15 @@
 
     # 发送任务执行日报
     if __name__ == '__main__' or fail_c>0:
         w.run_report(title = title,text = content,fail_count=fail_c,success_count=success_c,all_count=all_c,key=robot_key,user='刘益廷')
         print('\n任务执行日报发送成功')
 
 
-def sql_to_mail(m_id,mission_name,name,robot_key,sql,hosts,username,password,receivers=[],accs=[],links={},subject='test',contents='test',hosts_records = u.all_hosts('bi_report')):
+def sql_to_mail(m_id,mission_name,name,robot_key,sql,hosts,username,password,receivers=[],accs=[],links={},subject='test',contents='test',hosts_records = u.all_hosts('bi_report'),date=u.yesterday()):
     '''
     
     功能：
     从sql取数，导出成excel文件，上传邮箱附件，并发送给指定收件人，最后本地导出的删除文件。
     
 
     Parameters
@@ -2574,15 +2574,15 @@
 
     
     plan = '文件导出：{}'.format(name)
     logger.info(f'\n开始执行：{plan}\n')
     
     try:
     
-        file_name = f"{name}_{u.yestoday().replace('-','')}.xlsx"
+        file_name = f"{name}_{date.replace('-','')}.xlsx"
         df.to_excel(file_name,index=False)
         
         # -----------
         logger.info(f'{plan} success！')
         f_c = f_c + 1
         m_list.append('{}-{},success'.format(plan,len(df)))
     except Exception as e:
```

### Comparing `eliasliu-0.1.51/elias/picture.py` & `eliasliu-0.1.52/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/usual.py` & `eliasliu-0.1.52/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/elias/wechat.py` & `eliasliu-0.1.52/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.52/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.51
+Version: 0.1.52
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.51/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.52/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.51/setup.py` & `eliasliu-0.1.52/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.51',  # 版本号
+    version='0.1.52',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

