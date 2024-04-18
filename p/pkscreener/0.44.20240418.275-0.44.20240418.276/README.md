# Comparing `tmp/pkscreener-0.44.20240418.275.tar.gz` & `tmp/pkscreener-0.44.20240418.276.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240418.275.tar", last modified: Thu Apr 18 04:26:25 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240418.276.tar", last modified: Thu Apr 18 09:50:47 2024, max compression
```

## Comparing `pkscreener-0.44.20240418.275.tar` & `pkscreener-0.44.20240418.276.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:26:25.761053 pkscreener-0.44.20240418.275/
--rw-rw-rw-   0        0        0     1086 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-18 04:26:25.761053 pkscreener-0.44.20240418.275/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 04:26:25.745453 pkscreener-0.44.20240418.275/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:26:25.761053 pkscreener-0.44.20240418.275/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24899 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3237 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    28153 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17537 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8118 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   111107 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46418 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79037 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-18 04:26:19.000000 pkscreener-0.44.20240418.275/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   117360 2024-04-18 04:22:15.000000 pkscreener-0.44.20240418.275/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-18 04:22:16.000000 pkscreener-0.44.20240418.275/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-18 04:22:16.000000 pkscreener-0.44.20240418.275/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19839 2024-04-18 04:22:16.000000 pkscreener-0.44.20240418.275/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:26:25.761053 pkscreener-0.44.20240418.275/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-18 04:26:25.000000 pkscreener-0.44.20240418.275/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-18 04:26:25.761053 pkscreener-0.44.20240418.275/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-18 04:22:16.000000 pkscreener-0.44.20240418.275/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:50:47.586579 pkscreener-0.44.20240418.276/
+-rw-rw-rw-   0        0        0     1086 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-18 09:50:47.586579 pkscreener-0.44.20240418.276/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 09:50:47.570958 pkscreener-0.44.20240418.276/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:50:47.586579 pkscreener-0.44.20240418.276/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24899 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3237 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    28153 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17603 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   111107 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46418 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79127 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-18 09:50:40.000000 pkscreener-0.44.20240418.276/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   117414 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19783 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:50:47.570958 pkscreener-0.44.20240418.276/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-18 09:50:47.000000 pkscreener-0.44.20240418.276/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-18 09:50:47.586579 pkscreener-0.44.20240418.276/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-18 09:47:29.000000 pkscreener-0.44.20240418.276/setup.py
```

### Comparing `pkscreener-0.44.20240418.275/LICENSE` & `pkscreener-0.44.20240418.276/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/LICENSE-Others` & `pkscreener-0.44.20240418.276/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/PKG-INFO` & `pkscreener-0.44.20240418.276/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240418.275
+Version: 0.44.20240418.276
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.275.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.276.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.275/README.md` & `pkscreener-0.44.20240418.276/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener/__init__.py` & `pkscreener-0.44.20240418.276/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKScanRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,16 +298,17 @@
             + colorText.END
         )
         start_time = time.time()
         for worker in consumers:
             sys.stdout.write(f"{round(time.time() - start_time)}.")
             worker.daemon = True
             worker.start()
-        OutputControls().printOutput(f"Started all workers in {time.time() - start_time}s")
-        # sys.stdout.write("\x1b[1A")
+        OutputControls().printOutput(f"Started all workers in {round(time.time() - start_time,4)}s")
+        if OutputControls().enableMultipleLineOutput:
+            sys.stdout.write("\x1b[1A")
 
     def terminateAllWorkers(consumers, tasks_queue, testing):
         # Exit all processes. Without this, it threw error in next screening session
         for worker in consumers:
             try:
                 if testing: # pragma: no cover
                     if sys.platform.startswith("win"):
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKScheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             futures = []  # keep track of the jobs
             with multiprocessing.Manager() as manager:
                 # this is the key - we share some state between our 
                 # main process and our worker functions
                 _progress = manager.dict()
                 _results = manager.dict()
                 console.control(Control(*((ControlType.CURSOR_UP,1),))) # Cursor up 1 lines f"\x1b[{param}A"
-                sys.stdout.write("\x1b[2K")  # delete the last line
+                # sys.stdout.write("\x1b[2K")  # delete the last line
                 overall_progress_task = progress.add_task(f"[green]{label if label is not None else 'Pending jobs progress:'}")
 
                 lock = Lock()
                 with ProcessPoolExecutor(max_workers=n_workers,
                                          initializer=init_pool_processes,
                                          initargs=(lock,)) as executor:
                     for task in tasksList:  # iterate over the jobs we need to run
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,21 +121,21 @@
     def clearScreen(userArgs=None,clearAlways=False):
         if "RUNNER" in os.environ.keys() or (userArgs is not None and userArgs.prodbuild):
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
         elif (userArgs is not None and userArgs.runintradayanalysis):
             return
-        if clearAlways:
+        if clearAlways or OutputControls().enableMultipleLineOutput:
             if platform.system() == "Windows":
                 os.system("cls")
             else:
                 os.system("clear")
         try:
-            if clearAlways:
+            if clearAlways or OutputControls().enableMultipleLineOutput:
                 art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
                 OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
 
     # Print about developers and repository
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/classes/keys.py` & `pkscreener-0.44.20240418.276/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/courbd.ttf` & `pkscreener-0.44.20240418.276/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/globals.py` & `pkscreener-0.44.20240418.276/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2087,15 +2087,15 @@
                 )
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
-        OutputControls().printOutput(f"\x1b[1A")
+        OutputControls().printOutput(f"\x1b[{3 if OutputControls().enableMultipleLineOutput else 1}A")
         elapsed_time = time.time() - start_time
         if menuOption in ["X", "G", "C"]:
             # create extension
             screenResults = pd.DataFrame(lstscreen)
             saveResults = pd.DataFrame(lstsave)
 
     except KeyboardInterrupt:
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240418.276/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240418.276/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240418.276/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,16 @@
             if "RUNNER" not in os.environ.keys() and ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
                 OutputControls().printOutput(
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
                 OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
+
+        OutputControls(enableMultipleLineOutput=(not args.monitor)).printOutput("",end="\r")
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
@@ -383,19 +385,15 @@
     if args.prodbuild:
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
-    if args.monitor:
-        Utility.tools.clearScreen()
-        OutputControls().printOutput("Not Implemented Yet!")
-        # intradayMonitorInstance.monitor()
-        sys.exit(0)
+        
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     if args.options is not None and str(args.options) == "0":
         # Must be from unit tests to be able to break out of loops via eventing
         args.options = None
@@ -432,16 +430,16 @@
     if hasCronInterval:
         scheduleNextRun()
     else:
         runApplication()
 
 def runApplicationForScreening():
     try:
-        shouldBreak = args.exit or args.user is not None or args.testbuild
         hasCronInterval = args.croninterval is not None and str(args.croninterval).isnumeric()
+        shouldBreak = (args.exit and not hasCronInterval)or args.user is not None or args.testbuild
         runLoopOnScheduleOrStdApplication(hasCronInterval)
         while True:
             if shouldBreak:
                 break
             runLoopOnScheduleOrStdApplication(hasCronInterval)
         if args.v:
             disableSysOut(disable=False)
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240418.276/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240418.275
+Version: 0.44.20240418.276
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.275.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.276.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.274/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.275/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.275/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240418.276/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.275/setup.py` & `pkscreener-0.44.20240418.276/setup.py`

 * *Files identical despite different names*

