# Comparing `tmp/drumpler-2.2.7.tar.gz` & `tmp/drumpler-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.7.tar", last modified: Thu Apr 18 16:36:30 2024, max compression
+gzip compressed data, was "drumpler-2.2.8.tar", last modified: Thu Apr 18 17:19:36 2024, max compression
```

## Comparing `drumpler-2.2.7.tar` & `drumpler-2.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.468273 drumpler-2.2.7/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.466084 drumpler-2.2.7/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.7/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 16:36:30.467231 drumpler-2.2.7/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.7/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.464302 drumpler-2.2.7/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.7/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:58:42.000000 drumpler-2.2.7/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.7/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.7/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.7/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.7/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 16:36:30.468457 drumpler-2.2.7/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 16:36:25.000000 drumpler-2.2.7/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.465305 drumpler-2.2.7/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.7/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.950159 drumpler-2.2.8/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.948097 drumpler-2.2.8/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 17:19:36.000000 drumpler-2.2.8/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.8/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 17:19:36.949164 drumpler-2.2.8/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.8/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.945681 drumpler-2.2.8/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.8/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:58:42.000000 drumpler-2.2.8/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.8/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.8/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.8/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.8/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 17:19:36.950343 drumpler-2.2.8/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 17:19:26.000000 drumpler-2.2.8/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 17:19:36.946890 drumpler-2.2.8/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.8/test/test_drumpler.py
```

### Comparing `drumpler-2.2.7/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.8/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.7
+Version: 2.2.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.7/LICENSE` & `drumpler-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.7/PKG-INFO` & `drumpler-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.7
+Version: 2.2.8
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.7/README.md` & `drumpler-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.7/drumpler/drumpler.py` & `drumpler-2.2.8/drumpler/drumpler.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.7/drumpler/sql_job.py` & `drumpler-2.2.8/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.7/setup.py` & `drumpler-2.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.7',
+    version='2.2.8',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.7/test/test_drumpler.py` & `drumpler-2.2.8/test/test_drumpler.py`

 * *Files identical despite different names*

