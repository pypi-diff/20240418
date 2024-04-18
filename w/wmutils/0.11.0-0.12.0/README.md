# Comparing `tmp/wmutils-0.11.0.tar.gz` & `tmp/wmutils-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmutils-0.11.0.tar", last modified: Fri Mar  8 09:40:02 2024, max compression
+gzip compressed data, was "wmutils-0.12.0.tar", last modified: Thu Apr 18 15:31:47 2024, max compression
```

## Comparing `wmutils-0.11.0.tar` & `wmutils-0.12.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.148335 wmutils-0.11.0/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2024-01-27 10:48:31.000000 wmutils-0.11.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1893 2024-03-08 09:40:02.147947 wmutils-0.11.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      101 2024-03-08 09:36:13.000000 wmutils-0.11.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)      748 2024-03-08 09:36:13.000000 wmutils-0.11.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-03-08 09:40:02.148416 wmutils-0.11.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      540 2024-03-08 09:36:13.000000 wmutils-0.11.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.135487 wmutils-0.11.0/test/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-04 13:32:18.000000 wmutils-0.11.0/test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.136788 wmutils-0.11.0/test/collections/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-04 13:32:08.000000 wmutils-0.11.0/test/collections/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5153 2024-02-20 15:54:26.000000 wmutils-0.11.0/test/collections/test_dict_access.py
--rwxrwxrwx   0 root         (0) root         (0)     6964 2024-02-20 15:54:31.000000 wmutils-0.11.0/test/collections/test_safe_dict.py
--rwxrwxrwx   0 root         (0) root         (0)     4469 2024-02-20 15:54:20.000000 wmutils-0.11.0/test/test_multithreading.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.139999 wmutils-0.11.0/wmutils/
--rwxrwxrwx   0 root         (0) root         (0)       19 2024-03-08 09:35:37.000000 wmutils-0.11.0/wmutils/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.143447 wmutils-0.11.0/wmutils/collections/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-04 12:26:43.000000 wmutils-0.11.0/wmutils/collections/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5204 2024-02-16 13:56:01.000000 wmutils-0.11.0/wmutils/collections/dict_access.py
--rwxrwxrwx   0 root         (0) root         (0)      847 2024-02-05 15:28:47.000000 wmutils-0.11.0/wmutils/collections/list_access.py
--rwxrwxrwx   0 root         (0) root         (0)     4321 2024-02-04 13:34:38.000000 wmutils-0.11.0/wmutils/collections/safe_dict.py
--rwxrwxrwx   0 root         (0) root         (0)     1865 2024-02-05 15:33:11.000000 wmutils-0.11.0/wmutils/file.py
--rwxrwxrwx   0 root         (0) root         (0)      892 2024-02-05 15:32:46.000000 wmutils-0.11.0/wmutils/general.py
--rwxrwxrwx   0 root         (0) root         (0)     3903 2024-02-16 14:04:36.000000 wmutils-0.11.0/wmutils/iterators.py
--rwxrwxrwx   0 root         (0) root         (0)      177 2024-02-05 15:33:08.000000 wmutils-0.11.0/wmutils/json.py
--rwxrwxrwx   0 root         (0) root         (0)     7417 2024-02-04 11:53:32.000000 wmutils-0.11.0/wmutils/multithreading.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.144978 wmutils-0.11.0/wmutils/pandas/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-06 09:20:37.000000 wmutils-0.11.0/wmutils/pandas/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      890 2024-02-06 09:10:38.000000 wmutils-0.11.0/wmutils/pandas/dataframe.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.147036 wmutils-0.11.0/wmutils/pandas/figures/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-06 09:01:06.000000 wmutils-0.11.0/wmutils/pandas/figures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      746 2024-02-06 09:03:07.000000 wmutils-0.11.0/wmutils/pandas/figures/base.py
--rwxrwxrwx   0 root         (0) root         (0)     5607 2024-02-20 15:54:32.000000 wmutils-0.11.0/wmutils/pandas/figures/plots.py
--rwxrwxrwx   0 root         (0) root         (0)     3782 2024-02-20 15:54:33.000000 wmutils-0.11.0/wmutils/pandas/figures/pretty_plots.py
--rwxrwxrwx   0 root         (0) root         (0)     1109 2024-03-08 09:28:22.000000 wmutils-0.11.0/wmutils/pandas/transforms.py
--rwxrwxrwx   0 root         (0) root         (0)      629 2024-02-05 15:30:38.000000 wmutils-0.11.0/wmutils/regex.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:40:02.147494 wmutils-0.11.0/wmutils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1893 2024-03-08 09:40:02.000000 wmutils-0.11.0/wmutils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      802 2024-03-08 09:40:02.000000 wmutils-0.11.0/wmutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-03-08 09:40:02.000000 wmutils-0.11.0/wmutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-03-08 09:40:02.000000 wmutils-0.11.0/wmutils.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:47.217244 wmutils-0.12.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1070 2024-04-18 15:27:26.000000 wmutils-0.12.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1893 2024-04-18 15:31:47.208716 wmutils-0.12.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2024-04-18 15:31:34.000000 wmutils-0.12.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      748 2024-04-18 15:31:34.000000 wmutils-0.12.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-04-18 15:31:47.218330 wmutils-0.12.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      540 2024-04-18 15:31:34.000000 wmutils-0.12.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:46.680426 wmutils-0.12.0/test/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:26:52.000000 wmutils-0.12.0/test/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:46.739786 wmutils-0.12.0/test/collections/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:26:52.000000 wmutils-0.12.0/test/collections/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5153 2024-04-18 15:27:26.000000 wmutils-0.12.0/test/collections/test_dict_access.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6964 2024-04-18 15:27:26.000000 wmutils-0.12.0/test/collections/test_safe_dict.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4469 2024-04-18 15:27:26.000000 wmutils-0.12.0/test/test_multithreading.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:46.861257 wmutils-0.12.0/wmutils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2024-04-18 15:31:34.000000 wmutils-0.12.0/wmutils/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:47.014364 wmutils-0.12.0/wmutils/collections/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:26:52.000000 wmutils-0.12.0/wmutils/collections/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5204 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/collections/dict_access.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      847 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/collections/list_access.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4321 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/collections/safe_dict.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1865 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/file.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      892 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/general.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3903 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/iterators.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/json.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7417 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/multithreading.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:47.074972 wmutils-0.12.0/wmutils/pandas/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:26:52.000000 wmutils-0.12.0/wmutils/pandas/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      890 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/pandas/dataframe.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:47.172788 wmutils-0.12.0/wmutils/pandas/figures/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:26:52.000000 wmutils-0.12.0/wmutils/pandas/figures/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      746 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/pandas/figures/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5607 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/pandas/figures/plots.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3782 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/pandas/figures/pretty_plots.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1109 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/pandas/transforms.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      629 2024-04-18 15:27:26.000000 wmutils-0.12.0/wmutils/regex.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-18 15:31:47.197569 wmutils-0.12.0/wmutils.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1893 2024-04-18 15:31:46.000000 wmutils-0.12.0/wmutils.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2024-04-18 15:31:46.000000 wmutils-0.12.0/wmutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-18 15:31:46.000000 wmutils-0.12.0/wmutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2024-04-18 15:31:46.000000 wmutils-0.12.0/wmutils.egg-info/top_level.txt
```

### Comparing `wmutils-0.11.0/LICENSE` & `wmutils-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/PKG-INFO` & `wmutils-0.12.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmutils
-Version: 0.11.0
+Version: 0.12.0
 Summary: Contains a diverse set of utility methods I use in Python.
 Home-page: https://github.com/wmeijer221/my_python_utils
 Author: Willem Meijer
 Author-email: wmeijer221 <me@wmeijer.com>
 License: MIT License
         
         Copyright (c) 2024 Willem Meijer
@@ -34,8 +34,8 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # my_python_utils
 Contains a diverse set of utility methods I use in Python.
 
-Latest version: 0.11.0
+Latest version: 0.12.0
```

### Comparing `wmutils-0.11.0/pyproject.toml` & `wmutils-0.12.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "wmutils"
-version = "0.11.0"
+version = "0.12.0"
 description = "Contains a diverse set of utility methods I use in Python."
 readme = 'README.md'
 license = { file = 'LICENSE' }
 authors = [{ email = "me@wmeijer.com", name = "wmeijer221" }]
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `wmutils-0.11.0/setup.py` & `wmutils-0.12.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.11.0"
+version = "0.12.0"
 
 setup(
     name="wmutils",
     version=version,
     author="Willem Meijer",
     author_email="me@wmeijer.com",
     description="Contains a diverse set of utility methods I use in Python.",
```

### Comparing `wmutils-0.11.0/test/collections/test_dict_access.py` & `wmutils-0.12.0/test/collections/test_dict_access.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/test/collections/test_safe_dict.py` & `wmutils-0.12.0/test/collections/test_safe_dict.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/test/test_multithreading.py` & `wmutils-0.12.0/test/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/collections/dict_access.py` & `wmutils-0.12.0/wmutils/collections/dict_access.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/collections/list_access.py` & `wmutils-0.12.0/wmutils/collections/list_access.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/collections/safe_dict.py` & `wmutils-0.12.0/wmutils/collections/safe_dict.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/file.py` & `wmutils-0.12.0/wmutils/file.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/general.py` & `wmutils-0.12.0/wmutils/general.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/iterators.py` & `wmutils-0.12.0/wmutils/iterators.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/multithreading.py` & `wmutils-0.12.0/wmutils/multithreading.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/pandas/dataframe.py` & `wmutils-0.12.0/wmutils/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/pandas/figures/base.py` & `wmutils-0.12.0/wmutils/pandas/figures/base.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/pandas/figures/plots.py` & `wmutils-0.12.0/wmutils/pandas/figures/plots.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/pandas/figures/pretty_plots.py` & `wmutils-0.12.0/wmutils/pandas/figures/pretty_plots.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/pandas/transforms.py` & `wmutils-0.12.0/wmutils/pandas/transforms.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils/regex.py` & `wmutils-0.12.0/wmutils/regex.py`

 * *Files identical despite different names*

### Comparing `wmutils-0.11.0/wmutils.egg-info/PKG-INFO` & `wmutils-0.12.0/wmutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmutils
-Version: 0.11.0
+Version: 0.12.0
 Summary: Contains a diverse set of utility methods I use in Python.
 Home-page: https://github.com/wmeijer221/my_python_utils
 Author: Willem Meijer
 Author-email: wmeijer221 <me@wmeijer.com>
 License: MIT License
         
         Copyright (c) 2024 Willem Meijer
@@ -34,8 +34,8 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # my_python_utils
 Contains a diverse set of utility methods I use in Python.
 
-Latest version: 0.11.0
+Latest version: 0.12.0
```

### Comparing `wmutils-0.11.0/wmutils.egg-info/SOURCES.txt` & `wmutils-0.12.0/wmutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

