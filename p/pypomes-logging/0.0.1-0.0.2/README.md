# Comparing `tmp/pypomes_logging-0.0.1.tar.gz` & `tmp/pypomes_logging-0.0.2.tar.gz`

## Comparing `pypomes_logging-0.0.1.tar` & `pypomes_logging-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0    12020 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pypomes_logging-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/PKG-INFO
```

### Comparing `pypomes_logging-0.0.1/src/pypomes_logging/__init__.py` & `pypomes_logging-0.0.2/src/pypomes_logging/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .logging_pomes import (
     LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
     LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
-    logging_get_entries, logging_get_entries_from_request,
+    logging_get_entries, logging_send_entries,
     logging_log_msgs, logging_log_debug, logging_log_error,
     logging_log_info, logging_log_critical, logging_log_warning,
 )
 
 __all__ = [
     # logging_pomes
     "LOGGING_ID", "LOGGING_LEVEL", "LOGGING_FORMAT", "LOGGING_STYLE",
     "LOGGING_FILE_PATH", "LOGGING_FILE_MODE", "PYPOMES_LOGGER",
-    "logging_get_entries", "logging_get_entries_from_request",
+    "logging_get_entries", "logging_send_entries",
     "logging_log_msgs", "logging_log_debug", "logging_log_error",
     "logging_log_info", "logging_log_critical", "logging_log_warning",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_logging")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_logging-0.0.1/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.0.2/src/pypomes_logging/logging_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import logging
-from datetime import datetime
-from dateutil import parser
+from datetime import datetime, timedelta
 from flask import Request, Response, send_file
 from io import BytesIO
 from pathlib import Path
 from typing import Final, Literal, TextIO
 
 from pypomes_core import (
-    APP_PREFIX, DATETIME_FORMAT_INV, TEMP_DIR,
-    env_get_str, env_get_path
+    APP_PREFIX, DATETIME_FORMAT_INV, TEMP_DIR, DATETIME_FORMAT_COMPACT,
+    env_get_str, env_get_path, datetime_parse
 )
+from pypomes_http import http_get_parameters
 
 
 def __get_logging_level(level: Literal["debug", "info", "warning", "error", "critical"]) -> int:
     """
     Translate the log severity string *level* into the logging's internal severity value.
 
     :param level: the string log severity
@@ -65,15 +65,16 @@
                     level=LOGGING_LEVEL)
 for _handler in logging.root.handlers:
     _handler.addFilter(logging.Filter(LOGGING_ID))
 
 
 def logging_get_entries(errors: list[str],
                         log_level: Literal["debug", "info", "warning", "error", "critical"] = None,
-                        log_from: str = None, log_to: str = None,
+                        log_from: datetime = None,
+                        log_to: datetime = None,
                         log_path: Path | str = LOGGING_FILE_PATH) -> BytesIO:
     """
     Extract and return all entries in the logging file *log_path*.
 
     It is expected for this logging file to be compliant with *PYPOMES_LOGGER*'s default format.
     The extraction meets the criteria specified by *log_level*, and by the inclusive interval *[log_from, log_to]*.
 
@@ -87,114 +88,120 @@
     # inicializa variável de retorno
     result: BytesIO | None = None
 
     # obtain the logging level
     # noinspection PyTypeChecker
     logging_level: int = __get_logging_level(log_level)
 
-    # obtain the initial timestamp
-    from_stamp: datetime | None = None
-    if log_from:
-        from_stamp = parser.parse(log_from)
-        if not from_stamp:
-            errors.append(f"Value '{from_stamp}' of 'from' attribute invalid")
-
-    # obtain the final timestamp
-    to_stamp: datetime | None = None
-    if log_to:
-        to_stamp = parser.parse(log_to)
-        if not to_stamp or \
-           (from_stamp and from_stamp > to_stamp):
-            errors.append(f"Value '{to_stamp}' of 'to' attribute invalid")
-
-    file_path: Path = Path(log_path)
+    filepath: Path = Path(log_path)
     # does the log file exist ?
-    if not Path.exists(file_path):
+    if not Path.exists(filepath):
         # no, report the error
-        errors.append(f"File '{file_path}' not found")
+        errors.append(f"File '{filepath}' not found")
 
     # any error ?
     if len(errors) == 0:
         # no, proceed
         result = BytesIO()
-        with Path.open(file_path) as f:
+        with filepath.open() as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
                 # noinspection PyTypeChecker
                 msg_level: int = __get_logging_level(items[2])
                 if msg_level >= logging_level:
-                    timestamp: datetime = parser.parse(f"{items[0]} {items[1]}")
-                    if (not from_stamp or timestamp >= from_stamp) and \
-                       (not to_stamp or timestamp <= to_stamp):
-                        result.write(line.encode())
+                    if log_from or log_to:
+                        timestamp: datetime = datetime_parse(f"{items[0]} {items[1]}")
+                        if (not log_from or timestamp >= log_from) and \
+                           (not log_to or timestamp <= log_to):
+                            result.write(line.encode())
+                    else:
+                            result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
-def logging_get_entries_from_request(request: Request, as_attachment: bool = False) -> Response:
+def logging_send_entries(request: Request) -> Response:
     """
-    Retrieve from the log file, and return, the entries matching the criteria specified.
+    Retrieve from the log file, and send in response, the entries matching the criteria specified.
 
-    These criteria are specified in the query string of the HTTP request, according to the pattern
-    *path=<log-path>&level=<log-level>&from=YYYYMMDDhhmmss&to=YYYYMMDDhhmmss>*
+    These criteria are specified as imput parameters of the HTTP request, according to the pattern
+    *attach=<[t,true,f,false]>&log-path=<log-path>&level=<log-level>&
+     from=YYYYMMDDhhmmss&to=YYYYMMDDhhmmss&last-days=<n>&last-hours=<n>>*
 
     All criteria are optional:
-        - path: the path of the log file
+        - attach: whether browser should display or save file (defaults to True - save it)
+        - log-path: the path of the log file (defaults to LOGGING_FILE_PATH)
         - level: the logging level of the entries
         - from: the start timestamp
         - to: the finish timestamp
+        - last-days: how many days before current date
+        - last-hours: how may hours before current time
 
-    :param request: the HTTP request
-    :param as_attachment: indicate to browser that it should offer to save the file, or just display it
+    :param request: the 'Request' object
     :return: file containing the log entries requested on success, or incidental errors on fail
     """
     # declare the return variable
     result: Response
 
     # initialize the error messages list
     errors: list[str] = []
 
+    # obtain the request parameters
+    scheme: dict = http_get_parameters(request=request)
+
     # obtain the logging level
-    log_level: str = request.args.get("level")
+    log_level: str = scheme.get("level")
 
     # obtain the initial and final timestamps
-    log_from: str = request.args.get("from")
-    log_to: str = request.args.get("to")
+    log_from: datetime = datetime_parse(scheme.get("from"))
+    log_to: datetime = datetime_parse(scheme.get("to"))
+
+    # if 'from' and 'to' were not specified, try 'last-days' and 'last-hours'
+    if log_from is None and log_to is None:
+        last_days: str = scheme.get("last-days", "0")
+        last_hours: str = scheme.get("last-hours", "0")
+        offset_days: int = int(last_days) if last_days.isdigit() else 0
+        offset_hours: int = int(last_hours) if last_hours.isdigit() else 0
+        if offset_days or offset_hours:
+            log_from = datetime.now() - timedelta(days=offset_days, hours=offset_hours)
 
     # obtain the path for the log file
-    log_path: str = request.args.get("path") or LOGGING_FILE_PATH
+    log_path: Path | str = scheme.get("log-path", LOGGING_FILE_PATH)
 
     # retrieve the log entries
     # noinspection PyTypeChecker
     log_entries: BytesIO = logging_get_entries(errors, log_level, log_from, log_to, log_path)
 
     # any error ?
     if len(errors) == 0:
-        # no, return the log entries requested as an attached file
-        base: str = "entries" if not log_from or not log_to else \
-            (
-                f"{''.join(ch for ch in log_from if ch.isdigit())}"
-                f"{'_'.join(ch for ch in log_to if ch.isdigit())}"
-            )
+        # no, return the log entries requested
+        base: str = "entries"
+        if log_from:
+           base += f"-from_{log_from.strftime(DATETIME_FORMAT_COMPACT)}"
+        if log_to:
+           base += f"-to_{log_to.strftime(DATETIME_FORMAT_COMPACT)}"
         log_file = f"log_{base}.log"
+        param: str = scheme.get("attach", "true")
+        attach: bool = not (isinstance(param, str) and param.lower() in ["0", "f", "false"])
         log_entries.seek(0)
         result = send_file(path_or_file=log_entries,
                            mimetype="text/plain",
-                           as_attachment=as_attachment,
+                           as_attachment=attach,
                            download_name=log_file)
     else:
         # yes, report the failure
         result = Response(json.dumps({"errors": errors}), status=400,  mimetype="application/json")
 
     return result
 
 
-def logging_log_msgs(msgs: list[str], output_dev: TextIO = None,
+def logging_log_msgs(msgs: list[str],
+                     output_dev: TextIO = None,
                      log_level: Literal["debug", "info", "warning", "error", "critical"] = "error",
                      logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write all messages in *msgs* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
 
@@ -240,15 +247,16 @@
     :param logger: the logger to use
     """
     # log the message
     logger.debug(msg)
     __write_to_output(msg, output_dev)
 
 
-def logging_log_info(msg: str, output_dev: TextIO = None,
+def logging_log_info(msg: str,
+                     output_dev: TextIO = None,
                      logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write info-level message *msg* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
 
     :param msg: the message to log
@@ -256,15 +264,16 @@
     :param logger: the logger to use
     """
     # log the message
     logger.info(msg)
     __write_to_output(msg, output_dev)
 
 
-def logging_log_warning(msg: str, output_dev: TextIO = None,
+def logging_log_warning(msg: str,
+                        output_dev: TextIO = None,
                         logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write warning-level message *msg* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
 
     :param msg: the message to log
@@ -272,15 +281,16 @@
     :param logger: the logger to use
     """
     # log the message
     logger.warning(msg)
     __write_to_output(msg, output_dev)
 
 
-def logging_log_error(msg: str, output_dev: TextIO = None,
+def logging_log_error(msg: str,
+                      output_dev: TextIO = None,
                       logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write error-level message *msg* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
 
     :param msg: the message to log
@@ -288,15 +298,16 @@
     :param logger: the logger to use
     """
     # log the message
     logger.error(msg)
     __write_to_output(msg, output_dev)
 
 
-def logging_log_critical(msg: str, output_dev: TextIO = None,
+def logging_log_critical(msg: str,
+                         output_dev: TextIO = None,
                          logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write critical-level message *msg* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
 
     :param msg: the message to log
@@ -304,15 +315,16 @@
     :param logger: the logger to use
     """
     # log the message
     logger.critical(msg)
     __write_to_output(msg, output_dev)
 
 
-def __write_to_output(msg: str, output_dev: TextIO) -> None:
+def __write_to_output(msg: str,
+                      output_dev: TextIO) -> None:
 
     # has the output device been defined ?
     if output_dev:
         # yes, write the message to it
         output_dev.write(msg)
 
         # is the output device 'stderr' ou 'stdout' ?
```

### Comparing `pypomes_logging-0.0.1/LICENSE` & `pypomes_logging-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.1/pyproject.toml` & `pypomes_logging-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes-core>=0.8.3",
+    "pypomes_core>=0.8.7",
+    "pypomes_http>=0.1.3",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Logging"
```

### Comparing `pypomes_logging-0.0.1/PKG-INFO` & `pypomes_logging-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_logging
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.3
+Requires-Dist: pypomes-core>=0.8.7
+Requires-Dist: pypomes-http>=0.1.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

