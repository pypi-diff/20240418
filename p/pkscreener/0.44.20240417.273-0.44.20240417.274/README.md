# Comparing `tmp/pkscreener-0.44.20240417.273.tar.gz` & `tmp/pkscreener-0.44.20240417.274.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240417.273.tar", last modified: Wed Apr 17 10:58:47 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240417.274.tar", last modified: Wed Apr 17 22:21:20 2024, max compression
```

## Comparing `pkscreener-0.44.20240417.273.tar` & `pkscreener-0.44.20240417.274.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:58:47.585523 pkscreener-0.44.20240417.273/
--rw-rw-rw-   0        0        0     1086 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-17 10:58:47.585523 pkscreener-0.44.20240417.273/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 10:58:47.569902 pkscreener-0.44.20240417.273/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:58:47.585523 pkscreener-0.44.20240417.273/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3237 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48912 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113854 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    78109 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-17 10:58:40.000000 pkscreener-0.44.20240417.273/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   115366 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19391 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:58:47.569902 pkscreener-0.44.20240417.273/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-17 10:58:47.000000 pkscreener-0.44.20240417.273/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-17 10:58:47.585523 pkscreener-0.44.20240417.273/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-17 10:55:56.000000 pkscreener-0.44.20240417.273/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:21:20.431897 pkscreener-0.44.20240417.274/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-17 22:21:20.431897 pkscreener-0.44.20240417.274/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 22:21:20.416270 pkscreener-0.44.20240417.274/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:21:20.431897 pkscreener-0.44.20240417.274/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24899 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3237 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    28153 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17537 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8118 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   111107 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46418 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79034 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-17 22:21:13.000000 pkscreener-0.44.20240417.274/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   117360 2024-04-17 22:17:33.000000 pkscreener-0.44.20240417.274/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-17 22:17:34.000000 pkscreener-0.44.20240417.274/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-17 22:17:34.000000 pkscreener-0.44.20240417.274/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19839 2024-04-17 22:17:34.000000 pkscreener-0.44.20240417.274/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:21:20.416270 pkscreener-0.44.20240417.274/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-17 22:21:20.000000 pkscreener-0.44.20240417.274/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 22:21:20.431897 pkscreener-0.44.20240417.274/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-17 22:17:34.000000 pkscreener-0.44.20240417.274/setup.py
```

### Comparing `pkscreener-0.44.20240417.273/LICENSE` & `pkscreener-0.44.20240417.274/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/LICENSE-Others` & `pkscreener-0.44.20240417.274/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/PKG-INFO` & `pkscreener-0.44.20240417.274/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240417.273
+Version: 0.44.20240417.274
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.273.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.274.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.273/README.md` & `pkscreener-0.44.20240417.274/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/__init__.py` & `pkscreener-0.44.20240417.274/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/ConfigManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import os
 import sys
 
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
+from PKDevTools.classes.OutputControls import OutputControls
 parser = configparser.ConfigParser(strict=False)
 
 # Default attributes for Downloading Cache from Git repo
 default_period = "450d"
 default_duration = "1d"
 default_timeout = 2
 
@@ -110,21 +111,21 @@
             rootDir = [rootDir]
         for dir in rootDir:
             for f in glob.glob(pattern, root_dir=dir, recursive=recursive):
                 if excludeFile is not None:
                     if not f.endswith(excludeFile):
                         try:
                             os.remove(f if os.sep in f else os.path.join(dir,f))
-                        except:
+                        except Exception as e:
                             self.default_logger.debug(e, exc_info=True)
                             pass
                 else:
                     try:
                         os.remove(f if os.sep in f else os.path.join(dir,f))
-                    except:
+                    except Exception as e:
                         self.default_logger.debug(e, exc_info=True)
                         pass
 
     # Handle user input and save config
 
     def setConfig(self, parser, default=False, showFileCreatedText=True):
         if default:
@@ -164,37 +165,37 @@
             parser.set("config", "minimumVolume", str(self.minVolume))
             parser.set("config", "backtestPeriodFactor", str(self.backtestPeriodFactor))
             try:
                 fp = open("pkscreener.ini", "w")
                 parser.write(fp)
                 fp.close()
                 if showFileCreatedText:
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.GREEN
                         + "[+] Default configuration generated as user configuration is not found!"
                         + colorText.END
                     )
                     input("Press <Enter> to continue...")
                     return
             except IOError as e:  # pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Failed to save user config. Exiting.."
                     + colorText.END
                 )
                 input("Press <Enter> to continue...")
                 sys.exit(1)
         else:
             parser = configparser.ConfigParser(strict=False)
             parser.add_section("config")
-            print("")
-            print(
+            OutputControls().printOutput("")
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] PKScreener User Configuration:"
                 + colorText.END
             )
             self.period = input(
                 "[+] Enter number of days for which stock data to be downloaded (Days)(Optimal = 450): "
@@ -312,36 +313,36 @@
             parser.set("config", "maxBacktestWindow", self.maxBacktestWindow)
             parser.set("config", "morninganalysiscandlenumber", self.morninganalysiscandlenumber)
             parser.set("config", "morninganalysiscandleduration", self.morninganalysiscandleduration + "m")
             parser.set("config", "minimumVolume", self.minVolume)
             parser.set("config", "backtestPeriodFactor", self.backtestPeriodFactor)
             # delete stock data due to config change
             self.deleteFileWithPattern()
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cached Stock Data Deleted."
                 + colorText.END
             )
 
             try:
                 fp = open("pkscreener.ini", "w")
                 parser.write(fp)
                 fp.close()
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + "[+] User configuration saved."
                     + colorText.END
                 )
                 input("Press <Enter> to continue...")
                 return
             except IOError as e:  # pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Failed to save user config. Exiting.."
                     + colorText.END
                 )
                 input("Press <Enter> to continue...")
                 sys.exit(1)
@@ -480,30 +481,30 @@
         return self.period == "1d"
 
     # Print config file
     def showConfigFile(self, defaultAnswer=None):
         try:
             prompt = "[+] PKScreener User Configuration:"
             f = open("pkscreener.ini", "r")
-            print(colorText.BOLD + colorText.GREEN + prompt + colorText.END)
+            OutputControls().printOutput(colorText.BOLD + colorText.GREEN + prompt + colorText.END)
             configData = f.read()
             f.close()
-            print("\n" + configData)
+            OutputControls().printOutput("\n" + configData)
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
             return f"{prompt}\n{configData}"
         except Exception as e:  # pragma: no cover
             self.default_logger.debug(e, exc_info=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] User Configuration not found!"
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Configure the limits to continue."
                 + colorText.END
             )
             self.setConfig(parser, default=True, showFileCreatedText=False)
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Fetcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.Fetcher import StockDataEmptyException
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from pkscreener.classes.PKTask import PKTask
-
+from PKDevTools.classes.OutputControls import OutputControls
 # This Class Handles Fetching of Stock Data over the internet
 
 
 class screenerStockDataFetcher(nseStockDataFetcher):
     _tickersInfoDict={}
     def fetchStockDataWithArgs(self, *args):
         task = None
@@ -108,15 +108,15 @@
                 timeout=self.configManager.generalTimeout/4,
                 start=start,
                 end=end
             )
         if printCounter:
             sys.stdout.write("\r\033[K")
             try:
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + (
                         "[%d%%] Screened %d, Found %d. Fetching data & Analyzing %s..."
                         % (
                             int((screenCounter.value / totalSymbols) * 100),
                             screenCounter.value,
@@ -130,25 +130,25 @@
             except ZeroDivisionError as e: # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 pass
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 pass
             if len(data) == 0:
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "=> Failed to fetch!"
                     + colorText.END,
                     end="\r",
                     flush=True,
                 )
                 raise StockDataEmptyException
                 return None
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Done!" + colorText.END,
                 end="\r",
                 flush=True,
             )
         return data
 
     # Get Daily Nifty 50 Index:
@@ -203,38 +203,38 @@
     def fetchWatchlist(self):
         createTemplate = False
         data = pd.DataFrame()
         try:
             data = pd.read_excel("watchlist.xlsx")
         except FileNotFoundError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + f"[+] watchlist.xlsx not found in {os.getcwd()}"
                 + colorText.END
             )
             createTemplate = True
         try:
             if not createTemplate:
                 data = data["Stock Code"].values.tolist()
         except KeyError as e: # pragma: no cover
             default_logger().debug(e, exc_info=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + '[+] Bad Watchlist Format: First Column (A1) should have Header named "Stock Code"'
                 + colorText.END
             )
             createTemplate = True
         if createTemplate:
             sample = {"Stock Code": ["SBIN", "INFY", "TATAMOTORS", "ITC"]}
             sample_data = pd.DataFrame(sample, columns=["Stock Code"])
             sample_data.to_excel("watchlist_template.xlsx", index=False, header=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.BLUE
                 + f"[+] watchlist_template.xlsx created in {os.getcwd()} as a referance template."
                 + colorText.END
             )
             return None
         return data
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/MenuOptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     SOFTWARE.
 
 """
 from enum import Enum
 
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
-
+from PKDevTools.classes.OutputControls import OutputControls
 import pkscreener.classes.ConfigManager as ConfigManager
 
 configManager = ConfigManager.tools()
 
 level0MenuDict = {
     "X": "Scanners",
     "S": "Strategies",
@@ -443,21 +443,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select a menu option:"
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
     Enter your choice > (default is """
                 + colorText.WARN
                 + self.find("X").keyTextLabel()
@@ -486,21 +486,21 @@
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select a Strategy for Screening:"
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
     Enter your choice > """
                 ""
             )
@@ -517,21 +517,21 @@
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList, coloredValues=["15"])
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an Index for Screening:"
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
     Enter your choice > (default is """
                 + colorText.WARN
                 + self.find(str(configManager.defaultIndex)).keyTextLabel()
@@ -551,21 +551,21 @@
             else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select a Criterion for Stock Screening: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -582,21 +582,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -613,21 +613,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -644,21 +644,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -675,21 +675,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -706,21 +706,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -738,21 +738,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
@@ -770,21 +770,21 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Select an option: "
                 + colorText.END
             )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + menuText
                 + """
 
         """
                 + colorText.END
             )
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKScanRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
+from PKDevTools.classes.OutputControls import OutputControls
 
 import pkscreener.classes.Fetcher as Fetcher
 import pkscreener.classes.ScreeningStatistics as ScreeningStatistics
 import pkscreener.classes.Utility as Utility
 
 class PKScanRunner:
     configManager = tools()
@@ -244,15 +245,15 @@
                     consumers,
                     screenResults,
                     saveResults,
                     backtest_df,
                     testing=testing,
                 )
 
-        print(colorText.END)
+        OutputControls().printOutput(colorText.END)
         PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,scr
 
     def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDict, items):
         tasks_queue, results_queue, totalConsumers = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
@@ -286,27 +287,27 @@
         else:
             if sys.platform.startswith("win"):
                 import signal
 
                 cleanup_on_signal(signal.SIGBREAK)
             else:
                 cleanup_on_sigterm()
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + f"[+] Using Period:{PKScanRunner.configManager.period} and Duration:{PKScanRunner.configManager.duration} for scan! You can change this in user config."
             + colorText.END
         )
         start_time = time.time()
         for worker in consumers:
             sys.stdout.write(f"{round(time.time() - start_time)}.")
             worker.daemon = True
             worker.start()
-        print(f"Started all workers in {time.time() - start_time}s")
-        sys.stdout.write("\x1b[1A")
+        OutputControls().printOutput(f"Started all workers in {time.time() - start_time}s")
+        # sys.stdout.write("\x1b[1A")
 
     def terminateAllWorkers(consumers, tasks_queue, testing):
         # Exit all processes. Without this, it threw error in next screening session
         for worker in consumers:
             try:
                 if testing: # pragma: no cover
                     if sys.platform.startswith("win"):
@@ -327,15 +328,15 @@
             try:
                 _ = tasks_queue.get(False)
             except Exception as e:  # pragma: no cover
                 # default_logger().debug(e, exc_info=True)
                 break
 
     def shutdown(frame, signum):
-        print("Shutting down for test coverage")
+        OutputControls().printOutput("Shutting down for test coverage")
 
     def runScan(testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df, *otherArgs,resultsReceivedCb=None):
         queueCounter = 0
         counter = 0
         shouldContinue = True
         lastNonNoneResult = None
         while numStocks:
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKScheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
 import warnings
 import os
+import sys
 import time
 warnings.simplefilter("ignore", UserWarning,append=True)
 os.environ["PYTHONWARNINGS"]="ignore::UserWarning"
 import multiprocessing
 from multiprocessing import Lock
 
 # from time import sleep
@@ -84,14 +85,15 @@
             futures = []  # keep track of the jobs
             with multiprocessing.Manager() as manager:
                 # this is the key - we share some state between our 
                 # main process and our worker functions
                 _progress = manager.dict()
                 _results = manager.dict()
                 console.control(Control(*((ControlType.CURSOR_UP,1),))) # Cursor up 1 lines f"\x1b[{param}A"
+                sys.stdout.write("\x1b[2K")  # delete the last line
                 overall_progress_task = progress.add_task(f"[green]{label if label is not None else 'Pending jobs progress:'}")
 
                 lock = Lock()
                 with ProcessPoolExecutor(max_workers=n_workers,
                                          initializer=init_pool_processes,
                                          initargs=(lock,)) as executor:
                     for task in tasksList:  # iterate over the jobs we need to run
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/PortfolioXRay.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from pkscreener.classes import Utility
 from PKDevTools.classes.log import default_logger
 from pkscreener.classes.ConfigManager import parser, tools
 from pkscreener.classes.Portfolio import Portfolio, PortfolioCollection
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.PKScheduler import PKScheduler
+from PKDevTools.classes.OutputControls import OutputControls
 
 configManager = tools()
 configManager.getConfig(parser)
 
 def summariseAllStrategies(testing=False):
     reports = getSavedBacktestReportNames(testing=testing)
     df_all = None
     counter = 0
     for report in reports:
         counter += 1
-        print(f"Processing {counter} of {len(reports)}...")
+        OutputControls().printOutput(f"Processing {counter} of {len(reports)}...")
         df = bestStrategiesFromSummaryForReport(
             f"PKScreener_{report}_Insights_DateSorted.html", summary=True,includeLargestDatasets=True
         )
         if df is not None:
             df.insert(loc=0, column="Scanner", value=report)
             if df_all is not None:
                 df_all = pd.concat([df_all, df], axis=0)
@@ -280,16 +281,16 @@
         #     days += 1
         #     if days >= len(periods):
         #         break
         df = getBacktestDataFromCleanedData(userArgs, saveResults, df, periods,progressLabel)
         if df is None:
             return None
         df = cleanFormattingForStatsData(calcForDate, saveResults, df)
-        # print(f"All portfolios:\n{PortfolioCollection().portfoliosAsDataframe}")
-        # print(f"All portfoliosSummary:\n{PortfolioCollection().ledgerSummaryAsDataframe}")
+        # OutputControls().printOutput(f"All portfolios:\n{PortfolioCollection().portfoliosAsDataframe}")
+        # OutputControls().printOutput(f"All portfoliosSummary:\n{PortfolioCollection().ledgerSummaryAsDataframe}")
     if task is not None:
         if task.taskId > 0:
             task.progressStatusDict[task.taskId] = {'progress': 0, 'total': 1}
             task.resultsDict[task.taskId] = df
         else:
             task.result = df
     return df
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/ScreeningStatistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 
 from sys import float_info as sflt
 import pkscreener.classes.Utility as Utility
 from pkscreener import Imports
 from pkscreener.classes.Pktalib import pktalib
+from PKDevTools.classes.OutputControls import OutputControls
 from PKNSETools.morningstartools import Stock
 
 if sys.version_info >= (3, 11):
     import advanced_ta as ata
 
 # from sklearn.preprocessing import StandardScaler
 if Imports["scipy"]:
@@ -1178,35 +1179,35 @@
                 + colorText.GREEN
                 + outText
                 + colorText.END
                 + colorText.BOLD
             )
             sug = "Stay Bullish!"
         if PKDateUtilities.isClosingHour():
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "Note: The AI prediction should be executed After 3 PM or Near to Closing time as the Prediction Accuracy is based on the Closing price!"
                 + colorText.END
             )
         predictionText = "Market may Open {} next day! {}".format(out, sug)
         strengthText = "Probability/Strength of Prediction = {}%".format(
             Utility.tools.getSigmoidConfidence(pred[0])
         )
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.BLUE
             + "\n"
             + "[+] Nifty AI Prediction -> "
             + colorText.END
             + colorText.BOLD
             + predictionText
             + colorText.END
         )
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.BLUE
             + "\n"
             + "[+] Nifty AI Prediction -> "
             + colorText.END
             + strengthText
         )
@@ -2249,19 +2250,14 @@
             data = data.replace([np.inf, -np.inf], 0)
             tops = data[data.tops > 0]
             # bots = data[data.bots > 0]
             highestTop = round(tops.describe()["High"]["max"], 1)
             filteredTops = tops[
                 tops.tops > (highestTop - (highestTop * percentageFromTop))
             ]
-            # print(tops)
-            # print(filteredTops)
-            # print(tops.sort_values(by=['tops'], ascending=False))
-            # print(tops.describe())
-            # print(f"Till {highestTop-(highestTop*percentageFromTop)}")
             if filteredTops.equals(tops):  # Tops are in the range
                 lowPoints = []
                 for i in range(len(tops) - 1):
                     endDate = tops.iloc[i]["Date"]
                     startDate = tops.iloc[i + 1]["Date"]
                     lowPoints.append(
                         data[
@@ -2375,56 +2371,7 @@
             except IndexError as e: # pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
                 pass
             return False
         except Exception as e:  # pragma: no cover
             self.default_logger.debug(e, exc_info=True)
             return False
-
-    """
-    # Find out trend for days to lookback
-    def validateVCP(df, screenDict, saveDict, daysToLookback=ConfigManager.daysToLookback, stockName=None):
-        // De-index date
-        data = df.copy()
-        data.reset_index(inplace=True)
-        data.rename(columns={'index':'Date'}, inplace=True)
-        data = data.head(daysToLookback)
-        data = data[::-1]
-        data = data.set_index(np.arange(len(data)))
-        data = data.fillna(0)
-        data = data.replace([np.inf, -np.inf], 0)
-        data['tops'] = data['Close'].iloc[list(pktalib.argrelextrema(np.array(data['Close']), np.greater_equal, order=3)[0])]
-        data['bots'] = data['Close'].iloc[list(pktalib.argrelextrema(np.array(data['Close']), np.less_equal, order=3)[0])]
-        try:
-            try:
-                top_slope,top_c = np.polyfit(data.index[data.tops > 0], data['tops'][data.tops > 0], 1)
-                bot_slope,bot_c = np.polyfit(data.index[data.bots > 0], data['bots'][data.bots > 0], 1)
-                topAngle = math.degrees(math.atan(top_slope))
-                vcpAngle = math.degrees(math.atan(bot_slope) - math.atan(top_slope))
-
-                # print(math.degrees(math.atan(top_slope)))
-                # print(math.degrees(math.atan(bot_slope)))
-                # print(vcpAngle)
-                # print(topAngle)
-                # print(data.max()['bots'])
-                # print(data.max()['tops'])
-                if (vcpAngle > 20 and vcpAngle < 70) and (topAngle > -10 and topAngle < 10) and (data['bots'].max() <= data['tops'].max()) and (len(data['bots'][data.bots > 0]) > 1):
-                    print("---> GOOD VCP %s at %sRs" % (stockName, top_c))
-                    import os
-                    os.system("echo %s >> vcp_plots\VCP.txt" % stockName)
-
-                    import matplotlib.pyplot as plt                
-                    plt.scatter(data.index[data.tops > 0], data['tops'][data.tops > 0], c='g')
-                    plt.scatter(data.index[data.bots > 0], data['bots'][data.bots > 0], c='r')
-                    plt.plot(data.index, data['Close'])
-                    plt.plot(data.index, top_slope*data.index+top_c,'g--')
-                    plt.plot(data.index, bot_slope*data.index+bot_c,'r--')
-                    if stockName != None:
-                        plt.title(stockName)
-                    # plt.show()
-                    plt.savefig('vcp_plots\%s.png' % stockName)
-                    plt.clf()
-            except np.RankWarning:
-                pass
-        except np.linalg.LinAlgError:
-            return False
-    """
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/StockScreener.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from PKDevTools.classes.Fetcher import StockDataEmptyException
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 
 import pkscreener.classes.ScreeningStatistics as ScreeningStatistics
 from pkscreener import Imports
 from pkscreener.classes.CandlePatterns import CandlePatterns
-
+from PKDevTools.classes.OutputControls import OutputControls
 
 class StockScreener:
     def __init__(self):
         self.isTradingTime = PKDateUtilities.isTradingTime()
         self.configManager = None
 
     # @tracelog
@@ -563,16 +563,16 @@
         except OSError as e: # pragma: no cover
             pass
         except Exception as e:  # pragma: no cover
             hostRef.default_logger.debug(e, exc_info=True)
             if testbuild or printCounter:
                 import traceback
                 traceback.print_exc()
-                print(e)
-                print(
+                OutputControls().printOutput(e)
+                OutputControls().printOutput(
                     colorText.FAIL
                     + (
                         "\n[+] Exception Occured while Screening %s! Skipping this stock.."
                         % stock
                     )
                     + colorText.END
                 )
@@ -784,15 +784,15 @@
             else:
                 period = configManager.period
         return volumeRatio,period
 
     def printProcessingCounter(self, totalSymbols, stock, printCounter, hostRef):
         if printCounter:
             try:
-                print(
+                OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.GREEN
                             + (
                                 "[%d%%] Screened %d, Found %d. Fetching data & Analyzing %s..."
                                 % (
                                     int(
                                         (hostRef.processingCounter.value / totalSymbols)
@@ -802,15 +802,15 @@
                                     hostRef.processingResultsCounter.value,
                                     stock,
                                 )
                             )
                             + colorText.END,
                             end="",
                         )
-                print(
+                OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.GREEN
                             + "=> Done!"
                             + colorText.END,
                             end="\r",
                             flush=True,
                         )
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/Utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 import pkscreener.classes.Fetcher as Fetcher
 from pkscreener.classes import VERSION, Changelog
 from pkscreener.classes.MenuOptions import menus
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.MarketStatus import MarketStatus
 from pkscreener.classes.PKScheduler import PKScheduler
+from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.Utils import random_user_agent
 
 configManager = ConfigManager.tools()
 configManager.getConfig(ConfigManager.parser)
 nseFetcher = nseStockDataFetcher()
 fetcher = Fetcher.screenerStockDataFetcher()
 
@@ -113,49 +114,51 @@
 lastScreened = os.path.join(
     Archiver.get_user_outputs_dir(), "last_screened_results.pkl"
 )
 
 # Class for managing misc and utility methods
 
 class tools:
-    def clearScreen(userArgs=None):
+    def clearScreen(userArgs=None,clearAlways=False):
         if "RUNNER" in os.environ.keys() or (userArgs is not None and userArgs.prodbuild):
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
         elif (userArgs is not None and userArgs.runintradayanalysis):
             return
-        if platform.system() == "Windows":
-            os.system("cls")
-        else:
-            os.system("clear")
+        if clearAlways:
+            if platform.system() == "Windows":
+                os.system("cls")
+            else:
+                os.system("clear")
         try:
-            art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
-            print(art.encode('utf-8').decode(STD_ENCODING))
+            if clearAlways:
+                art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
+                OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
 
     # Print about developers and repository
     def showDevInfo(defaultAnswer=None):
-        print("\n" + Changelog.changelog())
+        OutputControls().printOutput("\n" + Changelog.changelog())
         devInfo = "\n[+] Developer: PK (PKScreener)"
         versionInfo = "[+] Version: %s" % VERSION
         homePage = "[+] Home Page: https://github.com/pkjmesra/PKScreener\nTelegram Bot:@nse_pkscreener_bot\nChannel:https://t.me/PKScreener\nDiscussions:https://t.me/PKScreeners"
         issuesInfo = (
             "[+] Read/Post Issues here: https://github.com/pkjmesra/PKScreener/issues"
         )
         communityInfo = "[+] Join Community Discussions: https://github.com/pkjmesra/PKScreener/discussions"
         latestInfo = "[+] Download latest software from https://github.com/pkjmesra/PKScreener/releases/latest"
-        print(colorText.BOLD + colorText.WARN + devInfo + colorText.END)
-        print(colorText.BOLD + colorText.WARN + versionInfo + colorText.END)
-        print(colorText.BOLD + homePage + colorText.END)
-        print(colorText.BOLD + colorText.FAIL + issuesInfo + colorText.END)
-        print(colorText.BOLD + colorText.GREEN + communityInfo + colorText.END)
-        print(colorText.BOLD + colorText.BLUE + latestInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.WARN + devInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.WARN + versionInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + homePage + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.FAIL + issuesInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.GREEN + communityInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.BLUE + latestInfo + colorText.END)
         if defaultAnswer is None:
             input(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Press <Enter> to continue!"
                 + colorText.END
             )
@@ -208,38 +211,38 @@
             pass
 
     # Load last screened result to pickle file
     def getLastScreenedResults(defaultAnswer=None):
         try:
             df = pd.read_pickle(lastScreened)
             if df is not None and len(df) > 0:
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + "\n[+] Showing recently screened results..\n"
                     + colorText.END
                 )
                 df.sort_values(by=["Volume"], ascending=False, inplace=True)
-                print(
+                OutputControls().printOutput(
                     colorText.miniTabulator().tabulate(
                         df, headers="keys", tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=tools.getMaxColumnWidths(df)
                     ).encode("utf-8").decode(STD_ENCODING)
                 )
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
                     + "[+] Note: Trend calculation is based on number of recent days to screen as per your configuration."
                     + colorText.END
                 )
             else:
-                print("Nothing to show here!")
+                OutputControls().printOutput("Nothing to show here!")
         except FileNotFoundError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Failed to load recently screened result table from disk! Skipping.."
                 + colorText.END
             )
         if defaultAnswer is None:
             input(
@@ -713,15 +716,15 @@
         repoText = f"{repoText}\n{tools.wrapFitLegendText(table,backtestSummary,disclaimer)}"
         repoText = f"{repoText}\n[+] Understanding this report:\n\n"
         return repoText
 
     def set_github_output(name, value):
         if "GITHUB_OUTPUT" in os.environ.keys():
             with open(os.environ["GITHUB_OUTPUT"], "a") as fh:
-                print(f"{name}={value}", file=fh)
+                OutputControls().printOutput(f"{name}={value}", file=fh)
 
     def afterMarketStockDataExists(intraday=False, forceLoad=False):
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         cache_date = PKDateUtilities.previousTradingDate(PKDateUtilities.nextTradingDate(curr)) #curr  # for monday to friday
         weekday = curr.weekday()
         isTrading = PKDateUtilities.isTradingTime()
@@ -756,29 +759,29 @@
                 os.makedirs(os.path.dirname(f"{outputFolder}{os.sep}"), exist_ok=True)
             configManager.deleteFileWithPattern(rootDir=outputFolder)
         cache_file = os.path.join(outputFolder, fileName)
         if not os.path.exists(cache_file) or forceSave or (loadCount >= 0 and len(stockDict) > (loadCount + 1)):
             try:
                 with open(cache_file, "wb") as f:
                     pickle.dump(stockDict.copy(), f, protocol=pickle.HIGHEST_PROTOCOL)
-                    print(colorText.BOLD + colorText.GREEN + "=> Done." + colorText.END)
+                    OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "=> Done." + colorText.END)
                 if downloadOnly:
                     Committer.execOSCommand(f"git add {cache_file} -f >/dev/null 2>&1")
             except pickle.PicklingError as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "=> Error while Caching Stock Data."
                     + colorText.END
                 )
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Already Cached." + colorText.END
             )
 
     def downloadLatestData(stockDict,configManager,stockCodes=[],exchangeSuffix=".NS"):
         numStocksPerIteration = int(len(stockCodes)/5) + 1
         queueCounter = 0
         iterations = int(len(stockCodes)/numStocksPerIteration) + 1
@@ -835,15 +838,15 @@
         if exists and not forceRedownload:
             with open(
                 os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb"
             ) as f:
                 try:
                     stockData = pickle.load(f)
                     if not downloadOnly:
-                        print(
+                        OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.GREEN
                             + f"[+] Automatically Using Cached Stock Data {'due to After-Market hours' if not PKDateUtilities.isTradingTime() else ''}!"
                             + colorText.END
                         )
                     if stockData is not None and len(stockData) > 0:
                         multiIndex = stockData.keys()
@@ -886,47 +889,47 @@
                     #     stockDict = stockDict | stockData
                     # else:
                     #     stockDict = stockData
                         stockDataLoaded = True
                 except pickle.UnpicklingError as e:
                     default_logger().debug(e, exc_info=True)
                     f.close()
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.FAIL
                         + "[+] Error while Reading Stock Cache."
                         + colorText.END
                     )
                     if tools.promptFileExists(defaultAnswer=defaultAnswer) == "Y":
                         configManager.deleteFileWithPattern()
                 except EOFError as e:  # pragma: no cover
                     default_logger().debug(e, exc_info=True)
                     f.close()
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.FAIL
                         + "[+] Stock Cache Corrupted."
                         + colorText.END
                     )
                     if tools.promptFileExists(defaultAnswer=defaultAnswer) == "Y":
                         configManager.deleteFileWithPattern()
         if (
             not stockDataLoaded
             and ("1d" if isIntraday else ConfigManager.default_period)
             == configManager.period
             and ("1m" if isIntraday else ConfigManager.default_duration)
             == configManager.duration
         ) or forceRedownload:
-            print(
+            OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Market Stock Data is not cached, or forced to redownload .."
                     + colorText.END
                 )
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] Downloading cache from server for faster processing, Please Wait.."
                 + colorText.END
             )
             cache_url = (
                 "https://raw.githubusercontent.com/pkjmesra/PKScreener/actions-data-download/actions-data-download/"
@@ -1019,15 +1022,15 @@
                                     # Probably, the "stock" got removed from the latest download
                                     # and so, was not found in stockDict
                                     continue
                             stockDataLoaded = True
                     except Exception as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         f.close()
-                        print("[!] Download Error - " + str(e))
+                        OutputControls().printOutput("[!] Download Error - " + str(e))
                 else:
                     default_logger().debug(
                         f"Stock data cache file:{cache_file} on server has length ->{filesize}{chunksize}"
                     )
                 if not retrial and not stockDataLoaded:
                     # Don't try for more than once.
                     stockDict = tools.loadStockData(
@@ -1039,15 +1042,15 @@
                         forceLoad=forceLoad,
                         stockCodes=stockCodes,
                         exchangeSuffix=exchangeSuffix,
                         isIntraday = isIntraday,
                         forceRedownload=forceRedownload
                     )
         if not stockDataLoaded:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cache unavailable on pkscreener server, Continuing.."
                 + colorText.END
             )
         # See if we need to save stock data
         if stockDataLoaded:
@@ -1091,40 +1094,40 @@
             filePath = ""
             try:
                 filePath = os.path.join(Archiver.get_user_outputs_dir(), filename)
                 df.to_excel(filePath, engine="xlsxwriter")  # openpyxl throws an error exporting % sign.
                 isSaved = True
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
-                print(
+                OutputControls().printOutput(
                     colorText.FAIL
                     + (
                         "[+] Error saving file at %s"
                         % filePath
                     )
                     + colorText.END
                 )
                 try:
                     filePath = os.path.join(desktop, filename)
                     df.to_excel(filePath, engine="xlsxwriter")  # openpyxl throws an error exporting % sign.
                     isSaved = True
                 except Exception as ex:  # pragma: no cover
                     default_logger().debug(ex, exc_info=True)
-                    print(
+                    OutputControls().printOutput(
                         colorText.FAIL
                         + (
                             "[+] Error saving file at %s"
                             % filePath
                         )
                         + colorText.END
                     )
                     filePath = os.path.join(tempfile.gettempdir(), filename)
                     df.to_excel(filePath,engine="xlsxwriter")
                     isSaved = True
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + (colorText.GREEN if isSaved else colorText.FAIL)
                 + (("[+] Results saved to %s" % filePath) if isSaved else "[+] Failed saving results into Excel file!")
                 + colorText.END
             )
             return filePath
         return None
@@ -1284,15 +1287,15 @@
                                 + "\n[+] Enter MA Length (E.g. 50 or 200): "
                                 + colorText.END
                             )
                         )
                         return resp, maLength
                     except ValueError as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
-                        print(
+                        OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.FAIL
                             + "\n[!] Invalid Input! MA Length should be single integer value!\n"
                             + colorText.END
                         )
                         raise ValueError
                 elif resp == 6:
@@ -1304,15 +1307,15 @@
                                 + "\n[+] Enter NR timeframe [Integer Number] (E.g. 4, 7, etc.): "
                                 + colorText.END
                             )
                         )
                         return resp, maLength
                     except ValueError as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
-                        print(
+                        OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.FAIL
                             + "\n[!] Invalid Input! NR timeframe should be single integer value!\n"
                             + colorText.END
                         )
                         raise ValueError
                 elif resp in [7,10]:
@@ -1406,15 +1409,15 @@
                 download = False
         else:
             download = True
         if download:
             for file_url in urls:
                 resp = fetcher.fetchURL(file_url, stream=True)
                 if resp is not None and resp.status_code == 200:
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.GREEN
                         + "[+] Downloading AI model (v2) for Nifty predictions, Please Wait.."
                         + colorText.END
                     )
                     try:
                         chunksize = 1024 * 1024 * 1
@@ -1438,15 +1441,15 @@
                                 f.write(data)
                                 progressbar(dl / filesize)
                                 if dl >= filesize:
                                     progressbar(1.0)
                         f.close()
                     except Exception as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
-                        print("[!] Download Error - " + str(e))
+                        OutputControls().printOutput("[!] Download Error - " + str(e))
             time.sleep(3)
         try:
             if os.path.isfile(files[0]) and os.path.isfile(files[1]):
                 pkl = joblib.load(files[1])
                 model = keras.models.load_model(files[0]) if Imports["keras"] else None
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
@@ -1466,15 +1469,15 @@
             in_max = 0.5
         return round(
             ((x - in_min) * (out_max - out_min) / (in_max - in_min) + out_min), 3
         )
 
     def alertSound(beeps=3, delay=0.2):
         for i in range(beeps):
-            print("\a")
+            OutputControls().printOutput("\a")
             sleep(delay)
     
     def getMaxColumnWidths(df):
         columnWidths = [None]
         addnlColumnWidths = [40 if (x in ["Trend(22Prds)"] or "-Pd" in x) else (20 if (x in ["Pattern"]) else None) for x in df.columns]
         columnWidths.extend(addnlColumnWidths)
         columnWidths = columnWidths[:-1]
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/classes/keys.py` & `pkscreener-0.44.20240417.274/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/courbd.ttf` & `pkscreener-0.44.20240417.274/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/globals.py` & `pkscreener-0.44.20240417.274/pkscreener/globals.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 import pkscreener.classes.Fetcher as Fetcher
 import pkscreener.classes.ScreeningStatistics as ScreeningStatistics
 import pkscreener.classes.Utility as Utility
 from pkscreener.classes.Utility import STD_ENCODING
 from pkscreener.classes import VERSION, PortfolioXRay
 from pkscreener.classes.Backtest import backtest, backtestSummary
 from pkscreener.classes.PKSpreadsheets import PKSpreadsheets
-
+from PKDevTools.classes.OutputControls import OutputControls
 from pkscreener.classes.MenuOptions import (
     level0MenuDict,
     level1_X_MenuDict,
     level2_X_MenuDict,
     level3_X_ChartPattern_MenuDict,
     level3_X_PopularStocks_MenuDict,
     level3_X_Reversal_MenuDict,
@@ -155,15 +155,15 @@
     intraday = intradayConfig or argsIntraday
     exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday)
     if exists:
         shouldReplace = Utility.tools.promptFileExists(
             cache_file=cache_file, defaultAnswer=defaultAnswer
         )
         if shouldReplace == "N":
-            print(
+            OutputControls().printOutput(
                 cache_file
                 + colorText.END
                 + " already exists. Exiting as user chose not to replace it!"
             )
             sys.exit(0)
         else:
             pattern = f"{'intraday_' if intraday else ''}stock_data_*.pkl"
@@ -347,24 +347,24 @@
                     colorText.BOLD
                     + colorText.WARN
                     + "\n[+] The Volume should be lowest since last how many candles? "
                 )
             )
     except ValueError as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
-        print(colorText.END)
-        print(
+        OutputControls().printOutput(colorText.END)
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "[+] Error: Non-numeric value entered! Please try again!"
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return
-    print(colorText.END)
+    OutputControls().printOutput(colorText.END)
     return daysForLowestVolume
 
 
 def handleSecondaryMenuChoices(
     menuOption, testing=False, defaultAnswer=None, user=None
 ):
     if menuOption == "H":
@@ -395,15 +395,15 @@
     global selectedChoice
     Utility.tools.clearScreen()
 
     m0.renderForMenu(selectedMenu=None)
     try:
         if menuOption is None:
             menuOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ")
-            print(colorText.END, end="")
+            OutputControls().printOutput(colorText.END, end="")
         if menuOption == "" or menuOption is None:
             menuOption = "X"
         menuOption = menuOption.upper()
         selectedMenu = m0.find(menuOption)
         if selectedMenu is not None:
             if selectedMenu.menuKey == "Z":
                 input(
@@ -430,32 +430,32 @@
 
 def initPostLevel0Execution(
     menuOption=None, indexOption=None, executeOption=None, skip=[], retrial=False
 ):
     global newlyListedOnly, selectedChoice
     Utility.tools.clearScreen()
     if menuOption is None:
-        print('You must choose an option from the previous menu! Defaulting to "X"...')
+        OutputControls().printOutput('You must choose an option from the previous menu! Defaulting to "X"...')
         menuOption = "X"
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + level0MenuDict[menuOption].strip()
         + colorText.END
     )
     if indexOption is None:
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
         if indexOption is None:
             indexOption = input(
                 colorText.BOLD + colorText.FAIL + "[+] Select option: "
             )
-            print(colorText.END, end="")
+            OutputControls().printOutput(colorText.END, end="")
         if indexOption == "" or indexOption is None:
             indexOption = int(configManager.defaultIndex)
         # elif indexOption == 'W' or indexOption == 'w' or indexOption == 'N' or indexOption == 'n' or indexOption == 'E' or indexOption == 'e':
         elif not str(indexOption).isnumeric():
             indexOption = indexOption.upper()
             if indexOption in ["M", "E", "N", "Z"]:
                 return indexOption, 0
@@ -470,15 +470,15 @@
             from pkscreener.classes.MarketStatus import MarketStatus
             MarketStatus().exchange = "^IXIC"
         selectedChoice["1"] = str(indexOption)
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] Please enter a valid numeric option & Try Again!"
             + colorText.END
         )
         if not retrial:
             sleep(2)
@@ -488,15 +488,15 @@
 
 
 def initPostLevel1Execution(indexOption, executeOption=None, skip=[], retrial=False):
     global selectedChoice
     if executeOption is None:
         if indexOption is not None and indexOption != "W":
             Utility.tools.clearScreen()
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] You chose: "
                 + level0MenuDict[selectedChoice["0"]].strip()
                 + " > "
                 + level1_X_MenuDict[selectedChoice["1"]].strip()
                 + colorText.END
@@ -505,15 +505,15 @@
             m2.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
         if indexOption is not None and indexOption != "W":
             if executeOption is None:
                 executeOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
                 )
-                print(colorText.END, end="")
+                OutputControls().printOutput(colorText.END, end="")
             if executeOption == "":
                 executeOption = 1
             if not str(executeOption).isnumeric():
                 executeOption = executeOption.upper()
             else:
                 executeOption = int(executeOption)
                 if executeOption < 0 or executeOption > 44:
@@ -521,15 +521,15 @@
         else:
             executeOption = 0
         selectedChoice["2"] = str(executeOption)
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] Please enter a valid numeric option & Try Again!"
             + colorText.END
         )
         if not retrial:
             sleep(2)
@@ -682,22 +682,22 @@
             selectedMenu = m0.find(menuOption)
             m1.strategyNames = PortfolioXRay.strategyNames()
             m1.renderForMenu(selectedMenu=selectedMenu)
             try:
                 userOption = input(
                             colorText.BOLD + colorText.FAIL + "[+] Select option: "
                         )
-                print(colorText.END, end="")
+                OutputControls().printOutput(colorText.END, end="")
                 if userOption == "":
                     userOption = "37" # NoFilter
                 elif userOption == "38":
                     userOption = input(
                             colorText.BOLD + colorText.FAIL + "[+] Enter Exact Pattern name:"
                         )
-                    print(colorText.END, end="")
+                    OutputControls().printOutput(colorText.END, end="")
                     if userOption == "":
                         userOption = "37" # NoFilter
                     else:
                         strategyFilter.append(f"[P]{userOption}")
                         userOption = "38"
             except EOFError:  # pragma: no cover
                 userOption = "37"  # NoFilter
@@ -710,38 +710,38 @@
                 # Go back to the caller. It will show the console menu again.
                 return
         elif userOption == "Z":
             handleExitRequest(userOption)
             return
         
         if userOption == "S":
-            print(
+            OutputControls().printOutput(
                 colorText.GREEN
                 + "[+] Collecting all metrics for summarising..."
                 + colorText.END
             )
             # Enable showing/saving past strategy data
             savedValue = configManager.showPastStrategyData
             configManager.showPastStrategyData = True
             df_all = PortfolioXRay.summariseAllStrategies()
             if df_all is not None and len(df_all) > 0:
-                print(
+                OutputControls().printOutput(
                     colorText.miniTabulator().tabulate(
                         df_all,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         showindex=False,
                         maxcolwidths=Utility.tools.getMaxColumnWidths(df_all)
                     ).encode("utf-8").decode(STD_ENCODING)
                 )
                 showBacktestResults(
                     df_all, sortKey="Scanner", optionalName="InsightsSummary"
                 )
             else:
-                print("[!] Nothing to show here yet. Check back later.")
+                OutputControls().printOutput("[!] Nothing to show here yet. Check back later.")
             # reinstate whatever was the earlier saved value
             configManager.showPastStrategyData = savedValue
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
             return
         else:
             userOptions = userOption.split(",")
@@ -755,15 +755,15 @@
             indexOption=indexOption,
             executeOption=executeOption,
             defaultAnswer=defaultAnswer,
             user=user,
         )
 
     else:
-        print("Not implemented yet! Try selecting a different option.")
+        OutputControls().printOutput("Not implemented yet! Try selecting a different option.")
         sleep(3)
         return
 
     handleMenu_XBG(menuOption, indexOption, executeOption)
     if indexOption == "M" or executeOption == "M":
         # Go back to the caller. It will show the console menu again.
         return
@@ -786,15 +786,15 @@
             elif str(options[3]).upper() == "D":
                 # Use a default value
                 minRSI = 60
                 maxRSI = 75
         else:
             minRSI, maxRSI = Utility.tools.promptRSIValues()
         if not minRSI and not maxRSI:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for RSI! Values should be in range of 0 to 100. Please try again!"
                 + colorText.END
             )
             input("PRess <Enter> to continue...")
             return
@@ -895,15 +895,15 @@
                 maxRSI = int(options[4])
             if str(options[3]).upper() == "D":
                 minRSI = -150
                 maxRSI = 250
         else:
             minRSI, maxRSI = Utility.tools.promptCCIValues()
         if not minRSI and not maxRSI:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for CCI! Values should be in range of -300 to 500. Please try again!"
                 + colorText.END
             )
             input("Press <Enter> to continue...")
             return
@@ -912,15 +912,15 @@
             if str(options[3]).isnumeric():
                 volumeRatio = float(options[3])
             elif str(options[3]).upper() == "D":
                 volumeRatio = configManager.volumeRatio
         else:
             volumeRatio = Utility.tools.promptVolumeMultiplier()
         if volumeRatio <= 0:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Error: Invalid values for Volume Ratio! Value should be a positive number. Please try again!"
                 + colorText.END
             )
             input("Press <Enter> to continue...")
             return
@@ -1002,15 +1002,15 @@
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
         return
     if executeOption >= 27 and executeOption <= 41:
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] Error: Option 25 to 41 Not implemented yet! Press <Enter> to continue."
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return
@@ -1067,21 +1067,21 @@
                 sys.exit(0)
             elif indexOption == "E":
                 return handleMonitorFiveEMA()
             else:
                 if str(menuOption).upper() == "C":
                     stockDict,endOfdayCandles = PKMarketOpenCloseAnalyser.getStockDataForSimulation()
                     if stockDict is None or endOfdayCandles is None:
-                        print(f"Cannot proceed! Stock data is unavailable. Please check the error logs/messages !")
+                        OutputControls().printOutput(f"Cannot proceed! Stock data is unavailable. Please check the error logs/messages !")
                         return
                     listStockCodes = sorted(list(filter(None,list(set(stockDict.keys())))))
                 listStockCodes = prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption)
         except urllib.error.URLError as e:
             default_logger().debug(e, exc_info=True)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n\n[+] Oops! It looks like you don't have an Internet connectivity at the moment!"
                 + colorText.END
             )
             input("Exiting now...")
             sys.exit(0)
@@ -1108,49 +1108,49 @@
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
             loadedStockData = True
         loadCount = len(stockDict) if stockDict is not None else 0
 
         if downloadOnly:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Starting download.. Press Ctrl+C to stop!"
             )
         if menuOption.upper() in ["B", "G"]:
-            print(
+            OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
                     + f"[+] A total of {configManager.backtestPeriod} trading periods' historical data will be considered for backtesting. You can change this in User Config."
                 )
         samplingDuration, fillerPlaceHolder, actualHistoricalDuration = PKScanRunner.getScanDurationParameters(testing, menuOption)
         totalStocksInReview = 0
         savedStocksCount = 0
         downloadedRecently = False
         items = []
         backtest_df = None
         bar, spinner = Utility.tools.getProgressbarStyle()
         # Lets begin from y days ago, evaluate from that date if the selected strategy had yielded any result
         # and then keep coming to the next day (x-1) until we get to today (actualHistoricalDuration = 0)
-        print(f"{colorText.GREEN}[+] Adding stocks to the queue...{colorText.END}")
+        OutputControls().printOutput(f"{colorText.GREEN}[+] Adding stocks to the queue...{colorText.END}")
         with alive_bar(actualHistoricalDuration, bar=bar, spinner=spinner) as progressbar:
             while actualHistoricalDuration >= 0:
                 daysInPast = PKScanRunner.getBacktestDaysForScan(userPassedArgs, backtestPeriod, menuOption, actualHistoricalDuration)
                 try:
                     listStockCodes, savedStocksCount, pastDate = PKScanRunner.getStocksListForScan(userPassedArgs, menuOption, totalStocksInReview, downloadedRecently, daysInPast) if menuOption not in ["C"] else (listStockCodes, 0, "")
                 except KeyboardInterrupt:
                     try:
                         keyboardInterruptEvent.set()
                         keyboardInterruptEventFired = True
                         actualHistoricalDuration = -1
                         break
                     except KeyboardInterrupt:
                         pass
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.FAIL
                         + "\n[+] Terminating Script, Please wait..."
                         + colorText.END
                     )
                 except Exception:
                     pass
@@ -1163,15 +1163,15 @@
                         + f"Total Stocks: {len(items)}. Added {savedStocksCount} to Stocks from {pastDate} saved from earlier..."
                         + colorText.END
                     )
                 fillerPlaceHolder = fillerPlaceHolder + 1
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
-        sys.stdout.write(f"\x1b[1A")
+        sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
             screenResults, saveResults, backtest_df, scr = PKScanRunner.runScanWithParams(keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners)
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDict,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
             if downloadOnly and menuOption in ["X"]:
                 scr.getFreshMFIStatus(stock="LatestCheckedOnDate")
@@ -1203,27 +1203,27 @@
                     #     except:
                     #         saveResults.loc[ticker, 'MCapWt%'] = 0
                     #         pass
                     #     numShares.append(saveResults.loc[ticker, 'MCapWt%'])
                     # screenResults["MCapWt%"] = numShares
                 if not newlyListedOnly and not configManager.showunknowntrends and screenResults is not None and len(screenResults) > 0:
                     screenResults, saveResults = removeUnknowns(screenResults, saveResults)
-                    print(colorText.FAIL + f"[+] Configuration to remove unknown cell values resulted into removing all rows!" + colorText.END)
+                    OutputControls().printOutput(colorText.FAIL + f"[+] Configuration to remove unknown cell values resulted into removing all rows!" + colorText.END)
                 if len(strategyFilter) > 0 and saveResults is not None and len(saveResults) > 0:
                     # We'd need to apply additional filters for selected strategy
                     df_screenResults = None
                     cleanedUpSaveResults = PortfolioXRay.cleanupData(saveResults)
                     for strFilter in strategyFilter:
                         cleanedUpSaveResults = PortfolioXRay.strategyForKey(strFilter)(cleanedUpSaveResults)
                         saveResults = saveResults[saveResults.index.isin(cleanedUpSaveResults.index.values)]
                     for stk in saveResults.index.values:
                         df_screenResults_filter = screenResults[screenResults.index.astype(str).str.contains(f"NSE%3A{stk}") == True]
                         df_screenResults = pd.concat([df_screenResults, df_screenResults_filter], axis=0)
                     if df_screenResults is None or len(df_screenResults) == 0:
-                        print(colorText.FAIL + f"[+] Of the {len(screenResults) if screenResults is not None else 0} stocks, no results matching the selected strategies!" + colorText.END)
+                        OutputControls().printOutput(colorText.FAIL + f"[+] Of the {len(screenResults) if screenResults is not None else 0} stocks, no results matching the selected strategies!" + colorText.END)
                     screenResults = df_screenResults
                 if executeOption == 26:
                     removedUnusedColumns(screenResults, saveResults, ["Date"],userArgs=userPassedArgs)
                     screen_copy = screenResults.copy()
                     screen_copy.reset_index(inplace=True)
                     dividend_df = pd.merge(screen_copy, dividend_df, on='Stock')
                     bonus_df = pd.merge(screen_copy, bonus_df, on='Stock')
@@ -1243,15 +1243,15 @@
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 # showindex = False,
                                 maxcolwidths=Utility.tools.getMaxColumnWidths(dividend_df)
                             ).encode("utf-8").decode(STD_ENCODING)
                             shouldSend = True
                         shareable_strings.append(tab_results)
-                        print(tab_results)
+                        OutputControls().printOutput(tab_results)
                     if shouldSend:
                         sendQuickScanResult(
                             menuChoiceHierarchy,
                             user,
                             shareable_strings[0],
                             Utility.tools.removeAllColorStyles(shareable_strings[0]),
                             "NSE Stocks with dividends/bonus/splits soon",
@@ -1292,35 +1292,35 @@
             df_xray = prepareGroupedXRay(backtestPeriod, backtest_df)
             summary_df, sorting, sortKeys = FinishBacktestDataCleanup(backtest_df, df_xray)
             while sorting:
                 sorting = showSortedBacktestData(backtest_df, summary_df, sortKeys)
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
         elif menuOption == "B":
-            print("Finished backtesting with no results to show!")
+            OutputControls().printOutput("Finished backtesting with no results to show!")
         elif menuOption == "G":
             if defaultAnswer is None:
                 input("Press <Enter> to continue...")
     newlyListedOnly = False
     # Change the config back to usual
     resetConfigToDefault()
     try:
         creds = None
         # Write into sheet only if it's the reglar scan alert trigger in the morning and evening
         if 'ALERT_TRIGGER' in os.environ.keys() and os.environ["ALERT_TRIGGER"] == 'Y':
             if "GSHEET_SERVICE_ACCOUNT_DEV" in os.environ.keys() and (userPassedArgs.backtestdaysago is None):# or userPassedArgs.log:
                 begin = time.time()
                 creds = os.environ.get("GSHEET_SERVICE_ACCOUNT_DEV")
-                print(f"{colorText.GREEN}[+] Saving data to Google Spreadsheets now...{colorText.END}")
+                OutputControls().printOutput(f"{colorText.GREEN}[+] Saving data to Google Spreadsheets now...{colorText.END}")
                 gClient = PKSpreadsheets(credentialDictStr=creds)
                 runOption = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 df = saveResults.copy()
                 df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDict)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
-                print(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
+                OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
     if userPassedArgs.runintradayanalysis:
         analysis_df = screenResults.copy()
         analysis_df.reset_index(inplace=True)
         if 'index' in analysis_df.columns:
             analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
@@ -1427,39 +1427,39 @@
     df_xray.loc[:, "Date"] = df_xray.loc[:, "Date"].apply(
                 lambda x: x.replace("-", "/")
             )
     
     return df_xray
 
 def showSortedBacktestData(backtest_df, summary_df, sortKeys):
-    print(
+    OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Would you like to sort the results?"
                     + colorText.END
                 )
-    print(
+    OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + "[+] Press :\n [+] s, v, t, m : sort by Stocks, Volume, Trend, MA-Signal\n [+] d : sort by date\n [+] 1,2,3...30 : sort by period\n [+] n : Exit sorting\n"
                     + colorText.END
                 )
     if defaultAnswer is None:
         choice = input(
                         colorText.BOLD + colorText.FAIL + "[+] Select option:"
                     )
-        print(colorText.END, end="")
+        OutputControls().printOutput(colorText.END, end="")
         if choice.upper() in sortKeys.keys():
             Utility.tools.clearScreen()
             showBacktestResults(backtest_df, sortKeys[choice.upper()])
             showBacktestResults(summary_df, optionalName="Summary")
         else:
             sorting = False
     else:
-        print("Finished backtesting!")
+        OutputControls().printOutput("Finished backtesting!")
         sorting = False
     return sorting
 
 def resetConfigToDefault():
     isIntraday = userPassedArgs.intraday is not None
     if configManager.isIntradayConfig() or isIntraday:
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
@@ -1469,32 +1469,32 @@
         updateMenuChoiceHierarchy()
     if listStockCodes is None or len(listStockCodes) == 0:
         if indexOption >= 0 and indexOption <= 14:
             listStockCodes = fetcher.fetchStockCodes(
                             indexOption, stockCode=None
                         )
         elif indexOption == 15:
-            print(colorText.BOLD + "[+] Getting Stock Codes From NASDAQ... ", end="")
+            OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NASDAQ... ", end="")
             nasdaq = PKNasdaqIndexFetcher(configManager)
             listStockCodes = nasdaq.fetchNasdaqIndexConstituents()
             if len(listStockCodes) > 10:
-                print(
+                OutputControls().printOutput(
                     colorText.GREEN
                     + ("=> Done! Fetched %d stock codes." % len(listStockCodes))
                     + colorText.END
                 )
                 if configManager.shuffleEnabled:
                     random.shuffle(listStockCodes)
-                    print(
+                    OutputControls().printOutput(
                         colorText.BLUE
                         + "[+] Stock shuffling is active."
                         + colorText.END
                     )
             else:
-                print(
+                OutputControls().printOutput(
                     colorText.FAIL
                     + ("=> Failed! Could not fetch stock codes from NASDAQ!")
                     + colorText.END
                 )
         if (listStockCodes is None or len(listStockCodes) == 0) and testing:
             listStockCodes = [TEST_STKCODE if indexOption < 15 else "AMD"]
     if indexOption == 0:
@@ -1522,45 +1522,45 @@
                 result_df = screener.monitorFiveEma(
                                 fetcher=fetcher,
                                 result_df=result_df,
                                 last_signal=last_signal,
                             )
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
-                print(
+                OutputControls().printOutput(
                                 colorText.BOLD
                                 + colorText.FAIL
                                 + "[+] There was an exception while monitoring 5-EMA"
                                 + "\n[+] If this continues to happen, please try and run with -l"
                                 + "\n[+] and collect all the logs, zip it and submit it to the developer."
                                 + "\n[+] For example:"
                                 + colorText.END
                                 + colorText.WARN
                                 + "pkscreener -l\n"
                                 + colorText.END
                             )
-            print(
+            OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.WARN
                             + "[+] 5-EMA : Live Intraday Scanner \t"
                             + colorText.END
                             + colorText.FAIL
                             + f'Last Scanned: {datetime.now().strftime("%H:%M:%S")}\n'
                             + colorText.END
                         )
             if result_df is not None and len(result_df) > 0:
-                print(
+                OutputControls().printOutput(
                                 colorText.miniTabulator().tabulate(
                                     result_df,
                                     headers="keys",
                                     tablefmt=colorText.No_Pad_GridFormat,
                                     maxcolwidths=Utility.tools.getMaxColumnWidths(result_df)
                                 ).encode("utf-8").decode(STD_ENCODING)
                             )
-            print("\nPress Ctrl+C to exit.")
+            OutputControls().printOutput("\nPress Ctrl+C to exit.")
             if result_df is not None and len(result_df) != last_result_len and not first_scan:
                 Utility.tools.alertSound(beeps=5)
             sleep(60)
             first_scan = False
     except KeyboardInterrupt:
         input("\nPress <Enter> to Continue...\n")
         return
@@ -1623,20 +1623,21 @@
             + f'>{level4_X_ChartPattern_BBands_SQZ_MenuDict[selectedChoice["4"]].strip()}'
         )
     elif selectedChoice["2"] == "21":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
         )
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
         + colorText.END
+        , enableMultipleLineOutput=True
     )
     default_logger().info(menuChoiceHierarchy)
 
 def printNotifySaveScreenedResults(
     screenResults, saveResults, selectedChoice, menuChoiceHierarchy, testing, user=None
 ):
     global userPassedArgs, elapsed_time
@@ -1651,19 +1652,20 @@
         screenResults = screenResults[~screenResults.index.duplicated(keep='first')]
         saveResults = saveResults[~saveResults.index.duplicated(keep='first')]
         if "Stock" in screenResults.columns:
             screenResults.drop_duplicates(keep="first", inplace=True)
         if "Stock" in saveResults.columns:
             saveResults.drop_duplicates(keep="first", inplace=True)
 
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + f"[+] You chose: {menuChoiceHierarchy}"
         + colorText.END
+        , enableMultipleLineOutput=True
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
     pngExtension = ".png"
     eligible = is_token_telegram_configured()
     targetDateG10k = prepareGrowthOf10kResults(saveResults, selectedChoice, menuChoiceHierarchy, testing, user, pngName, pngExtension, eligible)
     if saveResults is not None and "Date" in saveResults.columns and len(saveResults) > 0:
         recordDate = saveResults["Date"].iloc[0].replace("/","-")
@@ -1671,15 +1673,15 @@
 
     tabulated_results = ""
     if screenResults is not None and len(screenResults) > 0:
         tabulated_results = colorText.miniTabulator().tabulate(
             screenResults, headers="keys", tablefmt=colorText.No_Pad_GridFormat,
             maxcolwidths=Utility.tools.getMaxColumnWidths(screenResults)
         ).encode("utf-8").decode(STD_ENCODING)
-    print(tabulated_results)
+    OutputControls().printOutput(f"{tabulated_results}\n", enableMultipleLineOutput=True)
     _, reportNameInsights = getBacktestReportFilename(
         sortKey="Date", optionalName="Insights"
     )
     strategy_df = PortfolioXRay.bestStrategiesFromSummaryForReport(reportNameInsights,includeLargestDatasets=True)
     addendumLabel = (
         "[+] Strategies that have best results in the past for this scan option (calculated with 1 stock each with matching strategy in the result):"
     )
@@ -1688,16 +1690,16 @@
         tabulated_strategy = colorText.miniTabulator().tabulate(
             strategy_df,
             headers="keys",
             tablefmt=colorText.No_Pad_GridFormat,
             showindex=False,
             maxcolwidths=Utility.tools.getMaxColumnWidths(strategy_df)
         ).encode("utf-8").decode(STD_ENCODING)
-        print(addendumLabel)
-        print(tabulated_strategy)
+        OutputControls().printOutput(addendumLabel)
+        OutputControls().printOutput(tabulated_strategy)
     if screenResults is not None and len(screenResults) >= 1:
         choiceSegments = menuChoiceHierarchy.split(">")
         choiceSegments = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
         title = f'<b>{choiceSegments}</b>{"" if selectedChoice["0"] != "G" else " for Date:"+ targetDateG10k}'
         if (
             ("RUNNER" in os.environ.keys() and os.environ["RUNNER"] != "LOCAL_RUN_SCANNER")
             or "PKDevTools_Default_Log_Level" in os.environ.keys()
@@ -1794,23 +1796,23 @@
                                 caption=caption,
                                 user=user,
                             )
                             os.remove(pngName + backtestExtension)
                         except Exception as e:  # pragma: no cover
                             default_logger().debug(e, exc_info=True)
                             pass
-                            # print(e)
+                            # OutputControls().printOutput(e)
                             # traceback.print_exc()
                     else:
                         tabulateBacktestResults(saveResults)
             else:
                 tabulateBacktestResults(saveResults)
         else:
             tabulateBacktestResults(saveResults)
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + f"[+] Found {len(screenResults) if screenResults is not None else 0} Stocks in {str('{:.2f}'.format(elapsed_time))} sec.{(' with portfolio returns:' + summaryReturns) if len(summaryReturns) > 0 else ''}"
                 + colorText.END
             )
     elif user is not None:
         sendMessageToTelegramChannel(
@@ -1835,16 +1837,16 @@
                     headers="keys",
                     tablefmt=colorText.No_Pad_GridFormat,
                     showindex=False,
                     maxcolwidths=Utility.tools.getMaxColumnWidths(df)
                 ).encode("utf-8").decode(STD_ENCODING)
                 # Show only if the configuration dicttates showing strategy data
                 if configManager.showPastStrategyData:
-                    print(f"\n\n{titleLabelG10k}\n")
-                    print(g10kStyledTable)
+                    OutputControls().printOutput(f"\n\n{titleLabelG10k}\n")
+                    OutputControls().printOutput(g10kStyledTable)
                 g10kUnStyledTable = Utility.tools.removeAllColorStyles(g10kStyledTable)
                 if not testing and eligible:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         g10kStyledTable,
                         g10kUnStyledTable,
@@ -1917,29 +1919,29 @@
             detaildf,
             headers="keys",
             tablefmt=colorText.No_Pad_GridFormat,
             showindex=False,
             maxcolwidths=Utility.tools.getMaxColumnWidths(detaildf)
         ).encode("utf-8").decode(STD_ENCODING)
     if tabulated_backtest_summary != "":
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] For chosen scan, summary of correctness from past: [Example, 70% of (100) under 1-Pd, means out of 100 stocks that were in the scan result in the past, 70% of them gained next day.)"
             + colorText.END
         )
-        print(tabulated_backtest_summary)
+        OutputControls().printOutput(tabulated_backtest_summary)
     if tabulated_backtest_detail != "":
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "\n[+] 1 to 30 period gain/loss % on respective date for matching stocks from earlier predictions:[Example, 5% under 1-Pd, means the stock price actually gained 5% the next day from given date.]"
             + colorText.END
         )
-        print(tabulated_backtest_detail)
+        OutputControls().printOutput(tabulated_backtest_detail)
     return tabulated_backtest_summary, tabulated_backtest_detail
 
 
 def sendQuickScanResult(
     menuChoiceHierarchy,
     user,
     tabulated_results,
@@ -2048,22 +2050,22 @@
     result = None
     backtest_df = None
     reviewDate = getReviewDate(userPassedArgs)
     max_allowed = getMaxAllowedResultsCount(iterations, testing)
     try:
         originalNumberOfStocks = numStocks
         iterations, numStocksPerIteration = getIterationsAndStockCounts(numStocks, iterations)
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.GREEN
             + f"[+] For {reviewDate}, total Stocks under review: {numStocks} over {iterations} iterations..."
             + colorText.END
         )
         if not userPassedArgs.download:
-            print(colorText.WARN
+            OutputControls().printOutput(colorText.WARN
                 + f"[+] Starting {'Stock' if menuOption not in ['C'] else 'Intraday'} {'Screening' if menuOption=='X' else ('Analysis' if menuOption == 'C' else 'Backtesting.')}. Press Ctrl+C to stop!"
                 + colorText.END
             )
         bar, spinner = Utility.tools.getProgressbarStyle()
         with alive_bar(numStocks, bar=bar, spinner=spinner) as progressbar:
             lstscreen = []
             lstsave = []
@@ -2085,39 +2087,39 @@
                 )
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
-        print(f"\x1b[3A")
+        OutputControls().printOutput(f"\x1b[1A")
         elapsed_time = time.time() - start_time
         if menuOption in ["X", "G", "C"]:
             # create extension
             screenResults = pd.DataFrame(lstscreen)
             saveResults = pd.DataFrame(lstsave)
 
     except KeyboardInterrupt:
         try:
             global keyboardInterruptEventFired
             keyboardInterruptEvent.set()
             keyboardInterruptEventFired = True
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Terminating Script, Please wait..."
                 + colorText.END
             )
             PKScanRunner.terminateAllWorkers(consumers=consumers, tasks_queue=tasks_queue,testing=testing)
             logging.shutdown()
         except KeyboardInterrupt:
             pass
     except Exception as e:
         default_logger().debug(e, exc_info=True)
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + f"\nException:\n{e}\n[+] Terminating Script, Please wait..."
             + colorText.END
         )
         PKScanRunner.terminateAllWorkers(consumers=consumers, tasks_queue=tasks_queue,testing=testing)
         logging.shutdown()
@@ -2204,26 +2206,26 @@
     global userPassedArgs, keyboardInterruptEventFired
     argsIntraday = userPassedArgs is not None and userPassedArgs.intraday is not None
     intradayConfig = configManager.isIntradayConfig()
     intraday = intradayConfig or argsIntraday
     if not keyboardInterruptEventFired and (downloadOnly or (
         configManager.cacheEnabled and not PKDateUtilities.isTradingTime() and not testing
     )):
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.GREEN
             + "[+] Caching Stock Data for future use, Please Wait... "
             + colorText.END,
             end="",
         )
         Utility.tools.saveStockData(stockDict, configManager, loadCount, intraday)
         if downloadOnly:
             Utility.tools.saveStockData(stockDict, configManager, loadCount, intraday, downloadOnly=downloadOnly)
     else:
-        print(colorText.BOLD + colorText.GREEN + "[+] Skipped Saving!" + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "[+] Skipped Saving!" + colorText.END)
 
 
 def saveNotifyResultsFile(
     screenResults, saveResults, defaultAnswer, menuChoiceHierarchy, user=None
 ):
     global userPassedArgs, elapsed_time
     if user is None and userPassedArgs.user is not None:
@@ -2233,30 +2235,31 @@
         filename = Utility.tools.promptSaveResults(
             saveResults, defaultAnswer=defaultAnswer
         )
         # if filename is not None:
         #     sendMessageToTelegramChannel(
         #         document_filePath=filename, caption=caption, user=user
         #     )
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.WARN
             + "[+] Note: Trend calculation is based on number of days 'daysToLookBack' to scan as per your configuration."
             + colorText.END
         )
         try:
             if filename is not None:
                 os.remove(filename)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.GREEN
         + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
         + colorText.END
+        , enableMultipleLineOutput=True
     )
     if defaultAnswer is None:
         input("Press <Enter> to continue...")
 
 def sendGlobalMarketBarometer(userArgs=None):
     from pkscreener.classes import Barometer
     caption = "Global Market Barometer with India market Performance (top) and Valuation (bottom)"
@@ -2353,16 +2356,16 @@
         tabulated_text = colorText.miniTabulator().tabulate(
             backtest_df,
             headers="keys",
             tablefmt=colorText.No_Pad_GridFormat,
             showindex=False,
             maxcolwidths=Utility.tools.getMaxColumnWidths(backtest_df)
         ).encode("utf-8").decode(STD_ENCODING)
-    print(colorText.FAIL + summaryText + colorText.END + "\n")
-    print(tabulated_text + "\n")
+    OutputControls().printOutput(colorText.FAIL + summaryText + colorText.END + "\n")
+    OutputControls().printOutput(tabulated_text + "\n")
     choices, filename = getBacktestReportFilename(sortKey, optionalName)
     headerDict = {0: "<th></th>"}
     index = 1
     for col in backtest_df.columns:
         if col != "Stock":
             headerDict[index] = f"<th>{col}</th>"
             index += 1
@@ -2403,39 +2406,39 @@
                 f.write(oneline_text)
             Committer.execOSCommand(f"git add {onelineSummaryFile} -f >/dev/null 2>&1")
 
 def scanOutputDirectory(backtest=False):
     dirName = 'actions-data-scan' if not backtest else "Backtest-Reports"
     outputFolder = os.path.join(os.getcwd(),dirName)
     if not os.path.isdir(outputFolder):
-        print("Creating actions-data-scan directory now...")
+        OutputControls().printOutput("Creating actions-data-scan directory now...")
         os.makedirs(os.path.dirname(os.path.join(os.getcwd(),f"{dirName}{os.sep}")), exist_ok=True)
     return outputFolder
 
 def getBacktestReportFilename(sortKey="Stock", optionalName="backtest_result"):
     global userPassedArgs,selectedChoice
     choices = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
     filename = f"PKScreener_{choices}_{optionalName}_{sortKey if sortKey is not None else 'Default'}Sorted.html"
     return choices, filename
 
 def showOptionErrorMessage():
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "\n[+] Please enter a valid option & try Again!"
         + colorText.END
     )
     sleep(2)
     Utility.tools.clearScreen()
 
 def takeBacktestInputs(
     menuOption=None, indexOption=None, executeOption=None, backtestPeriod=0
 ):
     g10k = '"Growth of 10k"'
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.GREEN
         + f"[+] For {g10k if menuOption == 'G' else 'backtesting'}, you can choose from (1,2,3,4,5,10,15,22,30) or any other custom periods (< 450)."
     )
     try:
         if backtestPeriod == 0:
             backtestPeriod = int(
@@ -2468,15 +2471,15 @@
     )
     return indexOption, executeOption, backtestPeriod
 
 def toggleUserConfig():
     configManager.toggleConfig(
         candleDuration="1d" if configManager.isIntradayConfig() else "1m"
     )
-    print(
+    OutputControls().printOutput(
         colorText.BOLD
         + colorText.GREEN
         + "\nConfiguration toggled to duration: "
         + str(configManager.duration)
         + " and period: "
         + str(configManager.period)
         + colorText.END
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240417.274/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240417.274/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240417.274/pkscreener/pkscreenercli.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from time import sleep
 
 from PKDevTools.classes import log as log
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from pkscreener import Imports
+from PKDevTools.classes.OutputControls import OutputControls
 import pkscreener.classes.ConfigManager as ConfigManager
 
 multiprocessing.freeze_support()
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
 # from pkscreener.classes.IntradayMonitor import intradayMonitorInstance
 
@@ -239,46 +240,46 @@
     log_file_path = logFilePath()
 
     if os.path.exists(log_file_path):
         try:
             os.remove(log_file_path)
         except Exception:# pragma: no cover
             pass
-    print(colorText.FAIL + "\n[+] Logs will be written to:"+colorText.END)
-    print(colorText.GREEN + f"[+] {log_file_path}"+colorText.END)
-    print(colorText.FAIL + "[+] If you need to share, open this folder, copy and zip the log file to share.\n" + colorText.END)
+    OutputControls().printOutput(colorText.FAIL + "\n[+] Logs will be written to:"+colorText.END)
+    OutputControls().printOutput(colorText.GREEN + f"[+] {log_file_path}"+colorText.END)
+    OutputControls().printOutput(colorText.FAIL + "[+] If you need to share, open this folder, copy and zip the log file to share.\n" + colorText.END)
     # logger = multiprocessing.log_to_stderr(log.logging.DEBUG)
     log.setup_custom_logger(
         "pkscreener",
         log.logging.DEBUG,
         trace=trace,
         log_file_path=log_file_path,
         filter=None,
     )
     os.environ["PKDevTools_Default_Log_Level"] = str(log.logging.DEBUG)
 
 def warnAboutDependencies():
     if not Imports["talib"]:
-        print(
+        OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] TA-Lib is not installed. Looking for pandas_ta."
                 + colorText.END
             )
         sleep(1)
         if Imports["pandas_ta"]:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] Found and falling back on pandas_ta.\n[+] For full coverage(candle patterns), you may wish to read the README file in PKScreener repo : https://github.com/pkjmesra/PKScreener \n[+] or follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
                 + colorText.END
             )
             sleep(1)
         else:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
@@ -297,15 +298,15 @@
         # Delete any existing data from the previous run.
         configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
         for runOption in runOptions:
             args.options = runOption
             try:
                 optionalFinalOutcome_df = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
             except Exception as e:
-                print(e)
+                OutputControls().printOutput(e)
                 if args.log:
                     import traceback
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
@@ -325,15 +326,15 @@
                 )
             mark_down = colorText.miniTabulator().tabulate(
                                 final_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 showindex = False
                             ).encode("utf-8").decode(Utility.STD_ENCODING)
-            print(mark_down)
+            OutputControls().printOutput(mark_down)
             sendQuickScanResult(menuChoiceHierarchy="IntradayAnalysis",
                                 user="-1001785195297",
                                 tabulated_results=mark_down,
                                 markdown_results=mark_down,
                                 caption="IntradayAnalysis - Morning alert vs Market Close",
                                 pngName= f"PKS_IA_{PKDateUtilities.currentDateTime().strftime('%Y-%m-%d_%H:%M:%S')}",
                                 pngExtension= ".png"
@@ -348,18 +349,18 @@
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
             multiprocessing.set_start_method("fork")
         except RuntimeError as e:# pragma: no cover
             if "RUNNER" not in os.environ.keys() and ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
-                print(
+                OutputControls().printOutput(
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
-                print(e)
+                OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
@@ -373,26 +374,26 @@
     # multiprocessing behaves in unpredictable ways
     import pkscreener.classes.Utility as Utility
 
     configManager.default_logger = default_logger()
     if originalStdOut is None:
         # Clear only if this is the first time it's being called from some
         # loop within workflowtriggers.
-        Utility.tools.clearScreen(userArgs=args)
+        Utility.tools.clearScreen(userArgs=args, clearAlways=True)
     warnAboutDependencies()
     if args.prodbuild:
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
     if args.monitor:
         Utility.tools.clearScreen()
-        print("Not Implemented Yet!")
+        OutputControls().printOutput("Not Implemented Yet!")
         # intradayMonitorInstance.monitor()
         sys.exit(0)
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     if args.options is not None and str(args.options) == "0":
@@ -402,23 +403,23 @@
     if args.maxprice:
         configManager.maxLTP = args.maxprice
         configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
     if args.minprice:
         configManager.minLTP = args.minprice
         configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
     if args.testbuild and not args.prodbuild:
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "[+] Started in TestBuild mode!"
             + colorText.END
         )
         runApplication()
     elif args.download:
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "[+] Download ONLY mode! Stocks will not be screened!"
             + colorText.END
         )
         if args.intraday is None:
             configManager.toggleConfig(candleDuration="1d", clearCache=False)
@@ -446,29 +447,29 @@
             disableSysOut(disable=False)
             return
         sys.exit(0)
     except (RuntimeError, Exception) as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         if args.prodbuild:
             disableSysOut(disable=False)
-        print(
+        OutputControls().printOutput(
             f"{e}\n[+] An error occurred! Please run with '-l' option to collect the logs.\n[+] For example, 'pkscreener -l' and then contact the developer!"
         )
         if "RUNNER" in os.environ.keys() or ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
             traceback.print_exc()
         if args.v:
             disableSysOut(disable=False)
             return
         sys.exit(0)
 
 
 def scheduleNextRun():
     sleepUntilNextExecution = not PKDateUtilities.isTradingTime()
     while sleepUntilNextExecution:
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + (
                 "SecondsAfterClosingTime[%d] SecondsBeforeMarketOpen [%d]. Next run at [%s]"
                 % (
                     int(PKDateUtilities.secondsAfterCloseTime()),
                     int(PKDateUtilities.secondsBeforeOpenTime()),
@@ -489,15 +490,15 @@
         if (PKDateUtilities.secondsBeforeOpenTime() <= -3600) and (
             PKDateUtilities.secondsBeforeOpenTime() >= (-3600 - 1.5 * int(args.croninterval))
         ):
             sleepUntilNextExecution = False
         sleep(int(args.croninterval))
     global cron_runs
     if cron_runs > 0:
-        print(
+        OutputControls().printOutput(
             colorText.BOLD + colorText.GREEN + f'=> Going to fetch again in {int(args.croninterval)} sec. at {(PKDateUtilities.currentDateTime() + datetime.timedelta(seconds=120)).strftime("%Y-%m-%d %H:%M:%S")} IST...' + colorText.END,
             end="\r",
             flush=True,
         )
         sleep(int(args.croninterval) if not args.testbuild else 3)
     runApplication()
     cron_runs += 1
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240417.274/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240417.273
+Version: 0.44.20240417.274
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.273.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.274.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.270/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.273/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.273/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240417.274/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.273/setup.py` & `pkscreener-0.44.20240417.274/setup.py`

 * *Files identical despite different names*

