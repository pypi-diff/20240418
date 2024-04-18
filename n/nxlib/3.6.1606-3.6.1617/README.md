# Comparing `tmp/nxlib-3.6.1606.tar.gz` & `tmp/nxlib-3.6.1617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxlib-3.6.1606.tar", last modified: Fri Feb  2 10:36:03 2024, max compression
+gzip compressed data, was "nxlib-3.6.1617.tar", last modified: Tue Mar 19 11:29:37 2024, max compression
```

## Comparing `nxlib-3.6.1606.tar` & `nxlib-3.6.1617.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-02-02 10:36:03.377621 nxlib-3.6.1606/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1060 2023-12-15 14:52:39.000000 nxlib-3.6.1606/LICENSE.md.in
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2024-02-02 10:36:03.377621 nxlib-3.6.1606/PKG-INFO
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      898 2023-12-15 14:52:39.000000 nxlib-3.6.1606/README.md
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-02-02 10:36:03.373621 nxlib-3.6.1606/ensenso_nxlib/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      288 2023-12-15 14:52:39.000000 nxlib-3.6.1606/ensenso_nxlib/__init__.py
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-02-02 10:36:03.373621 nxlib-3.6.1606/nxlib/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      349 2023-12-15 14:52:39.000000 nxlib-3.6.1606/nxlib/__init__.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3173 2023-12-15 14:52:39.000000 nxlib-3.6.1606/nxlib/_helper.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22444 2024-01-16 14:36:14.000000 nxlib-3.6.1606/nxlib/api.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     5564 2024-01-16 14:36:14.000000 nxlib-3.6.1606/nxlib/command.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    33631 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib/constants.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    11223 2024-01-16 14:36:14.000000 nxlib-3.6.1606/nxlib/context.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2773 2024-01-16 14:36:14.000000 nxlib-3.6.1606/nxlib/exception.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22914 2023-12-15 14:52:39.000000 nxlib-3.6.1606/nxlib/item.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    12236 2023-12-15 14:52:39.000000 nxlib-3.6.1606/nxlib/log.py
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-02-02 10:36:03.373621 nxlib-3.6.1606/nxlib.egg-info/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib.egg-info/PKG-INFO
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      387 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib.egg-info/SOURCES.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib.egg-info/dependency_links.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2022-08-22 06:18:36.000000 nxlib-3.6.1606/nxlib.egg-info/not-zip-safe
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        6 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib.egg-info/requires.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)       20 2024-02-02 10:36:03.000000 nxlib-3.6.1606/nxlib.egg-info/top_level.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      198 2024-02-02 10:36:03.377621 nxlib-3.6.1606/setup.cfg
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2275 2024-02-02 10:33:53.000000 nxlib-3.6.1606/setup.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-03-19 11:29:37.729891 nxlib-3.6.1617/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1060 2024-02-13 11:06:38.000000 nxlib-3.6.1617/LICENSE.md.in
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2024-03-19 11:29:37.729891 nxlib-3.6.1617/PKG-INFO
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      898 2023-12-15 14:52:39.000000 nxlib-3.6.1617/README.md
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-03-19 11:29:37.725891 nxlib-3.6.1617/ensenso_nxlib/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      288 2023-12-15 14:52:39.000000 nxlib-3.6.1617/ensenso_nxlib/__init__.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-03-19 11:29:37.725891 nxlib-3.6.1617/nxlib/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      349 2023-12-15 14:52:39.000000 nxlib-3.6.1617/nxlib/__init__.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3173 2023-12-15 14:52:39.000000 nxlib-3.6.1617/nxlib/_helper.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22444 2024-03-19 11:27:35.000000 nxlib-3.6.1617/nxlib/api.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     5564 2024-03-19 11:27:35.000000 nxlib-3.6.1617/nxlib/command.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    33631 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib/constants.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    11223 2024-02-28 09:29:38.000000 nxlib-3.6.1617/nxlib/context.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2773 2024-03-19 11:27:35.000000 nxlib-3.6.1617/nxlib/exception.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22914 2023-12-15 14:52:39.000000 nxlib-3.6.1617/nxlib/item.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    12236 2023-12-15 14:52:39.000000 nxlib-3.6.1617/nxlib/log.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2024-03-19 11:29:37.725891 nxlib-3.6.1617/nxlib.egg-info/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib.egg-info/PKG-INFO
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      387 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2022-08-22 06:18:36.000000 nxlib-3.6.1617/nxlib.egg-info/not-zip-safe
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        6 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib.egg-info/requires.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)       20 2024-03-19 11:29:37.000000 nxlib-3.6.1617/nxlib.egg-info/top_level.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      198 2024-03-19 11:29:37.729891 nxlib-3.6.1617/setup.cfg
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2275 2024-03-19 11:27:35.000000 nxlib-3.6.1617/setup.py
```

### Comparing `nxlib-3.6.1606/LICENSE.md.in` & `nxlib-3.6.1617/LICENSE.md.in`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/PKG-INFO` & `nxlib-3.6.1617/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxlib
-Version: 3.6.1606
+Version: 3.6.1617
 Summary: Python interface to interact with the Ensenso NxLib
 Home-page: https://www.ensenso.com/python-api
 Author: Optonic GmbH
 Author-email: support@optonic.com
 License: MIT
 Description: > **Announcement:**
         With Ensenso SDK version 3.3 we stop the maintenance of our
```

### Comparing `nxlib-3.6.1606/README.md` & `nxlib-3.6.1617/README.md`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/_helper.py` & `nxlib-3.6.1617/nxlib/_helper.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/api.py` & `nxlib-3.6.1617/nxlib/api.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/command.py` & `nxlib-3.6.1617/nxlib/command.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/constants.py` & `nxlib-3.6.1617/nxlib/constants.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/context.py` & `nxlib-3.6.1617/nxlib/context.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/exception.py` & `nxlib-3.6.1617/nxlib/exception.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/item.py` & `nxlib-3.6.1617/nxlib/item.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib/log.py` & `nxlib-3.6.1617/nxlib/log.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.6.1606/nxlib.egg-info/PKG-INFO` & `nxlib-3.6.1617/nxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxlib
-Version: 3.6.1606
+Version: 3.6.1617
 Summary: Python interface to interact with the Ensenso NxLib
 Home-page: https://www.ensenso.com/python-api
 Author: Optonic GmbH
 Author-email: support@optonic.com
 License: MIT
 Description: > **Announcement:**
         With Ensenso SDK version 3.3 we stop the maintenance of our
```

### Comparing `nxlib-3.6.1606/setup.py` & `nxlib-3.6.1617/setup.py`

 * *Files identical despite different names*

