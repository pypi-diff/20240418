# Comparing `tmp/marzpy-0.0.4.tar.gz` & `tmp/marzpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marzpy-0.0.4.tar", last modified: Sun Apr 14 13:52:45 2024, max compression
+gzip compressed data, was "marzpy-0.0.5.tar", last modified: Thu Apr 18 14:53:25 2024, max compression
```

## Comparing `marzpy-0.0.4.tar` & `marzpy-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 13:52:39.000000 marzpy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 13:52:45.113135 marzpy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-14 13:52:39.000000 marzpy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy/api/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/send_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/marzban.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:52:45.113135 marzpy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-14 13:52:39.000000 marzpy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:25.064888 marzpy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 14:53:18.000000 marzpy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 14:53:25.064888 marzpy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-04-18 14:53:18.000000 marzpy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:25.060888 marzpy-0.0.5/marzpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:25.064888 marzpy-0.0.5/marzpy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/send_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 14:53:18.000000 marzpy-0.0.5/marzpy/marzban.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:25.064888 marzpy-0.0.5/marzpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 14:53:25.000000 marzpy-0.0.5/marzpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 14:53:25.000000 marzpy-0.0.5/marzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:53:25.000000 marzpy-0.0.5/marzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 14:53:25.000000 marzpy-0.0.5/marzpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 14:53:25.000000 marzpy-0.0.5/marzpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:53:25.064888 marzpy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 14:53:18.000000 marzpy-0.0.5/setup.py
```

### Comparing `marzpy-0.0.4/LICENSE` & `marzpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/README.md` & `marzpy-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # marzpy
 A Python library that helps you easily use [Marzban](https://github.com/Gozargah/Marzban)'s API panel
 >[!IMPORTANT]
 >**Status:** Working on new update 🔥
 ## installation
 ```shell
-pip install marzpy
+pip install marzpy --upgrade
 ```
 requirements : ```aiohttp```
 # How To Use
 ```python
 from marzpy import Marzban
 import asyncio
         
 async def main():
     panel = Marzban("username","password","https://example.com")
-    token = await await panel.get_token()
-    #await await panel.anyfunction(token)
+    token = await panel.get_token()
+    #await panel.anyfunction(token)
 
 asyncio.run(main())
 
 ```
 # Features
 
 - Admin
@@ -61,15 +61,15 @@
     - [add node](#add-node)
     - [get node](#get-node)
     - [modify node](#modify-node)
     - [remove node](#remove-node)
     - [get all nodes](#get-all-nodes)
     - [reconenct node](#reconenct-node)
     - [get all nodes usage](#get-node-usage)
-    - 
+      
 ## Thanks To 
 
 - [ErfanTech](https://github.com/ErfanTech) :laughing:
 
 # Examples
 ### Get Token
 ```python
@@ -191,14 +191,15 @@
         "vmess": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
         "vless": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
     },
     inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
     expire=0,
     data_limit=0,
     data_limit_reset_strategy="no_reset",
+    status="active"
 )
 result = await panel.add_user(user=user, token=token) #return new User object
 
 print(result.username) #-> Mewhrzad, #user.proxies, #user.inbounds, #user.expire, #user.data_limit, #userdata_limit_reset_strategy, #user.status, #user.used_traffic, #user.lifetime_used_traffic, #user.created_at, #user.links, #user.subscription_url, #user.excluded_inbounds
 ```
 ### Get User
 ```python
@@ -360,8 +361,8 @@
 ### Get Node Usage
 ```python
 result = await panel.get_nodes_usage(token=mytoken)
 for node in result:
     print(node)
 #output:{'node_id': 1, 'node_name': 'N1', 'uplink': 1000000000000, 'downlink': 1000000000000}
 # {'node_id': 2, 'node_name': 'N2', 'uplink': 1000000000000, 'downlink': 1000000000000}
-```
+```
```

### Comparing `marzpy-0.0.4/marzpy/api/admin.py` & `marzpy-0.0.5/marzpy/api/admin.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/core.py` & `marzpy-0.0.5/marzpy/api/core.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/node.py` & `marzpy-0.0.5/marzpy/api/node.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/subscription.py` & `marzpy-0.0.5/marzpy/api/subscription.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/system.py` & `marzpy-0.0.5/marzpy/api/system.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/template.py` & `marzpy-0.0.5/marzpy/api/template.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/marzpy/api/user.py` & `marzpy-0.0.5/marzpy/api/user.py`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.4/setup.py` & `marzpy-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setup(
     name="marzpy",
-    version="0.0.4",
+    version="0.0.5",
     author="Mewhrzad",
     description="a simple application with python to manage Marzban panel",
     long_description="text/markdown",
     url="https://github.com/Mewhrzad/marzpy",
     keywords=["marzpy", "Marzban", "Gozargah", "Marzban python", "Marzban API"],
     packages=find_packages(),
-    ins=["aiohttp"],
+    install_requires=["aiohttp"],
     classifiers=["Programming Language :: Python :: 3"],
 )
```

