# Comparing `tmp/drumpler-2.2.5.tar.gz` & `tmp/drumpler-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.2.5.tar", last modified: Wed Apr 17 19:28:22 2024, max compression
+gzip compressed data, was "drumpler-2.2.6.tar", last modified: Thu Apr 18 15:31:48 2024, max compression
```

## Comparing `drumpler-2.2.5.tar` & `drumpler-2.2.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.952908 drumpler-2.2.5/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.951195 drumpler-2.2.5/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-17 19:28:22.000000 drumpler-2.2.5/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.5/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-17 19:28:22.951995 drumpler-2.2.5/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.5/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.949746 drumpler-2.2.5/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.5/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.5/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)    10588 2024-04-17 18:46:46.000000 drumpler-2.2.5/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.5/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.5/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.5/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.5/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 19:28:22.953080 drumpler-2.2.5/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-17 19:28:14.000000 drumpler-2.2.5/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:28:22.950378 drumpler-2.2.5/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.5/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.818776 drumpler-2.2.6/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.816762 drumpler-2.2.6/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      336 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       71 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-18 15:31:48.000000 drumpler-2.2.6/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.6/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4175 2024-04-18 15:31:48.817821 drumpler-2.2.6/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.6/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.815483 drumpler-2.2.6/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       37 2024-04-17 19:28:07.000000 drumpler-2.2.6/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10636 2024-04-18 15:31:33.000000 drumpler-2.2.6/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)      100 2024-04-17 16:55:13.000000 drumpler-2.2.6/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      331 2024-04-17 16:56:03.000000 drumpler-2.2.6/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      602 2024-04-17 16:55:48.000000 drumpler-2.2.6/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      508 2024-04-17 16:55:19.000000 drumpler-2.2.6/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-18 15:31:48.818966 drumpler-2.2.6/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      800 2024-04-18 15:31:38.000000 drumpler-2.2.6/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-18 15:31:48.815980 drumpler-2.2.6/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.6/test/test_drumpler.py
```

### Comparing `drumpler-2.2.5/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.6/Drumpler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.5
+Version: 2.2.6
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.5/LICENSE` & `drumpler-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.5/PKG-INFO` & `drumpler-2.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.2.5
+Version: 2.2.6
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.2.5/README.md` & `drumpler-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.5/drumpler/drumpler.py` & `drumpler-2.2.6/drumpler/drumpler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-import os
 import json
-import sys
 import psutil
 from datetime import datetime, timezone
 from flask import Flask, request, jsonify
-from .config import Config
 from .sql_base import db, init_app  # Import db and the initialization function
 from .sql_request import SqlRequest
 from .sql_job import SqlJob
 from .sql_event import SqlEvent
 
 app = Flask(__name__)
-app.config['SQLALCHEMY_DATABASE_URI'] = Config.DATABASE_URI
-app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
-init_app(app)  # Initialize SQLAlchemy with the Flask app
 
 class Drumpler:
-    def __init__(self):
+    def __init__(self, authorization_key, host="http://127.0.0.1", port=5000, debug=True, database_uri='sqlite:///default.db'):
         self.app = app  # Use the global app instance
-        self.__init_env()
+        self.authorization_key = authorization_key
+        self.host = host
+        self.port = port
+        self.debug = debug
+        self.database_uri = database_uri
+
         self.__init_config()
         self.__init_db()
         self.__setup_routes()
 
     def __init_config(self):
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = self.database_uri
+        self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+
+        # set relative settings
         cpu_cores = psutil.cpu_count()
         total_memory_gb = psutil.virtual_memory().total / (1024 ** 3)
 
         # Example dynamic settings based on system resources
         pool_size = max(10, cpu_cores * 2)  # Starting at 10, increasing with more cores
         max_overflow = max(5, int(pool_size * 0.5))  # 50% of pool_size
         pool_timeout = 30  # Static setting, can adjust if needed
         pool_recycle = 1800  # Static setting, can adjust if needed
 
         self.app.config['SQLALCHEMY_POOL_SIZE'] = pool_size
         self.app.config['SQLALCHEMY_MAX_OVERFLOW'] = max_overflow
         self.app.config['SQLALCHEMY_POOL_TIMEOUT'] = pool_timeout
         self.app.config['SQLALCHEMY_POOL_RECYCLE'] = pool_recycle
 
-        self.AUTHORIZATION_KEY = Config.AUTHORIZATION_KEY
-        self.host = Config.DRUMPLER_HOST
-        self.port = Config.DRUMPLER_PORT
-        self.debug = Config.DRUMPLER_DEBUG
-
     def __init_db(self):
+        init_app(app)  # Initialize SQLAlchemy with the Flask app
         with self.app.app_context():
             db.create_all()  # Create tables based on the models if they don't exist
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
@@ -55,24 +54,20 @@
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
         self.app.add_url_rule('/jobs/next-pending', view_func=self.__get_next_pending_job, methods=['GET'])
         self.app.add_url_rule('/jobs/<int:job_id>', view_func=self.__update_job, methods=['PUT'])
         self.app.add_url_rule('/jobs/<int:job_id>/update-status', view_func=self.__update_job_status, methods=['PUT'])
         self.app.add_url_rule('/jobs/<int:job_id>/mark-handled', view_func=self.__mark_request_as_handled, methods=['PUT'])
         self.app.add_url_rule('/events', view_func=self.__create_event, methods=['POST'])
 
-    def __init_env(self):
-        if not os.path.exists(".env"):
-            sys.exit("ERROR! You must create a .env file that contains a single line 'AUTHORIZATION_KEY=YourAuthorizationKeyHere'")
-
     def __authorize_request(self):
         authorization = request.headers.get('Authorization')
         return authorization and authorization == f"Bearer {self.AUTHORIZATION_KEY}"
     
     def hello_world(self):
-        return "Hello World"
+        return "Hello Drumpler!"
 
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
         data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
         custom_value = request.args.get('custom_value', None)
@@ -224,12 +219,17 @@
         new_event = SqlEvent(job_id=data['job_id'], message=data['message'])
         db.session.add(new_event)
         db.session.commit()
         return jsonify({'event_id': new_event.id}), 201
 
     def run(self):
         app.run(host=self.host, port=self.port, debug=self.debug)
-        #self.app.run()
 
 if __name__ == '__main__':
-    drumpler = Drumpler()
+    drumpler = Drumpler(
+        authorization_key="YourAuthorizationKey",
+        host="http://127.0.0.1",
+        port=5000,
+        debug=True,
+        database_uri='sqlite:///path_to_your_database.db'
+    )
     drumpler.run()
```

### Comparing `drumpler-2.2.5/drumpler/sql_job.py` & `drumpler-2.2.6/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.2.5/setup.py` & `drumpler-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.2.5',
+    version='2.2.6',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.2.5/test/test_drumpler.py` & `drumpler-2.2.6/test/test_drumpler.py`

 * *Files identical despite different names*

