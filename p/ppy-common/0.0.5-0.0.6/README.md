# Comparing `tmp/ppy-common-0.0.5.tar.gz` & `tmp/ppy-common-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppy-common-0.0.5.tar", last modified: Wed Dec 13 13:13:52 2023, max compression
+gzip compressed data, was "ppy-common-0.0.6.tar", last modified: Thu Apr 18 04:19:02 2024, max compression
```

## Comparing `ppy-common-0.0.5.tar` & `ppy-common-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 13:13:52.508311 ppy-common-0.0.5/
--rw-rw-rw-   0        0        0    11549 2023-11-24 04:39:29.000000 ppy-common-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1964 2023-12-13 13:13:52.504322 ppy-common-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-11-24 04:39:29.000000 ppy-common-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-12-13 13:13:52.442980 ppy-common-0.0.5/ppy_common/
--rw-rw-rw-   0        0        0      394 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/__init__.py
--rw-rw-rw-   0        0        0     1596 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/ppy_common_helper.py
--rw-rw-rw-   0        0        0      341 2023-12-12 14:50:40.000000 ppy-common-0.0.5/ppy_common/ppy_data.py
--rw-rw-rw-   0        0        0     1215 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/ppy_data_util.py
--rw-rw-rw-   0        0        0     1547 2023-12-12 14:50:40.000000 ppy-common-0.0.5/ppy_common/ppy_date_util.py
--rw-rw-rw-   0        0        0      366 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/ppy_object_helper.py
--rw-rw-rw-   0        0        0     2982 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/ppyc_console_log.py
--rw-rw-rw-   0        0        0      819 2023-11-24 04:39:29.000000 ppy-common-0.0.5/ppy_common/ppyc_exception.py
-drwxrwxrwx   0        0        0        0 2023-12-13 13:13:52.502328 ppy-common-0.0.5/ppy_common.egg-info/
--rw-rw-rw-   0        0        0     1964 2023-12-13 13:13:52.000000 ppy-common-0.0.5/ppy_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-12-13 13:13:52.000000 ppy-common-0.0.5/ppy_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 13:13:52.000000 ppy-common-0.0.5/ppy_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-24 04:39:36.000000 ppy-common-0.0.5/ppy_common.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-12-13 13:13:52.000000 ppy-common-0.0.5/ppy_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-12-13 13:13:52.000000 ppy-common-0.0.5/ppy_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-13 13:13:52.508311 ppy-common-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-12-13 13:05:35.000000 ppy-common-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:19:02.899637 ppy-common-0.0.6/
+-rw-rw-rw-   0        0        0    11549 2023-11-24 04:39:29.000000 ppy-common-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1964 2024-04-18 04:19:02.898636 ppy-common-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-11-24 04:39:29.000000 ppy-common-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 04:19:02.875642 ppy-common-0.0.6/ppy_common/
+-rw-rw-rw-   0        0        0      394 2023-11-24 04:39:29.000000 ppy-common-0.0.6/ppy_common/__init__.py
+-rw-rw-rw-   0        0        0     2528 2024-04-18 04:17:02.000000 ppy-common-0.0.6/ppy_common/ppy_common_helper.py
+-rw-rw-rw-   0        0        0      341 2023-12-12 14:50:40.000000 ppy-common-0.0.6/ppy_common/ppy_data.py
+-rw-rw-rw-   0        0        0     1215 2023-11-24 04:39:29.000000 ppy-common-0.0.6/ppy_common/ppy_data_util.py
+-rw-rw-rw-   0        0        0     3361 2024-03-31 22:27:47.000000 ppy-common-0.0.6/ppy_common/ppy_date_util.py
+-rw-rw-rw-   0        0        0      366 2023-11-24 04:39:29.000000 ppy-common-0.0.6/ppy_common/ppy_object_helper.py
+-rw-rw-rw-   0        0        0     2982 2023-11-24 04:39:29.000000 ppy-common-0.0.6/ppy_common/ppyc_console_log.py
+-rw-rw-rw-   0        0        0      819 2023-11-24 04:39:29.000000 ppy-common-0.0.6/ppy_common/ppyc_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:19:02.897639 ppy-common-0.0.6/ppy_common.egg-info/
+-rw-rw-rw-   0        0        0     1964 2024-04-18 04:19:02.000000 ppy-common-0.0.6/ppy_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-18 04:19:02.000000 ppy-common-0.0.6/ppy_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 04:19:02.000000 ppy-common-0.0.6/ppy_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-24 04:39:36.000000 ppy-common-0.0.6/ppy_common.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-04-18 04:19:02.000000 ppy-common-0.0.6/ppy_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 04:19:02.000000 ppy-common-0.0.6/ppy_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 04:19:02.899637 ppy-common-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2024-04-18 04:18:40.000000 ppy-common-0.0.6/setup.py
```

### Comparing `ppy-common-0.0.5/LICENSE` & `ppy-common-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ppy-common-0.0.5/PKG-INFO` & `ppy-common-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppy-common
-Version: 0.0.5
+Version: 0.0.6
 Summary: PWeb Python Common is a library which help various common work to do easily
 Home-page: https://github.com/banglafighter/ppy-common
 Author: Bangla Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `ppy-common-0.0.5/README.md` & `ppy-common-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ppy-common-0.0.5/ppy_common/ppy_data_util.py` & `ppy-common-0.0.6/ppy_common/ppy_data_util.py`

 * *Files identical despite different names*

### Comparing `ppy-common-0.0.5/ppy_common/ppyc_console_log.py` & `ppy-common-0.0.6/ppy_common/ppyc_console_log.py`

 * *Files identical despite different names*

### Comparing `ppy-common-0.0.5/ppy_common/ppyc_exception.py` & `ppy-common-0.0.6/ppy_common/ppyc_exception.py`

 * *Files identical despite different names*

### Comparing `ppy-common-0.0.5/ppy_common.egg-info/PKG-INFO` & `ppy-common-0.0.6/ppy_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppy-common
-Version: 0.0.5
+Version: 0.0.6
 Summary: PWeb Python Common is a library which help various common work to do easily
 Home-page: https://github.com/banglafighter/ppy-common
 Author: Bangla Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `ppy-common-0.0.5/setup.py` & `ppy-common-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return dependency
 
     return dependency + []
 
 
 setup(
     name='ppy-common',
-    version='0.0.5',
+    version='0.0.6',
     url='https://github.com/banglafighter/ppy-common',
     license='Apache 2.0',
     author='Bangla Fighter',
     author_email='banglafighter.com@gmail.com',
     description='PWeb Python Common is a library which help various common work to do easily',
     long_description=README,
     long_description_content_type='text/markdown',
```

