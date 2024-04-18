# Comparing `tmp/emodeconnection-1.0.4.tar.gz` & `tmp/emodeconnection-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emodeconnection-1.0.4.tar", last modified: Tue Nov 21 22:25:19 2023, max compression
+gzip compressed data, was "emodeconnection-1.0.5.tar", last modified: Wed Apr 17 20:14:31 2024, max compression
```

## Comparing `emodeconnection-1.0.4.tar` & `emodeconnection-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 22:25:19.530398 emodeconnection-1.0.4/
--rw-rw-rw-   0        0        0     1471 2022-06-25 20:28:32.000000 emodeconnection-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      874 2023-11-21 22:25:19.530398 emodeconnection-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      361 2022-01-13 13:08:02.000000 emodeconnection-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-21 22:25:19.514739 emodeconnection-1.0.4/emodeconnection/
--rw-rw-rw-   0        0        0       61 2021-04-28 11:51:42.000000 emodeconnection-1.0.4/emodeconnection/__init__.py
--rw-rw-rw-   0        0        0     9008 2023-11-21 21:40:02.000000 emodeconnection-1.0.4/emodeconnection/emodeconnection.py
-drwxrwxrwx   0        0        0        0 2023-11-21 22:25:19.530398 emodeconnection-1.0.4/emodeconnection.egg-info/
--rw-rw-rw-   0        0        0      874 2023-11-21 22:25:19.000000 emodeconnection-1.0.4/emodeconnection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-11-21 22:25:19.000000 emodeconnection-1.0.4/emodeconnection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 22:25:19.000000 emodeconnection-1.0.4/emodeconnection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-11-21 22:25:19.000000 emodeconnection-1.0.4/emodeconnection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-21 22:25:19.000000 emodeconnection-1.0.4/emodeconnection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-21 22:25:19.530398 emodeconnection-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-11-21 22:24:30.000000 emodeconnection-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:14:31.369319 emodeconnection-1.0.5/
+-rw-rw-rw-   0        0        0     1471 2022-06-25 20:28:32.000000 emodeconnection-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      874 2024-04-17 20:14:31.369319 emodeconnection-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2022-01-13 13:08:02.000000 emodeconnection-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 20:14:31.353654 emodeconnection-1.0.5/emodeconnection/
+-rw-rw-rw-   0        0        0       61 2021-04-28 11:51:42.000000 emodeconnection-1.0.5/emodeconnection/__init__.py
+-rw-rw-rw-   0        0        0    12855 2024-04-17 16:25:58.000000 emodeconnection-1.0.5/emodeconnection/emodeconnection.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:14:31.369319 emodeconnection-1.0.5/emodeconnection.egg-info/
+-rw-rw-rw-   0        0        0      874 2024-04-17 20:14:31.000000 emodeconnection-1.0.5/emodeconnection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-17 20:14:31.000000 emodeconnection-1.0.5/emodeconnection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:14:31.000000 emodeconnection-1.0.5/emodeconnection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 20:14:31.000000 emodeconnection-1.0.5/emodeconnection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 20:14:31.000000 emodeconnection-1.0.5/emodeconnection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:14:31.369319 emodeconnection-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-17 20:13:57.000000 emodeconnection-1.0.5/setup.py
```

### Comparing `emodeconnection-1.0.4/LICENSE` & `emodeconnection-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emodeconnection-1.0.4/PKG-INFO` & `emodeconnection-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emodeconnection
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python connection for EMode
 Home-page: https://github.com/emode-photonix/emodeconnection
 Author: EMode Photonix LLC
 Author-email: hello@emodephotonix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `emodeconnection-1.0.4/emodeconnection.egg-info/PKG-INFO` & `emodeconnection-1.0.5/emodeconnection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emodeconnection
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python connection for EMode
 Home-page: https://github.com/emode-photonix/emodeconnection
 Author: EMode Photonix LLC
 Author-email: hello@emodephotonix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `emodeconnection-1.0.4/setup.py` & `emodeconnection-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="emodeconnection",
-    version="1.0.4",
+    version="1.0.5",
     author="EMode Photonix LLC",
     author_email="hello@emodephotonix.com",
     description="Python connection for EMode",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/emode-photonix/emodeconnection",
     packages=setuptools.find_packages(),
```

