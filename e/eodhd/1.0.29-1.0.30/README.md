# Comparing `tmp/eodhd-1.0.29.tar.gz` & `tmp/eodhd-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodhd-1.0.29.tar", last modified: Wed Mar 13 17:21:20 2024, max compression
+gzip compressed data, was "eodhd-1.0.30.tar", last modified: Thu Apr 18 06:35:48 2024, max compression
```

## Comparing `eodhd-1.0.29.tar` & `eodhd-1.0.30.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 17:21:20.498628 eodhd-1.0.29/
--rw-rw-rw-   0        0        0     1093 2023-04-09 14:12:05.000000 eodhd-1.0.29/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-09 14:12:05.000000 eodhd-1.0.29/MANIFEST.in
--rw-rw-rw-   0        0        0     1632 2024-03-13 17:21:20.497875 eodhd-1.0.29/PKG-INFO
--rw-rw-rw-   0        0        0      874 2023-09-20 05:58:29.000000 eodhd-1.0.29/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 17:21:20.383865 eodhd-1.0.29/eodhd/
-drwxrwxrwx   0        0        0        0 2024-03-13 17:21:20.493626 eodhd-1.0.29/eodhd/APIs/
--rw-rw-rw-   0        0        0     1873 2023-09-12 05:01:08.000000 eodhd-1.0.29/eodhd/APIs/BaseAPI.py
--rw-rw-rw-   0        0        0      465 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/BondsFundamentalsAPI.py
--rw-rw-rw-   0        0        0      815 2023-09-12 05:01:08.000000 eodhd-1.0.29/eodhd/APIs/BulkEodSplitsDividendsAPI.py
--rw-rw-rw-   0        0        0      382 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/EarningTrendsAPI.py
--rw-rw-rw-   0        0        0      999 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/EconomicEventsDataAPI.py
--rw-rw-rw-   0        0        0     1127 2023-09-27 12:28:06.000000 eodhd-1.0.29/eodhd/APIs/EodHistoricalStockMarketDataAPI.py
--rw-rw-rw-   0        0        0     3109 2023-12-10 15:36:45.000000 eodhd-1.0.29/eodhd/APIs/FinancialNewsAPI.py
--rw-rw-rw-   0        0        0      422 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/FundamentalDataAPI.py
--rw-rw-rw-   0        0        0      692 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/HistoricalDividendsAPI.py
--rw-rw-rw-   0        0        0      625 2023-12-10 15:30:38.000000 eodhd-1.0.29/eodhd/APIs/HistoricalMarketCapitalizationAPI.py
--rw-rw-rw-   0        0        0      685 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/HistoricalSplitsAPI.py
--rw-rw-rw-   0        0        0      775 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/InsiderTransactionsAPI.py
--rw-rw-rw-   0        0        0     1058 2023-09-27 12:18:12.000000 eodhd-1.0.29/eodhd/APIs/IntradayDataAPI.py
--rw-rw-rw-   0        0        0      623 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/ListOfExchangesAPI.py
--rw-rw-rw-   0        0        0      556 2023-09-12 05:01:08.000000 eodhd-1.0.29/eodhd/APIs/LiveStockPricesAPI.py
--rw-rw-rw-   0        0        0      488 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/MacroIndicatorsAPI.py
--rw-rw-rw-   0        0        0     1125 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/OptionsDataAPI.py
--rw-rw-rw-   0        0        0      815 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/StockMarketScreenerAPI.py
--rw-rw-rw-   0        0        0      982 2023-09-29 16:18:21.000000 eodhd-1.0.29/eodhd/APIs/StockMarketTickDataAPI.py
--rw-rw-rw-   0        0        0     3440 2023-10-29 13:00:32.000000 eodhd-1.0.29/eodhd/APIs/TechnicalIndicatorAPI.py
--rw-rw-rw-   0        0        0     1089 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/TradingHours_StockMarketHolidays_SymbolsChangeHistory.py
--rw-rw-rw-   0        0        0      631 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/UpcomingEarningsAPI.py
--rw-rw-rw-   0        0        0      525 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/UpcomingIPOsAPI.py
--rw-rw-rw-   0        0        0      531 2023-07-09 16:10:04.000000 eodhd-1.0.29/eodhd/APIs/UpcomingSplitsAPI.py
--rw-rw-rw-   0        0        0     1361 2023-12-10 15:41:09.000000 eodhd-1.0.29/eodhd/APIs/__init__.py
--rw-rw-rw-   0        0        0      279 2024-03-13 17:05:56.000000 eodhd-1.0.29/eodhd/__init__.py
--rw-rw-rw-   0        0        0    48515 2024-03-13 17:03:40.000000 eodhd-1.0.29/eodhd/apiclient.py
--rw-rw-rw-   0        0        0     4425 2023-04-07 08:56:14.000000 eodhd-1.0.29/eodhd/eodhdgraphs.py
--rw-rw-rw-   0        0        0    10040 2023-11-02 06:10:36.000000 eodhd-1.0.29/eodhd/websocketclient.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:21:20.496756 eodhd-1.0.29/eodhd.egg-info/
--rw-rw-rw-   0        0        0     1632 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-13 17:21:20.000000 eodhd-1.0.29/eodhd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 17:21:20.499172 eodhd-1.0.29/setup.cfg
--rw-rw-rw-   0        0        0     1608 2024-03-13 17:05:46.000000 eodhd-1.0.29/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:21:20.494626 eodhd-1.0.29/tests/
--rw-rw-rw-   0        0        0     1722 2023-04-09 14:12:05.000000 eodhd-1.0.29/tests/test_websocketclient.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:35:48.367028 eodhd-1.0.30/
+-rw-rw-rw-   0        0        0     1093 2023-04-09 14:12:05.000000 eodhd-1.0.30/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-09 14:12:05.000000 eodhd-1.0.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     1632 2024-04-18 06:35:48.365028 eodhd-1.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2023-09-20 05:58:29.000000 eodhd-1.0.30/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 06:35:48.298308 eodhd-1.0.30/eodhd/
+drwxrwxrwx   0        0        0        0 2024-04-18 06:35:48.361029 eodhd-1.0.30/eodhd/APIs/
+-rw-rw-rw-   0        0        0     1873 2023-09-12 05:01:08.000000 eodhd-1.0.30/eodhd/APIs/BaseAPI.py
+-rw-rw-rw-   0        0        0      465 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/BondsFundamentalsAPI.py
+-rw-rw-rw-   0        0        0      815 2023-09-12 05:01:08.000000 eodhd-1.0.30/eodhd/APIs/BulkEodSplitsDividendsAPI.py
+-rw-rw-rw-   0        0        0      382 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/EarningTrendsAPI.py
+-rw-rw-rw-   0        0        0      999 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/EconomicEventsDataAPI.py
+-rw-rw-rw-   0        0        0     1127 2023-09-27 12:28:06.000000 eodhd-1.0.30/eodhd/APIs/EodHistoricalStockMarketDataAPI.py
+-rw-rw-rw-   0        0        0     3109 2023-12-10 15:36:45.000000 eodhd-1.0.30/eodhd/APIs/FinancialNewsAPI.py
+-rw-rw-rw-   0        0        0      422 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/FundamentalDataAPI.py
+-rw-rw-rw-   0        0        0      692 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/HistoricalDividendsAPI.py
+-rw-rw-rw-   0        0        0      625 2023-12-10 15:30:38.000000 eodhd-1.0.30/eodhd/APIs/HistoricalMarketCapitalizationAPI.py
+-rw-rw-rw-   0        0        0      685 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/HistoricalSplitsAPI.py
+-rw-rw-rw-   0        0        0      775 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/InsiderTransactionsAPI.py
+-rw-rw-rw-   0        0        0     1058 2023-09-27 12:18:12.000000 eodhd-1.0.30/eodhd/APIs/IntradayDataAPI.py
+-rw-rw-rw-   0        0        0      623 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/ListOfExchangesAPI.py
+-rw-rw-rw-   0        0        0      556 2023-09-12 05:01:08.000000 eodhd-1.0.30/eodhd/APIs/LiveStockPricesAPI.py
+-rw-rw-rw-   0        0        0      488 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/MacroIndicatorsAPI.py
+-rw-rw-rw-   0        0        0     1125 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/OptionsDataAPI.py
+-rw-rw-rw-   0        0        0      815 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/StockMarketScreenerAPI.py
+-rw-rw-rw-   0        0        0      982 2023-09-29 16:18:21.000000 eodhd-1.0.30/eodhd/APIs/StockMarketTickDataAPI.py
+-rw-rw-rw-   0        0        0     3440 2023-10-29 13:00:32.000000 eodhd-1.0.30/eodhd/APIs/TechnicalIndicatorAPI.py
+-rw-rw-rw-   0        0        0     1089 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/TradingHours_StockMarketHolidays_SymbolsChangeHistory.py
+-rw-rw-rw-   0        0        0      631 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/UpcomingEarningsAPI.py
+-rw-rw-rw-   0        0        0      525 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/UpcomingIPOsAPI.py
+-rw-rw-rw-   0        0        0      531 2023-07-09 16:10:04.000000 eodhd-1.0.30/eodhd/APIs/UpcomingSplitsAPI.py
+-rw-rw-rw-   0        0        0     1361 2023-12-10 15:41:09.000000 eodhd-1.0.30/eodhd/APIs/__init__.py
+-rw-rw-rw-   0        0        0      279 2024-04-18 06:35:15.000000 eodhd-1.0.30/eodhd/__init__.py
+-rw-rw-rw-   0        0        0    48584 2024-04-18 06:29:23.000000 eodhd-1.0.30/eodhd/apiclient.py
+-rw-rw-rw-   0        0        0     4425 2023-04-07 08:56:14.000000 eodhd-1.0.30/eodhd/eodhdgraphs.py
+-rw-rw-rw-   0        0        0    10040 2023-11-02 06:10:36.000000 eodhd-1.0.30/eodhd/websocketclient.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:35:48.364789 eodhd-1.0.30/eodhd.egg-info/
+-rw-rw-rw-   0        0        0     1632 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 06:35:48.000000 eodhd-1.0.30/eodhd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:35:48.367028 eodhd-1.0.30/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2024-04-18 06:35:01.000000 eodhd-1.0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:35:48.363028 eodhd-1.0.30/tests/
+-rw-rw-rw-   0        0        0     1722 2023-04-09 14:12:05.000000 eodhd-1.0.30/tests/test_websocketclient.py
```

### Comparing `eodhd-1.0.29/LICENSE` & `eodhd-1.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/PKG-INFO` & `eodhd-1.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodhd
-Version: 1.0.29
+Version: 1.0.30
 Summary: Official EODHD API Python Library
 Home-page: https://whittle.medium.com
 Author: Michael Whittle
 Author-email: michael@lifecycle-ps.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eodhd-1.0.29/README.md` & `eodhd-1.0.30/README.md`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/BaseAPI.py` & `eodhd-1.0.30/eodhd/APIs/BaseAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/BulkEodSplitsDividendsAPI.py` & `eodhd-1.0.30/eodhd/APIs/BulkEodSplitsDividendsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/EconomicEventsDataAPI.py` & `eodhd-1.0.30/eodhd/APIs/EconomicEventsDataAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/EodHistoricalStockMarketDataAPI.py` & `eodhd-1.0.30/eodhd/APIs/EodHistoricalStockMarketDataAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/FinancialNewsAPI.py` & `eodhd-1.0.30/eodhd/APIs/FinancialNewsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/HistoricalDividendsAPI.py` & `eodhd-1.0.30/eodhd/APIs/HistoricalDividendsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/HistoricalMarketCapitalizationAPI.py` & `eodhd-1.0.30/eodhd/APIs/HistoricalMarketCapitalizationAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/HistoricalSplitsAPI.py` & `eodhd-1.0.30/eodhd/APIs/HistoricalSplitsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/InsiderTransactionsAPI.py` & `eodhd-1.0.30/eodhd/APIs/InsiderTransactionsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/IntradayDataAPI.py` & `eodhd-1.0.30/eodhd/APIs/IntradayDataAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/ListOfExchangesAPI.py` & `eodhd-1.0.30/eodhd/APIs/ListOfExchangesAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/LiveStockPricesAPI.py` & `eodhd-1.0.30/eodhd/APIs/LiveStockPricesAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/OptionsDataAPI.py` & `eodhd-1.0.30/eodhd/APIs/OptionsDataAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/StockMarketScreenerAPI.py` & `eodhd-1.0.30/eodhd/APIs/StockMarketScreenerAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/StockMarketTickDataAPI.py` & `eodhd-1.0.30/eodhd/APIs/StockMarketTickDataAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/TechnicalIndicatorAPI.py` & `eodhd-1.0.30/eodhd/APIs/TechnicalIndicatorAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/TradingHours_StockMarketHolidays_SymbolsChangeHistory.py` & `eodhd-1.0.30/eodhd/APIs/TradingHours_StockMarketHolidays_SymbolsChangeHistory.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/UpcomingEarningsAPI.py` & `eodhd-1.0.30/eodhd/APIs/UpcomingEarningsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/UpcomingIPOsAPI.py` & `eodhd-1.0.30/eodhd/APIs/UpcomingIPOsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/UpcomingSplitsAPI.py` & `eodhd-1.0.30/eodhd/APIs/UpcomingSplitsAPI.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/APIs/__init__.py` & `eodhd-1.0.30/eodhd/APIs/__init__.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/apiclient.py` & `eodhd-1.0.30/eodhd/apiclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,24 +326,25 @@
                     elif re_epoch.match(iso8601_end):
                         date_to = str(iso8601_end)
                     else:
                         date_to = str(int(datetime.today().timestamp()))
                 except ValueError:
                     self.console.log("invalid end date (yyyy-mm-ddThh-mm-ss OR yyyy-mm-dd OR nnnnnnnnnn):", iso8601_end)
                     sys.exit()
-
+            
+            LIMIT_FOR_1M = 120 # Limit for 1m interval
             if iso8601_start == "" or ((iso8601_start != "" and not re_iso8601.match(iso8601_start)) and (iso8601_start != "" and not re_date_only.match(iso8601_start))):
                 if interval == "d":
                     date_from = str(int((datetime.fromtimestamp(int(date_to)) - timedelta(days=(results - 1))).timestamp()))
                 elif interval == "w":
                     date_from = str(int((datetime.fromtimestamp(int(date_to)) - timedelta(weeks=((results - 1) - 1))).timestamp()))
                 elif interval == "m":
                     date_from = str(int((datetime.fromtimestamp(int(date_to)) - timedelta(months=(results - 1))).timestamp()))
                 else:
-                    date_from = str(int((datetime.fromtimestamp(int(date_to)) - timedelta(days=(results - 1))).timestamp()))
+                    date_from = str(int((datetime.fromtimestamp(int(date_to)) - timedelta(days=(LIMIT_FOR_1M))).timestamp()))
             else:
                 try:
                     if re_date_only.match(iso8601_start):
                         date_from = str(int(datetime.strptime(iso8601_start, "%Y-%m-%d").timestamp()))
                     elif re_iso8601.match(iso8601_start):
                         date_from = str(int(datetime.strptime(iso8601_start, "%Y-%m-%dT%H:%M:%S").timestamp()))
                     else:
```

### Comparing `eodhd-1.0.29/eodhd/eodhdgraphs.py` & `eodhd-1.0.30/eodhd/eodhdgraphs.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd/websocketclient.py` & `eodhd-1.0.30/eodhd/websocketclient.py`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/eodhd.egg-info/PKG-INFO` & `eodhd-1.0.30/eodhd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodhd
-Version: 1.0.29
+Version: 1.0.30
 Summary: Official EODHD API Python Library
 Home-page: https://whittle.medium.com
 Author: Michael Whittle
 Author-email: michael@lifecycle-ps.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eodhd-1.0.29/eodhd.egg-info/SOURCES.txt` & `eodhd-1.0.30/eodhd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eodhd-1.0.29/setup.py` & `eodhd-1.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="eodhd",
-    version="1.0.29",
+    version="1.0.30",
     description="Official EODHD API Python Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://whittle.medium.com",
     author="Michael Whittle",
     author_email="michael@lifecycle-ps.com",
     license="MIT",
```

### Comparing `eodhd-1.0.29/tests/test_websocketclient.py` & `eodhd-1.0.30/tests/test_websocketclient.py`

 * *Files identical despite different names*

