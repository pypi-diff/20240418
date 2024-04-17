# Comparing `tmp/easy_utils_dev-2.9.5.tar.gz` & `tmp/easy_utils_dev-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.5.tar", last modified: Wed Apr 17 22:03:07 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.6.tar", last modified: Wed Apr 17 22:06:11 2024, max compression
```

## Comparing `easy_utils_dev-2.9.5.tar` & `easy_utils_dev-2.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:03:07.930009 easy_utils_dev-2.9.5/
--rw-rw-rw-   0        0        0      174 2024-04-17 22:03:07.924970 easy_utils_dev-2.9.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 22:03:07.870219 easy_utils_dev-2.9.5/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.5/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.5/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.5/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    18664 2024-04-17 22:02:59.000000 easy_utils_dev-2.9.5/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.5/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.5/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.5/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.5/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.5/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.5/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.5/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.5/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.5/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.5/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.5/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.5/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:03:07.919834 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-17 22:03:07.000000 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-17 22:03:07.000000 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:03:07.000000 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-17 22:03:07.000000 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 22:03:07.000000 easy_utils_dev-2.9.5/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 22:03:07.930511 easy_utils_dev-2.9.5/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-17 22:03:04.000000 easy_utils_dev-2.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.140476 easy_utils_dev-2.9.6/
+-rw-rw-rw-   0        0        0      174 2024-04-17 22:06:11.136022 easy_utils_dev-2.9.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.102275 easy_utils_dev-2.9.6/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.6/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.6/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.6/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    18656 2024-04-17 22:05:58.000000 easy_utils_dev-2.9.6/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.6/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.6/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.6/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.6/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.6/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.6/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.6/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.6/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.6/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.133102 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 22:06:11.140476 easy_utils_dev-2.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-17 22:06:06.000000 easy_utils_dev-2.9.6/setup.py
```

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.6/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.6/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.6/easy_utils_dev/cplib.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.port = port
         self.username = username
         self.password = password
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
         self.client_id=client_id
         self.client_secret=client_secret
-        self.baseUrl = self.updateBaseUrl(address , port )
+        self.baseUrl = self.updateBaseUrl(address)
         self.sessions = {}
         self.auth_timestamp = None
 
     def set_debug_level(self , level ) :
         self.logger.set_level(level)    
 
     def updateBaseUrl( self, address ) :
```

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.6/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.6/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.6/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.6/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.6/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.6/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.6/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.6/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.6/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.6/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.6/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.6/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.5/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.6/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

