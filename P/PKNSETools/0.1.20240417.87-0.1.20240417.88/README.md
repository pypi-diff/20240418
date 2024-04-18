# Comparing `tmp/PKNSETools-0.1.20240417.87.tar.gz` & `tmp/PKNSETools-0.1.20240417.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240417.87.tar", last modified: Wed Apr 17 21:44:53 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240417.88.tar", last modified: Wed Apr 17 21:58:02 2024, max compression
```

## Comparing `PKNSETools-0.1.20240417.87.tar` & `PKNSETools-0.1.20240417.88.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.718425 PKNSETools-0.1.20240417.87/
--rw-rw-rw-   0        0        0     2661 2024-04-17 21:44:53.718425 PKNSETools-0.1.20240417.87/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.703401 PKNSETools-0.1.20240417.87/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.703401 PKNSETools-0.1.20240417.87/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.703401 PKNSETools-0.1.20240417.87/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3392 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12681 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-04-17 21:44:48.000000 PKNSETools-0.1.20240417.87/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.718425 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61965 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29930 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:44:53.703401 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-04-17 21:44:53.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-04-17 21:44:53.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:44:53.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 21:44:47.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-04-17 21:44:53.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 21:44:53.000000 PKNSETools-0.1.20240417.87/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/README.md
--rw-rw-rw-   0        0        0       86 2024-04-17 21:44:53.718425 PKNSETools-0.1.20240417.87/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-04-17 21:43:12.000000 PKNSETools-0.1.20240417.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/
+-rw-rw-rw-   0        0        0     2661 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.904470 PKNSETools-0.1.20240417.88/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3392 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    12681 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-04-17 21:57:57.000000 PKNSETools-0.1.20240417.88/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61965 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29930 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-04-17 21:58:02.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-04-17 21:58:02.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:58:02.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 21:57:56.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-04-17 21:58:02.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 21:58:02.000000 PKNSETools-0.1.20240417.88/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-04-17 21:56:17.000000 PKNSETools-0.1.20240417.88/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 21:58:02.920097 PKNSETools-0.1.20240417.88/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-04-17 21:56:18.000000 PKNSETools-0.1.20240417.88/setup.py
```

### Comparing `PKNSETools-0.1.20240417.87/PKG-INFO` & `PKNSETools-0.1.20240417.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240417.87
+Version: 0.1.20240417.88
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.87.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.88.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240417.88/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240417.88/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240417.88/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240417.88/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240417.88/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240417.88/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240417.88/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240417.87
+Version: 0.1.20240417.88
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.87.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.88.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240417.87/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240417.88/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/README.md` & `PKNSETools-0.1.20240417.88/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.87/setup.py` & `PKNSETools-0.1.20240417.88/setup.py`

 * *Files identical despite different names*

