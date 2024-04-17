# Comparing `tmp/CTid-programmer-1.4.2.tar.gz` & `tmp/CTid-programmer-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTid-programmer-1.4.2.tar", last modified: Mon Jul 10 21:39:52 2023, max compression
+gzip compressed data, was "CTid-programmer-1.4.3.tar", last modified: Wed Apr 17 22:11:02 2024, max compression
```

## Comparing `CTid-programmer-1.4.2.tar` & `CTid-programmer-1.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.157327 CTid-programmer-1.4.2/CTid_programmer.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1393 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       68 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/top_level.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/LICENSE
--rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/MANIFEST.in
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1393 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.2/README.rst
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.185326 CTid-programmer-1.4.2/ctid_programmer/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.225326 CTid-programmer-1.4.2/ctid_programmer/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.2/ctid_programmer/gui/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.233326 CTid-programmer-1.4.2/ctid_programmer/gui/images/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/gui/images/ctid-logo.svg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2022-05-05 19:33:57.000000 CTid-programmer-1.4.2/ctid_programmer/gui/main_window.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/main_window_rc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2023-07-10 17:59:24.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_ct.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2021-04-26 21:41:35.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_linear.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2020-10-07 04:04:19.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_ntc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_pulse.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_temp.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_volt.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/preferences_dialog.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/template_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2140 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/preferences.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    35995 2023-07-10 17:58:46.000000 CTid-programmer-1.4.2/ctid_programmer/programmer.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.233326 CTid-programmer-1.4.2/ctid_programmer/qt4/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.2/ctid_programmer/qt4/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.117327 CTid-programmer-1.4.2/ctid_programmer/resources/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.241325 CTid-programmer-1.4.2/ctid_programmer/resources/code/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/resources/code/ac.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.2/ctid_programmer/resources/code/powered.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    15071 2023-04-27 17:10:08.000000 CTid-programmer-1.4.2/ctid_programmer/sensor_params.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4969 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     7654 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn_egauge.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4075 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn_local.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2410 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/template.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2023-04-27 17:09:38.000000 CTid-programmer-1.4.2/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2023-07-10 18:19:50.000000 CTid-programmer-1.4.2/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.839902 CTid-programmer-1.4.3/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.723903 CTid-programmer-1.4.3/CTid_programmer.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1393 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       68 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2024-04-17 22:11:02.000000 CTid-programmer-1.4.3/CTid_programmer.egg-info/top_level.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.3/LICENSE
+-rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.3/MANIFEST.in
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1393 2024-04-17 22:11:02.839902 CTid-programmer-1.4.3/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.3/README.rst
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.763903 CTid-programmer-1.4.3/ctid_programmer/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.3/ctid_programmer/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.819902 CTid-programmer-1.4.3/ctid_programmer/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.3/ctid_programmer/gui/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.823902 CTid-programmer-1.4.3/ctid_programmer/gui/images/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.3/ctid_programmer/gui/images/ctid-logo.svg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2024-04-17 21:30:05.000000 CTid-programmer-1.4.3/ctid_programmer/gui/main_window.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/main_window_rc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2024-04-17 21:30:05.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_ct.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_linear.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_ntc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_pulse.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_temp.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.3/ctid_programmer/gui/param_volt.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/preferences_dialog.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2024-04-17 21:30:06.000000 CTid-programmer-1.4.3/ctid_programmer/gui/template_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2140 2023-04-27 17:10:07.000000 CTid-programmer-1.4.3/ctid_programmer/preferences.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    35995 2023-07-10 17:58:46.000000 CTid-programmer-1.4.3/ctid_programmer/programmer.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.827902 CTid-programmer-1.4.3/ctid_programmer/qt4/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.3/ctid_programmer/qt4/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.679904 CTid-programmer-1.4.3/ctid_programmer/resources/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2024-04-17 22:11:02.835902 CTid-programmer-1.4.3/ctid_programmer/resources/code/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.3/ctid_programmer/resources/code/ac.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.3/ctid_programmer/resources/code/powered.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    15071 2023-04-27 17:10:08.000000 CTid-programmer-1.4.3/ctid_programmer/sensor_params.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4969 2023-04-27 17:10:07.000000 CTid-programmer-1.4.3/ctid_programmer/sn.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8323 2024-04-17 21:23:52.000000 CTid-programmer-1.4.3/ctid_programmer/sn_egauge.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4075 2023-04-27 17:10:07.000000 CTid-programmer-1.4.3/ctid_programmer/sn_local.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2410 2023-04-27 17:10:07.000000 CTid-programmer-1.4.3/ctid_programmer/template.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2023-04-27 17:09:38.000000 CTid-programmer-1.4.3/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2024-04-17 22:11:02.843901 CTid-programmer-1.4.3/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2024-04-17 21:29:52.000000 CTid-programmer-1.4.3/setup.py
```

### Comparing `CTid-programmer-1.4.2/CTid_programmer.egg-info/PKG-INFO` & `CTid-programmer-1.4.3/CTid_programmer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTid-programmer
-Version: 1.4.2
+Version: 1.4.3
 Summary: A graphical user interface for programming CTid sensors.
 Home-page: https://bitbucket.org/egauge/CTid-programmer/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
```

### Comparing `CTid-programmer-1.4.2/CTid_programmer.egg-info/SOURCES.txt` & `CTid-programmer-1.4.3/CTid_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/LICENSE` & `CTid-programmer-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/PKG-INFO` & `CTid-programmer-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTid-programmer
-Version: 1.4.2
+Version: 1.4.3
 Summary: A graphical user interface for programming CTid sensors.
 Home-page: https://bitbucket.org/egauge/CTid-programmer/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
```

### Comparing `CTid-programmer-1.4.2/README.rst` & `CTid-programmer-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/images/ctid-logo.svg` & `CTid-programmer-1.4.3/ctid_programmer/gui/images/ctid-logo.svg`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/main_window.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/main_window_rc.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/main_window_rc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 5.15.1
+# Created by: The Resource Compiler for Qt version 5.15.2
 # WARNING! All changes made in this file will be lost!
 
 from PySide2 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x05l\
 \x00\
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_ct.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_ct.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_linear.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_linear.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_ntc.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_ntc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'param_ntc.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.1
+## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide2.QtCore import *
 from PySide2.QtGui import *
 from PySide2.QtWidgets import *
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_pulse.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_pulse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'param_pulse.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.1
+## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide2.QtCore import *
 from PySide2.QtGui import *
 from PySide2.QtWidgets import *
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_temp.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_temp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'param_temp.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.1
+## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide2.QtCore import *
 from PySide2.QtGui import *
 from PySide2.QtWidgets import *
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/param_volt.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/param_volt.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/preferences_dialog.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/preferences_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'preferences_dialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.1
+## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide2.QtCore import *
 from PySide2.QtGui import *
 from PySide2.QtWidgets import *
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/gui/template_dialog.py` & `CTid-programmer-1.4.3/ctid_programmer/gui/template_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'template_dialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.1
+## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide2.QtCore import *
 from PySide2.QtGui import *
 from PySide2.QtWidgets import *
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/preferences.py` & `CTid-programmer-1.4.3/ctid_programmer/preferences.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/programmer.py` & `CTid-programmer-1.4.3/ctid_programmer/programmer.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/resources/code/ac.hex` & `CTid-programmer-1.4.3/ctid_programmer/resources/code/ac.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/resources/code/powered.hex` & `CTid-programmer-1.4.3/ctid_programmer/resources/code/powered.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/sensor_params.py` & `CTid-programmer-1.4.3/ctid_programmer/sensor_params.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/sn.py` & `CTid-programmer-1.4.3/ctid_programmer/sn.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/sn_egauge.py` & `CTid-programmer-1.4.3/ctid_programmer/sn_egauge.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 # pylint: disable=no-name-in-module
 #
 """Serial number allocation via the eGauge serial-number API."""
 
+import json
 import logging
 import os
 
 from PySide2.QtWidgets import QMessageBox
 
 from egauge import ctid
 from egauge import webapi
@@ -42,14 +43,16 @@
 from egauge.webapi.cloud.credentials import CredentialsManager, LoginCanceled
 
 from ctid_programmer import sn
 
 log = logging.getLogger(__name__)
 
 
+BAD_STATUS = "Unexpected HTTP status code."
+
 class Manager(sn.Manager):
     def auth_wrapper(self, method, *args, **kwargs):
         while True:
             try:
                 ret = method(*args, *kwargs)
                 self.credentials_manager.previous_login_failed = False
                 return ret
@@ -82,28 +85,42 @@
             "set_product: manufacturer=%s, model=%s", manufacturer, model
         )
 
         mfg = ctid.mfg_short_name(manufacturer)
         if not super().set_product(mfg, model):
             return False
 
+        error = None
         model_list = None
         try:
             model_list = self.sn_api.get_models()
-        except webapi.Error:
-            pass
+        except webapi.Error as e:
+            error = e
 
         if model_list is None:
+            errmsg = ""
+            if isinstance(error, webapi.json_api.JSONAPIError) \
+               and error.args[0] == BAD_STATUS:
+                detail = "."
+                try:
+                    body = json.loads(error.args[2].decode("utf-8"))
+                    err = body.get("detail")
+                    if err is not None:
+                        detail = ": " + err
+                except (UnicodeError, ValueError):
+                    pass
+                status = error.args[1]
+                errmsg = f"\n\nServer returned status {status}{detail}"
             QMessageBox.critical(
                 self.ui,
                 "Serial-number service failed",
                 "Serial-number service failed to return "
                 "model-name list.  "
                 "Reverting to manual "
-                "serial numbers.",
+                "serial numbers." + errmsg,
                 QMessageBox.Ok,
             )
             return False
 
         found = False
         for r in model_list:
             if r["name"] == self.product:
```

### Comparing `CTid-programmer-1.4.2/ctid_programmer/sn_local.py` & `CTid-programmer-1.4.3/ctid_programmer/sn_local.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/ctid_programmer/template.py` & `CTid-programmer-1.4.3/ctid_programmer/template.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.2/setup.py` & `CTid-programmer-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name='CTid-programmer',
-    version='1.4.2',
+    version='1.4.3',
     packages=setuptools.find_packages(),
     package_data={
         '': ['resources/code/*.hex']
     },
     install_requires=['egauge-python>=0.7.3,!=0.21',
                       'importlib_resources', 'wheel'],
     entry_points={
```

