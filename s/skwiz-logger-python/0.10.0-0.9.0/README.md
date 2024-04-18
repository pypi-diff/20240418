# Comparing `tmp/skwiz_logger_python-0.10.0.tar.gz` & `tmp/skwiz_logger_python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skwiz_logger_python-0.10.0.tar", max compression
+gzip compressed data, was "skwiz_logger_python-0.9.0.tar", max compression
```

## Comparing `skwiz_logger_python-0.10.0.tar` & `skwiz_logger_python-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      747 2024-04-18 13:18:24.414379 skwiz_logger_python-0.10.0/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-18 12:49:24.452684 skwiz_logger_python-0.10.0/skwiz_logger_python/__init__.py
--rw-r--r--   0        0        0      438 2024-04-18 12:49:24.452758 skwiz_logger_python-0.10.0/skwiz_logger_python/colors.py
--rw-r--r--   0        0        0      726 2024-04-18 12:49:24.452837 skwiz_logger_python-0.10.0/skwiz_logger_python/config.py
--rw-r--r--   0        0        0     1438 2024-04-18 12:49:24.452920 skwiz_logger_python-0.10.0/skwiz_logger_python/error.py
--rw-r--r--   0        0        0     3608 2024-04-18 13:17:30.249211 skwiz_logger_python-0.10.0/skwiz_logger_python/formatter.py
--rw-r--r--   0        0        0      495 2024-04-18 12:49:24.453095 skwiz_logger_python-0.10.0/skwiz_logger_python/handler_udp.py
--rw-r--r--   0        0        0     2573 2024-04-18 13:17:32.395994 skwiz_logger_python-0.10.0/skwiz_logger_python/logger.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 skwiz_logger_python-0.10.0/setup.py
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 skwiz_logger_python-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0      706 2024-04-18 13:05:46.873498 skwiz_logger_python-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-18 12:49:24.452684 skwiz_logger_python-0.9.0/skwiz_logger_python/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-18 12:49:24.452758 skwiz_logger_python-0.9.0/skwiz_logger_python/colors.py
+-rw-r--r--   0        0        0      726 2024-04-18 12:49:24.452837 skwiz_logger_python-0.9.0/skwiz_logger_python/config.py
+-rw-r--r--   0        0        0     1438 2024-04-18 12:49:24.452920 skwiz_logger_python-0.9.0/skwiz_logger_python/error.py
+-rw-r--r--   0        0        0     3592 2024-04-18 12:49:24.453015 skwiz_logger_python-0.9.0/skwiz_logger_python/formatter.py
+-rw-r--r--   0        0        0      495 2024-04-18 12:49:24.453095 skwiz_logger_python-0.9.0/skwiz_logger_python/handler_udp.py
+-rw-r--r--   0        0        0     2549 2024-04-18 12:49:24.453176 skwiz_logger_python-0.9.0/skwiz_logger_python/logger.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 skwiz_logger_python-0.9.0/setup.py
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 skwiz_logger_python-0.9.0/PKG-INFO
```

### Comparing `skwiz_logger_python-0.10.0/pyproject.toml` & `skwiz_logger_python-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "skwiz-logger-python"
-version = "0.10.0"
+version = "0.9.0"
 description = "A saga logger for python projects"
-authors = ["hmoumal <henri.moumal@sagacify.com>", "quenting3 <quentin@skwiz.ai>"]
+authors = ["hmoumal <henri.moumal@sagacify.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 pytest = "^7.1.3"
@@ -14,14 +14,14 @@
 pylint = "2.14"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
-version_variable = "skwiz_logger_python/__init__.py:__version__"
+version_variable = "saga_logger/__init__.py:__version__"
 branch = "master"
 version_toml = "pyproject.toml:tool.poetry.version"
 commit_subject = 'chore(release): Release v{version} [skip ci]'
 upload_to_pypi = false
 upload_to_repository = false
 upload_to_release = false
```

### Comparing `skwiz_logger_python-0.10.0/skwiz_logger_python/config.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/config.py`

 * *Files identical despite different names*

### Comparing `skwiz_logger_python-0.10.0/skwiz_logger_python/error.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/error.py`

 * *Files identical despite different names*

### Comparing `skwiz_logger_python-0.10.0/skwiz_logger_python/formatter.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import datetime
 import json
 import os
 import socket
 import sys
 from logging import LogRecord
 
-from skwiz_logger_python.colors import color_message
-from skwiz_logger_python.error import error_serializer, is_error
+from saga_logger.colors import color_message
+from saga_logger.error import error_serializer, is_error
 
 
 def get_name_from_args():
     return (sys.argv[0] or sys.executable).split(os.sep)[-1]
 
 
 def get_app_name_version():
```

### Comparing `skwiz_logger_python-0.10.0/skwiz_logger_python/logger.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 
-from skwiz_logger_python import config
-from skwiz_logger_python.formatter import SagaFormatter
-from skwiz_logger_python.handler_udp import UdpHandler
+from saga_logger import config
+from saga_logger.formatter import SagaFormatter
+from saga_logger.handler_udp import UdpHandler
 
 LOG_LEVELS = {
     "fatal": 50,
     "error": 40,
     "warning": 30,
     "warn": 30,
     "info": 20,
```

### Comparing `skwiz_logger_python-0.10.0/setup.py` & `skwiz_logger_python-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['skwiz_logger_python']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'skwiz-logger-python',
-    'version': '0.10.0',
+    'version': '0.9.0',
     'description': 'A saga logger for python projects',
     'long_description': 'None',
     'author': 'hmoumal',
     'author_email': 'henri.moumal@sagacify.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

