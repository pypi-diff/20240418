# Comparing `tmp/mh-en-exec-1.0.2.tar.gz` & `tmp/mh_en_exec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\Work\Projects\MH\external_node_executor\dist\tmpypjolsdv\mh-en-exec-1.0.2.tar", last modified: Thu Jan 25 09:00:07 2024, max compression
+gzip compressed data, was "mh_en_exec-1.0.3.tar", last modified: Wed Apr 17 03:42:31 2024, max compression
```

## Comparing `mh-en-exec-1.0.2.tar` & `mh_en_exec-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/
--rw-rw-rw-   0        0        0     1086 2024-01-25 06:49:55.000000 mh-en-exec-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1469 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      941 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      957 2024-01-25 06:51:31.000000 mh-en-exec-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec/
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/
--rw-rw-rw-   0        0        0     3523 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_base.py
--rw-rw-rw-   0        0        0     5215 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_grpc.py
--rw-rw-rw-   0        0        0    42690 2024-01-25 02:03:04.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_pb2.py
--rw-rw-rw-   0        0        0    15326 2024-01-25 06:23:44.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_pb2_grpc.py
--rw-rw-rw-   0        0        0      183 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/connection/__init__.py
--rw-rw-rw-   0        0        0     3118 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/main.py
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/
--rw-rw-rw-   0        0        0    21768 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/common.py
--rw-rw-rw-   0        0        0       54 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/constants.py
--rw-rw-rw-   0        0        0      142 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/exceptions.py
--rw-rw-rw-   0        0        0    11418 2024-01-25 08:59:50.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_base.py
--rw-rw-rw-   0        0        0     1305 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_factory.py
--rw-rw-rw-   0        0        0     3134 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_manager.py
--rw-rw-rw-   0        0        0    13305 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/ports.py
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/views/
--rw-rw-rw-   0        0        0     8151 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/views/__init__.py
--rw-rw-rw-   0        0        0      110 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec/resource/
--rw-rw-rw-   0        0        0     5749 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/resource/resource_manager_grpc.py
--rw-rw-rw-   0        0        0       95 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/resource/__init__.py
--rw-rw-rw-   0        0        0      671 2024-01-24 09:45:12.000000 mh-en-exec-1.0.2/src/mh_en_exec/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-25 06:52:36.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1469 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/requires.txt
--rw-rw-rw-   0        0        0      933 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2024-01-25 09:00:07.000000 mh-en-exec-1.0.2/src/mh_en_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.725776 mh_en_exec-1.0.3/
+-rw-rw-rw-   0        0        0     1086 2024-01-25 06:49:55.000000 mh_en_exec-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1554 2024-04-17 03:42:31.724774 mh_en_exec-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 03:42:31.725776 mh_en_exec-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      957 2024-04-17 03:26:16.000000 mh_en_exec-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.695948 mh_en_exec-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.699458 mh_en_exec-1.0.3/src/mh_en_exec/
+-rw-rw-rw-   0        0        0      671 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.717482 mh_en_exec-1.0.3/src/mh_en_exec/connection/
+-rw-rw-rw-   0        0        0      183 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/connection/__init__.py
+-rw-rw-rw-   0        0        0     3523 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_base.py
+-rw-rw-rw-   0        0        0     5215 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_grpc.py
+-rw-rw-rw-   0        0        0     6560 2024-04-17 03:25:13.000000 mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_pb2.py
+-rw-rw-rw-   0        0        0    15326 2024-04-17 03:42:21.000000 mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3118 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.722775 mh_en_exec-1.0.3/src/mh_en_exec/nodes/
+-rw-rw-rw-   0        0        0      110 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/__init__.py
+-rw-rw-rw-   0        0        0    21768 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/common.py
+-rw-rw-rw-   0        0        0       54 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/constants.py
+-rw-rw-rw-   0        0        0      142 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/exceptions.py
+-rw-rw-rw-   0        0        0    11418 2024-01-25 08:59:50.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_base.py
+-rw-rw-rw-   0        0        0     1305 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_factory.py
+-rw-rw-rw-   0        0        0     3134 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_manager.py
+-rw-rw-rw-   0        0        0    13305 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/ports.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.722775 mh_en_exec-1.0.3/src/mh_en_exec/nodes/views/
+-rw-rw-rw-   0        0        0     8151 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/nodes/views/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.723775 mh_en_exec-1.0.3/src/mh_en_exec/resource/
+-rw-rw-rw-   0        0        0       95 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/resource/__init__.py
+-rw-rw-rw-   0        0        0     5749 2024-01-24 09:45:12.000000 mh_en_exec-1.0.3/src/mh_en_exec/resource/resource_manager_grpc.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:42:31.724774 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/
+-rw-rw-rw-   0        0        0     1554 2024-04-17 03:42:31.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2024-04-17 03:42:31.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 03:42:31.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-25 06:52:36.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-04-17 03:42:31.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:42:31.000000 mh_en_exec-1.0.3/src/mh_en_exec.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mh-en-exec-1.0.2/LICENSE` & `mh_en_exec-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/PKG-INFO` & `mh_en_exec-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: mh-en-exec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for executing machine heads external nodes
 Home-page: https://mheads.net/external_nodes
 Author: Opus
 Author-email: mh@opus.co.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio>=1.62.1
+Requires-Dist: grpcio-tools>=1.62.1
+Requires-Dist: opencv-python>=4.9.0.80
 
 # Machine Heads External Nodes
 
 ## Getting Started
 
 **Machine Heads External Nodes** is a python module for creating your own nodes for use on [Machine Heads](https://mheads.net).
 Using *External Nodes* you will be able to:
@@ -40,9 +42,7 @@
 
 There is also a sample code in the "examples" folder.
 To execute sample code, just install "mh_en_exec" and call the following command:
 
 ```
 python run.py
 ```
-
-
```

### Comparing `mh-en-exec-1.0.2/README.md` & `mh_en_exec-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/setup.py` & `mh_en_exec-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='mh-en-exec',
-  version='1.0.2',
+  version='1.0.3',
   description='Package for executing machine heads external nodes',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://mheads.net/external_nodes',
   author='Opus',
   author_email='mh@opus.co.jp',
   license='MIT',
   package_dir={"": "src"},
   packages=['mh_en_exec', 'mh_en_exec.connection', 'mh_en_exec.nodes', 'mh_en_exec.nodes.views', 'mh_en_exec.resource'],
   zip_safe=False,
   install_requires=[
-      'grpcio>=1.48.2',
-      'grpcio-tools>=1.48.2',
-      'opencv-python>=4.1.2.30'
+      'grpcio>=1.62.1',
+      'grpcio-tools>=1.62.1',
+      'opencv-python>=4.9.0.80'
   ],
   classifiers=[
       'Development Status :: 3 - Alpha',
       'License :: OSI Approved :: MIT License',
       'Programming Language :: Python :: 3',
       'Operating System :: OS Independent'
   ],
-  python_requires=">=3.6"
+  python_requires=">=3.9"
 )
```

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_base.py` & `mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_base.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_grpc.py` & `mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_grpc.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/connection/connection_pb2_grpc.py` & `mh_en_exec-1.0.3/src/mh_en_exec/connection/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/main.py` & `mh_en_exec-1.0.3/src/mh_en_exec/main.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/common.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/common.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_base.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_base.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_factory.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_factory.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/node_manager.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/node_manager.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/ports.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/ports.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/nodes/views/__init__.py` & `mh_en_exec-1.0.3/src/mh_en_exec/nodes/views/__init__.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/resource/resource_manager_grpc.py` & `mh_en_exec-1.0.3/src/mh_en_exec/resource/resource_manager_grpc.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec/__init__.py` & `mh_en_exec-1.0.3/src/mh_en_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec.egg-info/PKG-INFO` & `mh_en_exec-1.0.3/src/mh_en_exec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: mh-en-exec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for executing machine heads external nodes
 Home-page: https://mheads.net/external_nodes
 Author: Opus
 Author-email: mh@opus.co.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio>=1.62.1
+Requires-Dist: grpcio-tools>=1.62.1
+Requires-Dist: opencv-python>=4.9.0.80
 
 # Machine Heads External Nodes
 
 ## Getting Started
 
 **Machine Heads External Nodes** is a python module for creating your own nodes for use on [Machine Heads](https://mheads.net).
 Using *External Nodes* you will be able to:
@@ -40,9 +42,7 @@
 
 There is also a sample code in the "examples" folder.
 To execute sample code, just install "mh_en_exec" and call the following command:
 
 ```
 python run.py
 ```
-
-
```

### Comparing `mh-en-exec-1.0.2/src/mh_en_exec.egg-info/SOURCES.txt` & `mh_en_exec-1.0.3/src/mh_en_exec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

