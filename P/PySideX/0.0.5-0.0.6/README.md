# Comparing `tmp/PySideX-0.0.5.tar.gz` & `tmp/PySideX-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.5.tar", last modified: Thu Apr 18 05:38:05 2024, max compression
+gzip compressed data, was "PySideX-0.0.6.tar", last modified: Thu Apr 18 06:03:29 2024, max compression
```

## Comparing `PySideX-0.0.5.tar` & `PySideX-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:38:05.639861 PySideX-0.0.5/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-18 05:38:05.621338 PySideX-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 05:38:05.604108 PySideX-0.0.5/PySideX/
--rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.5/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:38:05.620072 PySideX-0.0.5/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-18 05:38:05.000000 PySideX-0.0.5/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-18 05:38:05.000000 PySideX-0.0.5/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:38:05.000000 PySideX-0.0.5/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 05:38:05.000000 PySideX-0.0.5/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 05:38:05.000000 PySideX-0.0.5/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 05:38:05.639861 PySideX-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-04-18 05:33:48.000000 PySideX-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.730082 PySideX-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1791 2024-04-18 06:03:29.730082 PySideX-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.693612 PySideX-0.0.6/PySideX/
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.713682 PySideX-0.0.6/PySideX/Assets/
+-rw-rw-rw-   0        0        0      308 2024-04-08 00:19:30.000000 PySideX-0.0.6/PySideX/Assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.715857 PySideX-0.0.6/PySideX/Components/
+-rw-rw-rw-   0        0        0       28 2024-04-18 02:38:56.000000 PySideX-0.0.6/PySideX/Components/__init__.py
+-rw-rw-rw-   0        0        0     1125 2024-04-18 02:47:34.000000 PySideX-0.0.6/PySideX/Components/box.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.728931 PySideX-0.0.6/PySideX/Widgets/
+-rw-rw-rw-   0        0        0      352 2024-04-10 05:33:42.000000 PySideX-0.0.6/PySideX/Widgets/__init__.py
+-rw-rw-rw-   0        0        0     1319 2024-04-08 15:21:11.000000 PySideX-0.0.6/PySideX/Widgets/button.py
+-rw-rw-rw-   0        0        0     1162 2024-04-18 02:48:36.000000 PySideX-0.0.6/PySideX/Widgets/dropdawn.py
+-rw-rw-rw-   0        0        0      871 2024-04-08 15:12:02.000000 PySideX-0.0.6/PySideX/Widgets/frame.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:05.000000 PySideX-0.0.6/PySideX/Widgets/horizontalBoxLayout.py
+-rw-rw-rw-   0        0        0      728 2024-04-08 16:26:56.000000 PySideX-0.0.6/PySideX/Widgets/image.py
+-rw-rw-rw-   0        0        0     1286 2024-04-18 02:50:33.000000 PySideX-0.0.6/PySideX/Widgets/input.py
+-rw-rw-rw-   0        0        0     1561 2024-04-10 03:02:16.000000 PySideX-0.0.6/PySideX/Widgets/label.py
+-rw-rw-rw-   0        0        0     2570 2024-04-10 05:32:57.000000 PySideX-0.0.6/PySideX/Widgets/messagebox.py
+-rw-rw-rw-   0        0        0      602 2024-04-08 14:52:08.000000 PySideX-0.0.6/PySideX/Widgets/spacerItem.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:01.000000 PySideX-0.0.6/PySideX/Widgets/verticalBoxLayout.py
+-rw-rw-rw-   0        0        0      956 2024-04-06 15:53:16.000000 PySideX-0.0.6/PySideX/Widgets/window.py
+-rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.6/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:03:29.712660 PySideX-0.0.6/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     1791 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 06:03:29.000000 PySideX-0.0.6/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:03:29.731108 PySideX-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-04-18 06:03:06.000000 PySideX-0.0.6/setup.py
```

### Comparing `PySideX-0.0.5/LICENSE` & `PySideX-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.5/PKG-INFO` & `PySideX-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.5/PySideX.egg-info/PKG-INFO` & `PySideX-0.0.6/PySideX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.5/setup.py` & `PySideX-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 with open("LICENSE", "r") as arq:
     licence = arq.read()
 
 setup(
     name="PySideX",
-    version="0.0.5",
+    version="0.0.6",
     license=licence,
     author="Ryan Souza Anselmo",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="ryansouza.cwb@email.com",
     keywords="pysidex",
     description="Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology",
-    packages=["PySideX"],
+    packages=find_packages(),
     install_requires=["PySide6"],
 )
```

