# Comparing `tmp/aioyoufone-0.3.1.tar.gz` & `tmp/aioyoufone-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioyoufone-0.3.1.tar", last modified: Fri Mar  8 14:59:51 2024, max compression
+gzip compressed data, was "aioyoufone-0.3.2.tar", last modified: Thu Apr 18 12:02:32 2024, max compression
```

## Comparing `aioyoufone-0.3.1.tar` & `aioyoufone-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:51.233726 aioyoufone-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-08 14:59:28.000000 aioyoufone-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-08 14:59:51.233726 aioyoufone-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-08 14:59:28.000000 aioyoufone-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:51.233726 aioyoufone-0.3.1/aioyoufone/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-08 14:59:28.000000 aioyoufone-0.3.1/aioyoufone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-03-08 14:59:28.000000 aioyoufone-0.3.1/aioyoufone/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-08 14:59:28.000000 aioyoufone-0.3.1/aioyoufone/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:51.233726 aioyoufone-0.3.1/aioyoufone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-08 14:59:51.000000 aioyoufone-0.3.1/aioyoufone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-08 14:59:51.000000 aioyoufone-0.3.1/aioyoufone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:59:51.000000 aioyoufone-0.3.1/aioyoufone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-08 14:59:51.000000 aioyoufone-0.3.1/aioyoufone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 14:59:51.000000 aioyoufone-0.3.1/aioyoufone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-08 14:59:51.233726 aioyoufone-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-08 14:59:31.000000 aioyoufone-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:32.269875 aioyoufone-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 12:02:12.000000 aioyoufone-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 12:02:32.269875 aioyoufone-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-18 12:02:12.000000 aioyoufone-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:32.265875 aioyoufone-0.3.2/aioyoufone/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:02:12.000000 aioyoufone-0.3.2/aioyoufone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-04-18 12:02:12.000000 aioyoufone-0.3.2/aioyoufone/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-18 12:02:12.000000 aioyoufone-0.3.2/aioyoufone/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:32.265875 aioyoufone-0.3.2/aioyoufone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 12:02:32.000000 aioyoufone-0.3.2/aioyoufone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:02:32.000000 aioyoufone-0.3.2/aioyoufone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:02:32.000000 aioyoufone-0.3.2/aioyoufone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:02:32.000000 aioyoufone-0.3.2/aioyoufone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 12:02:32.000000 aioyoufone-0.3.2/aioyoufone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-18 12:02:32.269875 aioyoufone-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-18 12:02:14.000000 aioyoufone-0.3.2/setup.py
```

### Comparing `aioyoufone-0.3.1/LICENSE` & `aioyoufone-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioyoufone-0.3.1/PKG-INFO` & `aioyoufone-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioyoufone
-Version: 0.3.1
+Version: 0.3.2
 Summary: Module to communicate to the Youfone API
 Home-page: https://github.com/geertmeersman/aioyoufone
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # aioyoufone
 
 Asynchronous library to communicate with the Youfone API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/s8JNwREmxV)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/aioyoufone?style=flat-square)](https://github.com/geertmeersman/aioyoufone/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aioyoufone)](https://github.com/geertmeersman/aioyoufone/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
@@ -47,15 +47,14 @@
 # Setup logging
 logger = logging.getLogger(__name__)
 
 async def main():
     client = YoufoneClient(
         "user@email.com",
         "YourPassword",
-        "nl",
         None,
         True
     )
 
     try:
         customer_data = await client.fetch_data()
         if isinstance(customer_data, dict) and 'error' in customer_data:
```

### Comparing `aioyoufone-0.3.1/README.md` & `aioyoufone-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # aioyoufone
 
 Asynchronous library to communicate with the Youfone API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/s8JNwREmxV)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/aioyoufone?style=flat-square)](https://github.com/geertmeersman/aioyoufone/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aioyoufone)](https://github.com/geertmeersman/aioyoufone/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
@@ -33,15 +33,14 @@
 # Setup logging
 logger = logging.getLogger(__name__)
 
 async def main():
     client = YoufoneClient(
         "user@email.com",
         "YourPassword",
-        "nl",
         None,
         True
     )
 
     try:
         customer_data = await client.fetch_data()
         if isinstance(customer_data, dict) and 'error' in customer_data:
```

### Comparing `aioyoufone-0.3.1/aioyoufone/client.py` & `aioyoufone-0.3.2/aioyoufone/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,56 +5,41 @@
 """
 
 from datetime import datetime, timedelta
 import logging
 
 import httpx
 
-from .const import API_BASE_URL, API_HEADERS, COUNTRY_CHOICES, DEFAULT_COUNTRY
+from .const import API_BASE_URL, API_HEADERS
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class YoufoneClient:
     """Class to communicate with the Youfone API."""
 
-    def __init__(self, email, password, country, custom_headers=None, debug=False):
+    def __init__(self, email, password, custom_headers=None, debug=False):
         """Initialize the API to get data.
 
         Args:
         ----
             email (str): The email associated with the Youfone account.
             password (str): The password associated with the Youfone account.
-            country (str): The country code for the Youfone account.
             custom_headers (dict, optional): Custom headers for HTTP requests. Defaults to None.
             debug (bool, optional): Whether to enable debug mode. Defaults to False.
 
         """
         self.email = email
         self.password = password
-        self.country = None
         self.client = None
         self.customer = None
         self.customer_id = None
         self.security_key = None  # Store the security key
         self.custom_headers = custom_headers or {}
         self.debug = debug  # Set debug mode
-        if country not in COUNTRY_CHOICES:
-            self.country = DEFAULT_COUNTRY
-        else:
-            self.country = country
-        self.base_api_endpoint = API_BASE_URL.replace(
-            f"youfone.{DEFAULT_COUNTRY}", f"youfone.{self.country}"
-        )
-
-        # Update API_HEADERS based on self.country
-        for key, value in API_HEADERS.items():
-            API_HEADERS[key] = value.replace(
-                f"youfone.{DEFAULT_COUNTRY}", f"youfone.{self.country}"
-            )
 
     async def start_session(self):
         """Start the httpx session."""
         if self.client is None:
             self.client = httpx.AsyncClient(headers=self.custom_headers, http2=True)
 
     async def close_session(self):
```

### Comparing `aioyoufone-0.3.1/aioyoufone.egg-info/PKG-INFO` & `aioyoufone-0.3.2/aioyoufone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioyoufone
-Version: 0.3.1
+Version: 0.3.2
 Summary: Module to communicate to the Youfone API
 Home-page: https://github.com/geertmeersman/aioyoufone
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # aioyoufone
 
 Asynchronous library to communicate with the Youfone API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/s8JNwREmxV)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/aioyoufone?style=flat-square)](https://github.com/geertmeersman/aioyoufone/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aioyoufone)](https://github.com/geertmeersman/aioyoufone/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aioyoufone.svg)](http://isitmaintained.com/project/geertmeersman/aioyoufone)
@@ -47,15 +47,14 @@
 # Setup logging
 logger = logging.getLogger(__name__)
 
 async def main():
     client = YoufoneClient(
         "user@email.com",
         "YourPassword",
-        "nl",
         None,
         True
     )
 
     try:
         customer_data = await client.fetch_data()
         if isinstance(customer_data, dict) and 'error' in customer_data:
```

### Comparing `aioyoufone-0.3.1/setup.cfg` & `aioyoufone-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioyoufone-0.3.1/setup.py` & `aioyoufone-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.3.1",
+    version="v0.3.2",
 )
```

