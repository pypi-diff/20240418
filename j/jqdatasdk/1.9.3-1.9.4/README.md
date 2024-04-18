# Comparing `tmp/jqdatasdk-1.9.3.tar.gz` & `tmp/jqdatasdk-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jqdatasdk-1.9.3.tar", last modified: Tue Mar 12 11:48:39 2024, max compression
+gzip compressed data, was "jqdatasdk-1.9.4.tar", last modified: Thu Apr 18 10:01:02 2024, max compression
```

## Comparing `jqdatasdk-1.9.3.tar` & `jqdatasdk-1.9.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-03-12 11:48:39.781331 jqdatasdk-1.9.3/
--rw-r--r--   0 huoty      (501) staff       (20)     2100 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/CHANGELOG.md
--rw-r--r--   0 huoty      (501) staff       (20)     1066 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/LICENSE
--rw-r--r--   0 huoty      (501) staff       (20)       26 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/MANIFEST.in
--rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-03-12 11:48:39.781216 jqdatasdk-1.9.3/PKG-INFO
--rw-r--r--   0 huoty      (501) staff       (20)     4767 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/README.md
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-03-12 11:48:39.778871 jqdatasdk-1.9.3/jqdatasdk/
--rw-r--r--   0 huoty      (501) staff       (20)     1893 2024-03-08 07:08:51.000000 jqdatasdk-1.9.3/jqdatasdk/__init__.py
--rw-r--r--   0 huoty      (501) staff       (20)    56654 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/alpha101.py
--rw-r--r--   0 huoty      (501) staff       (20)    88690 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/alpha191.py
--rw-r--r--   0 huoty      (501) staff       (20)    51403 2024-03-08 07:27:56.000000 jqdatasdk-1.9.3/jqdatasdk/api.py
--rw-r--r--   0 huoty      (501) staff       (20)     1680 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/calendar_service.py
--rw-r--r--   0 huoty      (501) staff       (20)    17327 2024-03-08 07:08:51.000000 jqdatasdk-1.9.3/jqdatasdk/client.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-03-12 11:48:39.779788 jqdatasdk-1.9.3/jqdatasdk/compat/
--rw-r--r--   0 huoty      (501) staff       (20)        0 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/compat/__init__.py
--rw-r--r--   0 huoty      (501) staff       (20)     8710 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/compat/pickle_compat.py
--rw-r--r--   0 huoty      (501) staff       (20)      166 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/exceptions.py
--rw-r--r--   0 huoty      (501) staff       (20)    10242 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/finance_service.py
--rw-r--r--   0 huoty      (501) staff       (20)    28674 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/finance_tables.py
--rw-r--r--   0 huoty      (501) staff       (20)    33828 2023-10-25 11:44:21.000000 jqdatasdk-1.9.3/jqdatasdk/fundamentals_tables_gen.py
--rw-r--r--   0 huoty      (501) staff       (20)     4235 2024-01-03 07:42:27.000000 jqdatasdk-1.9.3/jqdatasdk/table.py
--rw-r--r--   0 huoty      (501) staff       (20)   106372 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/technical_analysis.py
--rw-r--r--   0 huoty      (501) staff       (20)      836 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/thriftclient.py
--rw-r--r--   0 huoty      (501) staff       (20)    14833 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/jqdatasdk/utils.py
--rw-r--r--   0 huoty      (501) staff       (20)      422 2024-03-05 02:06:54.000000 jqdatasdk-1.9.3/jqdatasdk/version.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-03-12 11:48:39.779604 jqdatasdk-1.9.3/jqdatasdk.egg-info/
--rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-03-12 11:48:39.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/PKG-INFO
--rw-r--r--   0 huoty      (501) staff       (20)      795 2024-03-12 11:48:39.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/SOURCES.txt
--rw-r--r--   0 huoty      (501) staff       (20)        1 2024-03-12 11:48:39.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/dependency_links.txt
--rw-r--r--   0 huoty      (501) staff       (20)        1 2023-11-02 08:41:51.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/not-zip-safe
--rw-r--r--   0 huoty      (501) staff       (20)      106 2024-03-12 11:48:39.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/requires.txt
--rw-r--r--   0 huoty      (501) staff       (20)       10 2024-03-12 11:48:39.000000 jqdatasdk-1.9.3/jqdatasdk.egg-info/top_level.txt
--rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/requirements-py2.txt
--rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/requirements.txt
--rw-r--r--   0 huoty      (501) staff       (20)       38 2024-03-12 11:48:39.781366 jqdatasdk-1.9.3/setup.cfg
--rw-r--r--   0 huoty      (501) staff       (20)     2123 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/setup.py
-drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-03-12 11:48:39.780997 jqdatasdk-1.9.3/tests/
--rw-r--r--   0 huoty      (501) staff       (20)    78213 2024-03-12 10:40:22.000000 jqdatasdk-1.9.3/tests/test_api.py
--rw-r--r--   0 huoty      (501) staff       (20)      487 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/tests/test_client.py
--rw-r--r--   0 huoty      (501) staff       (20)     3670 2024-01-03 07:39:42.000000 jqdatasdk-1.9.3/tests/test_table.py
--rw-r--r--   0 huoty      (501) staff       (20)     2216 2023-10-09 02:41:53.000000 jqdatasdk-1.9.3/tests/test_utils.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.852576 jqdatasdk-1.9.4/
+-rw-r--r--   0 huoty      (501) staff       (20)     2100 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/CHANGELOG.md
+-rw-r--r--   0 huoty      (501) staff       (20)     1066 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/LICENSE
+-rw-r--r--   0 huoty      (501) staff       (20)       26 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/MANIFEST.in
+-rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-04-18 10:01:02.852452 jqdatasdk-1.9.4/PKG-INFO
+-rw-r--r--   0 huoty      (501) staff       (20)     4767 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/README.md
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.849860 jqdatasdk-1.9.4/jqdatasdk/
+-rw-r--r--   0 huoty      (501) staff       (20)     1893 2024-03-08 07:08:51.000000 jqdatasdk-1.9.4/jqdatasdk/__init__.py
+-rw-r--r--   0 huoty      (501) staff       (20)    56654 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/alpha101.py
+-rw-r--r--   0 huoty      (501) staff       (20)    88690 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/alpha191.py
+-rw-r--r--   0 huoty      (501) staff       (20)    53070 2024-04-18 09:40:52.000000 jqdatasdk-1.9.4/jqdatasdk/api.py
+-rw-r--r--   0 huoty      (501) staff       (20)     1680 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/calendar_service.py
+-rw-r--r--   0 huoty      (501) staff       (20)    17404 2024-03-13 06:29:19.000000 jqdatasdk-1.9.4/jqdatasdk/client.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.850813 jqdatasdk-1.9.4/jqdatasdk/compat/
+-rw-r--r--   0 huoty      (501) staff       (20)        0 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/compat/__init__.py
+-rw-r--r--   0 huoty      (501) staff       (20)     8710 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/compat/pickle_compat.py
+-rw-r--r--   0 huoty      (501) staff       (20)      166 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/exceptions.py
+-rw-r--r--   0 huoty      (501) staff       (20)    10242 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/finance_service.py
+-rw-r--r--   0 huoty      (501) staff       (20)    28674 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/finance_tables.py
+-rw-r--r--   0 huoty      (501) staff       (20)    33828 2023-10-25 11:44:21.000000 jqdatasdk-1.9.4/jqdatasdk/fundamentals_tables_gen.py
+-rw-r--r--   0 huoty      (501) staff       (20)     4235 2024-01-03 07:42:27.000000 jqdatasdk-1.9.4/jqdatasdk/table.py
+-rw-r--r--   0 huoty      (501) staff       (20)   106372 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/technical_analysis.py
+-rw-r--r--   0 huoty      (501) staff       (20)      836 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/thriftclient.py
+-rw-r--r--   0 huoty      (501) staff       (20)    14833 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/jqdatasdk/utils.py
+-rw-r--r--   0 huoty      (501) staff       (20)      422 2024-04-18 09:58:20.000000 jqdatasdk-1.9.4/jqdatasdk/version.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.850626 jqdatasdk-1.9.4/jqdatasdk.egg-info/
+-rw-r--r--   0 huoty      (501) staff       (20)     5489 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/PKG-INFO
+-rw-r--r--   0 huoty      (501) staff       (20)      795 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 huoty      (501) staff       (20)        1 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 huoty      (501) staff       (20)        1 2023-11-02 08:41:51.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/not-zip-safe
+-rw-r--r--   0 huoty      (501) staff       (20)      106 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/requires.txt
+-rw-r--r--   0 huoty      (501) staff       (20)       10 2024-04-18 10:01:02.000000 jqdatasdk-1.9.4/jqdatasdk.egg-info/top_level.txt
+-rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/requirements-py2.txt
+-rw-r--r--   0 huoty      (501) staff       (20)      106 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/requirements.txt
+-rw-r--r--   0 huoty      (501) staff       (20)       38 2024-04-18 10:01:02.852634 jqdatasdk-1.9.4/setup.cfg
+-rw-r--r--   0 huoty      (501) staff       (20)     2123 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/setup.py
+drwxr-xr-x   0 huoty      (501) staff       (20)        0 2024-04-18 10:01:02.852191 jqdatasdk-1.9.4/tests/
+-rw-r--r--   0 huoty      (501) staff       (20)    79416 2024-04-18 08:58:43.000000 jqdatasdk-1.9.4/tests/test_api.py
+-rw-r--r--   0 huoty      (501) staff       (20)      487 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/tests/test_client.py
+-rw-r--r--   0 huoty      (501) staff       (20)     3670 2024-01-03 07:39:42.000000 jqdatasdk-1.9.4/tests/test_table.py
+-rw-r--r--   0 huoty      (501) staff       (20)     2216 2023-10-09 02:41:53.000000 jqdatasdk-1.9.4/tests/test_utils.py
```

### Comparing `jqdatasdk-1.9.3/CHANGELOG.md` & `jqdatasdk-1.9.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/LICENSE` & `jqdatasdk-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/PKG-INFO` & `jqdatasdk-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqdatasdk
-Version: 1.9.3
+Version: 1.9.4
 Summary: jqdatasdk<easy utility for getting financial market data of China>
 Home-page: https://www.joinquant.com/data
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: tech_data
 Maintainer-email: tech_data@joinquant.com
 License: Apache License v2
```

### Comparing `jqdatasdk-1.9.3/README.md` & `jqdatasdk-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/__init__.py` & `jqdatasdk-1.9.4/jqdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/alpha101.py` & `jqdatasdk-1.9.4/jqdatasdk/alpha101.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/alpha191.py` & `jqdatasdk-1.9.4/jqdatasdk/alpha191.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/api.py` & `jqdatasdk-1.9.4/jqdatasdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1001,24 +1001,28 @@
         raise ParamsError("(start_date, count) only one param is required")
     start_date = to_date_str(start_date)
     end_date = to_date_str(end_date)
     return JQDataClient.instance().get_factor_style_returns(**locals())
 
 
 @assert_auth
-def get_factor_specific_returns(security, start_date=None, end_date=None, count=None,
-                                category="style"):
+def get_factor_specific_returns(security, start_date=None, end_date=None,
+                                count=None, category='style',
+                                universe=None, industry='sw_l1'):
     """获取风格因子的特异收益率
 
     参数:
         security : 股票代码, 或者股票代码组成的list
         start_date : 开始日期，字符串或 datetime 对象
         end_date : 结束日期，字符串或 datetime 对象，可以与 start_date 或 count 配合使用
         count : 截止 end_date 之前交易日的数量（含 end_date 当日）
         category : 风格因子分类, 可选 'style' 和 'style_pro', 默认 'style'
+        universe : 市场范围, 默认为 None 代表全市场, 可选 : 'hs300':沪深300; 'zz500':中证500'; zz800':中证800; 'zz1000':中证1000; 'zzqz':中证全指; 'zz2000':中证2000
+        industry : 行业选取, 默认为 'sw_l1',可选 : 'sw_l1':申万一级, 'jq_l1':聚宽一级
+
     返回:
         个股在风格因子上的特异收益率
     """
     if count and start_date:
         raise ParamsError("(start_date, count) only one param is required")
     start_date = to_date_str(start_date)
     end_date = to_date_str(end_date)
@@ -1125,14 +1129,42 @@
             alpha = [alpha]
         assert isinstance(alpha, list), "不合法的 alpha 类型"
 
     return JQDataClient.instance().get_all_alpha_191(**locals())
 
 
 @assert_auth
+def get_order_future_bar(symbol,
+                         future_type,
+                         start_dt,
+                         end_dt,
+                         unit='1d',
+                         fields=('date', 'open', 'high', 'low', 'close','volume', 'money', 'open_interest'),
+                         include_now=True):
+    """获取当月/次月/当季/隔季等合约拼接而成的行情数据
+    参数
+        symbol : 品种代码, 如 'IF'
+        future_type : 合约类型, 按当前可交易的合约顺序推算, 0 为当月, 1 为次月, 也可以按季度, '0q' 为当季(最近一个季月), '1q' 为次季 .....
+        start_dt : 开始时间
+        end_dt : 结束时间
+        unit : bar 频率, 只支持 (x)m 或者 1d, 划分方式同 get_bars, 不支持 1w 和 1M
+        fields : 获取字段, 同 get_bars, 默认为全部
+        include_now : 是否包含当前 bar
+    返回
+        DataFrame, columns 是 code + 参数 fields 中指定的列
+    """
+    start_dt = to_date_str(start_dt)
+    end_dt = to_date_str(end_dt)
+    assert unit.endswith("m") or unit.endswith("d"), 'unit 只支持 (x)m 或者 1d'
+    if not isinstance(fields, (list, tuple, set)):
+        fields = [fields]
+    return JQDataClient.instance().get_order_future_bar(**locals())
+
+
+@assert_auth
 def get_data(api_name, **kwargs):
     """通用数据获取接口
 
     获取非 run_query, alpha 因子, technical_analysis 查询的数据
     :param apis_name 接口名称
     :param kwargs 传入参数，且必须是关键字参数
     """
```

### Comparing `jqdatasdk-1.9.3/jqdatasdk/calendar_service.py` & `jqdatasdk-1.9.4/jqdatasdk/calendar_service.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/client.py` & `jqdatasdk-1.9.4/jqdatasdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,19 +176,22 @@
                     if key in cls._auth_params:
                         cls._auth_params.pop(key)
                 else:
                     cls._auth_params[key] = val
 
     @classmethod
     def set_auth_params(cls, **params):
-        instance = cls.instance(enable_env_param=False)
+        try:
+            instance = cls.instance(enable_env_param=False)
+        except Exception:
+            instance = None
         if params != cls._auth_params and instance:
             instance._reset()
             cls._threading_local._instance = None
-        cls._auth_params = params
+        cls._auth_params.update(params)
         cls.instance().ensure_auth()
 
     def _create_client(self):
         self.client = make_client(
             thrift.JqDataService,
             self.host,
             self.port,
```

### Comparing `jqdatasdk-1.9.3/jqdatasdk/compat/pickle_compat.py` & `jqdatasdk-1.9.4/jqdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/finance_service.py` & `jqdatasdk-1.9.4/jqdatasdk/finance_service.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/finance_tables.py` & `jqdatasdk-1.9.4/jqdatasdk/finance_tables.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/fundamentals_tables_gen.py` & `jqdatasdk-1.9.4/jqdatasdk/fundamentals_tables_gen.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/table.py` & `jqdatasdk-1.9.4/jqdatasdk/table.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/technical_analysis.py` & `jqdatasdk-1.9.4/jqdatasdk/technical_analysis.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/thriftclient.py` & `jqdatasdk-1.9.4/jqdatasdk/thriftclient.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk/utils.py` & `jqdatasdk-1.9.4/jqdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/jqdatasdk.egg-info/PKG-INFO` & `jqdatasdk-1.9.4/jqdatasdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqdatasdk
-Version: 1.9.3
+Version: 1.9.4
 Summary: jqdatasdk<easy utility for getting financial market data of China>
 Home-page: https://www.joinquant.com/data
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: tech_data
 Maintainer-email: tech_data@joinquant.com
 License: Apache License v2
```

### Comparing `jqdatasdk-1.9.3/jqdatasdk.egg-info/SOURCES.txt` & `jqdatasdk-1.9.4/jqdatasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/setup.py` & `jqdatasdk-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/tests/test_api.py` & `jqdatasdk-1.9.4/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1766,7 +1766,33 @@
     # 测试取交易日当天不存在的标的数据
     res_non_exits_m = get_money_flow_pro(['688981.XSHG'],
                                          datetime.datetime(2020, 7, 12, 8),
                                          datetime.datetime(2020, 7, 14, 8),
                                          frequency='1m',
                                          fields=fields)
     assert res_non_exits_m.empty
+
+
+def test_get_order_future_bar():
+    data = get_order_future_bar(symbol='IC',
+                                future_type='1',
+                                start_dt='2020-03-01',
+                                end_dt='2021-03-01',
+                                unit='1d')
+    assert data.date.min() == datetime.date(2020, 3, 2)
+    assert data.date.max() == datetime.date(2021, 2, 26)
+    assert set(data.code) == {
+        'IC2007.CCFX', 'IC2101.CCFX', 'IC2008.CCFX', 'IC2010.CCFX',
+        'IC2005.CCFX', 'IC2004.CCFX', 'IC2006.CCFX', 'IC2009.CCFX',
+        'IC2103.CCFX', 'IC2102.CCFX', 'IC2011.CCFX', 'IC2104.CCFX',
+        'IC2012.CCFX'}
+
+    data = get_order_future_bar(symbol='SC',
+                                future_type='4',
+                                start_dt='1999-03-01 09:00:00',
+                                end_dt='2019-02-27 21:30:00',
+                                unit='1m',
+                                fields=['date', 'close', 'volume'])
+    assert set(data.columns) == {'date', 'close', 'volume', 'code'}
+    assert set(data.code) == {
+        'SC1904.XINE', 'SC1903.XINE', 'SC1902.XINE', 'SC1906.XINE',
+        'SC1905.XINE', 'SC1901.XINE', 'SC1907.XINE'}
```

### Comparing `jqdatasdk-1.9.3/tests/test_table.py` & `jqdatasdk-1.9.4/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `jqdatasdk-1.9.3/tests/test_utils.py` & `jqdatasdk-1.9.4/tests/test_utils.py`

 * *Files identical despite different names*

