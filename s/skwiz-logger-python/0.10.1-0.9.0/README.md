# Comparing `tmp/skwiz_logger_python-0.10.1.tar.gz` & `tmp/skwiz_logger_python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skwiz_logger_python-0.10.1.tar", max compression
+gzip compressed data, was "skwiz_logger_python-0.9.0.tar", max compression
```

## Comparing `skwiz_logger_python-0.10.1.tar` & `skwiz_logger_python-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      748 2024-04-18 14:16:15.777647 skwiz_logger_python-0.10.1/pyproject.toml
--rw-r--r--   0        0        0       96 2024-04-18 14:16:15.773647 skwiz_logger_python-0.10.1/skwiz_logger_python/__init__.py
--rw-r--r--   0        0        0      438 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/colors.py
--rw-r--r--   0        0        0      726 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/config.py
--rw-r--r--   0        0        0     1438 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/error.py
--rw-r--r--   0        0        0     3612 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/formatter.py
--rw-r--r--   0        0        0      495 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/handler_udp.py
--rw-r--r--   0        0        0     2578 2024-04-18 14:16:01.229640 skwiz_logger_python-0.10.1/skwiz_logger_python/logger.py
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 skwiz_logger_python-0.10.1/PKG-INFO
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

### Comparing `skwiz_logger_python-0.10.1/pyproject.toml` & `skwiz_logger_python-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "skwiz-logger-python"
-version = "0.10.1"
-description = "A skwiz logger for python projects"
-authors = ["hmoumal <henri.moumal@sagacify.com>", "quenting3 <quentin@skwiz.ai>"]
+version = "0.9.0"
+description = "A saga logger for python projects"
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

### Comparing `skwiz_logger_python-0.10.1/skwiz_logger_python/config.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/config.py`

 * *Files identical despite different names*

### Comparing `skwiz_logger_python-0.10.1/skwiz_logger_python/error.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/error.py`

 * *Files identical despite different names*

### Comparing `skwiz_logger_python-0.10.1/skwiz_logger_python/formatter.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # pylint: disable=no-member
 """
-SkwizFormatter
+SagaFormatter
 
 Ensures logs are formatted as we want them.
 cfr: https://github.com/sagacify/logger
 """
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
@@ -33,19 +33,19 @@
     except AttributeError:
         app_name = None
         app_version = None
 
     return app_name, app_version
 
 
-class SkwizFormatter:
+class SagaFormatter:
     """
-    Skwiz Formatter.
+    Saga Formatter.
 
-    Formats mesages coming from a skwizlogger
+    Formats mesages coming from a sagalogger
     """
 
     def __init__(self, log_stack_level: int, max_error_length=0, colorized=False):
         self.app_name, self.app_version = get_app_name_version()
         self.hostname = socket.gethostname()
         self.log_stack_level = log_stack_level
         self.max_error_length = max_error_length
```

### Comparing `skwiz_logger_python-0.10.1/skwiz_logger_python/logger.py` & `skwiz_logger_python-0.9.0/skwiz_logger_python/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 
-from skwiz_logger_python import config
-from skwiz_logger_python.formatter import SkwizFormatter
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
@@ -20,15 +20,15 @@
     log_level = LOG_LEVELS[config["log_level_name"].lower()]
 
     log_stack_level = LOG_LEVELS[config["log_stack_level_name"].lower()]
 
     root_logger = logging.root
     root_logger.setLevel(log_level)
 
-    log_formatter = SkwizFormatter(
+    log_formatter = SagaFormatter(
         log_stack_level, config["log_error_message_length"], config["log_pretty"]
     )
 
     if config["log_endpoint"] is not None:
         [host, port] = config["log_endpoint"].split(":")
         # Udp handler must be formatted manually as the automatic formatting
         # does not seem to work
@@ -36,22 +36,22 @@
     else:
         log_handler = logging.StreamHandler(stream=sys.stdout)
         log_handler.setFormatter(log_formatter)
 
     root_logger.addHandler(log_handler)
 
 
-class SkwizLogger:
+class SagaLogger:
     setup_done = False
 
     def __init__(self, module: str = None, extra=None):
         # Setup the logging on root if not already done
-        if not SkwizLogger.setup_done:
+        if not SagaLogger.setup_done:
             setup()
-            SkwizLogger.setup_done = True
+            SagaLogger.setup_done = True
 
         self.logger = logging.getLogger(module)
         self.extra = extra if extra else {}
 
     def trace(self, message: str, index: dict = None, raw: dict = None):
         self.logger.trace(
             message, extra=dict(self.extra, **{"indexed": index, "raw": raw})
```

