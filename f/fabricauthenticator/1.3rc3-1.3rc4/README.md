# Comparing `tmp/fabricauthenticator-1.3rc3.tar.gz` & `tmp/fabricauthenticator-1.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabricauthenticator-1.3rc3.tar", last modified: Thu Sep  7 18:41:54 2023, max compression
+gzip compressed data, was "fabricauthenticator-1.3rc4.tar", last modified: Thu Sep  7 18:48:27 2023, max compression
```

## Comparing `fabricauthenticator-1.3rc3.tar` & `fabricauthenticator-1.3rc4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-09-07 14:25:42.474476 fabricauthenticator-1.3rc3/.gitignore
--rw-r--r--   0        0        0     1072 2023-09-07 14:25:42.474613 fabricauthenticator-1.3rc3/LICENSE
--rw-r--r--   0        0        0     1164 2023-09-07 14:25:42.474741 fabricauthenticator-1.3rc3/README.md
--rw-r--r--   0        0        0       23 2023-09-07 18:41:32.781200 fabricauthenticator-1.3rc3/fabricauthenticator/__init__.py
--rw-r--r--   0        0        0     8284 2023-09-07 18:41:28.487340 fabricauthenticator-1.3rc3/fabricauthenticator/fabricauthenticator.py
--rw-r--r--   0        0        0      798 2023-09-07 14:25:42.475263 fabricauthenticator-1.3rc3/pyproject.toml
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 fabricauthenticator-1.3rc3/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-09-07 14:25:42.474476 fabricauthenticator-1.3rc4/.gitignore
+-rw-r--r--   0        0        0     1072 2023-09-07 14:25:42.474613 fabricauthenticator-1.3rc4/LICENSE
+-rw-r--r--   0        0        0     1164 2023-09-07 14:25:42.474741 fabricauthenticator-1.3rc4/README.md
+-rw-r--r--   0        0        0       23 2023-09-07 18:48:16.533768 fabricauthenticator-1.3rc4/fabricauthenticator/__init__.py
+-rw-r--r--   0        0        0     8394 2023-09-07 18:48:12.605614 fabricauthenticator-1.3rc4/fabricauthenticator/fabricauthenticator.py
+-rw-r--r--   0        0        0      798 2023-09-07 14:25:42.475263 fabricauthenticator-1.3rc4/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 fabricauthenticator-1.3rc4/PKG-INFO
```

### Comparing `fabricauthenticator-1.3rc3/.gitignore` & `fabricauthenticator-1.3rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.3rc3/LICENSE` & `fabricauthenticator-1.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.3rc3/README.md` & `fabricauthenticator-1.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.3rc3/fabricauthenticator/fabricauthenticator.py` & `fabricauthenticator-1.3rc4/fabricauthenticator/fabricauthenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 in addition checks if user belongs to Fabric JUPYTERHUB COU.
 
 """
 import asyncio
 import concurrent
 import inspect
 import os
+from typing import Union
 
 import oauthenticator
+from ldap3.abstract import entry
 from tornado import web
 from ldap3 import Connection, Server, ALL
 
 
 JUPYTERHUB_COU = os.getenv('FABRIC_COU_JUPYTERHUB', 'CO:COU:Jupyterhub:members:active')
 
 
@@ -130,15 +132,15 @@
             if attributelist['isMemberOf']:
                 for attribute in attributelist['isMemberOf']:
                     if attribute == JUPYTERHUB_COU:
                         return True
         return False
 
     @staticmethod
-    def get_ldap_attributes(email, sub):
+    def get_ldap_attributes(email, sub) -> Union[entry.Entry, None]:
         """ Get the ldap attributes from Fabric CILogon instance.
 
             Args:
                 email: i.e. email
                 sub: i.e. sub
 
             Returns:
@@ -158,15 +160,15 @@
                                     ldap_search_filter,
                                     attributes=[
                                         'isMemberOf', 'uid', 'mail'
                                     ])
         if profile_found:
             attributes = conn.entries[0]
         else:
-            attributes = []
+            attributes = None
         conn.unbind()
         return attributes
 
     def check_username_claim(self, claimlist, resp_json):
         """
         CILogonOAuthenticator expects either ePPN or email to determine JH container user name
         To handle cases where only sub information is available; fetch email from LDAP and set it as username
@@ -183,16 +185,16 @@
 
         # Hack when user claims only has sub
         email = resp_json.get("email")
         sub = resp_json.get("sub")
         if sub is not None:
             attributelist = self.get_ldap_attributes(email, sub)
             if attributelist is not None:
-                self.log.info("attributelist acquired for determining user name.")
-                username = attributelist['mail']
+                self.log.info(f"attributelist acquired for determining user name. {attributelist}")
+                username = str(attributelist['mail'])
 
         if not username:
             if len(claimlist) < 2:
                 self.log.error(
                     "Username claim %s not found in response: %s",
                     self.username_claim,
                     sorted(resp_json.keys()),
```

### Comparing `fabricauthenticator-1.3rc3/pyproject.toml` & `fabricauthenticator-1.3rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.3rc3/PKG-INFO` & `fabricauthenticator-1.3rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabricauthenticator
-Version: 1.3rc3
+Version: 1.3rc4
 Summary: Fabric OAuth Authenticator
 Keywords: Swagger,Fabric OAuth Authenticator
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

