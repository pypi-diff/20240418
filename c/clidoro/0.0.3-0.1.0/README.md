# Comparing `tmp/clidoro-0.0.3.tar.gz` & `tmp/clidoro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidoro-0.0.3.tar", last modified: Thu Apr 18 06:40:58 2024, max compression
+gzip compressed data, was "clidoro-0.1.0.tar", last modified: Thu Apr 18 08:15:25 2024, max compression
```

## Comparing `clidoro-0.0.3.tar` & `clidoro-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/
--rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.0.3/LICENSE.MD
--rw-r--r--   0 juno      (1000) juno      (1000)     2500 2024-04-18 06:40:58.958819 clidoro-0.0.3/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)     1289 2024-04-18 05:46:55.000000 clidoro-0.0.3/README.md
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.954819 clidoro-0.0.3/clidoro/
--rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.0.3/clidoro/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2422 2024-04-18 04:51:34.000000 clidoro-0.0.3/clidoro/_utils.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.0.3/clidoro/chart.py
--rw-------   0 juno      (1000) juno      (1000)     3259 2024-04-18 06:32:04.000000 clidoro-0.0.3/clidoro/clidoro.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      449 2024-04-18 04:56:29.000000 clidoro-0.0.3/clidoro/data.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/clidoro/termgraph/
--rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.0.3/clidoro/termgraph/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.0.3/clidoro/termgraph/_termgraph.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.0.3/clidoro/termgraph/module.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.0.3/clidoro/termgraph/utils.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/clidoro.egg-info/
--rw-r--r--   0 juno      (1000) juno      (1000)     2500 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)      464 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/SOURCES.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/dependency_links.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/entry_points.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.0.3/clidoro.egg-info/not-zip-safe
--rw-rw-r--   0 juno      (1000) juno      (1000)       60 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/requires.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/top_level.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 06:40:58.962819 clidoro-0.0.3/setup.cfg
--rw-rw-r--   0 juno      (1000) juno      (1000)     1811 2024-04-18 06:40:27.000000 clidoro-0.0.3/setup.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.715319 clidoro-0.1.0/
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.0/LICENSE.MD
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:15:25.715319 clidoro-0.1.0/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.0/README.md
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.711319 clidoro-0.1.0/clidoro/
+-rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.0/clidoro/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.0/clidoro/_utils.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.1.0/clidoro/chart.py
+-rw-------   0 juno      (1000) juno      (1000)     3716 2024-04-18 08:12:17.000000 clidoro-0.1.0/clidoro/clidoro.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.0/clidoro/data.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.711319 clidoro-0.1.0/clidoro/termgraph/
+-rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.0/clidoro/termgraph/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.0/clidoro/termgraph/_termgraph.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.0/clidoro/termgraph/module.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.0/clidoro/termgraph/utils.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.715319 clidoro-0.1.0/clidoro.egg-info/
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)      464 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/SOURCES.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/dependency_links.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/entry_points.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.0/clidoro.egg-info/not-zip-safe
+-rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/requires.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/top_level.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 08:15:25.715319 clidoro-0.1.0/setup.cfg
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1831 2024-04-18 08:14:51.000000 clidoro-0.1.0/setup.py
```

### Comparing `clidoro-0.0.3/LICENSE.MD` & `clidoro-0.1.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.3/PKG-INFO` & `clidoro-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.0.3
+Version: 0.1.0
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
@@ -25,14 +25,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Requires-Dist: playsound
 Requires-Dist: alive-progress
 Requires-Dist: simple-term-menu
 Requires-Dist: requests
 Requires-Dist: colorama
+Requires-Dist: notify-py
 
 
 <pre>
         _   _     _                 
        | | (_)   | |                
    ___ | |  _  __| | ___  _ __ ___  
   / __|| | | |/ _` |/ _ \| '__/ _ \ 
@@ -55,7 +56,9 @@
 
 TODO:
 - [ ] add windows support (not tested)
 - [ ] add mac support (not tested)
 - [x] pypi
 - [ ] background sound
 - [ ] custom notification sound (use my [data-server](https://github.com/kingjuno/data-server))
+- [x] Desktop Notification popup
+- [x] Clear Database
```

### Comparing `clidoro-0.0.3/README.md` & `clidoro-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 
 
 TODO:
 - [ ] add windows support (not tested)
 - [ ] add mac support (not tested)
 - [x] pypi
 - [ ] background sound
-- [ ] custom notification sound (use my [data-server](https://github.com/kingjuno/data-server))
+- [ ] custom notification sound (use my [data-server](https://github.com/kingjuno/data-server))
+- [x] Desktop Notification popup
+- [x] Clear Database
```

### Comparing `clidoro-0.0.3/clidoro/chart.py` & `clidoro-0.1.0/clidoro/chart.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.3/clidoro/clidoro.py` & `clidoro-0.1.0/clidoro/clidoro.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from pathlib import Path
 
 from simple_term_menu import TerminalMenu
 
 from clidoro._utils import _timer, timestamp_to_datetime
 from clidoro.chart import history, history_all
-from clidoro.data import save_to_db
+from clidoro.data import clear_db, save_to_db
 
 TITLE = """        _   _     _                 
        | | (_)   | |                
    ___ | |  _  __| | ___  _ __ ___  
   / __|| | | |/ _` |/ _ \| '__/ _ \ 
  | (__ | | | | (_| | (_) | | | (_) |
   \___||_| |_|\__,_|\___/|_|  \___/ 
@@ -30,42 +30,54 @@
     start_time = timestamp_to_datetime(time.time())
     while True:
         menu_entry_index = menu.show()
         if menu_entry_index == len(menu._menu_entries) - 1:
             break
         else:
             _time = times[menu_entry_index]
-            stats = _timer(_time, "simple-notification", CACHE_DIR)
+            stats = _timer(
+                0.01, "simple-notification", CACHE_DIR, "pomodoro" if _save else "break"
+            )
         if _save and stats > 0:
             save_to_db([[start_time, _time]], CACHE_DIR)
 
 
 def history_menu(menu):
     while True:
         menu_entry_index = menu.show()
         if menu_entry_index == len(menu._menu_entries) - 1:
             break
         elif menu_entry_index == 0:
             _history = history(CACHE_DIR).replace("\n\n", "\n")
         elif menu_entry_index == 1:
             _history = history_all(CACHE_DIR)
+        elif menu_entry_index == 2:
+            delete_menu = TerminalMenu(
+                ["accept", "exit"],
+                accept_keys=("enter", "alt-d"),
+                menu_highlight_style=("bg_black", "fg_green"),
+            )
+            delete_index = delete_menu.show()
+            if delete_index == 0:
+                clear_db(CACHE_DIR)
+            return
         print(TITLE, _history, sep="\n")
         terminal_menu = TerminalMenu(
             ["exit"],
             accept_keys=("enter", "alt-d"),
             menu_highlight_style=("bg_black", "fg_green"),
         )
         terminal_menu.show()
 
 
 def main():
     cli_options = ["start", "break", "history", "exit"]
     pomodoro_options = ["20 mins", "25 mins", "30 mins", "45 mins", "60 mins", "back"]
     break_options = ["5 mins", "10 mins", "15 mins", "30 mins", "back"]
-    history_options = ["Pomodoros by weekdays", "Stats", "exit"]
+    history_options = ["Pomodoros by weekdays", "Stats", "clear DB", "exit"]
     terminal_menu = TerminalMenu(
         cli_options,
         title=TITLE,
         accept_keys=("enter", "alt-d"),
         clear_screen=True,
         menu_highlight_style=("bg_black", "fg_green"),
     )
```

### Comparing `clidoro-0.0.3/clidoro/termgraph/_termgraph.py` & `clidoro-0.1.0/clidoro/termgraph/_termgraph.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.3/clidoro/termgraph/module.py` & `clidoro-0.1.0/clidoro/termgraph/module.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.3/clidoro/termgraph/utils.py` & `clidoro-0.1.0/clidoro/termgraph/utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.3/clidoro.egg-info/PKG-INFO` & `clidoro-0.1.0/clidoro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.0.3
+Version: 0.1.0
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
@@ -25,14 +25,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Requires-Dist: playsound
 Requires-Dist: alive-progress
 Requires-Dist: simple-term-menu
 Requires-Dist: requests
 Requires-Dist: colorama
+Requires-Dist: notify-py
 
 
 <pre>
         _   _     _                 
        | | (_)   | |                
    ___ | |  _  __| | ___  _ __ ___  
   / __|| | | |/ _` |/ _ \| '__/ _ \ 
@@ -55,7 +56,9 @@
 
 TODO:
 - [ ] add windows support (not tested)
 - [ ] add mac support (not tested)
 - [x] pypi
 - [ ] background sound
 - [ ] custom notification sound (use my [data-server](https://github.com/kingjuno/data-server))
+- [x] Desktop Notification popup
+- [x] Clear Database
```

### Comparing `clidoro-0.0.3/setup.py` & `clidoro-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 MAJOR_VERSION = "0"
-MINOR_VERSION = "0"
-MICRO_VERSION = "3"
+MINOR_VERSION = "1"
+MICRO_VERSION = "0"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 
 setup(
     name="clidoro",
     packages=find_packages(exclude=["docs", "tests*", "examples"]),
     version=VERSION,
@@ -24,14 +24,15 @@
     keywords=["Productivity", "Pomodoro"],
     install_requires=[
         "playsound",
         "alive-progress",
         "simple-term-menu",
         "requests",
         "colorama",
+        "notify-py"
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Intended Audience :: System Administrators",
         "Operating System :: Unix",
         # TODO: Add Windows support
```

