# Comparing `tmp/grpcio-status-1.62.1.tar.gz` & `tmp/grpcio-status-1.63.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-status-1.62.1.tar", last modified: Fri Mar  8 00:12:17 2024, max compression
+gzip compressed data, was "grpcio-status-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:45 2024, max compression
```

## Comparing `grpcio-status-1.62.1.tar` & `grpcio-status-1.63.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:12:17.184146 grpcio-status-1.62.1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1318 2024-03-08 00:12:17.184146 grpcio-status-1.62.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:12:17.180146 grpcio-status-1.62.1/grpc_status/
--rw-r--r--   0 root         (0) root         (0)      580 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/grpc_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/grpc_status/_async.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/grpc_status/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:12:17.172146 grpcio-status-1.62.1/grpc_status/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:12:17.180146 grpcio-status-1.62.1/grpc_status/google/rpc/
--rw-r--r--   0 root         (0) root         (0)     1924 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpc_status/google/rpc/status.proto
--rw-r--r--   0 root         (0) root         (0)     2992 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/grpc_status/rpc_status.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:12:17.180146 grpcio-status-1.62.1/grpcio_status.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1318 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpcio_status.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpcio_status.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpcio_status.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpcio_status.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-08 00:12:17.000000 grpcio-status-1.62.1/grpcio_status.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 00:12:17.184146 grpcio-status-1.62.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-08 00:03:28.000000 grpcio-status-1.62.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.626782 grpcio-status-1.63.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpc_status/
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/_async.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.610780 grpcio-status-1.63.0rc1/grpc_status/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpc_status/google/rpc/
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpc_status/google/rpc/status.proto
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/rpc_status.py
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpcio_status.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:45.626782 grpcio-status-1.63.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/setup.py
```

### Comparing `grpcio-status-1.62.1/LICENSE` & `grpcio-status-1.63.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/PKG-INFO` & `grpcio-status-1.63.0rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.62.1
+Version: 1.63.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.62.1
+Requires-Dist: grpcio>=1.63.0rc1
 Requires-Dist: googleapis-common-protos>=1.5.5
 
 gRPC Python Status Proto
 ===========================
 
 Reference package for GRPC Python status proto mapping.
 
 Supported Python Versions
 -------------------------
-Python >= 3.7
+Python >= 3.8
 
 Dependencies
 ------------
 
 Depends on the `grpcio` package, available from PyPI via `pip install grpcio`.
```

### Comparing `grpcio-status-1.62.1/grpc_status/__init__.py` & `grpcio-status-1.63.0rc1/grpc_status/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/grpc_status/_async.py` & `grpcio-status-1.63.0rc1/grpc_status/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/grpc_status/_common.py` & `grpcio-status-1.63.0rc1/grpc_status/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/grpc_status/google/rpc/status.proto` & `grpcio-status-1.63.0rc1/grpc_status/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/grpc_status/rpc_status.py` & `grpcio-status-1.63.0rc1/grpc_status/rpc_status.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.62.1/grpcio_status.egg-info/PKG-INFO` & `grpcio-status-1.63.0rc1/grpcio_status.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.62.1
+Version: 1.63.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.62.1
+Requires-Dist: grpcio>=1.63.0rc1
 Requires-Dist: googleapis-common-protos>=1.5.5
 
 gRPC Python Status Proto
 ===========================
 
 Reference package for GRPC Python status proto mapping.
 
 Supported Python Versions
 -------------------------
-Python >= 3.7
+Python >= 3.8
 
 Dependencies
 ------------
 
 Depends on the `grpcio` package, available from PyPI via `pip install grpcio`.
```

### Comparing `grpcio-status-1.62.1/setup.py` & `grpcio-status-1.63.0rc1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,18 +43,14 @@
         pass
 
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -93,11 +89,11 @@
     author="The gRPC Authors",
     author_email="grpc-io@googlegroups.com",
     url="https://grpc.io",
     license="Apache License 2.0",
     classifiers=CLASSIFIERS,
     package_dir=PACKAGE_DIRECTORIES,
     packages=setuptools.find_packages("."),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     cmdclass=COMMAND_CLASS,
 )
```

