# Comparing `tmp/prosperity2bt-0.6.0.tar.gz` & `tmp/prosperity2bt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.6.0.tar", last modified: Wed Apr 17 01:33:42 2024, max compression
+gzip compressed data, was "prosperity2bt-0.6.1.tar", last modified: Thu Apr 18 18:25:51 2024, max compression
```

## Comparing `prosperity2bt-0.6.0.tar` & `prosperity2bt-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.112665 prosperity2bt-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-17 01:33:42.108665 prosperity2bt-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.092664 prosperity2bt-0.6.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.092664 prosperity2bt-0.6.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.092664 prosperity2bt-0.6.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.100664 prosperity2bt-0.6.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.108665 prosperity2bt-0.6.0/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-17 01:33:38.000000 prosperity2bt-0.6.0/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:33:42.108665 prosperity2bt-0.6.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 01:33:42.000000 prosperity2bt-0.6.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-17 01:33:39.000000 prosperity2bt-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:33:42.112665 prosperity2bt-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.065940 prosperity2bt-0.6.1/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.073940 prosperity2bt-0.6.1/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.073940 prosperity2bt-0.6.1/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-18 18:25:48.000000 prosperity2bt-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/setup.cfg
```

### Comparing `prosperity2bt-0.6.0/LICENSE` & `prosperity2bt-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/PKG-INFO` & `prosperity2bt-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
+Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
 This repository contains a backtester [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. The output it generates closely matches the format of the output generated by the official submission environment and is therefore compatible with my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (assuming your code contains the visualizer's required prerequisites as explained on the visualizer's homepage).
```

### Comparing `prosperity2bt-0.6.0/README.md` & `prosperity2bt-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/__main__.py` & `prosperity2bt-0.6.1/prosperity2bt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,25 +158,24 @@
     def end_headers(self) -> None:
         self.send_header("Access-Control-Allow-Origin", "*")
         return super().end_headers()
 
     def log_message(self, format: str, *args: Any) -> None:
         return
 
-def open_visualizer(output_file: Path) -> None:
+def open_visualizer(output_file: Path, no_requests: int) -> None:
     http_handler = partial(HTTPRequestHandler, directory=output_file.parent)
     http_server = HTTPServer(("localhost", 0), http_handler)
-    http_server.timeout = 5
 
     webbrowser.open(f"https://jmerle.github.io/imc-prosperity-2-visualizer/?open=http://localhost:{http_server.server_port}/{output_file.name}")
 
     # Chrome makes 2 requests: 1 OPTIONS request to check for CORS headers and 1 GET request to get the data
-    # Some users reported their browser only makes 1 request, in that case the second call is terminated after `http_server.timeout` seconds
-    http_server.handle_request()
-    http_server.handle_request()
+    # Some users reported their browser only makes 1 request, which is covered by the --vis-requests option
+    for _ in range(no_requests):
+        http_server.handle_request()
 
 def format_path(path: Path) -> str:
     cwd = Path.cwd()
     if path.is_relative_to(cwd):
         return str(path.relative_to(cwd))
     else:
         return str(path)
@@ -188,14 +187,16 @@
     parser.add_argument("--merge-pnl", action="store_true", help="merge profit and loss across days")
     parser.add_argument("--vis", action="store_true", help="open backtest result in visualizer when done")
     parser.add_argument("--out", type=str, help="path to save output log to (defaults to backtests/<timestamp>.log)")
     parser.add_argument("--data", type=str, help="path to data directory (must look similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources)")
     parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
     parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("--no-out", action="store_true", help="skip saving the output log to a file")
+    parser.add_argument("--no-progress", action="store_true", help="don't show progress bars")
+    parser.add_argument("--vis-requests", type=int, default=2, help="number of requests the visualizer is expected to make to the backtester's HTTP server when using --vis")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     if args.vis and args.no_out:
         print("Error: --vis and --no-out are mutually exclusive")
         sys.exit(1)
@@ -220,26 +221,26 @@
     results = []
     for day in days:
         print(f"Backtesting {args.algorithm} on round {day.round_num} day {day.day_num}")
 
         reload(trader_module)
         trader = trader_module.Trader()
 
-        result = run_backtest(trader, day, args.print, args.no_trades_matching)
+        result = run_backtest(trader, day, args.print, args.no_trades_matching, args.no_progress)
         print_day_summary(result)
 
         results.append(result)
 
     merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
 
     if len(days) > 1:
         print_overall_summary(results)
 
     if output_file is not None:
         write_output(output_file, merged_results)
         print(f"\nSuccessfully saved backtest results to {format_path(output_file)}")
 
     if args.vis:
-        open_visualizer(output_file)
+        open_visualizer(output_file, args.vis_requests)
 
 if __name__ == "__main__":
     main()
```

### Comparing `prosperity2bt-0.6.0/prosperity2bt/data.py` & `prosperity2bt-0.6.1/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.6.1/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/file_reader.py` & `prosperity2bt-0.6.1/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/models.py` & `prosperity2bt-0.6.1/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/prosperity2bt/runner.py` & `prosperity2bt-0.6.1/prosperity2bt/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from contextlib import closing, redirect_stdout
 from io import StringIO
 from IPython.utils.io import Tee
 from prosperity2bt.data import BacktestData, LIMITS
 from prosperity2bt.datamodel import Observation, Order, OrderDepth, Symbol, Trade, TradingState
 from prosperity2bt.models import ActivityLogRow, BacktestResult, MarketTrade, SandboxLogRow, TradeRow
+from tqdm import tqdm
 from typing import Any
 
 def prepare_state(state: TradingState, data: BacktestData) -> None:
     for product in data.products:
         order_depth = OrderDepth()
         row = data.prices[state.timestamp][product]
 
@@ -206,15 +207,21 @@
             trade.trade.quantity = min(trade.buy_quantity, trade.sell_quantity)
 
         remaining_market_trades = [t.trade for t in trades if t.trade.quantity > 0]
 
         state.market_trades[product] = remaining_market_trades
         result.trades.extend([TradeRow(trade) for trade in remaining_market_trades])
 
-def run_backtest(trader: Any, data: BacktestData, print_output: bool, disable_trades_matching: bool) -> BacktestResult:
+def run_backtest(
+    trader: Any,
+    data: BacktestData,
+    print_output: bool,
+    disable_trades_matching: bool,
+    disable_progress_bar: bool,
+) -> BacktestResult:
     trader_data = ""
     state = TradingState(
         traderData=trader_data,
         timestamp=0,
         listings={},
         order_depths={},
         own_trades={},
@@ -227,15 +234,18 @@
         round_num=data.round_num,
         day_num=data.day_num,
         sandbox_logs=[],
         activity_logs=[],
         trades=[],
     )
 
-    for timestamp in sorted(data.prices.keys()):
+    sorted_timestamps = sorted(data.prices.keys())
+    timestamps_iterator = sorted_timestamps if disable_progress_bar else tqdm(sorted_timestamps, ascii=True)
+
+    for timestamp in timestamps_iterator:
         state.timestamp = timestamp
         state.traderData = trader_data
 
         prepare_state(state, data)
 
         stdout = StringIO()
```

### Comparing `prosperity2bt-0.6.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.6.1/prosperity2bt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
+Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
 This repository contains a backtester [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. The output it generates closely matches the format of the output generated by the official submission environment and is therefore compatible with my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (assuming your code contains the visualizer's required prerequisites as explained on the visualizer's homepage).
```

### Comparing `prosperity2bt-0.6.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.6.1/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.0/pyproject.toml` & `prosperity2bt-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.6.0"
+version = "0.6.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">= 3.9"
-dependencies = ["ipython", "jsonpickle"]
+dependencies = ["ipython", "jsonpickle", "tqdm"]
 
 [project.scripts]
 prosperity2bt = "prosperity2bt.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/jmerle/imc-prosperity-2-backtester"
 Issues = "https://github.com/jmerle/imc-prosperity-2-backtester/issues"
```

