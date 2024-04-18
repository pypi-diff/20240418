# Comparing `tmp/trustauthx-0.7.3.tar.gz` & `tmp/trustauthx-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.7.3.tar", last modified: Fri Apr  5 17:58:18 2024, max compression
+gzip compressed data, was "trustauthx-0.8.1.tar", last modified: Thu Apr 18 14:36:46 2024, max compression
```

## Comparing `trustauthx-0.7.3.tar` & `trustauthx-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 17:58:09.000000 trustauthx-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-05 17:58:18.140673 trustauthx-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-05 17:58:09.000000 trustauthx-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:18.140673 trustauthx-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-05 17:58:09.000000 trustauthx-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.136673 trustauthx-0.7.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 17:58:09.000000 trustauthx-0.7.3/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41319 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-05 17:58:09.000000 trustauthx-0.7.3/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:18.140673 trustauthx-0.7.3/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 17:58:18.000000 trustauthx-0.7.3/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 14:36:37.000000 trustauthx-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-18 14:36:46.079297 trustauthx-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-18 14:36:37.000000 trustauthx-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:36:46.079297 trustauthx-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-18 14:36:37.000000 trustauthx-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.075297 trustauthx-0.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 14:36:37.000000 trustauthx-0.8.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41392 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.7.3/LICENSE` & `trustauthx-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.3/PKG-INFO` & `trustauthx-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.3
+Version: 0.8.1
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.7.3/README.md` & `trustauthx-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.3/setup.py` & `trustauthx-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="trustauthx",
-    version="0.7.3",
+    version="0.8.1",
     description="Official connector SDK for TrustAuthx",
     long_description=long_description,
     long_description_content_type="text/markdown",  # This is important!
     author="moonlightnexus",
     author_email="nexus@trustauthx.com",
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.7.3/trustauthx/authlite.py` & `trustauthx-0.8.1/trustauthx/authlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import sqlite3
 import threading
 from dataclasses import asdict
 from functools import wraps
 from lib2to3.pgen2.parse import ParseError
+from typing import Union
 
 import requests
 from jose import JWTError, jwt
 from jose.constants import ALGORITHMS
 from requests.exceptions import HTTPError
 
 from .scheme import *
@@ -683,15 +684,15 @@
         else:
             raise HTTPError(
                 "Request failed with status code : {} \n this code contains a msg : {}".format(
                     response.status_code, response.text
                 )
             )
 
-    def get_user(self, token, return_class=False) -> User | dict:
+    def get_user(self, token, return_class=False) -> Union[User, dict]:
         """
         Validates the given authentication token and returns user data.
 
         Args:
             token (str): The authentication token to validate.
 
         Returns:
@@ -915,20 +916,20 @@
             InMemory=self.in_memory,
         )
         return self.Roles
 
     def attach_role(
         self,
         uid: str,
-        rol_ids: str | list,
+        rol_ids: Union[str, list],
         signoff_session_and_assign=False,
         refresh_token=None,
         access_token=None,
         return_class: bool = False,
-    ) -> dict | SignOffSessionReplace:
+    ) -> Union[dict, SignOffSessionReplace]:
         """
         Attaches a role to a user.
 
         Args:
             uid (str): The user ID to attach the role to.
             rol_ids (str | list): The ID(s) of the role(s) to attach.
             signoff_session_and_assign (bool, optional): Whether to sign off the session and assign. Default is False.
@@ -980,20 +981,20 @@
                 return SignOffSessionReplace(response.json())
             else:
                 return SignOffSessionReplace(response.json()).to_dict()
 
     def remove_role(
         self,
         uid: str,
-        rol_ids: str | list,
+        rol_ids: Union[str, list],
         signoff_session_and_assign=False,
         refresh_token=None,
         access_token=None,
         return_class: bool = False,
-    ) -> dict | SignOffSessionReplace:
+    ) -> Union[dict, SignOffSessionReplace]:
         """
         Removes a role from a user.
 
         Args:
             uid (str): The user ID to remove the role from.
             rol_ids (str | list): The ID(s) of the role(s) to remove.
             signoff_session_and_assign (bool, optional): Whether to sign off the session and assign. Default is False.
@@ -1045,21 +1046,21 @@
                 return SignOffSessionReplace(response.json())
             else:
                 return SignOffSessionReplace(response.json()).to_dict()
 
     def update_role(
         self,
         uid: str,
-        rol_ids_to_add: str | list,
-        rol_ids_to_remove: str | list,
+        rol_ids_to_add: Union[str, list],
+        rol_ids_to_remove: Union[str, list],
         signoff_session_and_assign=False,
         refresh_token=None,
         access_token=None,
         return_class: bool = False,
-    ) -> dict | SignOffSessionReplace:
+    ) -> Union[dict, SignOffSessionReplace]:
         """
         Updates a user's roles by adding and/or removing roles.
 
         Args:
             uid (str): The user ID to update roles for.
             rol_ids_to_add (str | list): The ID(s) of the role(s) to add.
             rol_ids_to_remove (str | list): The ID(s) of the role(s) to remove.
```

### Comparing `trustauthx-0.7.3/trustauthx/cli.py` & `trustauthx-0.8.1/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.3/trustauthx/llmai.py` & `trustauthx-0.8.1/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.3/trustauthx/scheme.py` & `trustauthx-0.8.1/trustauthx/scheme.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.3/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.8.1/trustauthx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.3
+Version: 0.8.1
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

