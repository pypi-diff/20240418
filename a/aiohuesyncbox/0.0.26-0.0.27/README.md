# Comparing `tmp/aiohuesyncbox-0.0.26.tar.gz` & `tmp/aiohuesyncbox-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohuesyncbox-0.0.26.tar", last modified: Sun Aug 13 09:38:29 2023, max compression
+gzip compressed data, was "aiohuesyncbox-0.0.27.tar", last modified: Thu Apr 18 19:02:43 2024, max compression
```

## Comparing `aiohuesyncbox-0.0.26.tar` & `aiohuesyncbox-0.0.27.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 09:38:29.753904 aiohuesyncbox-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-13 09:38:29.753904 aiohuesyncbox-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 09:38:29.753904 aiohuesyncbox-0.0.26/aiohuesyncbox/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/hdmi.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/hsb_cacert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/hue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/huesyncbox.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/aiohuesyncbox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 09:38:29.753904 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-13 09:38:29.000000 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-13 09:38:29.000000 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 09:38:29.000000 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-13 09:38:29.000000 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-13 09:38:29.000000 aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-13 09:38:29.753904 aiohuesyncbox-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-13 09:38:16.000000 aiohuesyncbox-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:02:43.606881 aiohuesyncbox-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-18 19:02:43.606881 aiohuesyncbox-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:02:43.602881 aiohuesyncbox-0.0.27/aiohuesyncbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/hdmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/hsb_cacert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/huesyncbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/aiohuesyncbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:02:43.606881 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-18 19:02:43.000000 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-18 19:02:43.000000 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:02:43.000000 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 19:02:43.000000 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 19:02:43.000000 aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:02:43.606881 aiohuesyncbox-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-18 19:02:35.000000 aiohuesyncbox-0.0.27/setup.py
```

### Comparing `aiohuesyncbox-0.0.26/LICENSE` & `aiohuesyncbox-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/PKG-INFO` & `aiohuesyncbox-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.26
+Version: 0.0.27
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
+Requires-Dist: aiohttp<4
 
 AIOHUESYNCBOX
 =============
 
 Asyncio package to communicate with Philips Hue Play HDMI Sync Box.
 This package is aimed at basic control of the box. Initial setup and configuration is assumed to done with the official Hue app.
```

### Comparing `aiohuesyncbox-0.0.26/README.rst` & `aiohuesyncbox-0.0.27/README.rst`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/behavior.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/behavior.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/device.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/device.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/errors.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """Aiohuesyncbox errors."""
 
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 class AiohuesyncboxException(Exception):
     """Base error for aiohuesyncbox."""
 
 
 class RequestError(AiohuesyncboxException):
     """Unable to fulfill request.
@@ -32,8 +36,9 @@
     15: RequestError,
     16: InvalidState,
 }
 
 
 def raise_error(code: int, message: str) -> None:
     cls = ERRORS.get(code, AiohuesyncboxException)
+    logger.debug("raise_error, %s, %s, %s", code, message, cls)
     raise cls("{}: {}".format(code, message))
```

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/execution.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/execution.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/hdmi.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/hdmi.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/hsb_cacert.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/hsb_cacert.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/hue.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/hue.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox/huesyncbox.py` & `aiohuesyncbox-0.0.27/aiohuesyncbox/huesyncbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
             )
         else:
             hosts.append(await super().resolve(host, port=port, family=family))
 
         for host in hosts:
             host["hostname"] = self._common_name
 
+        logger.debug("Resolved hosts: %s", hosts)
+
         return hosts
 
 
 class HueSyncBox:
     """Control a Philips Hue Play HDMI Sync Box."""
 
     def __init__(
@@ -226,18 +228,20 @@
                             _raise_on_error(data)
                         else:
                             logger.error(
                                 "Received unexpected data format: %s" % str(data)
                             )
                 return data
         except aiohttp.ClientError as err:
+            logger.debug(err, exc_info=True)
             raise RequestError(
                 f"Error requesting data from {self._host}"
             ) from err
         except asyncio.TimeoutError as err:
+            logger.debug(err, exc_info=True)
             raise RequestError(
                 f"Timeout requesting data from {self._host}"
             ) from err
 
 
 def _raise_on_error(data: Dict):
     """Check response for error message."""
```

### Comparing `aiohuesyncbox-0.0.26/aiohuesyncbox.egg-info/PKG-INFO` & `aiohuesyncbox-0.0.27/aiohuesyncbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.26
+Version: 0.0.27
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
+Requires-Dist: aiohttp<4
 
 AIOHUESYNCBOX
 =============
 
 Asyncio package to communicate with Philips Hue Play HDMI Sync Box.
 This package is aimed at basic control of the box. Initial setup and configuration is assumed to done with the official Hue app.
```

### Comparing `aiohuesyncbox-0.0.26/setup.py` & `aiohuesyncbox-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="aiohuesyncbox",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.26",
+    version="0.0.27",
     description="Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.",
     long_description=long_description,
     # The project's main homepage.
     url="https://github.com/mvdwetering/aiohuesyncbox",
     # Author details
     author="Michel van de Wetering",
     author_email="michel.van.de.wetering@gmail.com",
```

