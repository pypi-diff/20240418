# Comparing `tmp/com.castsoftware.uc.python.common-1.1.8.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.1.8.tar", last modified: Tue Feb 13 17:28:56 2024, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.1.9.tar", last modified: Thu Feb 22 14:58:57 2024, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.1.8.tar` & `com.castsoftware.uc.python.common-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 17:28:56.452468 com.castsoftware.uc.python.common-1.1.8/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      810 2024-02-13 17:28:56.440960 com.castsoftware.uc.python.common-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-13 17:28:56.333462 com.castsoftware.uc.python.common-1.1.8/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    17076 2024-02-12 21:53:59.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0    25667 2024-02-12 21:53:35.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5868 2023-11-08 14:36:13.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1894 2023-09-21 19:02:51.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/logger.py
--rw-rw-rw-   0        0        0     2227 2024-02-12 21:52:51.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/mri.py
--rw-rw-rw-   0        0        0    28890 2024-02-13 14:53:43.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/powerpoint.py
--rw-rw-rw-   0        0        0     5491 2024-02-12 21:49:38.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     7270 2023-10-27 17:55:34.000000 com.castsoftware.uc.python.common-1.1.8/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2024-02-13 17:28:56.429939 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      810 2024-02-13 17:28:55.000000 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2024-02-13 17:28:55.000000 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 17:28:55.000000 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-02-13 17:28:55.000000 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-13 17:28:55.000000 com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      650 2024-02-13 14:47:06.000000 com.castsoftware.uc.python.common-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-13 17:28:56.452468 com.castsoftware.uc.python.common-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-13 17:28:56.416811 com.castsoftware.uc.python.common-1.1.8/test/
--rw-rw-rw-   0        0        0      494 2023-06-12 17:37:07.000000 com.castsoftware.uc.python.common-1.1.8/test/TestMultiInstance.py
--rw-rw-rw-   0        0        0     1376 2023-09-13 12:29:35.000000 com.castsoftware.uc.python.common-1.1.8/test/testFullOSS.py
+drwxrwxrwx   0        0        0        0 2024-02-22 14:58:57.568237 com.castsoftware.uc.python.common-1.1.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      810 2024-02-22 14:58:57.550756 com.castsoftware.uc.python.common-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-22 14:58:57.120359 com.castsoftware.uc.python.common-1.1.9/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    17076 2024-02-12 21:53:59.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0    25667 2024-02-12 21:53:35.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5868 2023-11-08 14:36:13.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1894 2023-09-21 19:02:51.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/logger.py
+-rw-rw-rw-   0        0        0     2227 2024-02-12 21:52:51.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/mri.py
+-rw-rw-rw-   0        0        0    28889 2024-02-22 14:55:59.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/powerpoint.py
+-rw-rw-rw-   0        0        0     5491 2024-02-12 21:49:38.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     7270 2023-10-27 17:55:34.000000 com.castsoftware.uc.python.common-1.1.9/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2024-02-22 14:58:57.216833 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      810 2024-02-22 14:58:56.000000 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2024-02-22 14:58:56.000000 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-22 14:58:56.000000 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-02-22 14:58:56.000000 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-02-22 14:58:56.000000 com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      650 2024-02-22 14:57:32.000000 com.castsoftware.uc.python.common-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-22 14:58:57.568237 com.castsoftware.uc.python.common-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-22 14:58:57.202570 com.castsoftware.uc.python.common-1.1.9/test/
+-rw-rw-rw-   0        0        0      494 2023-06-12 17:37:07.000000 com.castsoftware.uc.python.common-1.1.9/test/TestMultiInstance.py
+-rw-rw-rw-   0        0        0     1376 2023-09-13 12:29:35.000000 com.castsoftware.uc.python.common-1.1.9/test/testFullOSS.py
```

### Comparing `com.castsoftware.uc.python.common-1.1.8/LICENSE` & `com.castsoftware.uc.python.common-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/PKG-INFO` & `com.castsoftware.uc.python.common-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/aipRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/highlight.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/mri.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/mri.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/powerpoint.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/powerpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 
             if background:
                 cols = cols-1
             if forground:
                 cols = cols-1
 
             if background:
-                self.set_table_bgcolor(table,df[background],rows,cols,header_rows)
+                self.set_table_bgcolor(table,df[background],nrc,cols,header_rows)
             if forground:
                 try:
                     self.set_table_font_color(table,df[forground],rows,cols,header_rows)
                 except (KeyError):
                     self.log.warning(f'error setting forground for {name}')
 
             m = df.values
```

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/restAPI.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/cast_common/util.py` & `com.castsoftware.uc.python.common-1.1.9/cast_common/util.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.1.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt` & `com.castsoftware.uc.python.common-1.1.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.1.8/pyproject.toml` & `com.castsoftware.uc.python.common-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.1.8' #prod version
+version='1.1.9' #prod version
 
 dependencies = ['pandas','requests','XlsxWriter','tqdm']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `com.castsoftware.uc.python.common-1.1.8/test/testFullOSS.py` & `com.castsoftware.uc.python.common-1.1.9/test/testFullOSS.py`

 * *Files identical despite different names*

