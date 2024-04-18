# Comparing `tmp/CureQ-0.1.3.tar.gz` & `tmp/CureQ-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CureQ-0.1.3.tar", last modified: Thu Apr  4 13:48:41 2024, max compression
+gzip compressed data, was "CureQ-0.1.4.tar", last modified: Thu Apr 18 14:36:06 2024, max compression
```

## Comparing `CureQ-0.1.3.tar` & `CureQ-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 13:48:41.738768 CureQ-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-04 13:48:41.707014 CureQ-0.1.3/CureQ/
--rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.3/CureQ/__init__.py
--rw-rw-rw-   0        0        0    63693 2024-04-04 11:36:48.000000 CureQ-0.1.3/CureQ/mea.py
--rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.3/CureQ/mea_02_04.py
-drwxrwxrwx   0        0        0        0 2024-04-04 13:48:41.738768 CureQ-0.1.3/CureQ.egg-info/
--rw-rw-rw-   0        0        0     3343 2024-04-04 13:48:40.000000 CureQ-0.1.3/CureQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-04 13:48:41.000000 CureQ-0.1.3/CureQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 13:48:40.000000 CureQ-0.1.3/CureQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-04 13:48:40.000000 CureQ-0.1.3/CureQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 13:48:40.000000 CureQ-0.1.3/CureQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3343 2024-04-04 13:48:41.738768 CureQ-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2574 2024-04-04 13:18:54.000000 CureQ-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 13:48:41.738768 CureQ-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1636 2024-04-04 13:48:23.000000 CureQ-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:36:06.109994 CureQ-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-18 14:36:06.070978 CureQ-0.1.4/CureQ/
+-rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.4/CureQ/__init__.py
+-rw-rw-rw-   0        0        0    81461 2024-04-18 14:33:54.000000 CureQ-0.1.4/CureQ/mea.py
+-rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.4/CureQ/mea_02_04.py
+-rw-rw-rw-   0        0        0    81461 2024-04-18 13:54:31.000000 CureQ-0.1.4/CureQ/mea_18_04_2024.py
+-rw-rw-rw-   0        0        0    63693 2024-04-09 11:23:24.000000 CureQ-0.1.4/CureQ/mea_for_py_files.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:36:06.105804 CureQ-0.1.4/CureQ.egg-info/
+-rw-rw-rw-   0        0        0     3343 2024-04-18 14:36:05.000000 CureQ-0.1.4/CureQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-18 14:36:05.000000 CureQ-0.1.4/CureQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:36:05.000000 CureQ-0.1.4/CureQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-18 14:36:05.000000 CureQ-0.1.4/CureQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 14:36:05.000000 CureQ-0.1.4/CureQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3343 2024-04-18 14:36:06.107802 CureQ-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2574 2024-04-04 13:18:54.000000 CureQ-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:36:06.109994 CureQ-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1636 2024-04-08 11:40:44.000000 CureQ-0.1.4/setup.py
```

### Comparing `CureQ-0.1.3/CureQ/mea.py` & `CureQ-0.1.4/CureQ/mea_for_py_files.py`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.3/CureQ/mea_02_04.py` & `CureQ-0.1.4/CureQ/mea_02_04.py`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.3/CureQ.egg-info/PKG-INFO` & `CureQ-0.1.4/CureQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CureQ-0.1.3/LICENSE` & `CureQ-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.3/PKG-INFO` & `CureQ-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CureQ-0.1.3/README.md` & `CureQ-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.3/setup.py` & `CureQ-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Use the text in the README file for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setup metadata for initializing the library
 setuptools.setup(
     name="CureQ",
-    version="0.1.3",
+    version="0.1.4",
     author="CureQ",
     author_email="cureq-ft@hva.nl",
     description="Library for analyzing MEA files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CureQ/CureQ.git",
     packages=setuptools.find_packages(),
```

