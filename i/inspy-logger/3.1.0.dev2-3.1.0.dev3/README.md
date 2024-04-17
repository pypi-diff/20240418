# Comparing `tmp/inspy_logger-3.1.0.dev2.tar.gz` & `tmp/inspy_logger-3.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspy_logger-3.1.0.dev2.tar", max compression
+gzip compressed data, was "inspy_logger-3.1.0.dev3.tar", max compression
```

## Comparing `inspy_logger-3.1.0.dev2.tar` & `inspy_logger-3.1.0.dev3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev2/inspy_logger/__about__.py
--rw-r--r--   0        0        0     3421 2024-04-04 00:35:10.880027 inspy_logger-3.1.0.dev2/inspy_logger/__init__.py
--rw-r--r--   0        0        0     2504 2024-04-02 01:36:41.775167 inspy_logger-3.1.0.dev2/inspy_logger/common/__init__.py
--rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev2/inspy_logger/common/meta.py
--rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev2/inspy_logger/config/__init__.py
--rw-r--r--   0        0        0     3798 2024-04-04 02:23:50.449117 inspy_logger-3.1.0.dev2/inspy_logger/config/dirs.py
--rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev2/inspy_logger/config/levels.py
--rw-r--r--   0        0        0      475 2024-04-02 01:35:35.543818 inspy_logger-3.1.0.dev2/inspy_logger/constants.py
--rw-r--r--   0        0        0    21612 2024-04-04 00:32:11.168928 inspy_logger-3.1.0.dev2/inspy_logger/engine/__init__.py
--rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev2/inspy_logger/engine/errors.py
--rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev2/inspy_logger/engine/handlers.py
--rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev2/inspy_logger/errors/__init__.py
--rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev2/inspy_logger/helpers/__init__.py
--rw-r--r--   0        0        0     5047 2024-01-21 17:17:03.926574 inspy_logger-3.1.0.dev2/inspy_logger/helpers/base_classes.py
--rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev2/inspy_logger/helpers/command_line/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/__init__.py
--rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/environment.py
--rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/__init__.py
--rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/processor/__init__.py
--rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/winx/__init__.py
--rw-r--r--   0        0        0     9257 2024-04-01 21:11:09.678230 inspy_logger-3.1.0.dev2/inspy_logger/helpers/decorators.py
--rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev2/inspy_logger/helpers/descriptors.py
--rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev2/inspy_logger/helpers/network.py
--rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev2/inspy_logger/helpers/units.py
--rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev2/inspy_logger/manifest.py
--rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev2/inspy_logger/Scripts/main.py
--rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev2/inspy_logger/system/__init__.py
--rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev2/inspy_logger/system/linux.py
--rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev2/inspy_logger/system/mac_os.py
--rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev2/inspy_logger/system/win32.py
--rw-r--r--   0        0        0        0 2024-01-04 00:54:16.535190 inspy_logger-3.1.0.dev2/inspy_logger/tool/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev2/inspy_logger/tool/config/__init__.py
--rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev2/inspy_logger/tool/config/arguments/__init__.py
--rw-r--r--   0        0        0    14898 2024-04-08 07:53:41.405993 inspy_logger-3.1.0.dev2/inspy_logger/version/__init__.py
--rw-r--r--   0        0        0       13 2024-04-08 07:07:59.660863 inspy_logger-3.1.0.dev2/inspy_logger/version/VERSION.txt
--rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev2/LICENSE.md
--rw-r--r--   0        0        0     2304 2024-04-08 07:07:59.643795 inspy_logger-3.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev2/README.md
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev3/inspy_logger/__about__.py
+-rw-r--r--   0        0        0     3516 2024-04-17 05:01:31.534752 inspy_logger-3.1.0.dev3/inspy_logger/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-17 04:33:44.080244 inspy_logger-3.1.0.dev3/inspy_logger/common/__init__.py
+-rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev3/inspy_logger/common/meta.py
+-rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev3/inspy_logger/config/__init__.py
+-rw-r--r--   0        0        0     3754 2024-04-13 07:46:17.423404 inspy_logger-3.1.0.dev3/inspy_logger/config/dirs.py
+-rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev3/inspy_logger/config/levels.py
+-rw-r--r--   0        0        0      701 2024-04-18 02:24:15.649026 inspy_logger-3.1.0.dev3/inspy_logger/constants.py
+-rw-r--r--   0        0        0    22753 2024-04-18 02:08:22.644940 inspy_logger-3.1.0.dev3/inspy_logger/engine/__init__.py
+-rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev3/inspy_logger/engine/errors.py
+-rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev3/inspy_logger/engine/handlers.py
+-rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev3/inspy_logger/errors/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev3/inspy_logger/helpers/__init__.py
+-rw-r--r--   0        0        0     5113 2024-04-18 00:57:14.681285 inspy_logger-3.1.0.dev3/inspy_logger/helpers/base_classes.py
+-rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev3/inspy_logger/helpers/command_line/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/__init__.py
+-rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/environment.py
+-rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/__init__.py
+-rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/processor/__init__.py
+-rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/winx/__init__.py
+-rw-r--r--   0        0        0     9992 2024-04-18 02:13:36.979935 inspy_logger-3.1.0.dev3/inspy_logger/helpers/decorators.py
+-rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev3/inspy_logger/helpers/descriptors.py
+-rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev3/inspy_logger/helpers/network.py
+-rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev3/inspy_logger/helpers/units.py
+-rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev3/inspy_logger/manifest.py
+-rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev3/inspy_logger/Scripts/main.py
+-rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev3/inspy_logger/system/__init__.py
+-rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev3/inspy_logger/system/linux.py
+-rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev3/inspy_logger/system/mac_os.py
+-rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev3/inspy_logger/system/win32.py
+-rw-r--r--   0        0        0       57 2024-04-18 02:28:14.309687 inspy_logger-3.1.0.dev3/inspy_logger/tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev3/inspy_logger/tool/config/__init__.py
+-rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev3/inspy_logger/tool/config/arguments/__init__.py
+-rw-r--r--   0        0        0     4305 2024-04-17 04:21:12.630792 inspy_logger-3.1.0.dev3/inspy_logger/types.py
+-rw-r--r--   0        0        0    14877 2024-04-16 04:16:50.614788 inspy_logger-3.1.0.dev3/inspy_logger/version/__init__.py
+-rw-r--r--   0        0        0       13 2024-04-17 04:33:44.061283 inspy_logger-3.1.0.dev3/inspy_logger/version/VERSION.txt
+-rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev3/LICENSE.md
+-rw-r--r--   0        0        0     2304 2024-04-15 23:22:34.276364 inspy_logger-3.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev3/README.md
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev3/PKG-INFO
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
 MODULE_OBJ = sys.modules[__name__]
 
 CLIENT_PROG_NAME = determine_client_prog_name()
 
 INIT_LOG_LEVEL = determine_level(CLIENT_PROG_NAME)
 
+INTERACTIVE_SESSION = find_variable_in_call_stack('INSPY_INTERACTIVE_SESSION', default=False)
+
 
 def start_logger(override_block=True):
     """
     Starts the logger.
 
     Parameters:
         override_block (Union[bool, None], optional):
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/common/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 ]
 
 
 LEVELS = list(LEVEL_MAP.values())
 """The list of level names."""
 
 
-DEFAULT_LOGGING_LEVEL = logging.DEBUG
+DEFAULT_LOGGING_LEVEL = logging.INFO
 """The default logging level."""
 
 
 class InspyLogger:
     pass
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/common/meta.py` & `inspy_logger-3.1.0.dev3/inspy_logger/common/meta.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/config/dirs.py` & `inspy_logger-3.1.0.dev3/inspy_logger/config/dirs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 )
 
 from typing import Optional, Union
 
 
 INSPY_LOGGER_LOG_DIR_PATH = user_log_path(
     appname=PROG_NAME or find_valid_vars_in_call_stack(VALID_PROG_NAME_VARS),
-    appauthor=SOFTWARE_ORG,
-    ensure_exists=True
+    appauthor=SOFTWARE_ORG
 )
 
 INSPY_LOGGER_LOG_FILE_NAME = 'app.log'
 
 INSPY_LOGGER_LOG_FILE_PATH = INSPY_LOGGER_LOG_DIR_PATH.joinpath(INSPY_LOGGER_LOG_FILE_NAME)
 
 
@@ -120,15 +119,15 @@
 
     if not dev_name and prog_name:
         dev_name = find_valid_vars_in_call_stack(VALID_DEV_NAME_VARS.valid_vars)
 
     if prog_name:
         file_name = f"{prog_name}.log"
         if dev_name:
-            log_file_path = Path(user_log_path(appname=prog_name, appauthor=dev_name, ensure_exists=True)).joinpath(file_name)
+            log_file_path = Path(user_log_path(appname=prog_name, appauthor=dev_name).joinpath(file_name))
         else:
             log_file_path = INSPY_LOGGER_LOG_DIR_PATH.joinpath(file_name)
 
     return log_file_path or INSPY_LOGGER_LOG_FILE_PATH
 
 
 DEFAULT_LOG_FILE_PATH = get_log_file_path()
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/engine/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 import os
 import logging
 import sys
 
 from rich.logging import RichHandler
 
 from inspy_logger.config import DEFAULT_LOG_FILE_PATH
+from inspy_logger.constants import LEVELS, INTERACTIVE_SESSION, INTERNAL
 from inspy_logger.engine.handlers import BufferingHandler
 from inspy_logger.common import InspyLogger, DEFAULT_LOGGING_LEVEL
 from inspy_logger.helpers import translate_to_logging_level, CustomFormatter, get_level_name, RestrictedSetter
 from inspy_logger.helpers.decorators import add_aliases, method_alias, count_invocations, validate_type
 from typing import List, Union, Optional
 from pathlib import Path
 
 
 @add_aliases
 class Logger(InspyLogger):
     """
     A Singleton class responsible for managing the logging mechanisms of the application.
     """
 
+    LEVELS = LEVELS
+    INTERACTIVE_SESSION = INTERACTIVE_SESSION
     instances = {}  # A dictionary to hold instances of the Logger class.
 
     # Set the file path for the log file.
     file_path = RestrictedSetter('file_path', DEFAULT_LOG_FILE_PATH, allowed_types=(str, Path),preferred_type=Path)
 
     def __new__(cls, name, *args, **kwargs):
         """
@@ -48,14 +51,15 @@
             auto_set_up=True,
             console_level=DEFAULT_LOGGING_LEVEL,
             file_level=logging.DEBUG,
             file_name="app.log",
             file_path=DEFAULT_LOG_FILE_PATH.parent,
             no_file_logging=False,
             parent=None,
+            skip_interactive_check: bool=False
     ):
         """
         Initializes a logger instance.
 
         Parameters:
             name (str):
                 The name of the logger instance.
@@ -89,27 +93,27 @@
 
         self.__children = []
 
         self.__name = name
         self.__no_file_logging = None
         self.__file_path = None
 
+
         self.logger = logging.getLogger(name)
-        self.logger.debug('Debug message from logger')
         self.logger.setLevel(translate_to_logging_level(console_level))
 
         self.logger.propagate = False
         self.logger.start = self.start
 
         if 'inSPy-Logger' in self.logger.name:
             self.buffering_handler = BufferingHandler()
             self.logger.addHandler(self.buffering_handler)
-            self.logger.debug('Initializing logger with buffering handler.')
+            self.internal('Initializing logger with buffering handler.')
         else:
-            self.logger.debug('Initializing  logger without buffering handler.')
+            self.internal('Initializing  logger without buffering handler.')
 
         self.no_file_logging = no_file_logging
 
         self.set_file_path = Path(file_path).expanduser().absolute().joinpath(file_name)
 
         self.parent = parent
 
@@ -163,14 +167,15 @@
         Returns:
 
         """
         self.set_level(console_level=translate_to_logging_level(level))
 
     @property
     def console_level_name(self):
+        self.internal('Test message')
         return get_level_name(self.console_level)
 
     @property
     def device(self):
         """
         Returns the logger instance.
 
@@ -239,14 +244,18 @@
     #             new_path = Path(new)
     #             self.ensure_log_file_path()
     #         except Exception as e:
     #             self.__file_path = old
     #             raise e
 
     @property
+    def interactive_session(self):
+        return hasattr(sys, 'ps1') and sys.ps1
+
+    @property
     def name(self):
         """
         Returns the name of the logger instance.
 
         Returns:
             str:
                 The name of the logger instance.
@@ -300,14 +309,30 @@
                 The file handler for the logger.
         """
         for handler in self.logger.handlers:
             if isinstance(handler, logging.FileHandler):
 
                 return handler
 
+    def has_child(self, name):
+        """
+        Checks if the logger has a child with the specified name.
+
+        Args:
+            name (str):
+                The name of the child logger.
+
+        Returns:
+            bool:
+                True if the logger has a child with the specified name, else False.
+        """
+
+        return name in self.child_names
+
+
     @validate_type(str, Path, preferred_type=Path)
     def set_file_path(self, file_path):
         """
         Sets the file path for the logger.
 
         Args:
             file_path (str):
@@ -317,22 +342,20 @@
             old = self.file_path
             self.file_path = file_path
             self.ensure_log_file_path()
         except Exception as e:
             self.file_path = old
             raise
 
-
-
     def set_up_console(self):
         """
         Configures and attaches a console handler to the logger.
         """
 
-        self.logger.debug("Setting up console handler")
+        self.internal("Setting up console handler")
         console_handler = RichHandler(
             show_level=True, markup=True, rich_tracebacks=True, tracebacks_show_locals=True
         )
         formatter = CustomFormatter(
             f"[{self.logger.name}] %(message)s"
         )
         console_handler.setFormatter(formatter)
@@ -363,15 +386,15 @@
             file_level:
                 The logging level for the file.
 
         Returns:
             None
         """
 
-        self.logger.debug("Setting log levels")
+        self.internal("Setting log levels")
 
         # If we received a console level, update the console level.
         if console_level is not None:
             console_level = translate_to_logging_level(console_level)
 
             # Set the `console_level` property to the new value.
             self.__console_level = console_level
@@ -415,55 +438,51 @@
             file_level (int, optional):
                 The file log level for the child logger. Defaults to None.
 
         Returns:
             InspyLogger:
                 The child logger with the specified name, console level, and file level.
         """
-        # Determine the console level and file level for the child logger.
-
-        # If the console level is not provided, use the console level of the parent logger
-        console_level = console_level or self.console_level
-
-        # If the file level is not provided, use the file level of the parent logger
-        file_level = file_level or self.file_level
-
         # Get the name of the calling function if no name is provided
         caller_frame = inspect.stack()[1]
 
         cl_name = self.__build_name_from_caller(caller_frame, name)
 
-        cl_name
+        if found_child := self.find_child_by_name(cl_name, exact_match=True):
+            return found_child
+
+        # Determine the console level and file level for the child logger.
 
-        found_child = self.find_child_by_name(cl_name, exact_match=True)
+        # If the console level is not provided, use the console level of the parent logger
+        console_level = console_level or self.console_level
 
-        if found_child:
-            return found_child
+        # If the file level is not provided, use the file level of the parent logger
+        file_level = file_level or self.file_level
 
         child_logger = Logger(name=cl_name, console_level=console_level, file_level=file_level, parent=self)
 
         self.children.append(child_logger)
 
         return child_logger
 
     @method_alias('get_children_names', 'get_child_loggers')
     def get_child_names(self) -> List:
         """
         Fetches the names of all child loggers associated with this logger instance.
         """
 
-        self.logger.debug("Getting child logger names")
+        self.internal("Getting child logger names")
         return [child.logger.name for child in self.children]
 
     def get_parent(self) -> InspyLogger:
         """
         Fetches the parent logger associated with this logger instance.
         """
 
-        self.logger.debug("Getting parent logger")
+        self.internal("Getting parent logger")
         return self.parent
 
     def find_child_by_name(self, name: str, case_sensitive=True, exact_match=False) -> (List, InspyLogger):
         """
         Searches for a child logger by its name.
 
         Args:
@@ -477,15 +496,15 @@
                 Whether the search should only return exact matches. Defaults to False.
 
         Returns:
             list or Logger: If exact_match is True, returns the Logger instance if found, else returns an empty list.
                             If exact_match is False, returns a list of Logger instances whose names contain the
                             search term.
         """
-        self.logger.debug(f'Searching for child with name: {name}')
+        self.internal(f'Searching for child with name: {name}')
         results = []
 
         if not case_sensitive:
             name = name.lower()
 
         for logger in self.children:
             logger_name = logger.name if case_sensitive else logger.name.lower()
@@ -493,33 +512,46 @@
                 return logger
             elif not exact_match and name in logger_name:
                 results.append(logger)
 
         return results
 
     @count_invocations
-    def debug(self, message):
+    def debug(self, message, stack_level=3):
         """
         Logs a debug message.
 
         Args:
-          message (str): The message to log.
+            message (str): The message to log.
+
+            stack_level (int, optional):
+                The stacklevel to use when logging. Defaults to 3.
         """
-        self._log(logging.DEBUG, message, args=(), stacklevel=2)
+        self._log(logging.DEBUG, message, args=(), stacklevel=stack_level)
 
     @count_invocations
     def info(self, message):
         """
         Logs an info message.
 
         Args:
             message (str): The message to log.
         """
         self._log(logging.INFO, message, args=(), stacklevel=2)
 
+    def internal(self, message, *args, **kwargs):
+        """
+        Logs an internal message.
+
+        Args:
+            message (str): The message to log.
+        """
+        if self.logger.isEnabledFor(INTERNAL):
+            self._log(INTERNAL, message, args=args, stacklevel=2)
+
     @count_invocations
     def warning(self, message):
         """
         Logs a warning message.
 
 
         Args:
@@ -620,15 +652,15 @@
             'Buffering Handler': 'Yes' if getattr(self, 'buffering_handler', None) else 'No'
         }
 
     def start(self, *args, **kwargs):
         """
         Starts the logger.
         """
-        self.logger.warning('InspyLogger.start() is deprecated.')
+        self.warning('InspyLogger.start() is deprecated.')
         if not self.logger.handlers:
             self.set_up_handlers()
 
         if hasattr(self, 'buffering_handler'):
             self.replay_and_setup_handlers()
 
         return self
@@ -652,14 +684,19 @@
             return relative_path.replace(os.path.sep, '.').rstrip('.py')
         return None
 
     def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, stacklevel=1):
         """
         Low-level logging implementation, passing stacklevel to findCaller.
         """
+        #caller_frame = inspect.currentframe().f_back
+        #print(caller_frame.f_code.co_name)
+        if INTERACTIVE_SESSION:
+            stacklevel -= 1
+
         if self.logger.isEnabledFor(level):
             self.logger._log(level, msg, args, exc_info, extra, stack_info, stacklevel + 1)
 
     def __rich__(self):
         # Create a rich table with logger properties
         from rich.table import Table
         from rich import box
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/engine/errors.py` & `inspy_logger-3.1.0.dev3/inspy_logger/engine/errors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/engine/handlers.py` & `inspy_logger-3.1.0.dev3/inspy_logger/engine/handlers.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/errors/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/base_classes.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/base_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import inspect
 from inspy_logger import LOG_DEVICE, Logger
 
 
-
 class LoggableDescriptor:
     """
     Descriptor for accessing a logger specific to a class method.
     """
 
     def __get__(self, instance, owner):
         if instance is None:
@@ -15,15 +14,15 @@
 
         # Determine the calling method's name
         stack = inspect.stack()
         # Start from 1 to skip the current __get__ frame
         for frame_record in stack[1:]:
             if 'self' in frame_record.frame.f_locals and frame_record.frame.f_locals['self'] is instance:
                 method_name = frame_record.function
-                print(method_name)
+
                 break
         else:
             raise Exception("Could not determine the calling method's name.")
 
         # Get a child logger named after the class and method
         return instance.log_device.get_child(method_name)
 
@@ -68,14 +67,15 @@
             **kwargs: Additional keyword arguments.
 
         Returns:
             None
         """
         self.parent_log_device = parent_log_device
         self.__log_name = self.__class__.__name__
+
         if self.parent_log_device is not None:
             self.__log_device = self.parent_log_device.get_child(self.__log_name)
         else:
             self.__log_device = _get_parent_logging_device().get_child()
 
         # Set up class-level logger if it's not already set
         if self.__class__.class_logger is None:
@@ -102,33 +102,38 @@
             name (str, optional): The name of the child logger.
                 If not provided, the name of the calling function is used.
             override (bool, optional): A flag to override the membership check. Defaults to False.
 
         Returns:
             Logger: An instance of the Logger class that represents the child logger.
         """
-        if not override:
-            self.__is_member__()
-
         if name is None:
             name = inspect.stack()[1][
                 3
-            ]  # Get the name of the calling function if no name is provided
-        #print(inspect.stack()[1])
+            ]
+        if self.log_device.has_child(name):
+            return self.log_device.find_child_by_name(name)
+        if not override:
+            self.__is_member__()
+
         return self.log_device.get_child(name)
 
     def __is_member__(self):
         """
         Checks whether the caller of this method is a member of the same class.
 
         Raises:
             PermissionError: If the caller of this method is not a member of the same class.
         """
+        print(self.log_device.children)
+        log_name = f'{self.log_device.name}.__is_member__'
+
+
         log_device = self.log_device.get_child("__is_member__")
-        log = log_device.logger
+        log = log_device
 
         current_frame = inspect.currentframe()
         log.debug(f"Current frame: {current_frame}")
 
         caller_frame = current_frame.f_back
         log.debug(f"Caller frame: {caller_frame}")
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/command_line/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/environment.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/environment.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/processor/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/debug/system/winx/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/winx/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/decorators.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,35 @@
     'method_logger',
     'add_aliases',
     'count_invocations',
     'validate_type'
 ]
 
 
+def property_logging(func):
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        if self.creating_logger:
+            return
+        if found := self.class_logger.find_child_by_name(func.__name__, exact_match=True):
+            log = found
+        else:
+            self.creating_logger = True
+            log = self.class_logger.add_child(func.__name__)
+            self.creating_logger = False
+
+        log.debug(f'Getting {func.__name__} from instance of {self.__class__.__name__}...', stack_level=4)
+        res = func(self, *args, **kwargs)
+        log.debug(f'Got {func.__name__} from instance of {self.__class__.__name__}: {res}', stack_level=4)
+
+        return res
+    return wrapper
+
+
+
 def method_alias(*alias_names: (str, list[str])):
     """
     A decorator that allows you to add aliases to a class's method.
 
     Args:
         *alias_names (str, list[str]):
             The name(s) of the alias(es) to add.
@@ -158,15 +179,15 @@
         >>> obj.my_property = "hello"  # This is also accepted and set
         >>> obj.my_property = "Hi"  # This raises ValueError
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(self, value):
-            if not isinstance(value, allowed_types):
+            if not isinstance(value, tuple(allowed_types)):
                 allowed = ', '.join([t.__name__ for t in allowed_types])
                 raise TypeError(f"Value must be of type {allowed}, got type {type(value).__name__}")
 
             if preferred_type and not isinstance(value, preferred_type):
                 try:
                     value = preferred_type(value)
                 except Exception as e:
```

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/descriptors.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/descriptors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/network.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/network.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/helpers/units.py` & `inspy_logger-3.1.0.dev3/inspy_logger/helpers/units.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/manifest.py` & `inspy_logger-3.1.0.dev3/inspy_logger/manifest.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/Scripts/main.py` & `inspy_logger-3.1.0.dev3/inspy_logger/Scripts/main.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/system/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/system/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/system/win32.py` & `inspy_logger-3.1.0.dev3/inspy_logger/system/win32.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/tool/config/arguments/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/tool/config/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/inspy_logger/version/__init__.py` & `inspy_logger-3.1.0.dev3/inspy_logger/version/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,17 +216,14 @@
         return self.version_info['release']
 
     @property
     def release_num(self):
         return self.version_info['release_num']
 
 
-print(__file__)
-
-
 def parse_version_file():
     with open(Path(__file__).parent.joinpath('VERSION.txt'), 'r') as f:
         return VersionParser(f.read().strip())
 
 
 VERSION_PARSER = parse_version_file()
```

### Comparing `inspy_logger-3.1.0.dev2/LICENSE.md` & `inspy_logger-3.1.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/pyproject.toml` & `inspy_logger-3.1.0.dev3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspy-logger"
-version = "3.1.0-dev.2"
+version = "3.1.0-dev.3"
 description = "Colorable, scalable logger for CLI"
 authors = ["Taylor-Jayde Blackstone <tayjaybabee@gmail.com>"]
 homepage = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 repository = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 documentation = 'https://inspy-logger.readthedocs.io/en/latest/'
 readme = 'README.md'
 license = 'MIT'
```

### Comparing `inspy_logger-3.1.0.dev2/README.md` & `inspy_logger-3.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev2/PKG-INFO` & `inspy_logger-3.1.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy-logger
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: Colorable, scalable logger for CLI
 Home-page: https://github.com/Inspyre-Softworks/inSPy-Logger
 License: MIT
 Keywords: cli,color,logging,log,terminal,console,colorama,colorlog,rich
 Author: Taylor-Jayde Blackstone
 Author-email: tayjaybabee@gmail.com
 Requires-Python: >=3.9,<4.0
```

