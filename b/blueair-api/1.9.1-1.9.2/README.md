# Comparing `tmp/blueair_api-1.9.1.tar.gz` & `tmp/blueair_api-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueair_api-1.9.1.tar", last modified: Mon Mar 18 23:47:44 2024, max compression
+gzip compressed data, was "blueair_api-1.9.2.tar", last modified: Thu Apr 18 08:37:06 2024, max compression
```

## Comparing `blueair_api-1.9.1.tar` & `blueair_api-1.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:47:44.451217 blueair_api-1.9.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1066 2024-03-18 23:47:30.000000 blueair_api-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-18 23:47:44.451217 blueair_api-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-18 23:47:30.000000 blueair_api-1.9.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-03-18 23:47:30.000000 blueair_api-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 23:47:44.451217 blueair_api-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-18 23:47:38.000000 blueair_api-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:47:44.447217 blueair_api-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:47:44.451217 blueair_api-1.9.1/src/blueair_api/
--rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/device_aws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/http_aws_blueair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/http_blueair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/util_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-18 23:47:30.000000 blueair_api-1.9.1/src/blueair_api/util_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:47:44.451217 blueair_api-1.9.1/src/blueair_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-18 23:47:44.000000 blueair_api-1.9.1/src/blueair_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-18 23:47:44.000000 blueair_api-1.9.1/src/blueair_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 23:47:44.000000 blueair_api-1.9.1/src/blueair_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 23:47:44.000000 blueair_api-1.9.1/src/blueair_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-18 23:47:44.000000 blueair_api-1.9.1/src/blueair_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:37:06.270020 blueair_api-1.9.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1066 2024-04-18 08:36:53.000000 blueair_api-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-18 08:37:06.270020 blueair_api-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-18 08:36:53.000000 blueair_api-1.9.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-18 08:36:53.000000 blueair_api-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:37:06.270020 blueair_api-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-18 08:37:01.000000 blueair_api-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:37:06.266019 blueair_api-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:37:06.270020 blueair_api-1.9.2/src/blueair_api/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/device_aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/http_aws_blueair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/http_blueair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/util_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-18 08:36:53.000000 blueair_api-1.9.2/src/blueair_api/util_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:37:06.270020 blueair_api-1.9.2/src/blueair_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-18 08:37:06.000000 blueair_api-1.9.2/src/blueair_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 08:37:06.000000 blueair_api-1.9.2/src/blueair_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:37:06.000000 blueair_api-1.9.2/src/blueair_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 08:37:06.000000 blueair_api-1.9.2/src/blueair_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 08:37:06.000000 blueair_api-1.9.2/src/blueair_api.egg-info/top_level.txt
```

### Comparing `blueair_api-1.9.1/LICENSE` & `blueair_api-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/PKG-INFO` & `blueair_api-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueair_api
-Version: 1.9.1
+Version: 1.9.2
 Summary: Blueair Api Wrapper
 Home-page: https://github.com/dahlb/blueair_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 Project-URL: Bug Reports, https://github.com/dahlb/blueair_api/issues
 Project-URL: Source, https://github.com/dahlb/blueair_api
 Keywords: blueair,api
```

### Comparing `blueair_api-1.9.1/README.md` & `blueair_api-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/setup.py` & `blueair_api-1.9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 LONG_DESCRIPTION = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "1.9.1"
+VERSION = "1.9.2"
 
 # Setting up
 setup(
     name="blueair_api",
     version=VERSION,
     author="Brendan Dahl",
     author_email="dahl.brendan@gmail.com",
```

### Comparing `blueair_api-1.9.1/src/blueair_api/callbacks.py` & `blueair_api-1.9.2/src/blueair_api/callbacks.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/const.py` & `blueair_api-1.9.2/src/blueair_api/const.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/device.py` & `blueair_api-1.9.2/src/blueair_api/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
             self.brightness = int(attributes["brightness"])
         else:
             self.brightness = 0
         self.child_lock = bool(attributes["child_lock"])
         if "night_mode" in attributes:
             self.night_mode = bool(attributes["night_mode"])
         self.fan_speed = int(attributes["fan_speed"])
-        self.filter_expired = attributes["filter_status"] != "OK"
+        if "filter_status":
+            self.filter_expired = attributes["filter_status"] != "OK"
+        else:
+            self.filter_expired = None
         self.fan_mode = attributes["mode"]
         if "wifi_status" in attributes:
             self.wifi_working = attributes["wifi_status"] == "1"
         else:
             self.wifi_working = 0
         self.publish_updates()
```

### Comparing `blueair_api-1.9.1/src/blueair_api/device_aws.py` & `blueair_api-1.9.2/src/blueair_api/device_aws.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/http_aws_blueair.py` & `blueair_api-1.9.2/src/blueair_api/http_aws_blueair.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/http_blueair.py` & `blueair_api-1.9.2/src/blueair_api/http_blueair.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/stub.py` & `blueair_api-1.9.2/src/blueair_api/stub.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/util.py` & `blueair_api-1.9.2/src/blueair_api/util.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/util_bootstrap.py` & `blueair_api-1.9.2/src/blueair_api/util_bootstrap.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api/util_http.py` & `blueair_api-1.9.2/src/blueair_api/util_http.py`

 * *Files identical despite different names*

### Comparing `blueair_api-1.9.1/src/blueair_api.egg-info/PKG-INFO` & `blueair_api-1.9.2/src/blueair_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueair_api
-Version: 1.9.1
+Version: 1.9.2
 Summary: Blueair Api Wrapper
 Home-page: https://github.com/dahlb/blueair_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 Project-URL: Bug Reports, https://github.com/dahlb/blueair_api/issues
 Project-URL: Source, https://github.com/dahlb/blueair_api
 Keywords: blueair,api
```

### Comparing `blueair_api-1.9.1/src/blueair_api.egg-info/SOURCES.txt` & `blueair_api-1.9.2/src/blueair_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

