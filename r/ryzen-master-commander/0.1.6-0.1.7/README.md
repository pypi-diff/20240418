# Comparing `tmp/ryzen-master-commander-0.1.6.tar.gz` & `tmp/ryzen-master-commander-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryzen-master-commander-0.1.6.tar", last modified: Thu Apr 11 20:45:27 2024, max compression
+gzip compressed data, was "ryzen-master-commander-0.1.7.tar", last modified: Wed Apr 17 23:25:28 2024, max compression
```

## Comparing `ryzen-master-commander-0.1.6.tar` & `ryzen-master-commander-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:45:27.452494 ryzen-master-commander-0.1.6/
--rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.6/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)      191 2024-04-11 20:45:27.452494 ryzen-master-commander-0.1.6/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     3590 2024-04-11 20:44:08.000000 ryzen-master-commander-0.1.6/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:45:27.451494 ryzen-master-commander-0.1.6/app/
--rw-r--r--   0 sam       (1000) sam       (1000)      241 2024-04-11 20:33:33.000000 ryzen-master-commander-0.1.6/app/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.6/app/graphs.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7027 2024-04-11 20:06:15.000000 ryzen-master-commander-0.1.6/app/main_window.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.6/app/profile_manager.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-11 19:19:29.000000 ryzen-master-commander-0.1.6/app/system_utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:45:27.452494 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      191 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-11 20:45:27.000000 ryzen-master-commander-0.1.6/ryzen_master_commander.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-11 20:45:27.452494 ryzen-master-commander-0.1.6/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      443 2024-04-11 20:45:16.000000 ryzen-master-commander-0.1.6/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-17 23:25:28.345649 ryzen-master-commander-0.1.7/
+-rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.7/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     3789 2024-04-17 23:25:28.345649 ryzen-master-commander-0.1.7/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     3557 2024-04-12 19:02:10.000000 ryzen-master-commander-0.1.7/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-17 23:25:28.344649 ryzen-master-commander-0.1.7/app/
+-rw-r--r--   0 sam       (1000) sam       (1000)      241 2024-04-11 20:33:33.000000 ryzen-master-commander-0.1.7/app/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.7/app/graphs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6958 2024-04-11 20:47:27.000000 ryzen-master-commander-0.1.7/app/main_window.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.7/app/profile_manager.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-17 23:17:46.000000 ryzen-master-commander-0.1.7/app/system_utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-17 23:25:28.345649 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     3789 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-17 23:25:28.000000 ryzen-master-commander-0.1.7/ryzen_master_commander.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-17 23:25:28.345649 ryzen-master-commander-0.1.7/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)     4080 2024-04-17 23:25:16.000000 ryzen-master-commander-0.1.7/setup.py
```

### Comparing `ryzen-master-commander-0.1.6/LICENSE` & `ryzen-master-commander-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.6/README.md` & `ryzen-master-commander-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 
 ### Prerequisites
 
 Make sure you have the following dependencies installed on your system:
 
 - Python 3.6 or higher 🐍
 - TCL and Tk libraries 🖼️
-- `nbfc` and `ryzenadj` command-line tools 🔧
+- `nbfc-linux` and `ryzenadj` command-line tools 🔧 from the following projects: 
+  - https://github.com/nbfc-linux/nbfc-linux
+  - https://github.com/FlyGoat/RyzenAdj
 
 #### Installing Dependencies on Arch Linux
 
 ```
 sudo pacman -S python tcl tk nbfc ryzenadj
 ```
 
 #### Installing Dependencies on Debian-based Systems (Ubuntu, Debian, etc.)
 
-```
-sudo apt update
-sudo apt install python3 python3-pip tcl tk nbfc ryzenadj
-```
+Install tkinter: `sudo apt install python3-tk`
+
+Follow the instructions for your linux distribution on the respective project package page above to install nbfc-linux and ryzenadj.
 
 ### Installation
 
 Install Ryzen Master Commander using pip:
 
 ```
 pip install ryzen-master-commander
@@ -55,17 +56,14 @@
 ryzen-master-commander
 ```
 
 The application will prompt you for your sudo password, which is required for controlling the fan speed and applying TDP settings. 🔑
 
 That's it! You're now ready to use Ryzen Master Commander to monitor and control your Ryzen-based system. Enjoy! 😊
 
-You can add this Quick Start guide to your README.md file to provide users with a concise set of instructions to get up and running with Ryzen Master Commander quickly. Feel free to adjust the wording or formatting as needed to fit the style of your README.
-
-
 ### Installing from Source
 
 To install Ryzen Master Commander from source, follow these steps:
 
 1. Clone the repository:
 
 ```
@@ -110,8 +108,8 @@
 
 ## License 📜
 
 This project is licensed under the [Apache License 2.0](LICENSE).
 
 ## Acknowledgements 🙏
 
-Ryzen Master Commander was developed on Arch Linux for the GPD Win Mini, but it should work on other Ryzen-based devices as well. Special thanks to the developers of the `nbfc` and `ryzenadj` tools, which make this application possible. 👏
+Ryzen Master Commander was developed on Arch Linux for the GPD Win Mini, but it should work on other Ryzen-based devices as well. Special thanks to the developers of the `nbfc-linux` and `ryzenadj` tools, which make this application possible. 👏
```

### Comparing `ryzen-master-commander-0.1.6/app/graphs.py` & `ryzen-master-commander-0.1.7/app/graphs.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.6/app/main_window.py` & `ryzen-master-commander-0.1.7/app/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import ttkbootstrap as ttk
 from ttkbootstrap.constants import *
 from tkinter.simpledialog import askstring
 import sys
-# import json
-# import os
-# from json.decoder import JSONDecodeError
 import subprocess
 from app.graphs import TemperatureGraph, FanSpeedGraph
 from app.system_utils import get_system_readings, apply_tdp_settings
 from app.profile_manager import ProfileManager
 
 class MainWindow:
     def __init__(self, root):
```

### Comparing `ryzen-master-commander-0.1.6/app/profile_manager.py` & `ryzen-master-commander-0.1.7/app/profile_manager.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.6/app/system_utils.py` & `ryzen-master-commander-0.1.7/app/system_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         for key, value in current_profile.items():
             if key in ["fast-limit", "slow-limit"]:
                 command.extend([f'--{key}={value * 1000}'])
             elif key == "slow-time":
                 command.extend([f'--{key}={value * 1000}'])
             elif key not in ["name", "max_performance", "power_saving"]:
                 command.extend([f'--{key}={value}'])
-        if current_profile.get("max_performance"):
-            command.append("--max-performance")
-        elif current_profile.get("power_saving"):
+        if current_profile.get("power_saving"):
             command.append("--power-saving")
+        elif current_profile.get("max_performance"):
+            command.append("--max-performance")
         try:
             subprocess.run(command, input=sudo_password + '\n', text=True)
         except subprocess.CalledProcessError as e:
             print(f"Error applying TDP settings: {e}")
```

