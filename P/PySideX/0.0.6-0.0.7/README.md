# Comparing `tmp/PySideX-0.0.6.tar.gz` & `tmp/PySideX-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.6.tar", last modified: Thu Apr 18 06:03:29 2024, max compression
+gzip compressed data, was "PySideX-0.0.7.tar", last modified: Thu Apr 18 15:58:06 2024, max compression
```

## Comparing `PySideX-0.0.6.tar` & `PySideX-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.730082 PySideX-0.0.6/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-18 06:03:29.730082 PySideX-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.693612 PySideX-0.0.6/PySideX/
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.713682 PySideX-0.0.6/PySideX/Assets/
--rw-rw-rw-   0        0        0      308 2024-04-08 00:19:30.000000 PySideX-0.0.6/PySideX/Assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.715857 PySideX-0.0.6/PySideX/Components/
--rw-rw-rw-   0        0        0       28 2024-04-18 02:38:56.000000 PySideX-0.0.6/PySideX/Components/__init__.py
--rw-rw-rw-   0        0        0     1125 2024-04-18 02:47:34.000000 PySideX-0.0.6/PySideX/Components/box.py
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.728931 PySideX-0.0.6/PySideX/Widgets/
--rw-rw-rw-   0        0        0      352 2024-04-10 05:33:42.000000 PySideX-0.0.6/PySideX/Widgets/__init__.py
--rw-rw-rw-   0        0        0     1319 2024-04-08 15:21:11.000000 PySideX-0.0.6/PySideX/Widgets/button.py
--rw-rw-rw-   0        0        0     1162 2024-04-18 02:48:36.000000 PySideX-0.0.6/PySideX/Widgets/dropdawn.py
--rw-rw-rw-   0        0        0      871 2024-04-08 15:12:02.000000 PySideX-0.0.6/PySideX/Widgets/frame.py
--rw-rw-rw-   0        0        0      300 2024-04-08 15:08:05.000000 PySideX-0.0.6/PySideX/Widgets/horizontalBoxLayout.py
--rw-rw-rw-   0        0        0      728 2024-04-08 16:26:56.000000 PySideX-0.0.6/PySideX/Widgets/image.py
--rw-rw-rw-   0        0        0     1286 2024-04-18 02:50:33.000000 PySideX-0.0.6/PySideX/Widgets/input.py
--rw-rw-rw-   0        0        0     1561 2024-04-10 03:02:16.000000 PySideX-0.0.6/PySideX/Widgets/label.py
--rw-rw-rw-   0        0        0     2570 2024-04-10 05:32:57.000000 PySideX-0.0.6/PySideX/Widgets/messagebox.py
--rw-rw-rw-   0        0        0      602 2024-04-08 14:52:08.000000 PySideX-0.0.6/PySideX/Widgets/spacerItem.py
--rw-rw-rw-   0        0        0      300 2024-04-08 15:08:01.000000 PySideX-0.0.6/PySideX/Widgets/verticalBoxLayout.py
--rw-rw-rw-   0        0        0      956 2024-04-06 15:53:16.000000 PySideX-0.0.6/PySideX/Widgets/window.py
--rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.6/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.712660 PySideX-0.0.6/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 06:03:29.731108 PySideX-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      670 2024-04-18 06:03:06.000000 PySideX-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.795407 PySideX-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1791 2024-04-18 15:58:06.795407 PySideX-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.755902 PySideX-0.0.7/PySideX/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.778750 PySideX-0.0.7/PySideX/Assets/
+-rw-rw-rw-   0        0        0      308 2024-04-08 00:19:30.000000 PySideX-0.0.7/PySideX/Assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.780782 PySideX-0.0.7/PySideX/Components/
+-rw-rw-rw-   0        0        0       28 2024-04-18 15:52:34.000000 PySideX-0.0.7/PySideX/Components/__init__.py
+-rw-rw-rw-   0        0        0     1125 2024-04-18 02:47:34.000000 PySideX-0.0.7/PySideX/Components/box.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.793397 PySideX-0.0.7/PySideX/Widgets/
+-rw-rw-rw-   0        0        0      384 2024-04-18 15:52:15.000000 PySideX-0.0.7/PySideX/Widgets/__init__.py
+-rw-rw-rw-   0        0        0     1319 2024-04-08 15:21:11.000000 PySideX-0.0.7/PySideX/Widgets/button.py
+-rw-rw-rw-   0        0        0     1162 2024-04-18 02:48:36.000000 PySideX-0.0.7/PySideX/Widgets/dropdawn.py
+-rw-rw-rw-   0        0        0      871 2024-04-08 15:12:02.000000 PySideX-0.0.7/PySideX/Widgets/frame.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:05.000000 PySideX-0.0.7/PySideX/Widgets/horizontalBoxLayout.py
+-rw-rw-rw-   0        0        0      728 2024-04-08 16:26:56.000000 PySideX-0.0.7/PySideX/Widgets/image.py
+-rw-rw-rw-   0        0        0     1286 2024-04-18 02:50:33.000000 PySideX-0.0.7/PySideX/Widgets/input.py
+-rw-rw-rw-   0        0        0     1561 2024-04-10 03:02:16.000000 PySideX-0.0.7/PySideX/Widgets/label.py
+-rw-rw-rw-   0        0        0     2570 2024-04-10 05:32:57.000000 PySideX-0.0.7/PySideX/Widgets/messagebox.py
+-rw-rw-rw-   0        0        0      602 2024-04-08 14:52:08.000000 PySideX-0.0.7/PySideX/Widgets/spacerItem.py
+-rw-rw-rw-   0        0        0     1298 2024-04-18 15:53:07.000000 PySideX-0.0.7/PySideX/Widgets/textArea.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:01.000000 PySideX-0.0.7/PySideX/Widgets/verticalBoxLayout.py
+-rw-rw-rw-   0        0        0      956 2024-04-06 15:53:16.000000 PySideX-0.0.7/PySideX/Widgets/window.py
+-rw-rw-rw-   0        0        0      386 2024-04-18 15:52:46.000000 PySideX-0.0.7/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:58:06.777745 PySideX-0.0.7/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     1791 2024-04-18 15:58:06.000000 PySideX-0.0.7/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-04-18 15:58:06.000000 PySideX-0.0.7/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:58:06.000000 PySideX-0.0.7/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 15:58:06.000000 PySideX-0.0.7/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 15:58:06.000000 PySideX-0.0.7/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:58:06.795407 PySideX-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-04-18 15:57:43.000000 PySideX-0.0.7/setup.py
```

### Comparing `PySideX-0.0.6/LICENSE` & `PySideX-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PKG-INFO` & `PySideX-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.6/PySideX/Components/box.py` & `PySideX-0.0.7/PySideX/Components/box.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/button.py` & `PySideX-0.0.7/PySideX/Widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/dropdawn.py` & `PySideX-0.0.7/PySideX/Widgets/dropdawn.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/frame.py` & `PySideX-0.0.7/PySideX/Widgets/frame.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/image.py` & `PySideX-0.0.7/PySideX/Widgets/image.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/input.py` & `PySideX-0.0.7/PySideX/Widgets/input.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/label.py` & `PySideX-0.0.7/PySideX/Widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/messagebox.py` & `PySideX-0.0.7/PySideX/Widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/spacerItem.py` & `PySideX-0.0.7/PySideX/Widgets/spacerItem.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX/Widgets/window.py` & `PySideX-0.0.7/PySideX/Widgets/window.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.6/PySideX.egg-info/PKG-INFO` & `PySideX-0.0.7/PySideX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.6/PySideX.egg-info/SOURCES.txt` & `PySideX-0.0.7/PySideX.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 PySideX/Widgets/frame.py
 PySideX/Widgets/horizontalBoxLayout.py
 PySideX/Widgets/image.py
 PySideX/Widgets/input.py
 PySideX/Widgets/label.py
 PySideX/Widgets/messagebox.py
 PySideX/Widgets/spacerItem.py
+PySideX/Widgets/textArea.py
 PySideX/Widgets/verticalBoxLayout.py
 PySideX/Widgets/window.py
```

### Comparing `PySideX-0.0.6/setup.py` & `PySideX-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = arq.read()
 
 with open("LICENSE", "r") as arq:
     licence = arq.read()
 
 setup(
     name="PySideX",
-    version="0.0.6",
+    version="0.0.7",
     license=licence,
     author="Ryan Souza Anselmo",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="ryansouza.cwb@email.com",
     keywords="pysidex",
     description="Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology",
```

