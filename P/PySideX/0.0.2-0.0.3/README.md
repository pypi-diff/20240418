# Comparing `tmp/PySideX-0.0.2.tar.gz` & `tmp/PySideX-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.2.tar", last modified: Tue Apr 16 18:56:59 2024, max compression
+gzip compressed data, was "PySideX-0.0.3.tar", last modified: Thu Apr 18 05:21:43 2024, max compression
```

## Comparing `PySideX-0.0.2.tar` & `PySideX-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.460606 PySideX-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-16 18:56:59.459567 PySideX-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.451557 PySideX-0.0.2/PySideX/
--rw-rw-rw-   0        0        0      365 2024-04-16 18:49:37.000000 PySideX-0.0.2/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.458559 PySideX-0.0.2/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2024-04-06 01:07:23.000000 PySideX-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 18:56:59.460606 PySideX-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-04-16 18:52:45.000000 PySideX-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.546714 PySideX-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1791 2024-04-18 05:21:43.545715 PySideX-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.520711 PySideX-0.0.3/PySideX/
+-rw-rw-rw-   0        0        0      371 2024-04-18 02:39:02.000000 PySideX-0.0.3/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:21:43.544712 PySideX-0.0.3/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     1791 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-18 05:21:43.000000 PySideX-0.0.3/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 05:21:42.000000 PySideX-0.0.3/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      288 2024-04-06 01:07:23.000000 PySideX-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:21:43.546714 PySideX-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      666 2024-04-18 05:21:12.000000 PySideX-0.0.3/setup.py
```

### Comparing `PySideX-0.0.2/LICENSE` & `PySideX-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.2/PKG-INFO` & `PySideX-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.2/PySideX.egg-info/PKG-INFO` & `PySideX-0.0.3/PySideX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.2/setup.py` & `PySideX-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("PySideX/README.md", "r") as arq:
         readme = arq.read()
 
 with open("PySideX/LICENSE", "r") as arq:
         licence = arq.read()
 
 setup(name='PySideX',
-    version='0.0.2',
+    version='0.0.3',
     license=licence,
     author='Ryan Souza Anselmo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='ryansouza.cwb@email.com',
     keywords='pysidex',
     description=u'Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology',
```

