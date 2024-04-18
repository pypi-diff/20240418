# Comparing `tmp/dm_aiomqtt-0.4.1.tar.gz` & `tmp/dm_aiomqtt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.1.tar", last modified: Thu Apr 18 16:03:57 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.2.tar", last modified: Thu Apr 18 16:44:20 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.1.tar` & `dm_aiomqtt-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:57.926432 dm_aiomqtt-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:03:57.926432 dm_aiomqtt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-18 16:03:50.000000 dm_aiomqtt-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:57.922433 dm_aiomqtt-0.4.1/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 16:03:50.000000 dm_aiomqtt-0.4.1/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-18 16:03:50.000000 dm_aiomqtt-0.4.1/dm_aiomqtt/dm_aiomqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:03:57.926432 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:03:57.926432 dm_aiomqtt-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 16:03:57.000000 dm_aiomqtt-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-04-18 16:44:12.000000 dm_aiomqtt-0.4.2/dm_aiomqtt/dm_aiomqtt_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:44:20.637940 dm_aiomqtt-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 16:44:20.000000 dm_aiomqtt-0.4.2/setup.py
```

### Comparing `dm_aiomqtt-0.4.1/PKG-INFO` & `dm_aiomqtt-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.1
+Version: 0.4.2
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.1/README.md` & `dm_aiomqtt-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.1/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.2/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     async def __connect_loop(self) -> None:
         while True:
             try:
                 async with aiomqtt.Client(**self.__mqtt_config) as self.__client:
                     self.__logger.info("Connected!")
                     self.__connected_event.set()
+                    await self.__subscribe()
                     await self.__listen()
             except Exception as e:
                 if self.__connected_event.is_set():
                     self.__logger.error(f"Error: {e}")
                 self.__connected_event.clear()
                 self.__connecting = False
```

### Comparing `dm_aiomqtt-0.4.1/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.2/dm_aiomqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.1
+Version: 0.4.2
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.1/setup.py` & `dm_aiomqtt-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.1',
+    version='v0.4.2',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```

