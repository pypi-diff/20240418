# Comparing `tmp/pytse_filter-1.32.tar.gz` & `tmp/pytse_filter-1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytse_filter-1.32.tar", last modified: Tue Apr 16 15:37:00 2024, max compression
+gzip compressed data, was "pytse_filter-1.33.tar", last modified: Thu Apr 18 12:16:00 2024, max compression
```

## Comparing `pytse_filter-1.32.tar` & `pytse_filter-1.33.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 15:37:00.219368 pytse_filter-1.32/
--rw-rw-rw-   0        0        0       94 2024-03-21 14:02:36.000000 pytse_filter-1.32/MANIFEST.in
--rw-rw-rw-   0        0        0     4798 2024-04-16 15:37:00.215370 pytse_filter-1.32/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 15:36:59.595882 pytse_filter-1.32/docs/
--rw-rw-rw-   0        0        0   187418 2024-04-06 17:46:37.000000 pytse_filter-1.32/docs/HistoryVariables.xlsx
--rw-rw-rw-   0        0        0    11144 2024-04-16 14:08:03.000000 pytse_filter-1.32/docs/RealTimeVariables.xlsx
--rw-rw-rw-   0        0        0     9994 2024-03-31 17:57:17.000000 pytse_filter-1.32/docs/user guide.md
--rw-rw-rw-   0        0        0    29893 2024-04-09 20:03:39.000000 pytse_filter-1.32/docs/راهنمای کاربر.docx
--rw-rw-rw-   0        0        0    13618 2024-03-31 17:57:42.000000 pytse_filter-1.32/docs/راهنمای کاربر.md
--rw-rw-rw-   0        0        0  1142189 2024-04-09 20:05:37.000000 pytse_filter-1.32/docs/راهنمای کاربر.pdf
-drwxrwxrwx   0        0        0        0 2024-04-16 15:36:59.743798 pytse_filter-1.32/examples/
--rw-rw-rw-   0        0        0      250 2024-03-18 16:27:50.000000 pytse_filter-1.32/examples/code2code.py
--rw-rw-rw-   0        0        0       69 2024-04-10 10:30:47.000000 pytse_filter-1.32/examples/code2code.txt
--rw-rw-rw-   0        0        0      672 2024-04-10 10:31:43.000000 pytse_filter-1.32/examples/combine_history_realtime.py
--rw-rw-rw-   0        0        0      807 2024-03-18 15:57:39.000000 pytse_filter-1.32/examples/disappear_sell_queue.py
--rw-rw-rw-   0        0        0      803 2024-04-10 12:42:17.000000 pytse_filter-1.32/examples/hot_money.py
--rw-rw-rw-   0        0        0     1754 2024-03-18 16:31:29.000000 pytse_filter-1.32/examples/market_overview.py
--rw-rw-rw-   0        0        0     1024 2024-04-10 10:28:48.000000 pytse_filter-1.32/examples/simple_history_filters.py
--rw-rw-rw-   0        0        0     1091 2024-04-10 10:27:24.000000 pytse_filter-1.32/examples/simple_realtime_filters.py
--rw-rw-rw-   0        0        0     1110 2024-02-22 12:28:42.000000 pytse_filter-1.32/license.md
--rw-rw-rw-   0        0        0     3463 2024-03-22 16:16:51.000000 pytse_filter-1.32/readme.md
--rw-rw-rw-   0        0        0      331 2024-04-09 21:03:15.000000 pytse_filter-1.32/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 15:37:00.219368 pytse_filter-1.32/setup.cfg
--rw-rw-rw-   0        0        0     1286 2024-04-16 14:10:28.000000 pytse_filter-1.32/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:36:59.246083 pytse_filter-1.32/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 15:37:00.133602 pytse_filter-1.32/src/pytse_filter/
--rw-rw-rw-   0        0        0      255 2024-03-16 15:42:50.000000 pytse_filter-1.32/src/pytse_filter/__init__.py
--rw-rw-rw-   0        0        0     1252 2024-03-27 15:23:51.000000 pytse_filter-1.32/src/pytse_filter/calculate_client_data.py
--rw-rw-rw-   0        0        0     2430 2024-04-09 20:58:03.000000 pytse_filter-1.32/src/pytse_filter/calculate_indicators.py
--rw-rw-rw-   0        0        0     1178 2024-03-27 15:25:25.000000 pytse_filter-1.32/src/pytse_filter/client_setting.py
--rw-rw-rw-   0        0        0     3815 2024-04-16 13:55:34.000000 pytse_filter-1.32/src/pytse_filter/config.py
--rw-rw-rw-   0        0        0     6228 2024-04-16 13:41:23.000000 pytse_filter-1.32/src/pytse_filter/download_history.py
--rw-rw-rw-   0        0        0     9564 2024-04-16 13:54:25.000000 pytse_filter-1.32/src/pytse_filter/download_realtime.py
--rw-rw-rw-   0        0        0     8407 2024-04-16 13:43:24.000000 pytse_filter-1.32/src/pytse_filter/history.py
--rw-rw-rw-   0        0        0     5065 2024-03-20 10:48:40.000000 pytse_filter-1.32/src/pytse_filter/inds_setting.py
--rw-rw-rw-   0        0        0     7347 2024-03-30 10:57:00.000000 pytse_filter-1.32/src/pytse_filter/realtime.py
--rw-rw-rw-   0        0        0    32725 2024-03-18 15:21:37.000000 pytse_filter-1.32/src/pytse_filter/syms.json
--rw-rw-rw-   0        0        0     1401 2024-03-18 16:46:27.000000 pytse_filter-1.32/src/pytse_filter/syms_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:37:00.214370 pytse_filter-1.32/src/pytse_filter.egg-info/
--rw-rw-rw-   0        0        0     4798 2024-04-16 15:36:59.000000 pytse_filter-1.32/src/pytse_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-16 15:36:59.000000 pytse_filter-1.32/src/pytse_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 15:36:59.000000 pytse_filter-1.32/src/pytse_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      312 2024-04-16 15:36:59.000000 pytse_filter-1.32/src/pytse_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-16 15:36:59.000000 pytse_filter-1.32/src/pytse_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.860867 pytse_filter-1.33/
+-rw-rw-rw-   0        0        0       94 2024-03-21 14:02:36.000000 pytse_filter-1.33/MANIFEST.in
+-rw-rw-rw-   0        0        0     4798 2024-04-18 12:16:00.856871 pytse_filter-1.33/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.253515 pytse_filter-1.33/docs/
+-rw-rw-rw-   0        0        0   187418 2024-04-06 17:46:37.000000 pytse_filter-1.33/docs/HistoryVariables.xlsx
+-rw-rw-rw-   0        0        0    11144 2024-04-16 14:08:03.000000 pytse_filter-1.33/docs/RealTimeVariables.xlsx
+-rw-rw-rw-   0        0        0     9994 2024-03-31 17:57:17.000000 pytse_filter-1.33/docs/user guide.md
+-rw-rw-rw-   0        0        0    29893 2024-04-09 20:03:39.000000 pytse_filter-1.33/docs/راهنمای کاربر.docx
+-rw-rw-rw-   0        0        0    13618 2024-03-31 17:57:42.000000 pytse_filter-1.33/docs/راهنمای کاربر.md
+-rw-rw-rw-   0        0        0  1142189 2024-04-09 20:05:37.000000 pytse_filter-1.33/docs/راهنمای کاربر.pdf
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.486081 pytse_filter-1.33/examples/
+-rw-rw-rw-   0        0        0      250 2024-03-18 16:27:50.000000 pytse_filter-1.33/examples/code2code.py
+-rw-rw-rw-   0        0        0       69 2024-04-10 10:30:47.000000 pytse_filter-1.33/examples/code2code.txt
+-rw-rw-rw-   0        0        0      672 2024-04-10 10:31:43.000000 pytse_filter-1.33/examples/combine_history_realtime.py
+-rw-rw-rw-   0        0        0      807 2024-03-18 15:57:39.000000 pytse_filter-1.33/examples/disappear_sell_queue.py
+-rw-rw-rw-   0        0        0      803 2024-04-10 12:42:17.000000 pytse_filter-1.33/examples/hot_money.py
+-rw-rw-rw-   0        0        0     1754 2024-03-18 16:31:29.000000 pytse_filter-1.33/examples/market_overview.py
+-rw-rw-rw-   0        0        0     1024 2024-04-10 10:28:48.000000 pytse_filter-1.33/examples/simple_history_filters.py
+-rw-rw-rw-   0        0        0     1091 2024-04-10 10:27:24.000000 pytse_filter-1.33/examples/simple_realtime_filters.py
+-rw-rw-rw-   0        0        0     1110 2024-02-22 12:28:42.000000 pytse_filter-1.33/license.md
+-rw-rw-rw-   0        0        0     3463 2024-03-22 16:16:51.000000 pytse_filter-1.33/readme.md
+-rw-rw-rw-   0        0        0      331 2024-04-09 21:03:15.000000 pytse_filter-1.33/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:16:00.860867 pytse_filter-1.33/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-04-18 12:11:31.000000 pytse_filter-1.33/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.043576 pytse_filter-1.33/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.800902 pytse_filter-1.33/src/pytse_filter/
+-rw-rw-rw-   0        0        0      255 2024-03-16 15:42:50.000000 pytse_filter-1.33/src/pytse_filter/__init__.py
+-rw-rw-rw-   0        0        0     1252 2024-03-27 15:23:51.000000 pytse_filter-1.33/src/pytse_filter/calculate_client_data.py
+-rw-rw-rw-   0        0        0     2430 2024-04-09 20:58:03.000000 pytse_filter-1.33/src/pytse_filter/calculate_indicators.py
+-rw-rw-rw-   0        0        0     1178 2024-03-27 15:25:25.000000 pytse_filter-1.33/src/pytse_filter/client_setting.py
+-rw-rw-rw-   0        0        0     3815 2024-04-16 13:55:34.000000 pytse_filter-1.33/src/pytse_filter/config.py
+-rw-rw-rw-   0        0        0     6211 2024-04-18 12:13:27.000000 pytse_filter-1.33/src/pytse_filter/download_history.py
+-rw-rw-rw-   0        0        0     9564 2024-04-16 13:54:25.000000 pytse_filter-1.33/src/pytse_filter/download_realtime.py
+-rw-rw-rw-   0        0        0     8407 2024-04-16 13:43:24.000000 pytse_filter-1.33/src/pytse_filter/history.py
+-rw-rw-rw-   0        0        0     5065 2024-03-20 10:48:40.000000 pytse_filter-1.33/src/pytse_filter/inds_setting.py
+-rw-rw-rw-   0        0        0     7347 2024-03-30 10:57:00.000000 pytse_filter-1.33/src/pytse_filter/realtime.py
+-rw-rw-rw-   0        0        0    32725 2024-03-18 15:21:37.000000 pytse_filter-1.33/src/pytse_filter/syms.json
+-rw-rw-rw-   0        0        0     1401 2024-03-18 16:46:27.000000 pytse_filter-1.33/src/pytse_filter/syms_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.854871 pytse_filter-1.33/src/pytse_filter.egg-info/
+-rw-rw-rw-   0        0        0     4798 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-04-18 12:16:00.000000 pytse_filter-1.33/src/pytse_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      312 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/top_level.txt
```

### Comparing `pytse_filter-1.32/PKG-INFO` & `pytse_filter-1.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytse_filter
-Version: 1.32
+Version: 1.33
 Summary: A user-friendly project to filter symbols of Tehran Stock Exchange
 Home-page: https://github.com/farhad-mohammadi/pytse_filter
 Author: Farhad Mohammadi
 Author-email: farhad.mohammadi60@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytse_filter-1.32/docs/HistoryVariables.xlsx` & `pytse_filter-1.33/docs/HistoryVariables.xlsx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/docs/RealTimeVariables.xlsx` & `pytse_filter-1.33/docs/RealTimeVariables.xlsx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/docs/user guide.md` & `pytse_filter-1.33/docs/user guide.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/docs/راهنمای کاربر.docx` & `pytse_filter-1.33/docs/راهنمای کاربر.docx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/docs/راهنمای کاربر.md` & `pytse_filter-1.33/docs/راهنمای کاربر.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/docs/راهنمای کاربر.pdf` & `pytse_filter-1.33/docs/راهنمای کاربر.pdf`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/combine_history_realtime.py` & `pytse_filter-1.33/examples/combine_history_realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/disappear_sell_queue.py` & `pytse_filter-1.33/examples/disappear_sell_queue.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/hot_money.py` & `pytse_filter-1.33/examples/hot_money.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/market_overview.py` & `pytse_filter-1.33/examples/market_overview.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/simple_history_filters.py` & `pytse_filter-1.33/examples/simple_history_filters.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/examples/simple_realtime_filters.py` & `pytse_filter-1.33/examples/simple_realtime_filters.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/license.md` & `pytse_filter-1.33/license.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/readme.md` & `pytse_filter-1.33/readme.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/setup.py` & `pytse_filter-1.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from os import path
 
-__version__ = 1.32
+__version__ = 1.33
 
 with open( ".\\readme.md", "r") as f:
     long_description = f.read()
 
 with open(".\\requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
```

### Comparing `pytse_filter-1.32/src/pytse_filter/calculate_client_data.py` & `pytse_filter-1.33/src/pytse_filter/calculate_client_data.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/calculate_indicators.py` & `pytse_filter-1.33/src/pytse_filter/calculate_indicators.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/client_setting.py` & `pytse_filter-1.33/src/pytse_filter/client_setting.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/config.py` & `pytse_filter-1.33/src/pytse_filter/config.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/download_history.py` & `pytse_filter-1.33/src/pytse_filter/download_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     if inscode is None :
         if symbol is None: return
         inscode =         symbol_to_inscode(symbol)
         if inscode is None : return
     try:
         datas = requests.get(config.ADJUSTED_PRICE_HISTORY.format(inscode), headers= config.HEADERS, timeout= 3).text.split(';')
-    except Exception as e:
-        return e
+    except:
+        return
     rows = []
     for data in datas:
         rows.append(data.split(','))
     if len(rows) == 0 : return
     columns = ['date',  'high', 'low', 'open', 'close', 'volume', 'adj_close']
     df = pd.DataFrame(rows, columns= columns)
     df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
```

### Comparing `pytse_filter-1.32/src/pytse_filter/download_realtime.py` & `pytse_filter-1.33/src/pytse_filter/download_realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/history.py` & `pytse_filter-1.33/src/pytse_filter/history.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/inds_setting.py` & `pytse_filter-1.33/src/pytse_filter/inds_setting.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/realtime.py` & `pytse_filter-1.33/src/pytse_filter/realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/syms.json` & `pytse_filter-1.33/src/pytse_filter/syms.json`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter/syms_manager.py` & `pytse_filter-1.33/src/pytse_filter/syms_manager.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.32/src/pytse_filter.egg-info/PKG-INFO` & `pytse_filter-1.33/src/pytse_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytse_filter
-Version: 1.32
+Version: 1.33
 Summary: A user-friendly project to filter symbols of Tehran Stock Exchange
 Home-page: https://github.com/farhad-mohammadi/pytse_filter
 Author: Farhad Mohammadi
 Author-email: farhad.mohammadi60@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytse_filter-1.32/src/pytse_filter.egg-info/SOURCES.txt` & `pytse_filter-1.33/src/pytse_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

