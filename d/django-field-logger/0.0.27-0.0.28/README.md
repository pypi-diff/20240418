# Comparing `tmp/django_field_logger-0.0.27.tar.gz` & `tmp/django_field_logger-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_field_logger-0.0.27.tar", last modified: Sun Apr 14 05:55:18 2024, max compression
+gzip compressed data, was "django_field_logger-0.0.28.tar", last modified: Wed Apr 17 23:54:34 2024, max compression
```

## Comparing `django_field_logger-0.0.27.tar` & `django_field_logger-0.0.28.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django_field_logger-0.0.27/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django_field_logger-0.0.27/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7679 2024-04-12 03:39:00.000000 django_field_logger-0.0.27/README.rst
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      554 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2012 2024-04-14 05:54:20.000000 django_field_logger-0.0.27/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1385 2024-04-14 05:50:25.000000 django_field_logger-0.0.27/fieldlogger/encoding.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      969 2024-04-14 05:37:12.000000 django_field_logger-0.0.27/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2816 2024-04-14 05:50:03.000000 django_field_logger-0.0.27/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      381 2024-04-14 05:36:16.000000 django_field_logger-0.0.27/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django_field_logger-0.0.27/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/setup.cfg
--rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django_field_logger-0.0.27/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1783 2024-04-14 05:52:42.000000 django_field_logger-0.0.27/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django_field_logger-0.0.28/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django_field_logger-0.0.28/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9999 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7764 2024-04-17 23:38:01.000000 django_field_logger-0.0.28/README.rst
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9999 2024-04-17 23:54:34.000000 django_field_logger-0.0.28/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      554 2024-04-17 23:54:34.000000 django_field_logger-0.0.28/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-17 23:54:34.000000 django_field_logger-0.0.28/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-17 23:54:34.000000 django_field_logger-0.0.28/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-17 23:54:34.000000 django_field_logger-0.0.28/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:51.000000 django_field_logger-0.0.28/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-04-12 05:21:51.000000 django_field_logger-0.0.28/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2213 2024-04-17 05:22:00.000000 django_field_logger-0.0.28/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1385 2024-04-14 05:50:25.000000 django_field_logger-0.0.28/fieldlogger/encoding.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      969 2024-04-14 05:37:12.000000 django_field_logger-0.0.28/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-04-12 05:21:51.000000 django_field_logger-0.0.28/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2816 2024-04-14 05:50:03.000000 django_field_logger-0.0.28/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1665 2024-04-17 22:45:35.000000 django_field_logger-0.0.28/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      381 2024-04-14 05:36:16.000000 django_field_logger-0.0.28/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django_field_logger-0.0.28/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/setup.cfg
+-rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django_field_logger-0.0.28/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:54:34.769800 django_field_logger-0.0.28/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:35.000000 django_field_logger-0.0.28/tests/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1630 2024-04-17 23:36:16.000000 django_field_logger-0.0.28/tests/settings.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3993 2024-04-17 22:08:59.000000 django_field_logger-0.0.28/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2105 2024-04-17 23:06:39.000000 django_field_logger-0.0.28/tests/tests.py
```

### Comparing `django_field_logger-0.0.27/LICENSE` & `django_field_logger-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.27/PKG-INFO` & `django_field_logger-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.27
+Version: 0.0.28
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
@@ -85,26 +85,27 @@
 -  ``FAIL_SILENTLY`` is optional. If it is set to ``False``, exceptions
    will be raised if the callback function fails.
 -  ``LOGGING_APPS`` apps to be logged.
 
    -  ``models`` models to be logged.
 
       -  ``fields`` is optional. If you want to log only specific
-         fields, you can specify them here.
+         fields, you can specify them here. If you want to log all
+         fields, you can use ``__all__`` as a value.
       -  ``exclude_fields`` is optional. If ``fields`` is not specified,
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
          function in yourapp/callbacks.py. Callback functions must have
-         the following signature:
-         ``python   def callback(instance, fields, logs):       pass``
+         three parameters as follows:
+         ``python   def your_callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
 
 How it works?
```

### Comparing `django_field_logger-0.0.27/README.rst` & `django_field_logger-0.0.28/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,27 @@
 -  ``FAIL_SILENTLY`` is optional. If it is set to ``False``, exceptions
    will be raised if the callback function fails.
 -  ``LOGGING_APPS`` apps to be logged.
 
    -  ``models`` models to be logged.
 
       -  ``fields`` is optional. If you want to log only specific
-         fields, you can specify them here.
+         fields, you can specify them here. If you want to log all
+         fields, you can use ``__all__`` as a value.
       -  ``exclude_fields`` is optional. If ``fields`` is not specified,
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
          function in yourapp/callbacks.py. Callback functions must have
-         the following signature:
-         ``python   def callback(instance, fields, logs):       pass``
+         three parameters as follows:
+         ``python   def your_callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
 
 How it works?
```

### Comparing `django_field_logger-0.0.27/django_field_logger.egg-info/PKG-INFO` & `django_field_logger-0.0.28/django_field_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.27
+Version: 0.0.28
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
@@ -85,26 +85,27 @@
 -  ``FAIL_SILENTLY`` is optional. If it is set to ``False``, exceptions
    will be raised if the callback function fails.
 -  ``LOGGING_APPS`` apps to be logged.
 
    -  ``models`` models to be logged.
 
       -  ``fields`` is optional. If you want to log only specific
-         fields, you can specify them here.
+         fields, you can specify them here. If you want to log all
+         fields, you can use ``__all__`` as a value.
       -  ``exclude_fields`` is optional. If ``fields`` is not specified,
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
          function in yourapp/callbacks.py. Callback functions must have
-         the following signature:
-         ``python   def callback(instance, fields, logs):       pass``
+         three parameters as follows:
+         ``python   def your_callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
 
 How it works?
```

### Comparing `django_field_logger-0.0.27/django_field_logger.egg-info/SOURCES.txt` & `django_field_logger-0.0.28/django_field_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.27/fieldlogger/config.py` & `django_field_logger-0.0.28/fieldlogger/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 from functools import reduce
-from typing import Dict, FrozenSet, List, Union
+from typing import Any, Dict, FrozenSet, List, Union
 
+from django.apps import apps
 from django.conf import settings
 from django.utils.module_loading import import_string
 
 from .models import Callback, LoggableModel
 
-SETTINGS = getattr(settings, "FIELD_LOGGER_SETTINGS", {}).copy()
+SETTINGS = getattr(settings, "FIELD_LOGGER_SETTINGS", {})
 
 
 def _cfg_reduce(op, key, *configs, default=None):
     return reduce(
         op,
         [config.get(key, default) for config in configs],
         SETTINGS.get(key.upper(), default),
     )
 
 
-def logging_enabled(*configs: Dict[str, bool]) -> bool:
+def _logging_enabled(*configs: Dict[str, bool]) -> bool:
     return _cfg_reduce(lambda a, b: a and b, "logging_enabled", *configs, default=True)
 
 
-def fail_silently(*configs: Dict[str, bool]) -> bool:
+def _fail_silently(*configs: Dict[str, bool]) -> bool:
     return _cfg_reduce(lambda a, b: a and b, "fail_silently", *configs, default=True)
 
 
-def callbacks(*configs: Dict[str, List[Union[str, Callback]]]) -> List[Callback]:
+def _callbacks(*configs: Dict[str, List[Union[str, Callback]]]) -> List[Callback]:
     callbacks = _cfg_reduce(lambda a, b: a + b, "callbacks", *configs, default=[])
 
     callbacks = [
         import_string(callback) if isinstance(callback, str) else callback
         for callback in callbacks
     ]
 
     return callbacks
 
 
-def logging_fields(instance: LoggableModel) -> FrozenSet[str]:
-    model_config = LOGGING_CONFIG.get(instance._meta.label, {})
-
+def _logging_fields(
+    model_class: LoggableModel, model_config: Dict[str, Any]
+) -> FrozenSet[str]:
+    fields = model_config.get("fields", [])
     exclude_fields = model_config.get("exclude_fields", [])
-    if not exclude_fields:
-        return frozenset(model_config.get("fields", []))
+    model_fields = [field.name for field in model_class._meta.fields]
 
-    return frozenset(
-        field.name for field in instance._meta.fields if field.name not in exclude_fields
+    return frozenset(model_fields if fields == "__all__" else fields) - frozenset(
+        exclude_fields
     )
 
 
 LOGGING_CONFIG = {}
 for app, app_config in SETTINGS.get("LOGGING_APPS", {}).items():
-    if not app_config or not logging_enabled(app_config):
+    if not app_config or not _logging_enabled(app_config):
         continue
 
     for model, model_config in app_config.get("models", {}).items():
-        if not model_config or not logging_enabled(app_config, model_config):
+        if not model_config or not _logging_enabled(app_config, model_config):
             continue
 
-        model_config["callbacks"] = callbacks(app_config, model_config)
-        model_config["fail_silently"] = fail_silently(app_config, model_config)
+        try:
+            model_class = apps.get_model(app, model)
+        except LookupError:
+            continue
 
-        LOGGING_CONFIG[f"{app}.{model}"] = model_config
+        LOGGING_CONFIG[f"{app}.{model}"] = {
+            "fail_silently": _fail_silently(app_config, model_config),
+            "callbacks": _callbacks(app_config, model_config),
+            "logging_fields": _logging_fields(model_class, model_config),
+        }
```

### Comparing `django_field_logger-0.0.27/fieldlogger/encoding.py` & `django_field_logger-0.0.28/fieldlogger/encoding.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.27/fieldlogger/fieldlogger.py` & `django_field_logger-0.0.28/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.27/fieldlogger/models.py` & `django_field_logger-0.0.28/fieldlogger/models.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.27/fieldlogger/signals.py` & `django_field_logger-0.0.28/fieldlogger/signals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from django.db.models.signals import post_save, pre_save
 
-from .config import LOGGING_CONFIG, logging_fields
+from .config import LOGGING_CONFIG
 from .fieldlogger import log_fields
 
 
 def pre_save_log_fields(sender, instance, *args, **kwargs):
-    using_fields = logging_fields(instance)
+    using_fields = LOGGING_CONFIG.get(sender._meta.label, {}).get(
+        "logging_fields", frozenset()
+    )
 
     update_fields = kwargs["update_fields"] or frozenset()
     if update_fields:
         using_fields = using_fields & update_fields
 
     instance._fieldlogger_using_fields = using_fields
 
@@ -22,25 +24,26 @@
     pre_instance = getattr(instance, "_fieldlogger_pre_instance", None)
 
     if using_fields and (pre_instance or created):
         # Get logs
         logs = log_fields(instance, using_fields, pre_instance)
 
         # Run callbacks
-        callbacks = LOGGING_CONFIG[sender._meta.label].get("callbacks", [])
+        callbacks = LOGGING_CONFIG[sender._meta.label]["callbacks"]
         for callback in callbacks:
             try:
                 callback(instance, using_fields, logs)
             except Exception as e:
                 if LOGGING_CONFIG[sender._meta.label]["fail_silently"]:
                     continue
                 raise e
 
     # Clean up
-    del instance._fieldlogger_using_fields
+    if hasattr(instance, "_fieldlogger_using_fields"):
+        del instance._fieldlogger_using_fields
     if hasattr(instance, "_fieldlogger_pre_instance"):
         del instance._fieldlogger_pre_instance
 
 
 for label in LOGGING_CONFIG:
     pre_save.connect(pre_save_log_fields, label)
     post_save.connect(post_save_log_fields, label)
```

### Comparing `django_field_logger-0.0.27/setup.cfg` & `django_field_logger-0.0.28/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-field-logger
-version = 0.0.27
+version = 0.0.28
 description = A Django app for logging changes in model fields.
 long_description = file: README.rst, LICENSE
 author = Sergio Rodríguez
 author_email = srodriguez3441@gmail.com
 maintainer = Sergio Rodríguez
 maintainer_email = srodriguez3441@gmail.com
 url = https://github.com/nibblex/django-field-logger
```

### Comparing `django_field_logger-0.0.27/tests/test_utils.py` & `django_field_logger-0.0.28/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from shutil import rmtree
 from uuid import UUID
 
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.utils import timezone
 
-from fieldlogger import config
+from fieldlogger import config, signals
 
-now = timezone.now()
+NOW = timezone.now()
 
 
 CREATE_FORM = {
     "test_big_integer_field": 1,
     "test_binary_field": bytes("test", "utf-8"),
     "test_boolean_field": True,
     "test_char_field": "test",
-    "test_date_field": now.date(),
-    "test_datetime_field": now,
+    "test_date_field": NOW.date(),
+    "test_datetime_field": NOW,
     "test_decimal_field": Decimal(3.1499),
     "test_duration_field": timedelta(days=1),
     "test_email_field": "test@test.com",
     "test_file_field": ContentFile("test", "test.txt"),
     "test_file_path_field": "test.txt",
     "test_float_field": 1.0,
     "test_generic_ip_address_field": "127.0.0.1",
@@ -32,26 +32,26 @@
     "test_json_field": {"test": "test"},
     "test_positive_big_integer_field": 1,
     "test_positive_integer_field": 1,
     "test_positive_small_integer_field": 1,
     "test_slug_field": "test",
     "test_small_integer_field": 1,
     "test_text_field": "test",
-    "test_time_field": now.time(),
+    "test_time_field": NOW.time(),
     "test_url_field": "https://test.com",
     "test_uuid_field": UUID("550e8400-e29b-41d4-a716-446655440000"),
 }
 
 UPDATE_FORM = {
     "test_big_integer_field": 2,
     "test_binary_field": bytes("test2", "utf-8"),
     "test_boolean_field": False,
     "test_char_field": "test2",
-    "test_date_field": now.date() + timedelta(days=1),
-    "test_datetime_field": now + timedelta(days=1),
+    "test_date_field": NOW.date() + timedelta(days=1),
+    "test_datetime_field": NOW + timedelta(days=1),
     "test_decimal_field": Decimal(3.1415),
     "test_duration_field": timedelta(days=2),
     "test_email_field": "test2@test.com",
     "test_file_field": ContentFile("test2", "test2.txt"),
     "test_file_path_field": "test2.txt",
     "test_float_field": 2.0,
     "test_generic_ip_address_field": "127.0.0.2",
@@ -60,55 +60,56 @@
     "test_json_field": {"test": "test2"},
     "test_positive_big_integer_field": 2,
     "test_positive_integer_field": 2,
     "test_positive_small_integer_field": 2,
     "test_slug_field": "test2",
     "test_small_integer_field": 2,
     "test_text_field": "test2",
-    "test_time_field": (now + timedelta(hours=1)).time(),
+    "test_time_field": (NOW + timedelta(hours=1)).time(),
     "test_url_field": "https://test2.com",
     "test_uuid_field": UUID("550e8400-e29b-41d4-a716-446655440001"),
 }
 
 
-def _set_config(cfg, scope):
+def set_config(cfg, scope):
     for name, value in cfg.items():
         if scope == "global":
             settings.FIELD_LOGGER_SETTINGS[name.upper()] = value
         elif scope == "testapp":
             settings.FIELD_LOGGER_SETTINGS["LOGGING_APPS"]["testapp"][name] = value
         elif scope == "testmodel":
             settings.FIELD_LOGGER_SETTINGS["LOGGING_APPS"]["testapp"]["models"][
                 "TestModel"
             ][name] = value
         else:
             raise ValueError(f"Invalid scope: {scope}")
 
     reload(config)
+    reload(signals)
 
 
 def set_attributes(instance, form, update_fields=False):
     for field, value in form.items():
         setattr(instance, field, value)
         if update_fields:
             instance.save(update_fields=[field])
 
     if not update_fields:
         instance.save()
 
     rmtree(settings.MEDIA_ROOT, ignore_errors=True)
 
 
-def check_logs(instance, created=False):
-    logs = instance.fieldlog_set.filter(created=created)
-    assert logs.count() == len(CREATE_FORM if created else UPDATE_FORM)
+def check_logs(instance, expected_count, created=False):
+    assert instance.fieldlog_set.count() == expected_count
 
+    logs = instance.fieldlog_set.filter(created=created)
     for log in logs:
         prev_log = log.previous_log
         assert (prev_log is None) == created
         assert log.app_label == "testapp"
         assert log.model == "testmodel"
         assert log.instance_id == instance.pk
         assert log.old_value == (prev_log.new_value if prev_log else None)
         assert log.new_value == getattr(instance, log.field)
-        assert log.extra_data == {"global": True, "testapp": True}
+        assert log.extra_data == {"global": True, "testapp": True, "testmodel": True}
         assert log.created == created
```

