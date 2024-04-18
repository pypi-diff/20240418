# Comparing `tmp/PySideX-0.0.3.tar.gz` & `tmp/PySideX-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.3.tar", last modified: Thu Apr 18 05:21:43 2024, max compression
+gzip compressed data, was "PySideX-0.0.4.tar", last modified: Thu Apr 18 05:28:47 2024, max compression
```

## Comparing `PySideX-0.0.3.tar` & `PySideX-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.546714 PySideX-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-18 05:21:43.545715 PySideX-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.520711 PySideX-0.0.3/PySideX/
--rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.3/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.544712 PySideX-0.0.3/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-18 05:21:43.000000 PySideX-0.0.3/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2024-04-06 01:07:23.000000 PySideX-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 05:21:43.546714 PySideX-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-04-18 05:21:12.000000 PySideX-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:28:47.073989 PySideX-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1791 2024-04-18 05:28:47.073989 PySideX-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 05:28:47.065113 PySideX-0.0.4/PySideX/
+-rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.4/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:28:47.071978 PySideX-0.0.4/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     1791 2024-04-18 05:28:47.000000 PySideX-0.0.4/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-18 05:28:47.000000 PySideX-0.0.4/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:28:47.000000 PySideX-0.0.4/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 05:28:47.000000 PySideX-0.0.4/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 05:28:47.000000 PySideX-0.0.4/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:28:47.074997 PySideX-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-04-18 05:28:26.000000 PySideX-0.0.4/setup.py
```

### Comparing `PySideX-0.0.3/LICENSE` & `PySideX-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.3/PKG-INFO` & `PySideX-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.3/PySideX.egg-info/PKG-INFO` & `PySideX-0.0.4/PySideX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.3/setup.py` & `PySideX-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup
 
-with open("PySideX/README.md", "r") as arq:
-        readme = arq.read()
+with open("README.md", "r") as arq:
+    readme = arq.read()
 
-with open("PySideX/LICENSE", "r") as arq:
-        licence = arq.read()
+with open("LICENSE", "r") as arq:
+    licence = arq.read()
 
-setup(name='PySideX',
-    version='0.0.3',
+setup(
+    name="PySideX",
+    version="0.0.4",
     license=licence,
-    author='Ryan Souza Anselmo',
+    author="Ryan Souza Anselmo",
     long_description=readme,
     long_description_content_type="text/markdown",
-    author_email='ryansouza.cwb@email.com',
-    keywords='pysidex',
-    description=u'Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology',
-    packages=['PySideX'],
-    install_requires=['PySide6'],)
+    author_email="ryansouza.cwb@email.com",
+    keywords="pysidex",
+    description="Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology",
+    packages=["PySideX"],
+    install_requires=["PySide6"],
+)
```

