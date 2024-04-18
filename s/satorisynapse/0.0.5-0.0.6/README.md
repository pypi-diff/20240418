# Comparing `tmp/satorisynapse-0.0.5.tar.gz` & `tmp/satorisynapse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.0.5.tar", last modified: Wed Apr 17 21:27:30 2024, max compression
+gzip compressed data, was "satorisynapse-0.0.6.tar", last modified: Thu Apr 18 20:16:13 2024, max compression
```

## Comparing `satorisynapse-0.0.5.tar` & `satorisynapse-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.348275 satorisynapse-0.0.5/satorisynapse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.186349 satorisynapse-0.0.6/satorisynapse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/setup.py
```

### Comparing `satorisynapse-0.0.5/LICENSE` & `satorisynapse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.5/PKG-INFO` & `satorisynapse-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.5
+Version: 0.0.6
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.5/satorisynapse/lib/domain.py` & `satorisynapse-0.0.6/satorisynapse/lib/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import json
 import typing as t
+import json
 
-### CLASSES (coped from satorineuron.synergy.domain) ###
-
-# don't forget to use t.Dict in place of dict and t.Union inplace of Union
-# don't forget to comment out the references to Vesicle objects other than Ping
+SYNAPSE_PORT = 24600
 
 
 class Vesicle():
     '''
     any object sent over the wire to a peer must inhereit from this so it's
     guaranteed to be convertable to dict so we can have nested dictionaries
     then convert them all to json once at the end (rather than nested json).
```

### Comparing `satorisynapse-0.0.5/satorisynapse/lib/requests.py` & `satorisynapse-0.0.6/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.5/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.0.6/satorisynapse/synapse/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 import time
 import typing as t
 import socket
 import asyncio
 import requests  # ==2.31.0
 import aiohttp  # ==3.8.4
 from satorisynapse.lib.error import SseTimeoutFailure
-from satorisynapse.lib.domain import Envelope, Ping
+from satorisynapse.lib.domain import Envelope, Ping, SYNAPSE_PORT
 from satorisynapse.lib.requests import requests
 from satorisynapse.lib.utils import greyPrint
 
 
 class Synapse():
     ''' go-between for the flask server and the remote peers '''
 
-    def __init__(self, port: int = 24600):
-        self.port = port
+    def __init__(self, port: int = None):
+        self.port = port or SYNAPSE_PORT
         self.socketListener = None
         self.neuronListener = None
         self.peers: t.List[str] = []
         self.session = aiohttp.ClientSession()
         self.socket: socket.socket = self.createSocket()
         self.loop = asyncio.get_event_loop()
         self.broke = asyncio.Event()
@@ -207,15 +207,15 @@
             if r.status_code == 200:
                 return
         except Exception as _:
             pass
         time.sleep(1)
 
 
-async def main(port: int = 24600):
+async def main(port: int = None):
 
     async def waitForNeuron():
         notified = False
         while True:
             try:
                 r = requests.get(Synapse.satoriUrl('/ping'))
                 if r.status_code == 200:
@@ -242,15 +242,15 @@
             pass
         except Exception as _:
             pass
         finally:
             await synapse.shutdown()
 
 
-def runSynapse(port: int = 24600):
+def runSynapse(port: int = None):
     try:
         asyncio.run(main(port))
     except KeyboardInterrupt:
         print('Interrupted by user')
 
 
 if __name__ == '__main__':
```

### Comparing `satorisynapse-0.0.5/satorisynapse/synapse/threaded.py` & `satorisynapse-0.0.6/satorisynapse/synapse/threaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 import typing as t
 import time
 import threading
 import socket
 import urllib.request
 import urllib.parse
 from satorisynapse.lib.error import SseTimeoutFailure
-from satorisynapse.lib.domain import Envelope, Ping
+from satorisynapse.lib.domain import Envelope, Ping, SYNAPSE_PORT
 from satorisynapse.lib.requests import requests
 from satorisynapse.lib.utils import greyPrint
 
 
 class Synapse():
     ''' go-between for the flask server and the remote peers '''
 
-    def __init__(self, port: int = 24600):
-        self.port = port
+    def __init__(self, port: int = None):
+        self.port = port or SYNAPSE_PORT
         self.running = False
         self.neuronListener = None
         self.peers: t.List[str] = []
         self.socket: socket.socket = self.createSocket()
         self.run()
 
     @staticmethod
@@ -201,15 +201,15 @@
         except Exception as _:
             if not notified:
                 greyPrint('waiting for Satori Neuron')
                 notified = True
         time.sleep(1)
 
 
-def main(port: int = 24600):
+def main(port: int = None):
     while True:
         waitForNeuron()
         try:
             greyPrint("Satori P2P is running. Press Ctrl+C to stop.")
             synapse = Synapse(port)
             synapse.listenToSocket()
         except KeyboardInterrupt:
@@ -220,15 +220,15 @@
             pass
         finally:
             greyPrint('Satori P2P is shutting down')
             synapse.shutdown()
             time.sleep(5)
 
 
-def runSynapse(port: int = 24600):
+def runSynapse(port: int = None):
     try:
         greyPrint('Synapse started')
         main(port)
     except KeyboardInterrupt:
         greyPrint('Synapse exited by user')
```

### Comparing `satorisynapse-0.0.5/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.6/satorisynapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.5
+Version: 0.0.6
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.5/setup.py` & `satorisynapse-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,45 +15,47 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.5'
+    return '0.0.6'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
     return []
 
 
-setup(
-    name=get_name(),
-    version=get_version(),
-    description='satorisynapse contains domain model and apis for the Satori Network',
-    long_description=get_long_description(),
-    long_description_content_type="text/markdown",
-    packages=[f'{get_name()}.{p}' for p in find_packages(where=get_name())],
-    install_requires=get_requirements(),
-    dependency_links=[
-        'git+https://github.com/SatoriNetwork/python-evrmorelib.git#egg=python-evrmorelib'
-    ],
-    python_requires='>=3.7',
-    author='Jordan Miller',
-    author_email="jordan@satorinet.io",
-    url=f'https://github.com/SatoriNetwork/{get_name()}',
-    download_url=f'https://github.com/SatoriNetwork/{get_name()}',
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    entry_points={
-        "console_scripts": [
-            f"{get_name()} = {get_name()}.cli:main",
-        ]
-    },
-)
+if __name__ == '__main__':
+    setup(
+        name=get_name(),
+        version=get_version(),
+        description='satorisynapse contains domain model and apis for the Satori Network',
+        long_description=get_long_description(),
+        long_description_content_type="text/markdown",
+        packages=[f'{get_name()}.{p}' for p in find_packages(
+            where=get_name())],
+        install_requires=get_requirements(),
+        dependency_links=[
+            'git+https://github.com/SatoriNetwork/python-evrmorelib.git#egg=python-evrmorelib'
+        ],
+        python_requires='>=3.7',
+        author='Jordan Miller',
+        author_email="jordan@satorinet.io",
+        url=f'https://github.com/SatoriNetwork/{get_name()}',
+        download_url=f'https://github.com/SatoriNetwork/{get_name()}',
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        entry_points={
+            "console_scripts": [
+                f"{get_name()} = {get_name()}.cli:main",
+            ]
+        },
+    )
```

