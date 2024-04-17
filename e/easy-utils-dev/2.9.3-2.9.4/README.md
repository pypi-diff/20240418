# Comparing `tmp/easy_utils_dev-2.9.3.tar.gz` & `tmp/easy_utils_dev-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.3.tar", last modified: Wed Apr 17 21:21:00 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.4.tar", last modified: Wed Apr 17 21:58:04 2024, max compression
```

## Comparing `easy_utils_dev-2.9.3.tar` & `easy_utils_dev-2.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.324983 easy_utils_dev-2.9.3/
--rw-rw-rw-   0        0        0      174 2024-04-17 21:21:00.320772 easy_utils_dev-2.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.280196 easy_utils_dev-2.9.3/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.3/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.3/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.3/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    18363 2024-04-17 21:19:43.000000 easy_utils_dev-2.9.3/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.3/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.3/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.3/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.3/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.3/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.3/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.3/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.3/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.3/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.3/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:21:00.316718 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 21:20:59.000000 easy_utils_dev-2.9.3/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 21:21:00.325985 easy_utils_dev-2.9.3/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-17 21:20:55.000000 easy_utils_dev-2.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:04.732392 easy_utils_dev-2.9.4/
+-rw-rw-rw-   0        0        0      174 2024-04-17 21:58:04.727507 easy_utils_dev-2.9.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:04.662860 easy_utils_dev-2.9.4/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.4/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.4/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.4/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    18691 2024-04-17 21:57:43.000000 easy_utils_dev-2.9.4/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.4/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.4/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.4/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.4/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.4/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.4/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.4/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.4/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.4/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.4/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.4/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.4/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:58:04.722628 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-17 21:58:04.000000 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-17 21:58:04.000000 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:58:04.000000 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 21:58:04.000000 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 21:58:04.000000 easy_utils_dev-2.9.4/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 21:58:04.733367 easy_utils_dev-2.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-17 21:57:56.000000 easy_utils_dev-2.9.4/setup.py
```

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.4/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.4/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.4/easy_utils_dev/cplib.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,22 +132,27 @@
         cli = f"cat /opt/wavesuite/etc/host.info"
         output = subprocess.getoutput(cli).replace('\n' ,'')
         self.logger.debug(f'active host status {output}') 
         if output == 'active':
             return True , output
         elif output == 'inactive' :
             return False , output
+        else :
+            return False , 'NOT_VALID'
 
     def getActiveServer( self , address1 , address2, update_baseurl=True ) :
         self.logger.info(f'Checking active server status: | {address1} | {address2} ')
         isThisServerActive , output =  self.isCurrentServerActive()
         self.logger.info(f'Current server status is {output}')
         allAddresesArray = self.getLinuxIpAddress()
         self.logger.debug(f'all interfaces addresses {allAddresesArray}')
         active_address = ''
+        if output == 'NOT_VALID' :
+            self.logger.error(f"check active server failed due to unexpected HA status. check host.info file in host VM.")
+            raise Exception(f"check active server failed due to unexpected HA status. check host.info file in host VM.")
         if address1 in allAddresesArray :
             self.logger.info(f"This server address is {address1}")
         elif address2 in allAddresesArray :
             self.logger.info(f"This server address is {address2}")
         else :
             self.logger.error(f"Couldn't determine the this server address. whether {address1} or {address2}.")
             raise Exception(f"Couldn't determine the this server address.")
@@ -418,15 +423,14 @@
         self.logger.debug(f'raw response in {jobName} {response.text}')
         if response.status_code == 200 :
             self.logger.debug(f'response is 200 , return the response')
             return response.json().get('id')  , response.json()
         else :
             self.logger.error(f'Error {jobName}  {response.text}')
             return False , {}
-        
 
         
 if __name__ == '__main__':
     pass
```

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.4/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.4/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.4/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.4/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.4/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.4/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.4/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.4/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.4/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.4/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.4/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.4/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.3/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.4/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

