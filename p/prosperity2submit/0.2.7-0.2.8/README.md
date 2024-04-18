# Comparing `tmp/prosperity2submit-0.2.7.tar.gz` & `tmp/prosperity2submit-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.7.tar", last modified: Tue Apr 16 13:55:37 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.8.tar", last modified: Thu Apr 18 18:26:22 2024, max compression
```

## Comparing `prosperity2submit-0.2.7.tar` & `prosperity2submit-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:37.206309 prosperity2submit-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 13:55:33.000000 prosperity2submit-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-16 13:55:37.206309 prosperity2submit-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 13:55:33.000000 prosperity2submit-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:37.202309 prosperity2submit-0.2.7/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:33.000000 prosperity2submit-0.2.7/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 13:55:33.000000 prosperity2submit-0.2.7/prosperity2submit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-16 13:55:33.000000 prosperity2submit-0.2.7/prosperity2submit/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:37.206309 prosperity2submit-0.2.7/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 13:55:37.000000 prosperity2submit-0.2.7/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-16 13:55:35.000000 prosperity2submit-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:55:37.206309 prosperity2submit-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:26:22.988600 prosperity2submit-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 18:26:14.000000 prosperity2submit-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-18 18:26:22.988600 prosperity2submit-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-18 18:26:14.000000 prosperity2submit-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:26:22.988600 prosperity2submit-0.2.8/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:26:14.000000 prosperity2submit-0.2.8/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 18:26:14.000000 prosperity2submit-0.2.8/prosperity2submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-18 18:26:14.000000 prosperity2submit-0.2.8/prosperity2submit/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:26:22.988600 prosperity2submit-0.2.8/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 18:26:22.000000 prosperity2submit-0.2.8/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 18:26:19.000000 prosperity2submit-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:26:22.988600 prosperity2submit-0.2.8/setup.cfg
```

### Comparing `prosperity2submit-0.2.7/LICENSE` & `prosperity2submit-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.7/PKG-INFO` & `prosperity2submit-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.7
+Version: 0.2.8
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.7/README.md` & `prosperity2submit-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.7/prosperity2submit/__main__.py` & `prosperity2submit-0.2.8/prosperity2submit/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 def main() -> int:
     parser = ArgumentParser(prog="prosperity2submit", description="Submit an algorithm.")
     parser.add_argument("algorithm", type=str, help="path to the Python file containing the algorithm to submit")
     parser.add_argument("--out", type=str, help="path to save submission logs to (defaults to submissions/<timestamp>.log)")
     parser.add_argument("--no-logs", action="store_true", help="don't download logs when done")
     parser.add_argument("--vis", action="store_true", help="open submission in visualizer when done")
+    parser.add_argument("--vis-requests", type=int, default=2, help="number of requests the visualizer is expected to make to the submitter's HTTP server when using --vis")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     if args.out is not None and args.no_logs:
         print(f"--out and --no-logs are mutually exclusive")
         sys.exit(1)
@@ -32,11 +33,11 @@
         output_file = Path(args.out).expanduser().resolve()
     elif args.no_logs:
         output_file = None
     else:
         timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         output_file = Path.cwd() / "submissions" / f"{timestamp}.log"
 
-    submit(algorithm_file, output_file, args.vis)
+    submit(algorithm_file, output_file, args.vis, args.vis_requests)
 
 if __name__ == "__main__":
     main()
```

### Comparing `prosperity2submit-0.2.7/prosperity2submit/core.py` & `prosperity2submit-0.2.8/prosperity2submit/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,27 +159,26 @@
     def end_headers(self) -> None:
         self.send_header("Access-Control-Allow-Origin", "*")
         return super().end_headers()
 
     def log_message(self, format: str, *args: Any) -> None:
         return
 
-def open_in_visualizer(output_file: Path) -> None:
+def open_in_visualizer(output_file: Path, no_requests: int) -> None:
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
 
-def submit(algorithm_file: Path, output_file: Optional[Path], open_visualizer: bool) -> None:
+def submit(algorithm_file: Path, output_file: Optional[Path], open_visualizer: bool, visualizer_requests: int) -> None:
     round = get_current_round()
 
     submit_algorithm(algorithm_file)
     data = monitor_status(round, algorithm_file)
 
     if output_file is not None:
         download_logs(data, output_file)
@@ -187,8 +186,8 @@
         if data["status"] == "FINISHED":
             log_profit_loss(output_file)
 
     if open_visualizer:
         if data["status"] == "ERROR":
             print("Submission errored, not opening visualizer")
         else:
-            open_in_visualizer(output_file)
+            open_in_visualizer(output_file, visualizer_requests)
```

### Comparing `prosperity2submit-0.2.7/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.8/prosperity2submit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.7
+Version: 0.2.8
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.7/pyproject.toml` & `prosperity2submit-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.7"
+version = "0.2.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

