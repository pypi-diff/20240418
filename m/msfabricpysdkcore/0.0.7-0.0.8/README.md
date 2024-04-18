# Comparing `tmp/msfabricpysdkcore-0.0.7.tar.gz` & `tmp/msfabricpysdkcore-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.7.tar", last modified: Wed Apr 17 15:03:31 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.8.tar", last modified: Thu Apr 18 12:10:12 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.7.tar` & `msfabricpysdkcore-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.693594 msfabricpysdkcore-0.0.7/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    16383 2024-04-17 15:03:31.690585 msfabricpysdkcore-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.590930 msfabricpysdkcore-0.0.7/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_item.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_workspace.py
--rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/adminapi.py
--rw-rw-rw-   0        0        0     1929 2024-04-12 14:12:32.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/coreapi.py
--rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/domain.py
--rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/onelakeshortcut.py
--rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/otheritems.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.680446 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2048 2024-04-17 14:16:01.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_admin_apis.py
--rw-rw-rw-   0        0        0     4635 2024-04-17 14:16:20.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_domains.py
--rw-rw-rw-   0        0        0     2399 2024-04-17 14:16:25.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0    21117 2024-04-17 14:15:50.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2391 2024-04-17 14:16:33.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6549 2024-04-17 14:16:38.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.686224 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    16383 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-17 14:22:06.000000 msfabricpysdkcore-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 15:03:31.694608 msfabricpysdkcore-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-17 14:22:14.000000 msfabricpysdkcore-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.436507 msfabricpysdkcore-0.0.8/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    16383 2024-04-18 12:10:12.431981 msfabricpysdkcore-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.210181 msfabricpysdkcore-0.0.8/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     2436 2024-04-18 10:49:14.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1197 2024-04-18 10:46:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/onelakeshortcut.py
+-rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/otheritems.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.424012 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-04-17 14:16:01.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4635 2024-04-17 14:16:20.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2399 2024-04-17 14:16:25.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0    21185 2024-04-17 14:45:21.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2391 2024-04-17 14:16:33.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6549 2024-04-17 14:16:38.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.429980 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16383 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-18 12:07:11.000000 msfabricpysdkcore-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:10:12.436507 msfabricpysdkcore-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-18 12:07:06.000000 msfabricpysdkcore-0.0.8/setup.py
```

### Comparing `msfabricpysdkcore-0.0.7/LICENSE` & `msfabricpysdkcore-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/PKG-INFO` & `msfabricpysdkcore-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `msfabricpysdkcore-0.0.7/README.md` & `msfabricpysdkcore-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_item.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_workspace.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/adminapi.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/adminapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import requests
 from abc import abstractmethod
 from azure.identity import AzureCliCredential
-
+try:
+    from notebookutils import mssparkutils
+except ImportError:
+    pass
 class FabricAuth():
     """FabricAuth class to interact with Entra ID"""
 
     @abstractmethod
     def get_token(self):
         """Get token from Azure AD"""
         pass
@@ -54,8 +57,21 @@
             'client_id': f'{self.client_id}',
             'client_secret': f'{self.client_secret}',
             'scope': self.scope
         }
         response = requests.post(url, data=payload)
         access_token = response.json().get('access_token')
         return access_token
-    
+    
+class FabricSparkUtilsAuthentication(FabricAuth):
+    """FabricSparkUtilsAuthentication class to interact with Entra ID"""
+
+    def __init__(self):
+        mssparkutils.credentials.getToken("pbi")
+        print("Using Synapse Spark Utils for authentication")
+
+    def get_token(self):
+        """Get token from Azure AD"""
+        token = mssparkutils.credentials.getToken("pbi")
+        return token.token
+    
+
```

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/capacity.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
 from time import sleep
 
-from msfabricpysdkcore.auth import FabricAuthClient, FabricServicePrincipal
+from msfabricpysdkcore.auth import FabricAuthClient, FabricServicePrincipal, FabricSparkUtilsAuthentication
 
 class FabricClient():
     """FabricClient class to interact with Fabric API"""
 
     def __init__(self, tenant_id = None, client_id = None, client_secret = None) -> None:
         """Initialize FabricClient object"""
         self.tenant_id = tenant_id if tenant_id else os.getenv("FABRIC_TENANT_ID")
         self.client_id = client_id if client_id else os.getenv("FABRIC_CLIENT_ID")
         self.client_secret = client_secret if client_secret else os.getenv("FABRIC_CLIENT_SECRET")
 
+        self.scope = "https://api.fabric.microsoft.com/.default"
+
         if self.client_id is None or self.client_secret is None or self.tenant_id is None:
-            self.auth = FabricAuthClient()
+            try:
+                self.auth = FabricSparkUtilsAuthentication()
+            except:
+                self.auth = FabricAuthClient()
         else:
             self.auth = FabricServicePrincipal(tenant_id = self.tenant_id,
                                                client_id = self.client_id, 
-                                               client_secret = self.client_secret)
-
-        self.scope = "https://api.fabric.microsoft.com/.default"
+                                               client_secret = self.client_secret)
```

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/coreapi.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/coreapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/domain.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/domain.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/job_instance.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/otheritems.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/otheritems.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_admin_apis.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_admin_apis.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_domains.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_items_incl_lakehouse.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_items_incl_lakehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,16 +298,16 @@
         self.assertEqual(status_code, 200)
 
     def test_ml_models(self):
 
         fc = self.fc
         workspace = fc.get_workspace_by_name("testitems")
         workspace_id = workspace.id
-
-        model_name = "mlmodel12345"
+        datetime_str = datetime.now().strftime("%Y%m%d%H%M%S")
+        model_name = "mlm" + datetime_str
 
         ml_model = fc.create_ml_model(workspace_id, display_name=model_name)
         self.assertEqual(ml_model.display_name, model_name)
         
         ml_models = fc.list_ml_models(workspace_id)
         ml_model_names = [ml.display_name for ml in ml_models]
         self.assertGreater(len(ml_models), 0)
```

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_shortcuts.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore/workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.7/pyproject.toml` & `msfabricpysdkcore-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.7"
+version = "0.0.8"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.10"
```

