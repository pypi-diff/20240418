# Comparing `tmp/fins-driver-0.2.0.tar.gz` & `tmp/fins-driver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fins-driver-0.2.0.tar", last modified: Thu Nov 16 09:45:06 2023, max compression
+gzip compressed data, was "fins-driver-0.3.0.tar", last modified: Thu Apr 18 03:43:24 2024, max compression
```

## Comparing `fins-driver-0.2.0.tar` & `fins-driver-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 iori       (501) staff       (20)        0 2023-11-16 09:45:06.223631 fins-driver-0.2.0/
--rw-r--r--   0 iori       (501) staff       (20)     1071 2023-11-07 07:06:56.000000 fins-driver-0.2.0/LICENSE
--rw-r--r--   0 iori       (501) staff       (20)       60 2023-11-07 07:06:56.000000 fins-driver-0.2.0/MANIFEST.in
--rw-r--r--   0 iori       (501) staff       (20)     4995 2023-11-16 09:45:06.223725 fins-driver-0.2.0/PKG-INFO
--rw-r--r--   0 iori       (501) staff       (20)     4243 2023-11-09 13:58:55.000000 fins-driver-0.2.0/README.md
-drwxr-xr-x   0 iori       (501) staff       (20)        0 2023-11-16 09:45:06.222563 fins-driver-0.2.0/fins/
--rw-r--r--   0 iori       (501) staff       (20)      281 2023-11-07 07:06:56.000000 fins-driver-0.2.0/fins/__init__.py
--rw-r--r--   0 iori       (501) staff       (20)      683 2023-11-09 13:58:55.000000 fins-driver-0.2.0/fins/adapters.py
--rw-r--r--   0 iori       (501) staff       (20)     5561 2023-11-09 13:58:55.000000 fins-driver-0.2.0/fins/client.py
--rw-r--r--   0 iori       (501) staff       (20)     3235 2023-11-07 07:06:56.000000 fins-driver-0.2.0/fins/command.py
--rw-r--r--   0 iori       (501) staff       (20)       41 2023-11-07 07:06:56.000000 fins-driver-0.2.0/fins/exceptions.py
--rw-r--r--   0 iori       (501) staff       (20)     2058 2023-11-07 07:06:56.000000 fins-driver-0.2.0/fins/header.py
--rw-r--r--   0 iori       (501) staff       (20)     6266 2023-11-09 13:58:55.000000 fins-driver-0.2.0/fins/memory.py
--rw-r--r--   0 iori       (501) staff       (20)     2208 2023-11-09 13:58:55.000000 fins-driver-0.2.0/fins/response.py
--rw-r--r--   0 iori       (501) staff       (20)     4684 2023-11-07 07:06:56.000000 fins-driver-0.2.0/fins/response_codes.py
--rw-r--r--   0 iori       (501) staff       (20)       22 2023-11-16 09:41:02.000000 fins-driver-0.2.0/fins/version.py
-drwxr-xr-x   0 iori       (501) staff       (20)        0 2023-11-16 09:45:06.223461 fins-driver-0.2.0/fins_driver.egg-info/
--rw-r--r--   0 iori       (501) staff       (20)     4995 2023-11-16 09:45:06.000000 fins-driver-0.2.0/fins_driver.egg-info/PKG-INFO
--rw-r--r--   0 iori       (501) staff       (20)      392 2023-11-16 09:45:06.000000 fins-driver-0.2.0/fins_driver.egg-info/SOURCES.txt
--rw-r--r--   0 iori       (501) staff       (20)        1 2023-11-16 09:45:06.000000 fins-driver-0.2.0/fins_driver.egg-info/dependency_links.txt
--rw-r--r--   0 iori       (501) staff       (20)        1 2023-11-16 09:45:06.000000 fins-driver-0.2.0/fins_driver.egg-info/not-zip-safe
--rw-r--r--   0 iori       (501) staff       (20)        5 2023-11-16 09:45:06.000000 fins-driver-0.2.0/fins_driver.egg-info/top_level.txt
--rw-r--r--   0 iori       (501) staff       (20)       74 2023-11-16 09:45:06.224043 fins-driver-0.2.0/setup.cfg
--rw-r--r--   0 iori       (501) staff       (20)     1232 2023-11-07 07:08:15.000000 fins-driver-0.2.0/setup.py
+drwxr-xr-x   0 iori       (501) staff       (20)        0 2024-04-18 03:43:24.370277 fins-driver-0.3.0/
+-rw-r--r--   0 iori       (501) staff       (20)     1071 2024-02-25 03:07:18.000000 fins-driver-0.3.0/LICENSE
+-rw-r--r--   0 iori       (501) staff       (20)       60 2024-02-25 03:07:18.000000 fins-driver-0.3.0/MANIFEST.in
+-rw-r--r--   0 iori       (501) staff       (20)     5141 2024-04-18 03:43:24.370181 fins-driver-0.3.0/PKG-INFO
+-rw-r--r--   0 iori       (501) staff       (20)     4243 2024-02-25 03:07:18.000000 fins-driver-0.3.0/README.md
+drwxr-xr-x   0 iori       (501) staff       (20)        0 2024-04-18 03:43:24.369253 fins-driver-0.3.0/fins/
+-rw-r--r--   0 iori       (501) staff       (20)      281 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/__init__.py
+-rw-r--r--   0 iori       (501) staff       (20)      710 2024-04-10 13:35:14.000000 fins-driver-0.3.0/fins/adapters.py
+-rw-r--r--   0 iori       (501) staff       (20)     5586 2024-04-10 13:30:08.000000 fins-driver-0.3.0/fins/client.py
+-rw-r--r--   0 iori       (501) staff       (20)     3235 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/command.py
+-rw-r--r--   0 iori       (501) staff       (20)       41 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/exceptions.py
+-rw-r--r--   0 iori       (501) staff       (20)     2058 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/header.py
+-rw-r--r--   0 iori       (501) staff       (20)     6266 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/memory.py
+-rw-r--r--   0 iori       (501) staff       (20)     2208 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/response.py
+-rw-r--r--   0 iori       (501) staff       (20)     4684 2024-02-25 03:07:18.000000 fins-driver-0.3.0/fins/response_codes.py
+-rw-r--r--   0 iori       (501) staff       (20)       22 2024-04-18 03:41:39.000000 fins-driver-0.3.0/fins/version.py
+drwxr-xr-x   0 iori       (501) staff       (20)        0 2024-04-18 03:43:24.369892 fins-driver-0.3.0/fins_driver.egg-info/
+-rw-r--r--   0 iori       (501) staff       (20)     5141 2024-04-18 03:43:24.000000 fins-driver-0.3.0/fins_driver.egg-info/PKG-INFO
+-rw-r--r--   0 iori       (501) staff       (20)      392 2024-04-18 03:43:24.000000 fins-driver-0.3.0/fins_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 iori       (501) staff       (20)        1 2024-04-18 03:43:24.000000 fins-driver-0.3.0/fins_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 iori       (501) staff       (20)        1 2024-04-18 03:43:24.000000 fins-driver-0.3.0/fins_driver.egg-info/not-zip-safe
+-rw-r--r--   0 iori       (501) staff       (20)        5 2024-04-18 03:43:24.000000 fins-driver-0.3.0/fins_driver.egg-info/top_level.txt
+-rw-r--r--   0 iori       (501) staff       (20)       74 2024-04-18 03:43:24.370607 fins-driver-0.3.0/setup.cfg
+-rw-r--r--   0 iori       (501) staff       (20)     1375 2024-02-25 03:10:25.000000 fins-driver-0.3.0/setup.py
```

### Comparing `fins-driver-0.2.0/LICENSE` & `fins-driver-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/PKG-INFO` & `fins-driver-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: fins-driver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python FINS driver for Omron PLC
 Home-page: https://github.com/indrarudianto/fins-driver
 Author: Indra Rudianto
 Author-email: indrarudianto.official@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fins-driver
 
 FINS (Factory Interface Network Service) Python driver for Omron PLC.
```

### Comparing `fins-driver-0.2.0/README.md` & `fins-driver-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins/adapters.py` & `fins-driver-0.3.0/fins/adapters.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class BaseDataAdapter:
     def __call__(self, data: bytes) -> bytes:
         return data
 
 
 class MultipleMemoryAreaReadDataAdapter(BaseDataAdapter):
     def __init__(self, addresses: List[MemoryArea]) -> None:
+        super().__init__()
         self.addresses = addresses
 
     def __call__(self, data: bytes) -> List[bytes]:
         values: List[bytes] = []
         buf = io.BytesIO(data)
         for addr in self.addresses:
             buf.read(1)  # Read memory area code.
```

### Comparing `fins-driver-0.2.0/fins/client.py` & `fins-driver-0.3.0/fins/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,17 @@
         self.da1: int = 0
         self.da2: int = 0
         self.sna: int = 0
         self.sa1: int = 1
         self.sa2: int = 0
         self.sid: int = 0
 
-    def send(self, command: Command, adapter: Optional[callable] = None) -> bytes:
+    def send(
+        self, command: Command, adapter: Optional[callable] = None
+    ) -> Response[bytes]:
         self._socket.send(command.raw)
         data = self._socket.recv(self.buffer_size)
         return Response(
             header=Header.from_bytes(data[:10]),
             command_code=data[10:12],
             code=data[12:14],
             data=data[14:],
@@ -94,15 +96,15 @@
         return self.send(cmd)
 
     def memory_area_fill(
         self, address: Union[str, bytes], data: bytes, num_items: int = 1
     ) -> Response[bytes]:
         addr = MemoryArea(address)
         cmd = Command(
-            code=MemoryArea.MEMORY_AREA_FILL,
+            code=CommandCode.MEMORY_AREA_FILL,
             data=addr.raw + num_items.to_bytes(2, "big") + data,
             header=self._build_header(),
         )
         return self.send(cmd)
 
     def multiple_memory_area_read(
         self, *addresses: Union[str, bytes]
```

### Comparing `fins-driver-0.2.0/fins/command.py` & `fins-driver-0.3.0/fins/command.py`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins/header.py` & `fins-driver-0.3.0/fins/header.py`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins/memory.py` & `fins-driver-0.3.0/fins/memory.py`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins/response.py` & `fins-driver-0.3.0/fins/response.py`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins/response_codes.py` & `fins-driver-0.3.0/fins/response_codes.py`

 * *Files identical despite different names*

### Comparing `fins-driver-0.2.0/fins_driver.egg-info/PKG-INFO` & `fins-driver-0.3.0/fins_driver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: fins-driver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python FINS driver for Omron PLC
 Home-page: https://github.com/indrarudianto/fins-driver
 Author: Indra Rudianto
 Author-email: indrarudianto.official@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fins-driver
 
 FINS (Factory Interface Network Service) Python driver for Omron PLC.
```

### Comparing `fins-driver-0.2.0/setup.py` & `fins-driver-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,9 +33,12 @@
         "Operating System :: POSIX :: Linux",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: Scientific/Engineering",
+        "License :: OSI Approved :: MIT License",
     ],
 )
```

