# Comparing `tmp/tactigon_gear-5.0.4.post1.tar.gz` & `tmp/tactigon_gear-5.0.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tactigon_gear-5.0.4.post1.tar", last modified: Tue Apr 16 08:44:30 2024, max compression
+gzip compressed data, was "tactigon_gear-5.0.4.post2.tar", last modified: Thu Apr 18 13:04:00 2024, max compression
```

## Comparing `tactigon_gear-5.0.4.post1.tar` & `tactigon_gear-5.0.4.post2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.930371 tactigon_gear-5.0.4.post1/
--rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_gear-5.0.4.post1/LICENSE
--rw-rw-rw-   0        0        0      383 2024-03-27 15:43:10.000000 tactigon_gear-5.0.4.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     3619 2024-04-16 08:44:30.929367 tactigon_gear-5.0.4.post1/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2024-03-07 11:04:20.000000 tactigon_gear-5.0.4.post1/README.md
--rw-rw-rw-   0        0        0       92 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 08:44:30.941373 tactigon_gear-5.0.4.post1/setup.cfg
--rw-rw-rw-   0        0        0     2690 2024-03-27 15:42:57.000000 tactigon_gear-5.0.4.post1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.725233 tactigon_gear-5.0.4.post1/tactigon_gear/
--rw-rw-rw-   0        0        0     2427 2024-04-16 08:37:01.000000 tactigon_gear-5.0.4.post1/tactigon_gear/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.820232 tactigon_gear-5.0.4.post1/tactigon_gear/client/
--rw-rw-rw-   0        0        0     8673 2024-04-16 08:42:53.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/Data_Collection.py
--rw-rw-rw-   0        0        0     5871 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/models.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.827234 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/
--rw-rw-rw-   0        0        0     2527 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/Client_Account_Managment.py
--rw-rw-rw-   0        0        0     6841 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.832233 tactigon_gear-5.0.4.post1/tactigon_gear/hal/
--rw-rw-rw-   0        0        0       41 2024-03-15 10:16:54.000000 tactigon_gear-5.0.4.post1/tactigon_gear/hal/__init__.py
--rw-rw-rw-   0        0        0    10310 2024-04-16 08:42:10.000000 tactigon_gear-5.0.4.post1/tactigon_gear/hal/ble.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.877808 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/
--rw-rw-rw-   0        0        0   443371 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Audio.c
--rw-rw-rw-   0        0        0   499540 2024-04-16 08:44:11.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Gesture.c
--rw-rw-rw-   0        0        0   430462 2024-04-16 08:44:11.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Recorder.c
--rw-rw-rw-   0        0        0      243 2024-03-27 15:44:22.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.911375 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/
--rw-rw-rw-   0        0        0   518832 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Data_Preprocessor.c
--rw-rw-rw-   0        0        0   701641 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c
--rw-rw-rw-   0        0        0      212 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/__init__.py
--rw-rw-rw-   0        0        0     4755 2024-03-15 09:33:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/models.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.925370 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/
--rw-rw-rw-   0        0        0     3619 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.931893 tactigon_gear-5.0.4.post2/
+-rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_gear-5.0.4.post2/LICENSE
+-rw-rw-rw-   0        0        0      383 2024-03-27 15:43:10.000000 tactigon_gear-5.0.4.post2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3619 2024-04-18 13:04:00.931893 tactigon_gear-5.0.4.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     2856 2024-03-07 11:04:20.000000 tactigon_gear-5.0.4.post2/README.md
+-rw-rw-rw-   0        0        0       92 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:04:00.933888 tactigon_gear-5.0.4.post2/setup.cfg
+-rw-rw-rw-   0        0        0     2690 2024-03-27 15:42:57.000000 tactigon_gear-5.0.4.post2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.676093 tactigon_gear-5.0.4.post2/tactigon_gear/
+-rw-rw-rw-   0        0        0     2427 2024-04-18 13:03:28.000000 tactigon_gear-5.0.4.post2/tactigon_gear/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.802378 tactigon_gear-5.0.4.post2/tactigon_gear/client/
+-rw-rw-rw-   0        0        0     8673 2024-04-16 08:42:53.000000 tactigon_gear-5.0.4.post2/tactigon_gear/client/Data_Collection.py
+-rw-rw-rw-   0        0        0     5871 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/client/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/client/models.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.819365 tactigon_gear-5.0.4.post2/tactigon_gear/client/utilities/
+-rw-rw-rw-   0        0        0     2527 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/client/utilities/Client_Account_Managment.py
+-rw-rw-rw-   0        0        0     6841 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/client/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.847394 tactigon_gear-5.0.4.post2/tactigon_gear/hal/
+-rw-rw-rw-   0        0        0       41 2024-03-15 10:16:54.000000 tactigon_gear-5.0.4.post2/tactigon_gear/hal/__init__.py
+-rw-rw-rw-   0        0        0    10310 2024-04-18 13:03:22.000000 tactigon_gear-5.0.4.post2/tactigon_gear/hal/ble.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.897985 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/
+-rw-rw-rw-   0        0        0   443371 2024-04-18 13:03:35.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Audio.c
+-rw-rw-rw-   0        0        0   499540 2024-04-18 13:03:35.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Gesture.c
+-rw-rw-rw-   0        0        0   430462 2024-04-18 13:03:35.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Recorder.c
+-rw-rw-rw-   0        0        0      243 2024-03-27 15:44:22.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.916892 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/
+-rw-rw-rw-   0        0        0   518832 2024-04-18 13:03:35.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/Data_Preprocessor.c
+-rw-rw-rw-   0        0        0   701641 2024-04-18 13:03:35.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c
+-rw-rw-rw-   0        0        0      212 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/__init__.py
+-rw-rw-rw-   0        0        0     4755 2024-03-15 09:33:23.000000 tactigon_gear-5.0.4.post2/tactigon_gear/models.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:04:00.924929 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/
+-rw-rw-rw-   0        0        0     3619 2024-04-18 13:04:00.000000 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2024-04-18 13:04:00.000000 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:04:00.000000 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-18 13:04:00.000000 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 13:04:00.000000 tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/top_level.txt
```

### Comparing `tactigon_gear-5.0.4.post1/PKG-INFO` & `tactigon_gear-5.0.4.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_gear
-Version: 5.0.4.post1
+Version: 5.0.4.post2
 Summary: Tactigon Gear to connect to Tactigon Skin wereable platform
 Home-page: https://www.thetactigon.com
 Maintainer: Next Industries s.r.l.
 Maintainer-email: info@thetactigon.com
 License: MIT
 Keywords: tactigon,wereable,gestures controller,human interface
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tactigon_gear-5.0.4.post1/README.md` & `tactigon_gear-5.0.4.post2/README.md`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/setup.py` & `tactigon_gear-5.0.4.post2/setup.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/__init__.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.0.4.post1"
+__version__ = "5.0.4.post2"
 __all__ = ["TSkin", "TSkinConfig", "GestureConfig", "TSkinState", "Hand", "Touch", "Angle", "Gyro", "Acceleration", "Gesture", "OneFingerGesture", "TwoFingerGesture"]
 
 import logging
 from typing import Optional
 from multiprocessing import Pipe
 
 from .hal import Ble
```

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/client/Data_Collection.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/client/Data_Collection.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/client/__init__.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/client/models.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/client/models.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/Client_Account_Managment.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/client/utilities/Client_Account_Managment.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/__init__.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/client/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/hal/ble.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/hal/ble.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 math.sqrt(math.pow(accX, 2) + math.pow(accY, 2)) / accZ
             )
 
         accX = accX - G_CONST * math.sin(_roll)
         accY = accY + G_CONST * math.sin(_pitch)
         accZ = accZ - G_CONST * math.cos(beta)
 
-        return accX, accY, accZ, gyroX, gyroY, gyroX, roll, pitch, yaw
+        return accX, accY, accZ, gyroX, gyroY, gyroZ, roll, pitch, yaw
 
     @property
     def connected(self) -> bool:
         return (True if self.client.is_connected else False) if self.client else False
     
     @property
     def angle(self) -> Optional[Angle]:
```

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Audio.c` & `tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Audio.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Gesture.c` & `tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Gesture.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Recorder.c` & `tactigon_gear-5.0.4.post2/tactigon_gear/middleware/Tactigon_Recorder.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Data_Preprocessor.c` & `tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/Data_Preprocessor.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c` & `tactigon_gear-5.0.4.post2/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear/models.py` & `tactigon_gear-5.0.4.post2/tactigon_gear/models.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/PKG-INFO` & `tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_gear
-Version: 5.0.4.post1
+Version: 5.0.4.post2
 Summary: Tactigon Gear to connect to Tactigon Skin wereable platform
 Home-page: https://www.thetactigon.com
 Maintainer: Next Industries s.r.l.
 Maintainer-email: info@thetactigon.com
 License: MIT
 Keywords: tactigon,wereable,gestures controller,human interface
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/SOURCES.txt` & `tactigon_gear-5.0.4.post2/tactigon_gear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

