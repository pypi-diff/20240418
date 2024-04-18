# Comparing `tmp/drumpler-2.2.4.tar.gz` & `tmp/drumpler-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.4.tar", last modified: Wed Apr 17 18:47:10 2024, max compression
+gzip compressed data, was "drumpler-2.2.5.tar", last modified: Wed Apr 17 19:28:22 2024, max compression
```

## Comparing `drumpler-2.2.4.tar` & `drumpler-2.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.569818 drumpler-2.2.4/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.567684 drumpler-2.2.4/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 18:47:10.000000 drumpler-2.2.4/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.4/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 18:47:10.568738 drumpler-2.2.4/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.4/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.566115 drumpler-2.2.4/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.4/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.4/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)    10588 2024-04-17 18:46:46.000000 drumpler-2.2.4/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.4/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.4/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.4/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.4/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 18:47:10.570003 drumpler-2.2.4/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 18:46:58.000000 drumpler-2.2.4/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 18:47:10.566711 drumpler-2.2.4/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.4/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.952908 drumpler-2.2.5/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.951195 drumpler-2.2.5/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.5/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 19:28:22.951995 drumpler-2.2.5/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.5/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.949746 drumpler-2.2.5/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.5/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.5/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10588 2024-04-17 18:46:46.000000 drumpler-2.2.5/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.5/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.5/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.5/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.5/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 19:28:22.953080 drumpler-2.2.5/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 19:28:14.000000 drumpler-2.2.5/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.950378 drumpler-2.2.5/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.5/test/test_drumpler.py
```

### Comparing `drumpler-2.2.4/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.5/Drumpler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.4
+Version: 2.2.5
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.4/LICENSE` & `drumpler-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.4/PKG-INFO` & `drumpler-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.4
+Version: 2.2.5
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.4/README.md` & `drumpler-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.4/drumpler/config.py` & `drumpler-2.2.5/drumpler/config.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.4/drumpler/drumpler.py` & `drumpler-2.2.5/drumpler/drumpler.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.4/drumpler/sql_job.py` & `drumpler-2.2.5/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.4/setup.py` & `drumpler-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.4',
+    version='2.2.5',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.4/test/test_drumpler.py` & `drumpler-2.2.5/test/test_drumpler.py`

 * *Files identical despite different names*

