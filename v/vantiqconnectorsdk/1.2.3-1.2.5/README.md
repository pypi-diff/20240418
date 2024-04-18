# Comparing `tmp/vantiqconnectorsdk-1.2.3.tar.gz` & `tmp/vantiqconnectorsdk-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqconnectorsdk-1.2.3.tar", last modified: Mon Mar 25 19:22:27 2024, max compression
+gzip compressed data, was "vantiqconnectorsdk-1.2.5.tar", last modified: Wed Apr 17 23:57:57 2024, max compression
```

## Comparing `vantiqconnectorsdk-1.2.3.tar` & `vantiqconnectorsdk-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-03-25 19:22:27.690070 vantiqconnectorsdk-1.2.3/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.3/LICENSE
--rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-03-25 19:22:27.686509 vantiqconnectorsdk-1.2.3/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)    17913 2023-12-01 23:54:03.000000 vantiqconnectorsdk-1.2.3/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.3/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      714 2024-03-25 19:22:27.693061 vantiqconnectorsdk-1.2.3/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-03-25 19:22:27.662155 vantiqconnectorsdk-1.2.3/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-03-25 19:22:27.662321 vantiqconnectorsdk-1.2.3/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-03-25 19:22:27.678859 vantiqconnectorsdk-1.2.3/src/main/python/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-03-25 19:22:27.685335 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-03-25 19:22:27.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      369 2024-03-25 19:22:27.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-03-25 19:22:27.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       33 2024-03-25 19:22:27.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       19 2024-03-25 19:22:27.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
--rw-r--r--   0 fcarter    (501) staff       (20)    40374 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-17 23:57:57.467112 vantiqconnectorsdk-1.2.5/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.5/LICENSE
+-rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-04-17 23:57:57.465189 vantiqconnectorsdk-1.2.5/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)    17913 2023-12-01 23:54:03.000000 vantiqconnectorsdk-1.2.5/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)       80 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.5/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      714 2024-04-17 23:57:57.468999 vantiqconnectorsdk-1.2.5/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-17 23:57:57.455857 vantiqconnectorsdk-1.2.5/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-17 23:57:57.455973 vantiqconnectorsdk-1.2.5/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-17 23:57:57.460655 vantiqconnectorsdk-1.2.5/src/main/python/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-17 23:57:57.464618 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)    19609 2024-04-17 23:57:57.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      369 2024-04-17 23:57:57.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-04-17 23:57:57.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       33 2024-04-17 23:57:57.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       19 2024-04-17 23:57:57.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/top_level.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)    40374 2022-08-10 20:55:53.000000 vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.py
```

### Comparing `vantiqconnectorsdk-1.2.3/LICENSE` & `vantiqconnectorsdk-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vantiqconnectorsdk-1.2.3/PKG-INFO` & `vantiqconnectorsdk-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.2.3
+Version: 1.2.5
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vantiqconnectorsdk-1.2.3/README.md` & `vantiqconnectorsdk-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vantiqconnectorsdk-1.2.3/setup.cfg` & `vantiqconnectorsdk-1.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vantiqconnectorsdk
-version = 1.2.3
+version = 1.2.5
 description = SDK for building Vantiq extension sources/connectors in Python
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/Vantiq/vantiq-extension-sources
 author = Vantiq, Inc
 author_email = fcarter@vantiq.com
 license = MIT
```

### Comparing `vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO` & `vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqconnectorsdk
-Version: 1.2.3
+Version: 1.2.5
 Summary: SDK for building Vantiq extension sources/connectors in Python
 Home-page: https://github.com/Vantiq/vantiq-extension-sources
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vantiqconnectorsdk-1.2.3/src/main/python/vantiqconnectorsdk.py` & `vantiqconnectorsdk-1.2.5/src/main/python/vantiqconnectorsdk.py`

 * *Files identical despite different names*

