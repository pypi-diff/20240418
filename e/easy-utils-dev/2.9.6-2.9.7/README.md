# Comparing `tmp/easy_utils_dev-2.9.6.tar.gz` & `tmp/easy_utils_dev-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.6.tar", last modified: Wed Apr 17 22:06:11 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.7.tar", last modified: Wed Apr 17 22:58:52 2024, max compression
```

## Comparing `easy_utils_dev-2.9.6.tar` & `easy_utils_dev-2.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.140476 easy_utils_dev-2.9.6/
--rw-rw-rw-   0        0        0      174 2024-04-17 22:06:11.136022 easy_utils_dev-2.9.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.102275 easy_utils_dev-2.9.6/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.6/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.6/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.6/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    18656 2024-04-17 22:05:58.000000 easy_utils_dev-2.9.6/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.6/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.6/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.6/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.6/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.6/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.6/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.6/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.6/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.6/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.6/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:06:11.133102 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 22:06:10.000000 easy_utils_dev-2.9.6/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 22:06:11.140476 easy_utils_dev-2.9.6/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-17 22:06:06.000000 easy_utils_dev-2.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:58:52.981340 easy_utils_dev-2.9.7/
+-rw-rw-rw-   0        0        0      174 2024-04-17 22:58:52.976462 easy_utils_dev-2.9.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 22:58:52.929051 easy_utils_dev-2.9.7/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.7/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.7/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.7/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    19604 2024-04-17 22:58:43.000000 easy_utils_dev-2.9.7/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.7/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.7/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.7/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.7/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.7/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.7/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.7/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.7/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.7/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.7/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.7/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.7/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:58:52.971582 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-17 22:58:52.000000 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-17 22:58:52.000000 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:58:52.000000 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 22:58:52.000000 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 22:58:52.000000 easy_utils_dev-2.9.7/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 22:58:52.981340 easy_utils_dev-2.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-17 22:58:46.000000 easy_utils_dev-2.9.7/setup.py
```

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.7/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.7/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.7/easy_utils_dev/cplib.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
         self.client_id=client_id
         self.client_secret=client_secret
         self.baseUrl = self.updateBaseUrl(address)
         self.sessions = {}
         self.auth_timestamp = None
+        self.server_address_array = []
+        self.this_server_address = None
 
     def set_debug_level(self , level ) :
         self.logger.set_level(level)    
 
     def updateBaseUrl( self, address ) :
         self.baseUrl = f"https://{address}:{self.port}/wavesuite/cp/admin"
         self.logger.debug(f'baseUrl={self.baseUrl}')
@@ -120,61 +122,80 @@
         if json :
             self.logger.debug(f"json content type is Enabled. adding Content-type as application/json ")
             _h.update({'Content-type': 'application/json'})
         _h.update(headers)
         return _h
 
     def getLinuxIpAddress(self) :
-        return subprocess.getoutput(r"ip addr show | grep inet | awk '{print $2}' | cut -d '/' -f1").splitlines()
+        if self.server_address_array.length == 0 :
+            self.server_address_array = subprocess.getoutput(r"ip addr show | grep inet | awk '{print $2}' | cut -d '/' -f1").splitlines()
+            return self.server_address_array
+        return self.server_address_array
     
+    def getThisServerAddress(self, address1 , address2 ) :
+        if not self.this_server_address :
+            allAddresesArray = self.getLinuxIpAddress()
+            if address1 in allAddresesArray :
+                self.logger.debug(f"This server address is {address1}")
+                self.this_server_address = address1
+                return address1
+            elif address2 in allAddresesArray :
+                self.logger.debug(f"This server address is {address2}")
+                self.this_server_address = address2
+                return address2
+            else :
+                return None
+        return self.this_server_address
+
+    def getRemoteServerAddress( self , address1 , address2 ) :
+        this = self.getThisServerAddress(address1, address2)
+        if address1 == this :
+            return address2
+        elif address2 == this :
+            return address1
+
     def isCurrentServerActive(self) :
         self.logger.info('Checking HA active and standby hosts ..') 
         cli = f"cat /opt/wavesuite/etc/host.info"
         output = subprocess.getoutput(cli).replace('\n' ,'')
         self.logger.debug(f'active host status {output}') 
         if output == 'active':
             return True , output
         elif output == 'inactive' :
             return False , output
         else :
             return False , 'NOT_VALID'
 
+
     def getActiveServer( self , address1 , address2, update_baseurl=True ) :
         self.logger.info(f'Checking active server status: | {address1} | {address2} ')
         isThisServerActive , output =  self.isCurrentServerActive()
         self.logger.info(f'Current server status is {output}')
         allAddresesArray = self.getLinuxIpAddress()
         self.logger.debug(f'all interfaces addresses {allAddresesArray}')
         active_address = ''
+        thisServerAddress = self.getThisServerAddress(address1 , address2 )
         if output == 'NOT_VALID' :
             self.logger.error(f"check active server failed due to unexpected HA status. check host.info file in host VM.")
             raise Exception(f"check active server failed due to unexpected HA status. check host.info file in host VM.")
-        if address1 in allAddresesArray :
-            self.logger.info(f"This server address is {address1}")
-        elif address2 in allAddresesArray :
-            self.logger.info(f"This server address is {address2}")
-        else :
+        self.logger.info(f'this server address is {thisServerAddress}')
+        if not thisServerAddress :
             self.logger.error(f"Couldn't determine the this server address. whether {address1} or {address2}.")
             raise Exception(f"Couldn't determine the this server address.")
+        # if the local address is the active server address.
         if isThisServerActive :
             self.logger.debug(f"in statment where local server is active ..")
-            if address1 in allAddresesArray :
-                active_address = address1
-                self.logger.info(f'Setting [this] {active_address} as active server')
-            elif address2 in allAddresesArray :
-                active_address= address2
-                self.logger.info(f'Setting [this] {active_address} as active server')
+            active_address= self.getThisServerAddress(address1 , address2 )
+            self.logger.info(f'Setting [this] {active_address} as active server')
+        # ######################################################################################        
+        # if the remote address is the active server address.
         elif not isThisServerActive :
             self.logger.debug(f"in statment where remote server is active ..")
-            if address1 in allAddresesArray :
-                active_address= address2 
-                self.logger.info(f'Setting [remote] {active_address} as active server')
-            elif address2 in allAddresesArray :
-                active_address= address1 
-                self.logger.info(f'Setting [remote] {active_address} as active server')
+            active_address= self.getRemoteServerAddress(address1 , address2 )
+            self.logger.info(f'Setting [this] {active_address} as active server')
         if update_baseurl:
             self.updateBaseUrl(active_address)
         self.logger.info(f'Checking active server status: | {address1} | {address2} Completed ')
         return active_address
 
     def logout(self) :
         self.logger.info('Starting to logout form CP platform ..')
```

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.7/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.7/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.7/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.7/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.7/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.7/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.7/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.7/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.7/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.7/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.7/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.7/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.6/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.7/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

