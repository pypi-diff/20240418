# Comparing `tmp/ddreport-4.5.tar.gz` & `tmp/ddreport-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddreport-4.5.tar", last modified: Thu Feb  1 08:48:55 2024, max compression
+gzip compressed data, was "ddreport-4.6.tar", last modified: Thu Apr 18 04:44:04 2024, max compression
```

## Comparing `ddreport-4.5.tar` & `ddreport-4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 08:48:55.167760 ddreport-4.5/
--rw-rw-rw-   0        0        0       27 2023-12-28 03:40:30.000000 ddreport-4.5/MANIFEST.in
--rw-rw-rw-   0        0        0      494 2024-02-01 08:48:55.167760 ddreport-4.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-01 08:48:55.135265 ddreport-4.5/ddreport/
--rw-rw-rw-   0        0        0        0 2023-10-31 10:31:51.000000 ddreport-4.5/ddreport/__init__.py
--rw-rw-rw-   0        0        0     9310 2023-12-27 03:06:36.000000 ddreport-4.5/ddreport/api.py
--rw-rw-rw-   0        0        0     2745 2023-10-31 10:31:51.000000 ddreport-4.5/ddreport/db.py
--rw-rw-rw-   0        0        0      389 2023-10-31 10:31:51.000000 ddreport-4.5/ddreport/exceptd.py
--rw-rw-rw-   0        0        0     2208 2023-11-16 09:53:06.000000 ddreport-4.5/ddreport/func.py
--rw-rw-rw-   0        0        0     2016 2023-10-31 10:31:51.000000 ddreport-4.5/ddreport/handle.py
-drwxrwxrwx   0        0        0        0 2024-02-01 08:48:55.163771 ddreport-4.5/ddreport/template/
--rw-rw-rw-   0        0        0    23843 2024-02-01 03:28:13.000000 ddreport-4.5/ddreport/template/index.html
--rw-rw-rw-   0        0        0    14714 2024-02-01 06:21:18.000000 ddreport-4.5/ddreport/testReport.py
-drwxrwxrwx   0        0        0        0 2024-02-01 08:48:55.155759 ddreport-4.5/ddreport.egg-info/
--rw-rw-rw-   0        0        0      494 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-01 08:48:55.000000 ddreport-4.5/ddreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-01 08:48:55.167760 ddreport-4.5/setup.cfg
--rw-rw-rw-   0        0        0     1699 2024-02-01 03:03:51.000000 ddreport-4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:44:04.099376 ddreport-4.6/
+-rw-rw-rw-   0        0        0       27 2024-04-12 09:29:28.000000 ddreport-4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2008 2024-04-18 04:44:04.098366 ddreport-4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2024-04-16 08:06:27.000000 ddreport-4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 04:44:04.083366 ddreport-4.6/ddreport/
+-rw-rw-rw-   0        0        0    14136 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-17 03:26:35.000000 ddreport-4.6/ddreport/api.py
+-rw-rw-rw-   0        0        0     3460 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/db.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/exceptd.py
+-rw-rw-rw-   0        0        0     3504 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/func.py
+-rw-rw-rw-   0        0        0     2018 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/handle.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:44:04.097366 ddreport-4.6/ddreport/template/
+-rw-rw-rw-   0        0        0    24005 2024-04-16 10:27:59.000000 ddreport-4.6/ddreport/template/index.html
+drwxrwxrwx   0        0        0        0 2024-04-18 04:44:04.097366 ddreport-4.6/ddreport.egg-info/
+-rw-rw-rw-   0        0        0     2008 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 04:44:04.000000 ddreport-4.6/ddreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 04:44:04.099376 ddreport-4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2024-04-18 04:43:57.000000 ddreport-4.6/setup.py
```

### Comparing `ddreport-4.5/ddreport/api.py` & `ddreport-4.6/ddreport/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ddreport.exceptd import ExceptInfo
 from jsonpath import jsonpath
 import requests
 import traceback
-import warnings
 requests.packages.urllib3.disable_warnings()
 
 
 class RequestObj(object):
     __slots__ = ('__query', '__status_code', '__resp_headers', '__resp_cookies', '__response')
 
     def __init__(self):
@@ -76,34 +75,29 @@
     def typed(self):
         return self.__typed
 
     @typed.setter
     def typed(self, value):
         self.__typed = value
 
-def session():
-	# 这行告警代码被识别到
-    warnings.warn("some_old_function is deprecated", DeprecationWarning)
-    return
 
-
-
-class CustomQuery():
-    def __init__(self, gg, host=''):
+class DDreportQuery:
+    def __init__(self, gg, host='', temp_save_data={}):
         self.host = host
         self.__GG = gg
         self.headers = dict()
         self.cookies = dict()
         self.verify = None
         self.proxies = None
         self.cert = None
+        self.__temp_save_data = temp_save_data
 
     def __assert(self, r, is_json, assert_list, E, Q):
         if not assert_list:
-            if r.status_code != 200:
+            if r.status_code >= 400:
                 E.typed = 20                                                                           # 状态码错误
                 E.msg_dict = r.status_code
                 ExceptInfo(Q, E).raised()
             else:
                 return r
         if isinstance(assert_list, list) is False:
             E.typed = 11                                                                                # 断言类型错误
@@ -223,14 +217,15 @@
             if cookies:
                 self.cookies.update(cookies)
             try:
                 response, is_json = r.json(), True
             except Exception:
                 response, is_json = r.text, False
             Q.status_code, Q.resp_headers, Q.resp_cookies, Q.response = status_code, headers, cookies, response
-            self.__GG.set("@@ddreportQuery", Q)
+            self.__temp_save_data["ddquery"] = Q
+            self.__assert(r, is_json, asserts, E, Q)
+            return r
         except Exception:
-            E.typed = 10
-            E.msg_dict = traceback.format_exc()
+            if not E.typed:
+                E.typed = 10
+                E.msg_dict = traceback.format_exc()
             ExceptInfo(Q, E).raised()
-        self.__assert(r, is_json, asserts, E, Q)
-        return r
```

### Comparing `ddreport-4.5/ddreport/db.py` & `ddreport-4.6/ddreport/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import psycopg2.extras
 import pymysql
 from sshtunnel import SSHTunnelForwarder
 
 
-class PytestMysql:
+class DDreportMysql:
     def __init__(self, db_config):
         if db_config and db_config.get('ssh'):
             self.__SSH = True
             db_ssh = db_config.get('ssh')
             ssh_address_or_host = (db_ssh["host"], db_ssh['port'])
             ssh_username = db_ssh['user']
             remote_bind_address = (db_config['host'], db_config['port'])
@@ -58,8 +59,27 @@
             raise ConnectionError("Mysql Connection timed out: Connect failed")
 
     def off(self):
         if self.__conn:
             self.__cursor.close()  # 关闭游标
             self.__conn.close()  # 关闭数据库连接
             if self.__SSH is True:
-                self.__server.close()
+                self.__server.close()
+                
+
+class DDreportPg:
+    def __init__(self, pg_config):
+        try:
+            connection = psycopg2.connect(**pg_config)
+            self.__cursor = connection.cursor(cursor_factory=psycopg2.extras.RealDictCursor)
+            self.__dbStatus = True
+        except Exception:
+            self.__dbStatus = False
+
+    def query(self, selector):
+        if self.__dbStatus:
+            self.__cursor.execute(selector)
+            pg_res = self.__cursor.fetchall()
+            res = pg_res and list(map(lambda x: dict(x), pg_res)) or []
+            return res
+        else:
+            raise ConnectionError("pgsql Connection timed out: Connect failed")
```

### Comparing `ddreport-4.5/ddreport/handle.py` & `ddreport-4.6/ddreport/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 def escape(data):
     if "<" in data or ">" in data:
         return data.replace('<', '&lt;').replace('>', '&gt;')
     return data
 
+
 def set_default(obj):
     if not isinstance(obj, (list, dict)):
         return escape(str(obj))
 
 
 class Process:
     def __init__(self):
```

### Comparing `ddreport-4.5/ddreport/template/index.html` & `ddreport-4.6/ddreport/template/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,23 @@
         margin-right: 40px;
     }
 
     .row-expand {
         background-color: #f5f5f5;
         padding: 10px;
     }
+
+    .el-tabs__item.is-disabled {
+        padding: 0 !important;
+    }
+
+    .custom-tabs-label {
+        padding: 0 20px;
+        cursor: default;
+    }
 </style>
 <body>
 <div id="app">
     <el-scrollbar height="100vh">
         <h2 class="title">{{sourceData.title}}</h2>
         <el-row style="margin: 10px;">
             <el-col :span="20" :push="2">
```

### Comparing `ddreport-4.5/ddreport/testReport.py` & `ddreport-4.6/ddreport/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 #############################################
 # File Name: ddreport
 # Author: duanliangcong
 # Mail: 137562703@qq.com
 # Created Time:  2022-11-02 15:00:00
 #############################################
+import ast
+import json
+import os
+import pytest
+import re
+import requests
+import sys
+import time
+import traceback
 from _pytest.python import Function
 from _pytest.runner import runtestprotocol
-from jsonpath import jsonpath
 from collections.abc import Iterable
-from ddreport.api import CustomQuery
-from ddreport.db import PytestMysql
-from ddreport.func import PytestFunctions
-from ddreport.handle import Process
 from itertools import product
-import requests
-import pytest
-import time
-import json
-import os, sys
-import re
-import ast
-import traceback
-
+from jsonpath import jsonpath
+from ddreport.api import DDreportQuery
+from ddreport.db import DDreportMysql, DDreportPg
+from ddreport.func import DDreportFunctions, DataDiff
+from ddreport.handle import Process
 
 requests.packages.urllib3.disable_warnings()
 
+
 test_result = {
     "title": "",
     "desc": "",
     "tester": "",
     "start_time": "",
     "end_time": "",
     "failed": 0,
     "passed": 0,
     "skipped": 0,
     "error": 0,
     "cases": [],
 }
 
-dict_data = {
-    'show_success': False
-}
-
-Result = {"nowResponse": {}}
-
 
 class Gvalues(object):
-    __slots__ = ('__value')
+    __slots__ = '__value'
 
     def __init__(self):
         self.__value = dict()
 
     def set(self, key, value):
         self.__value.update({key: value})
 
@@ -63,355 +58,352 @@
     def extend(self, key, value):
         self.__value.get(key).extend(value)
 
     def insert(self, key, index, value):
         self.__value.get(key).insert(index, value)
 
 
-GG = Gvalues()
-
-dd_paramet = dict()
-
-exit_info = {"fail": False, "status": "passed"}
-
-
-def getEnvData(env_path, env_name):
-    try:
-        with open(env_path, 'r', encoding='utf-8')as f:
-            envs = json.loads(f.read())
-        return jsonpath(envs, f'$..[?(@.env_name=="{env_name}")]')[0]
-    except Exception:
-        return dict()
+class Image(object):
+    def __init__(self):
+        self.src = ''
 
 
-def node_handle(node, item, call):
-    d = dict()
-    # 模块
-    d['model'] = item.module.__name__
-    # 类
-    d['classed'] = '' if item.parent.obj == item.module else item.parent.obj.__name__
-    # 方法
-    d['method'] = item.originalname
-    # 描述
-    d['doc'] = item.function.__doc__
-    # 响应时间
-    d['duration'] = call.duration
-    # 结果
-    d['status'] = node.outcome
-    # 详细内容
-    if node.sections:
-        d["print"] = ''.join(node.sections[0][1:]).replace('<', '&lt;').replace('>', '&gt;')
-    # 异常信息展示
-    if call.excinfo:
-        excobj = node.longrepr
-        try:
-            if d['status'] == 'skipped':
-                d["skipped"] = excobj[-1].replace('<', '&lt;').replace('>', '&gt;')
-            else:
-                # 错误的响应信息，如没有设置verfy
-                d.update(call.excinfo.value.value.query_info)
-                d.update(call.excinfo.value.value.error_info)
-        except Exception:
-            # 异常情况
-            try:
-                exc_list = ["file " + excobj.reprcrash.path + ", line " + str(excobj.reprcrash.lineno), excobj.reprcrash.message.replace('<', '&lt;').replace('>', '&gt;')]
-            except Exception:
-                try:
-                    exc_list = excobj.tblines
-                    errorstring = excobj.errorstring
-                    exc_list.append(errorstring)
-                except Exception:
-                    exc_list = [str(call.excinfo).replace('<', '&lt;').replace('>', '&gt;')]
-            d.update(dict(msg_dict="\n".join(exc_list)))
-            # 失败的的类型
-            failed_list = ["AssertionError", "assert"]
-            # 如果不是失败类型就是错误的
-            if not any([exc_list[-1].startswith(ee) for ee in failed_list]):
-                d['status'] = "error"
-                node.outcome = "error"
+_dict_data = {
+    "apiresult": False,
+    "response": {},
+    "host": "",
+    "mysql_config": None,
+    "pg_config": None,
+    "loop_name": "",
+    "fail": False,
+    "status": "passed",
+    "imgs": Image(),
+    "teme_save_query": {"ddquery": None},
+}
 
-    # 打印正确请求
-    if GG.get("@@ddreportQuery") and dict_data['show_success'] is True:
-        queryData = GG.get("@@ddreportQuery")
-        if queryData:
-            Pro = Process()
-            Pro.data_process(queryData, None)
-            d.update(Pro.query_info)
-    return d
+GG = Gvalues()
 
+_paramet_dict_data = dict()
 
 def pytest_addoption(parser):
     """添加main的可调用参数"""
-    group = parser.getgroup("testreport")
-    group.addoption(
+    # group = parser.getgroup("testreport")
+
+    parser.addoption(
         "--ddreport",
         action="store",
         default=None,
         help="测试报告标识",
     )
-    group.addoption(
+    parser.addoption(
         "--title",
         action="store",
         default=None,
         help="测试报告最顶部标题",
     )
-    group.addoption(
+    parser.addoption(
         "--desc",
         action="store",
         default=None,
         help="当前测试报告的说明",
     )
-    group.addoption(
+    parser.addoption(
         "--tester",
         action="store",
         default=None,
         help="测试人员",
     )
-    group.addoption(
-        "--env_path",
+    parser.addoption(
+        "--envpath",
         action="store",
         default=None,
         help="环境配置路径",
     ),
-    group.addoption(
-        "--env_name",
+    parser.addoption(
+        "--envname",
         action="store",
         default=None,
         help="环境名称",
     ),
-    group.addoption(
+    parser.addoption(
         "--receive",
         action="store",
         default=None,
         help="接收一个字典类型的参数",
     ),
-    group.addoption(
-        "--api_success",
+    parser.addoption(
+        "--apiresult",
         action="store",
         default=None,
         help="是否打印正确的api请求信息",
-    ),
+    )
+
+
+def pytest_report_teststatus(config, report):
+    # 更新终端打印（.  s   F  E）
+    if report.outcome == 'error':
+        return report.outcome, 'E', None
 
 
 def pytest_sessionstart(session):
     test_result['start_time'] = time.strftime("%Y-%m-%d %H:%M:%S")
     test_result['title'] = session.config.getoption('--title') or ''
     test_result['tester'] = session.config.getoption('--tester') or ''
     test_result['desc'] = session.config.getoption('--desc') or ''
     # 是否展示正确的请求及响应信息
-    success_show = session.config.getoption('--api_success')
-    try:
-        if success_show.upper() == "TRUE" or int(success_show) == 1:
-            dict_data['show_success'] = True
-        else:
-            dict_data['show_success'] = False
-    except Exception:
-        dict_data['show_success'] = False
+    apiresult = session.config.getoption('--apiresult')
+    _dict_data["apiresult"] = apiresult == "1"
     # 记录命令传过来的参数
     receive_dict = session.config.getoption("--receive")
     if receive_dict:
         try:
             receive_dict = json.loads(receive_dict)
         except Exception:
             try:
                 receive_dict = ast.literal_eval(receive_dict)
             except Exception:
                 receive_dict = {}
         for k, v in receive_dict.items():
             GG.set(k, v)
+    # 环境获取
+    envpath = session.config.getoption("--envpath")
+    envname = session.config.getoption("--envname")
+    env_data = get_env(envpath, envname)
+    host = env_data.get('host') or ''
+    mysql_config = env_data.get('mysql')
+    pg_config = env_data.get('pg')
+    _dict_data["host"] = host
+    _dict_data["mysql_config"] = mysql_config
+    _dict_data["pg_config"] = pg_config
 
 
 def pytest_sessionfinish(session, exitstatus):
-    def set_default(obj):
-        if isinstance(obj, (list, dict)):
-            return str(obj).replace('<', '&lt;').replace('>', '&gt;')
     test_result['end_time'] = time.strftime("%Y-%m-%d %H:%M:%S")
-    ddreport = session.config.getoption('--ddreport')
-    if ddreport:
-        report_dirOrFile = ddreport.replace('\\', '/').strip()
-        if not report_dirOrFile.endswith('.html'):
-            report_dir, report_name = report_dirOrFile, f'testReport {time.strftime("%Y-%m-%d_%H%M%S")}.html'
+    ddreport_path = session.config.getoption('--ddreport')
+    if ddreport_path:
+        report_dir_File = ddreport_path.replace('\\', '/').strip()
+        if not report_dir_File.endswith('.html'):
+            report_dir, report_name = report_dir_File, f'report_{time.strftime("%Y%m%d-%H%M%S")}.html'
         else:
-            report_dir, report_name = '/'.join(report_dirOrFile.split('/')[:-1]), report_dirOrFile.split('/')[-1]
+            report_dir, report_name = '/'.join(report_dir_File.split('/')[:-1]), report_dir_File.split('/')[-1]
         if not os.path.exists(report_dir):
             os.makedirs(report_dir)
         report_save_path = os.path.join(report_dir, report_name)
         # 读取测试报告文件
-        template_path = os.path.join(os.path.dirname(__file__), './template')
-        with open(f'{template_path}/index.html', 'r', encoding='utf-8')as f:
+        template_path = os.path.join(os.path.dirname(__file__), 'template', 'index.html')
+        with open(f'{template_path}', 'r', encoding='utf-8') as f:
             template = f.read()
         report_template = template.replace('templateData', json.dumps(test_result))
         with open(report_save_path, 'w', encoding='utf-8') as f:
             f.write(report_template)
 
 
-@pytest.hookimpl(tryfirst=True, hookwrapper=True)
-def pytest_runtest_makereport(item, call):
-    outcome = yield
-    report = outcome.get_result()
-    call.duration = '%.2f' % call.duration          # 科学计数转普通格式
-    info = {}
-    if report.when == 'call':
-        # 过滤不需要的funcargs
-        dd_paramet.clear()
-        params_keys = [om.args[0] for om in item.own_markers if om.args]
-        for k in item.fixturenames:
-            if k in ["_session_faker", "request"]:
-                continue
-            elif params_keys and k in params_keys:
-                continue
-            else:
-                dd_paramet[k] = item.funcargs[k]
-        info = node_handle(report, item, call)
-        test_result[report.outcome] += 1
-        # 失败结束标签
-        if item.funcargs.get("ddreport") and item.funcargs["ddreport"].pyexit is True:
-            exit_info["fail"] = True
-            exit_info["status"] = report.outcome
-            if report.outcome != "passed":
-                info["fail_tag"] = "用例标记为: 非成功用例，程序结束"
-    elif report.outcome == 'failed':
-        report.outcome = 'error'
-        info = node_handle(report, item, call)
-        test_result['error'] += 1
-    elif report.outcome == 'skipped':
-        info = node_handle(report, item, call)
-        test_result[report.outcome] += 1
-    if report.when == 'teardown':
-        # 是否有图片信息
-        if GG.get("@ddImage"):
-            Result["nowResponse"].update(dict(img=GG.get("@ddImage")))
-        test_result["cases"].append(Result["nowResponse"])
-        GG.set("@@ddreportQuery", None)
-        GG.set("@ddImage", None)
-        if exit_info["fail"]:
-            if exit_info["status"] != "passed":
-                pytest.exit()
-            else:
-                item.funcargs["ddreport"].pyexit = False
-                exit_info.update({"fail": False, "status": "passed"})
-    Result["nowResponse"] = info
-
-
-@pytest.fixture(scope='session')
-def ddreport(request):
-    # 环境获取
-    env_path = request.config.getoption("--env_path")
-    env_name = request.config.getoption("--env_name")
-    get_env = getEnvData(env_path, env_name)
-    host = get_env.get('host') or ''
-    mysqlConfig = get_env.get('mysql')
-    return DDreport(host, mysqlConfig)
-
-
-class DDreport:
-    def __init__(self, host, mysqlConfig):
-        self.gval = GG
-        self.api = CustomQuery(GG, host)
-        self.fc = PytestFunctions()
-        self.mysql = None
-        if mysqlConfig:
-            from ddreport.db import PytestMysql
-            self.mysql = PytestMysql(mysqlConfig)
-        self.pyexit = False      # 失败后结束程序
-        super().__init__()
-
-
 def pytest_runtest_protocol(item, nextitem):
-
     # 笛卡尔乘积索引
     def cartesian_product_index(input_list):
         if len(input_list) == 0:
             return [[]]
         result = []
-        for i, element in enumerate(input_list[0]):
+        for ele, element in enumerate(input_list[0]):
             for sub_index in cartesian_product_index(input_list[1:]):
-                result.append([(i, element)] + sub_index)
+                result.append([(ele, element)] + sub_index)
         return result
 
     # copy-item-function
     def copy_item(curitem):
         newitem = Function.from_parent(name=curitem.originalname, parent=curitem.parent, callspec=curitem.callspec,
                                        fixtureinfo=curitem._fixtureinfo, originalname=curitem.originalname)
         return newitem
 
-    # 是否使用ddreport的动态参数化
+    # item.funcargs赋值
+    def item_funcargs(item):
+        for k, v in _paramet_dict_data.items():
+            item.funcargs[k] = _paramet_dict_data[k]
+
+    module_name = item._request.node.module.__name__
+    class_name = item._request.node.parent.obj.__name__
+    function_name = item._request.node.originalname
+    all_name = module_name + class_name + function_name
+    if _dict_data["loop_name"] == all_name:
+        return True
+    # 是否使用动态参数化
     is_cus_loop = False
     data_list = list()
     for i in item.own_markers:
         if i.name == "parametrize":
             args_key = i.args[0]
-            args_str = i.args[-1]
-            if isinstance(args_str, str) and args_str.endswith("}") and any([args_str.startswith(k) for k in ["{self.", "{cls.", "{dd."]]):
+            args_var = i.args[-1]
+            if isinstance(args_var, set):
                 is_cus_loop = True
-                args_name = args_str[1:-1]
-                if args_name.startswith("self.") or args_name.startswith("cls."):
-                    obj_names = args_name.replace("self.", "").replace("cls.", "").split("[")
-                    obj_name, obj_item = obj_names[0], obj_names[-1][1:-2]
-                    if obj_item:
-                        data = item.parent._obj.__dict__.get(obj_name, {}).get(obj_item)
-                    else:
-                        data = item.parent._obj.__dict__.get(obj_name)
-                elif args_name.startswith("dd."):
-                    obj_name = args_name.replace("dd.", "")
-                    data = GG.get(obj_name) or None
+                _dict_data["loop_name"] = all_name
+                var_name = list(args_var)[0]
+                if var_name.startswith("dd."):
+                    data = GG.get(var_name[3:]) or None
+                else:
+                    data = item.module.__dict__.get(var_name, None)
             else:
-                data = args_str
-            if not isinstance(data,Iterable):
+                data = args_var
+            if not isinstance(data, Iterable):
                 data = [data]
             data_list.append({args_key: data})
-
     if is_cus_loop:
         ks = list(map(lambda x: list(x.keys())[0], data_list))
         vals = list(map(lambda x: list(x.values())[0], data_list))
         index_list = cartesian_product_index(vals)
+        import copy
         for loop_data in index_list:
-            new_item = copy_item(item)
+            item = copy_item(item)
             params_d = dict()
             indices_d = dict()
             for n, it in enumerate(loop_data):
                 indices_val = it[0]
                 params_val = it[1]
                 indices_d.update({ks[n]: indices_val})
                 params_d.update({ks[n]: params_val})
-            new_item.callspec.params.update(params_d)
-            new_item.callspec.indices.update(indices_d)
-            for k, v in dd_paramet.items():
-                new_item.funcargs[k] = dd_paramet[k]
-            runtestprotocol(new_item, nextitem=None)
+            item.callspec.params.update(params_d)
+            item.callspec.indices.update(indices_d)
+            item_funcargs(item)
+            runtestprotocol(item, nextitem=None)
         return True
     else:
-        for k, v in dd_paramet.items():
-            item.funcargs[k] = dd_paramet[k]
+        item_funcargs(item)
 
 
-def pytest_report_teststatus(config, report):
-    # 更新终端打印（.  s   F  E）
-    if report.outcome == 'error':
-        return report.outcome, 'E', None
+@pytest.hookimpl(hookwrapper=True, tryfirst=True)
+def pytest_runtest_makereport(item, call):
+    outcome = yield
+    report = outcome.get_result()
+    call.duration = '%.2f' % float(call.duration)  # 科学计数转普通格式
+    info = {}
+    if report.when == 'call':
+        # 过滤不需要的funcargs
+        _paramet_dict_data.clear()
+        params_keys = [om.args[0] for om in item.own_markers if om.args]
+        for k in item.fixturenames:
+            if k in ["_session_faker", "request"]:
+                continue
+            elif params_keys and k in params_keys:
+                continue
+            else:
+                _paramet_dict_data[k] = item.funcargs[k]
+        info = node_handle(report, item, call)
+        test_result[report.outcome] += 1
+        # 失败结束标签
+        if item.funcargs:
+            for k, ele_func in item.funcargs.items():
+                if ele_func.__class__.__name__ == "DDreportClass" and ele_func.failexit is True:
+                    _dict_data["fail"] = True
+                    _dict_data["status"] = report.outcome
+                    if report.outcome != "passed":
+                        info["fail_tag"] = "用例标记为: 非成功用例，程序结束"
+    elif report.outcome == 'failed':
+        report.outcome = 'error'
+        info = node_handle(report, item, call)
+        test_result['error'] += 1
+    elif report.outcome == 'skipped':
+        info = node_handle(report, item, call)
+        test_result[report.outcome] += 1
+    if report.when == 'teardown':
+        # 是否有图片信息
+        if _dict_data["imgs"].src:
+            _dict_data["response"].update(dict(img=_dict_data["imgs"].src + ""))
+        test_result["cases"].append(_dict_data["response"])
+        # 初始化数据
+        _dict_data["imgs"].src = ""
+        _dict_data["teme_save_query"]["ddquery"] = {}
+        # 是否条件结束程序
+        if _dict_data["fail"] and _dict_data["status"] != "passed":
+            pytest.exit("条件终止程序")
+        # 修改条件结束参数
+        if item.funcargs:
+            for k, ele_func in item.funcargs.items():
+                if ele_func.__class__.__name__ == "DDreportClass":
+                    ele_func.failexit = False
+                    _dict_data.update({"fail": False, "status": "passed"})
+    _dict_data["response"] = info
 
 
-def pytest_collection_modifyitems(session, config, items):
-    # 处理用例收集函数
-    new_items = list()
-    parame_name = list()
-    for i in items:
-        if not i.own_markers:
-            new_items.append(i)
-        else:
-            for p in i.own_markers:
-                if p.name == "parametrize":
-                    if isinstance(p.args[-1], str) and p.args[-1].startswith("{") and p.args[-1].endswith("}"):
-                        args_name = p.args[-1][1:-1]
-                        if args_name.startswith("self.") or args_name.startswith("dd."):
-                            item_name = i.module.__name__ + "&" + i.originalname
-                            if item_name not in parame_name:
-                                parame_name.append(item_name)
-                                new_items.append(i)
-                            break
-                    new_items.append(i)
-                else:
-                    new_items.append(i)
+def node_handle(node, item, call):
+    d = dict()
+    # 模块
+    d['model'] = item.module.__name__
+    # 类
+    d['classed'] = '' if item.parent.obj == item.module else item.parent.obj.__name__
+    # 方法
+    d['method'] = item.originalname
+    # 描述
+    d['doc'] = item.function.__doc__
+    # 响应时间
+    d['duration'] = float(call.duration)
+    # 结果
+    d['status'] = node.outcome
+    # 详细内容
+    if node.sections:
+        d["print"] = node.sections[-1][1].replace('<', '&lt;').replace('>', '&gt;')
+    # 异常信息展示
+    if call.excinfo:
+        excobj = node.longrepr
+        try:
+            if d['status'] == 'skipped':
+                d["skipped"] = excobj[-1].replace('<', '&lt;').replace('>', '&gt;')
+            else:
+                # 错误的响应信息，如没有设置verfy
+                d.update(call.excinfo.value.value.query_info)
+                d.update(call.excinfo.value.value.error_info)
+        except Exception:
+            # 异常情况
+            try:
+                exc_list = ["file " + excobj.reprcrash.path + ", line " + str(excobj.reprcrash.lineno),
+                            excobj.reprcrash.message.replace('<', '&lt;').replace('>', '&gt;')]
+            except Exception:
+                try:
+                    exc_list = excobj.tblines
+                    errorstring = excobj.errorstring
+                    exc_list.append(errorstring)
+                except Exception:
+                    exc_list = [str(call.excinfo).replace('<', '&lt;').replace('>', '&gt;')]
+            d.update(dict(msg_dict="\n".join(exc_list)))
+            # 失败的的类型
+            failed_list = ["AssertionError", "assert"]
+            # 如果不是失败类型就是错误的
+            if not any([exc_list[-1].startswith(ee) for ee in failed_list]):
+                d['status'] = "error"
+                node.outcome = "error"
+    # 打印正确请求
+    if _dict_data["teme_save_query"].get("ddquery") and _dict_data["apiresult"] is True:
+        query_data = _dict_data["teme_save_query"].get("ddquery")
+        if query_data:
+            pro = Process()
+            pro.data_process(query_data, None)
+            d.update(pro.query_info)
+    return d
+
+
+def get_env(env_path, env_name):
+    try:
+        with open(env_path, 'r', encoding='utf-8') as f:
+            envs = json.loads(f.read())
+        return jsonpath(envs, f'$..[?(@.env_name=="{env_name}")]')[0]
+    except Exception:
+        return dict()
+
+
+class DDreportClass:
+    def __init__(self):
+        self.host = _dict_data["host"]
+        self.failexit = False  # 失败后结束程序
+        self.gval = GG
+        self.api = DDreportQuery(GG, self.host, _dict_data["teme_save_query"])
+        self.fc = DDreportFunctions()
+        self.assertion = DataDiff()
+        self.img = _dict_data["imgs"]
+        self.mysql = None
+        self.pg = None
+        if _dict_data.get("mysql_config"):
+            self.mysql = DDreportMysql(_dict_data["mysql_config"])
+        if _dict_data.get("pg_config"):
+            self.pg = DDreportPg(_dict_data["pg_config"])
+        super().__init__()
+
 
-    session.items = new_items
-    items = new_items
-    config.pluginmanager.get_plugin("terminalreporter")._numcollected = len(session.items)
+def ddreport():
+    return DDreportClass()
```

### Comparing `ddreport-4.5/setup.py` & `ddreport-4.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,31 +23,38 @@
     setup.py        当前文件
 
 1.cmd进入UPSDIST目录
 2.执行命令：python setup.py sdist
 3.执行命令：twine upload dist/*
 '''
 
-
-
-#### 每次更新需要修改 version 字段
-
+# 每次更新需要修改 version 字段
 from setuptools import setup, find_packages, find_namespace_packages
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
-    name = "ddreport",
-    version = "4.5",
-    # keywords = ("pip", "pytest","testReport"),
-    description = "pytest测试报告",
-    long_description = "1.当请求成功时，编辑信息头将不会再覆盖请求时设置的信息头内容; 2.关键字改为小写（API->api, GVALUE->gval, FC->fc, MYSQL->mysql）; 3.一条用例支持多个参数化; 4.重写动态参数化实现逻辑",
-    license = "MIT Licence",
+    name="ddreport",
+    version="4.6",
+    keywords=("pytest", "ddreport", "pytestReport"),
+    description="pytest测试报告",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url="https://zhuanlan.zhihu.com/p/692810160",
+    author="duanliangcong",
+    author_email="137562703@qq.com",
+    classifiers=[
+        'Framework :: Pytest',
+        'Programming Language :: Python',
+        'Topic :: Software Development :: Testing'
+    ],
+    license="MIT Licence",
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={"pytest11": ["testreport=ddreport"]},
+    platforms="any",
+    install_requires=["requests", "sshtunnel", "pymysql", "psycopg2", "jsonpath", 'openpyxl', 'deepdiff', 'python-dateutil'],
+)
 
-    url = "https://blog.csdn.net/weixin_43975720/article/details/130559489",
-    author = "duanliangcong",
-    author_email = "137562703@qq.com",
-    entry_points={"pytest11": ["test_report=ddreport.testReport"]},
 
-    packages = find_packages(),
-    include_package_data = True,
-    platforms = "any",
-    install_requires = ["pytest", "requests", "sshtunnel", "pymysql", "jsonpath", 'openpyxl', 'deepdiff'],
-)
```

