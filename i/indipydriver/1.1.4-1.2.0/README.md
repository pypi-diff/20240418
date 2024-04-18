# Comparing `tmp/indipydriver-1.1.4.tar.gz` & `tmp/indipydriver-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.1.4.tar` & `indipydriver-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.1.4/LICENSE
--rw-r--r--   0        0        0     2470 2024-04-14 12:44:57.000000 indipydriver-1.1.4/README.md
--rw-r--r--   0        0        0      573 2024-04-14 13:06:50.000000 indipydriver-1.1.4/indipydriver/__init__.py
--rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.1.4/indipydriver/comms.py
--rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.1.4/indipydriver/events.py
--rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.1.4/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    12064 2024-02-07 20:19:44.000000 indipydriver-1.1.4/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.1.4/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.1.4/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-04-14 13:06:41.000000 indipydriver-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 indipydriver-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.0/README.md
+-rw-r--r--   0        0        0      573 2024-04-17 19:58:31.000000 indipydriver-1.2.0/indipydriver/__init__.py
+-rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.2.0/indipydriver/comms.py
+-rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.2.0/indipydriver/events.py
+-rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.2.0/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    11951 2024-04-18 08:46:27.000000 indipydriver-1.2.0/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.2.0/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.2.0/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2024-04-17 19:57:42.000000 indipydriver-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.0/PKG-INFO
```

### Comparing `indipydriver-1.1.4/LICENSE` & `indipydriver-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/README.md` & `indipydriver-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
 
 async def snoopevent(self, event)
 
 This is only used if the device is monitoring (snooping) on other devices.
 
-Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object::
+Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object:
 
     server = IPyServer([driver], host="localhost", port=7624, maxconnections=5)
     asyncio.run(server.asyncrun())
 
 A connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
```

### Comparing `indipydriver-1.1.4/indipydriver/__init__.py` & `indipydriver-1.2.0/indipydriver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.1.4"
+version = "1.2.0"
```

### Comparing `indipydriver-1.1.4/indipydriver/comms.py` & `indipydriver-1.2.0/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/indipydriver/events.py` & `indipydriver-1.2.0/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/indipydriver/ipydriver.py` & `indipydriver-1.2.0/indipydriver/ipydriver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/indipydriver/ipyserver.py` & `indipydriver-1.2.0/indipydriver/ipyserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,14 @@
         for driver in drivers:
             # an instance of _DriverComms is created for each driver
             # each _DriverComms object has a list of drivers, not including its own driver
             # these will be used to send snooping traffic, sent by its own driver
             otherdrivers = [ d for d in drivers if not d is driver]
             driver.comms = _DriverComms(self.serverwriterque, self.connectionpool, otherdrivers)
 
-        for driver in drivers:
-            driver.comms.otherdrivers = [ d for d in drivers if not d is driver]
-
         self.drivers = drivers
         self.host = host
         self.port = port
 
     async def runserver(self):
         "Runs the server on the given host and port"
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
```

### Comparing `indipydriver-1.1.4/indipydriver/propertymembers.py` & `indipydriver-1.2.0/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/indipydriver/propertyvectors.py` & `indipydriver-1.2.0/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.4/pyproject.toml` & `indipydriver-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.1.4"
+version = "1.2.0"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.1.4/PKG-INFO` & `indipydriver-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.1.4
+Version: 1.2.0
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -45,15 +45,15 @@
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
 
 async def snoopevent(self, event)
 
 This is only used if the device is monitoring (snooping) on other devices.
 
-Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object::
+Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object:
 
     server = IPyServer([driver], host="localhost", port=7624, maxconnections=5)
     asyncio.run(server.asyncrun())
 
 A connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
```

