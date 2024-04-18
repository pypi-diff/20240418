# Comparing `tmp/drumpler-2.2.6.tar.gz` & `tmp/drumpler-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.6.tar", last modified: Thu Apr 18 15:31:48 2024, max compression
+gzip compressed data, was "drumpler-2.2.7.tar", last modified: Thu Apr 18 16:36:30 2024, max compression
```

## Comparing `drumpler-2.2.6.tar` & `drumpler-2.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.818776 drumpler-2.2.6/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.816762 drumpler-2.2.6/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.6/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 15:31:48.817821 drumpler-2.2.6/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.6/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.815483 drumpler-2.2.6/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.6/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:31:33.000000 drumpler-2.2.6/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.6/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.6/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.6/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.6/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 15:31:48.818966 drumpler-2.2.6/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 15:31:38.000000 drumpler-2.2.6/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.815980 drumpler-2.2.6/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.6/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.468273 drumpler-2.2.7/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.466084 drumpler-2.2.7/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 16:36:30.000000 drumpler-2.2.7/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.7/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 16:36:30.467231 drumpler-2.2.7/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.7/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.464302 drumpler-2.2.7/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.7/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:58:42.000000 drumpler-2.2.7/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.7/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.7/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.7/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.7/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 16:36:30.468457 drumpler-2.2.7/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 16:36:25.000000 drumpler-2.2.7/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 16:36:30.465305 drumpler-2.2.7/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.7/test/test_drumpler.py
```

### Comparing `drumpler-2.2.6/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.7/Drumpler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.6
+Version: 2.2.7
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.6/LICENSE` & `drumpler-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.6/PKG-INFO` & `drumpler-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.6
+Version: 2.2.7
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.6/README.md` & `drumpler-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.6/drumpler/drumpler.py` & `drumpler-2.2.7/drumpler/drumpler.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.app.add_url_rule('/jobs/<int:job_id>', view_func=self.__update_job, methods=['PUT'])
         self.app.add_url_rule('/jobs/<int:job_id>/update-status', view_func=self.__update_job_status, methods=['PUT'])
         self.app.add_url_rule('/jobs/<int:job_id>/mark-handled', view_func=self.__mark_request_as_handled, methods=['PUT'])
         self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
     def __authorize_request(self):
         authorization = request.headers.get('Authorization')
-        return authorization and authorization == f"Bearer {self.AUTHORIZATION_KEY}"
+        return authorization and authorization == f"Bearer {self.authorization_key}"
     
     def hello_world(self):
         return "Hello Drumpler!"
 
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
```

### Comparing `drumpler-2.2.6/drumpler/sql_job.py` & `drumpler-2.2.7/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.6/setup.py` & `drumpler-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.6',
+    version='2.2.7',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.6/test/test_drumpler.py` & `drumpler-2.2.7/test/test_drumpler.py`

 * *Files identical despite different names*

