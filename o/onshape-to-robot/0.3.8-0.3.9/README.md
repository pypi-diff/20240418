# Comparing `tmp/onshape-to-robot-0.3.8.tar.gz` & `tmp/onshape-to-robot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onshape-to-robot-0.3.8.tar", last modified: Fri Feb 26 13:23:15 2021, max compression
+gzip compressed data, was "dist/onshape-to-robot-0.3.9.tar", last modified: Tue Mar  2 11:07:17 2021, max compression
```

## Comparing `onshape-to-robot-0.3.8.tar` & `onshape-to-robot-0.3.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      408 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1098 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/setup.cfg
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2021-02-26 13:23:14.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1098 2021-02-26 13:23:14.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      870 2021-02-26 13:23:14.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       68 2021-02-26 13:23:14.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       17 2021-02-26 13:23:14.000000 onshape-to-robot-0.3.8/onshape_to_robot.egg-info/top_level.txt
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      211 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape-to-robot-clear-cache
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/onshape_to_robot/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    16040 2020-12-28 17:46:48.000000 onshape-to-robot-0.3.8/onshape_to_robot/simulation.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      793 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/edit_shape.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5142 2021-02-26 13:18:00.000000 onshape-to-robot-0.3.8/onshape_to_robot/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14017 2021-02-26 13:16:44.000000 onshape-to-robot-0.3.8/onshape_to_robot/load_robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4793 2020-09-18 16:22:44.000000 onshape-to-robot-0.3.8/onshape_to_robot/pure_sketch.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-02-26 13:23:15.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11797 2021-02-17 15:29:22.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8266 2021-02-17 12:54:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/onshape.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1713 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      267 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/__init__.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     1891 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/bullet.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3971 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/csg.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3217 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/stl_combine.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3523 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/features.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       33 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape_to_robot/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    20114 2021-02-09 22:43:56.000000 onshape-to-robot-0.3.8/onshape_to_robot/robot_description.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     8780 2020-12-02 08:51:02.000000 onshape-to-robot-0.3.8/onshape_to_robot/onshape_to_robot.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       65 2020-09-18 15:49:45.000000 onshape-to-robot-0.3.8/onshape-to-robot-pure-sketch
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1181 2021-02-26 13:23:12.000000 onshape-to-robot-0.3.8/setup.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       70 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape-to-robot
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       60 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape-to-robot-bullet
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       64 2020-08-27 08:30:51.000000 onshape-to-robot-0.3.8/onshape-to-robot-edit-shape
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       64 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape-to-robot-edit-shape
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/setup.cfg
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       70 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape-to-robot
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      870 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1098 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       68 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       17 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot.egg-info/top_level.txt
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       65 2020-09-18 09:56:33.000000 onshape-to-robot-0.3.9/onshape-to-robot-pure-sketch
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    16040 2021-03-02 11:02:47.000000 onshape-to-robot-0.3.9/onshape_to_robot/simulation.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5142 2021-03-02 11:02:47.000000 onshape-to-robot-0.3.9/onshape_to_robot/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      793 2020-10-14 08:42:36.000000 onshape-to-robot-0.3.9/onshape_to_robot/edit_shape.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3971 2020-10-14 08:42:39.000000 onshape-to-robot-0.3.9/onshape_to_robot/csg.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13783 2021-03-02 11:06:32.000000 onshape-to-robot-0.3.9/onshape_to_robot/load_robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4793 2020-10-22 16:06:20.000000 onshape-to-robot-0.3.9/onshape_to_robot/pure_sketch.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       33 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape_to_robot/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    20114 2021-03-02 11:02:47.000000 onshape-to-robot-0.3.9/onshape_to_robot/robot_description.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3217 2020-10-14 10:01:59.000000 onshape-to-robot-0.3.9/onshape_to_robot/stl_combine.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3523 2020-10-21 16:40:12.000000 onshape-to-robot-0.3.9/onshape_to_robot/features.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11797 2021-03-02 11:02:47.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      267 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8266 2021-03-02 11:02:47.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/onshape.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1713 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/utils.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     8780 2020-10-22 16:16:50.000000 onshape-to-robot-0.3.9/onshape_to_robot/onshape_to_robot.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     1891 2020-10-14 08:42:15.000000 onshape-to-robot-0.3.9/onshape_to_robot/bullet.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      211 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape-to-robot-clear-cache
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       60 2020-07-02 08:39:55.000000 onshape-to-robot-0.3.9/onshape-to-robot-bullet
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1098 2021-03-02 11:07:17.000000 onshape-to-robot-0.3.9/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      408 2020-10-12 13:58:28.000000 onshape-to-robot-0.3.9/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1181 2021-03-02 11:06:45.000000 onshape-to-robot-0.3.9/setup.py
```

### Comparing `onshape-to-robot-0.3.8/PKG-INFO` & `onshape-to-robot-0.3.9/onshape_to_robot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onshape-to-robot
-Version: 0.3.8
+Version: 0.3.9
 Summary: Converting OnShape assembly to robot definition (SDF or URDF) through OnShape API 
 Home-page: https://github.com/rhoban/onshape-to-robot/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Description: # Onshape to robot (URDF/SDF)
```

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot.egg-info/PKG-INFO` & `onshape-to-robot-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onshape-to-robot
-Version: 0.3.8
+Version: 0.3.9
 Summary: Converting OnShape assembly to robot definition (SDF or URDF) through OnShape API 
 Home-page: https://github.com/rhoban/onshape-to-robot/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Description: # Onshape to robot (URDF/SDF)
```

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot.egg-info/SOURCES.txt` & `onshape-to-robot-0.3.9/onshape_to_robot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/simulation.py` & `onshape-to-robot-0.3.9/onshape_to_robot/simulation.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/edit_shape.py` & `onshape-to-robot-0.3.9/onshape_to_robot/edit_shape.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/config.py` & `onshape-to-robot-0.3.9/onshape_to_robot/config.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/load_robot.py` & `onshape-to-robot-0.3.9/onshape_to_robot/load_robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 
 # If a versionId is provided, it will be used, else the main workspace is retrieved
 if config['versionId'] != '':
     print("\n" + Style.BRIGHT + '* Using configuration version ID ' +
           config['versionId']+' ...' + Style.RESET_ALL)
 elif config['workspaceId'] != '':
     print("\n" + Style.BRIGHT + '* Using configuration workspace ID ' +
-          config['workspace']+' ...' + Style.RESET_ALL)
+          config['workspaceId']+' ...' + Style.RESET_ALL)
+    workspaceId = config['workspaceId']
 else:
     print("\n" + Style.BRIGHT + '* Retrieving workspace ID ...' + Style.RESET_ALL)
     document = client.get_document(config['documentId']).json()
     workspaceId = document['defaultWorkspace']['id']
     print(Fore.GREEN + "+ Using workspace id: " + workspaceId + Style.RESET_ALL)
 
 # Now, finding the assembly, according to given name in configuration, or else the first possible one
 print("\n" + Style.BRIGHT +
       '* Retrieving elements in the document, searching for the assembly...' + Style.RESET_ALL)
 if config['versionId'] != '':
     elements = client.list_elements(
         config['documentId'], config['versionId'], 'v').json()
-elif config['workspaceId'] != '':
-    elements = client.list_elements(
-        config['documentId'], config['workspaceId'], 'w').json()
 else:
     elements = client.list_elements(config['documentId'], workspaceId).json()
 assemblyId = None
 assemblyName = ''
 for element in elements:
     if element['type'] == 'Assembly' and \
             (config['assemblyName'] is False or element['name'] == config['assemblyName']):
@@ -50,17 +48,14 @@
 
 # Retrieving the assembly
 print("\n" + Style.BRIGHT + '* Retrieving assembly "' +
       assemblyName+'" with id '+assemblyId + Style.RESET_ALL)
 if config['versionId'] != '':
     assembly = client.get_assembly(
         config['documentId'], config['versionId'], assemblyId, 'v')
-elif config['workspaceId'] != '':
-    assembly = client.get_assembly(
-        config['documentId'], config['workspaceId'], assemblyId, 'w')
 else:
     assembly = client.get_assembly(
         config['documentId'], workspaceId, assemblyId)
 
 root = assembly['rootAssembly']
 
 # Finds a (leaf) instance given the full path, typically A B C where A and B would be subassemblies and C
```

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/pure_sketch.py` & `onshape-to-robot-0.3.9/onshape_to_robot/pure_sketch.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/client.py` & `onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/client.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/onshape.py` & `onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/onshape.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/onshape_api/utils.py` & `onshape-to-robot-0.3.9/onshape_to_robot/onshape_api/utils.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/bullet.py` & `onshape-to-robot-0.3.9/onshape_to_robot/bullet.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/csg.py` & `onshape-to-robot-0.3.9/onshape_to_robot/csg.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/stl_combine.py` & `onshape-to-robot-0.3.9/onshape_to_robot/stl_combine.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/features.py` & `onshape-to-robot-0.3.9/onshape_to_robot/features.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/robot_description.py` & `onshape-to-robot-0.3.9/onshape_to_robot/robot_description.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/onshape_to_robot/onshape_to_robot.py` & `onshape-to-robot-0.3.9/onshape_to_robot/onshape_to_robot.py`

 * *Files identical despite different names*

### Comparing `onshape-to-robot-0.3.8/setup.py` & `onshape-to-robot-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README-pypi.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="onshape-to-robot",
-    version="0.3.8",
+    version="0.3.9",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Converting OnShape assembly to robot definition (SDF or URDF) through OnShape API ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/onshape-to-robot/",
     packages=setuptools.find_packages(),
```

