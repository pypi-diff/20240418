# Comparing `tmp/pymycobot-3.4.5.tar.gz` & `tmp/pymycobot-3.4.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.4.5.tar", last modified: Tue Apr  9 10:02:31 2024, max compression
+gzip compressed data, was "pymycobot-3.4.6b1.tar", last modified: Thu Apr 18 11:14:01 2024, max compression
```

## Comparing `pymycobot-3.4.5.tar` & `pymycobot-3.4.6b1.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.007134 pymycobot-3.4.5/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.5/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0    63942 2024-04-09 10:02:31.006135 pymycobot-3.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:30.971629 pymycobot-3.4.5/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2067 2024-04-09 09:58:11.000000 pymycobot-3.4.5/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    21490 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/common.py
--rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.5/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/error.py
--rw-rw-rw-   0        0        0    44048 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.5/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.5/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0     7042 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    16852 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.5/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.5/pymycobot/mercurychassisocket.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.5/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.5/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/myarm.py
--rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    85325 2024-04-09 09:54:24.000000 pymycobot-3.4.5/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.5/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.5/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.005134 pymycobot-3.4.5/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63942 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:02:31.007134 pymycobot-3.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.004134 pymycobot-3.4.5/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.391361 pymycobot-3.4.6b1/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.389362 pymycobot-3.4.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.6b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.349795 pymycobot-3.4.6b1/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2171 2024-04-18 11:13:40.000000 pymycobot-3.4.6b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    24930 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.6b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.6b1/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    16852 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.6b1/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/mercurychassisocket.py
+-rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.6b1/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.6b1/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    16331 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarm_api.py
+-rw-rw-rw-   0        0        0      273 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmc.py
+-rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmm.py
+-rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    85159 2024-04-18 01:28:43.000000 pymycobot-3.4.6b1/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.6b1/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.388356 pymycobot-3.4.6b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1126 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.6b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:14:01.392361 pymycobot-3.4.6b1/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.6b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.386801 pymycobot-3.4.6b1/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_utils.py
```

### Comparing `pymycobot-3.4.5/LICENSE` & `pymycobot-3.4.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/PKG-INFO` & `pymycobot-3.4.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.5
+Version: 3.4.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.5/README.md` & `pymycobot-3.4.6b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/Interface.py` & `pymycobot-3.4.6b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/__init__.py` & `pymycobot-3.4.6b1/pymycobot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from pymycobot.elephantrobot import ElephantRobot
 from pymycobot.mercury import Mercury
 from pymycobot.myagv import MyAgv
 from pymycobot.mecharmsocket import MechArmSocket
 from pymycobot.mercurychassis import MercuryChassis
 from pymycobot.mercurysocket import MercurySocket
 from pymycobot.mycobotpro630 import Phoenix
-
+from pymycobot.myarmm import MyArmM
+from pymycobot.myarmc import MyArmC
 __all__ = [
     "MyCobot",
     "CommandGenerator",
     "Angle",
     "Coord",
     "utils",
     "MyPalletizer",
@@ -46,23 +47,25 @@
     "ElephantRobot",
     "Mercury",
     "MyAgv",
     "MechArmSocket",
     "MyArmSocket",
     "MercuryChassis",
     "MercurySocket",
-    "Phoenix"
+    "Phoenix",
+    "MyArmM",
+    "MyArmC"
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.4.5"
+__version__ = "3.4.6b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.4.5/pymycobot/bluet.py` & `pymycobot-3.4.6b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/common.py` & `pymycobot-3.4.6b1/pymycobot/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,24 +212,52 @@
     MERCURY_JOG_BASE_COORD = 0xF3
     
     MERCURY_DRAG_TECH_SAVE = 0x70
     MERCURY_DRAG_TECH_EXECUTE = 0x71
     MERCURY_DRAG_TECH_PAUSE = 0x72
     MERCURY_DRAG_TEACH_CLEAN = 0x73
 
+    GET_ROBOT_MODIFIED_VERSION = 1
+    GET_ROBOT_FIRMWARE_VERSION = 2
+    GET_ROBOT_AUXILIARY_FIRMWARE_VERSION = 3
+    GET_ROBOT_ATOM_MODIFIED_VERSION = 4
+    GET_ROBOT_TOOL_FIRMWARE_VERSION = 9
+    GET_ROBOT_SERIAL_NUMBER = 5
+    SET_ROBOT_ERROR_CHECK_STATE = 6
+    GET_ROBOT_ERROR_CHECK_STATE = 7
+    GET_ROBOT_ERROR_STATUS = 0x15
+    GET_ATOM_PRESS_STATUS = 0x6b
+    GET_ATOM_LED_COLOR = 0x6a
+    SET_ATOM_PIN_STATUS = 0x61
+    GET_ATOM_PIN_STATUS = 0x62
+    SET_MASTER_PIN_STATUS = 0x65
+    GET_MASTER_PIN_STATUS = 0x66
+    SET_AUXILIARY_PIN_STATUS = 0xa0
+    GET_AUXILIARY_PIN_STATUS = 0xa1
+    SET_SERVO_MOTOR_CLOCKWISE = 0x73
+    GET_SERVO_MOTOR_CLOCKWISE = 0Xea
+    SET_SERVO_MOTOR_COUNTER_CLOCKWISE = 0x74
+    GET_SERVO_MOTOR_COUNTER_CLOCKWISE = 0xeb
+    SET_SERVO_MOTOR_CONFIG = 0x52
+    GET_SERVO_MOTOR_CONFIG = 0x53
+    CLEAR_RECV_QUEUE = 0x19
+    GET_RECV_QUEUE_LENGTH = 0x08
     GET_BASE_COORDS = 0xF0
     BASE_TO_SINGLE_COORDS = 0xF1
     COLLISION = 0xF2
     GET_BASE_COORD = 0xF3
     GET_ALL_BASE_COORDS = 0xF4
     WRITE_BASE_COORD = 0xF5
     WRITE_BASE_COORDS = 0xF6
     JOG_INC_COORD = 0xF7
     COLLISION_SWITCH = 0xF8
     IS_COLLISION_ON = 0xF9
+    CLEAR_ROBOT_ERROR = 0x16
+    GET_RECV_QUEUE_SIZE = 0x17
+    SET_RECV_QUEUE_SIZE = 0x18
 
     # IIC
     # SET_IIC_STATE = 0xA4
     # GET_IIS_BYTE = 0xA5
     # SET_IIC_BYTE = 0xA6
 
     # ultraArm
@@ -261,14 +289,54 @@
     IS_MOVING_END = "M9"
     GET_GRIPPER_ANGLE = "M50"
     SET_SYSTEM_VALUE = "M51"
     GET_SYSTEM_VALUE = "M52"
 
 
 class DataProcessor(object):
+    def _mesg(self, genre, *args, **kwargs):
+        """
+        Args:
+            genre: command type (Command)
+            *args: other data.
+                   It is converted to octal by default.
+                   If the data needs to be encapsulated into hexadecimal,
+                   the array is used to include them. (Data cannot be nested)
+            **kwargs: support `has_reply`
+                has_reply: Whether there is a return value to accept.
+        """
+        command_data = self._process_data_command(genre, self.__class__.__name__, args)
+        if genre == 178:
+            # 修改wifi端口
+            command_data = self._encode_int16(command_data)
+            
+        elif genre in [76, 77]:
+            command_data = [command_data[0]] + self._encode_int16(command_data[1]*10)
+        elif genre == 115 and self.__class__.__name__ not in  ["MyArmC", "MyArmM"]:
+            command_data = [command_data[1],command_data[3]]
+        LEN = len(command_data) + 2
+        
+        command = [
+                ProtocolCode.HEADER,
+                ProtocolCode.HEADER,
+                LEN,
+                genre,
+            ]
+        if command_data:
+            command.extend(command_data)
+        if self.__class__.__name__ in ["Mercury", "MercurySocket"]:
+            command[2] += 1
+            command.extend(self.crc_check(command))
+        else:
+            command.append(ProtocolCode.FOOTER)
+
+        real_command = self._flatten(command)
+        has_reply = kwargs.get("has_reply", False)
+        return real_command, has_reply
+
     # Functional approach
     def _encode_int8(self, data):
         return struct.pack("b", data)
 
     def _encode_int16(self, data):
         if isinstance(data, int):
             return [
@@ -342,27 +410,27 @@
         for index in range(len(args)):
             if isinstance(args[index], list):
                 if genre == ProtocolCode.SET_ENCODERS_DRAG and index == 0 and _class in ["Mercury", "MercurySocket"]:
                     for data in args[index]:
                         byte_value = data.to_bytes(4, byteorder='big', signed=True)
                         res = []
                         for i in range(len(byte_value)):
-                           res.append(byte_value[i])
+                            res.append(byte_value[i])
                         processed_args.extend(res)
                 else:
                     processed_args.extend(self._encode_int16(args[index]))
             else:
                 if isinstance(args[index], str):
                     processed_args.append(args[index])
                 else:
                     if genre == ProtocolCode.SET_SERVO_DATA and _class in ["Mercury", "MercurySocket"] and index == 2:
                         byte_value = args[index].to_bytes(2, byteorder='big', signed=True)
                         res = []
                         for i in range(len(byte_value)):
-                           res.append(byte_value[i])
+                            res.append(byte_value[i])
                         processed_args.extend(res)
                     else:
                         processed_args.append(args[index])
 
         return processed_args
 
     def _is_frame_header(self, data, pos1, pos2):
@@ -378,26 +446,26 @@
             return []
         data = bytearray(data)
         data_len = len(data)
         # Get valid header: 0xfe0xfe
         header_i, header_j = 0, 1
         while header_j < data_len - 4:
             if self._is_frame_header(data, header_i, header_j):
-                if arm in [6, 7, 14]:
+                if arm in [6, 7, 14, 8]:
                     cmd_id = data[header_i + 3]
                 elif arm == 12:
                     cmd_id = data[header_i + 4]
                 # compare send header and received header
                 if cmd_id == genre:
                     break
             header_i += 1
             header_j += 1
         else:
             return []
-        if arm in [6, 7]:
+        if arm in [6, 7, 8]:
             data_len = data[header_i + 2] - 2
         elif arm == 12:
             data_len = data[header_i + 3] - 2
         elif arm == 14:
             data_len = data[header_i + 2] - 3
             
         unique_data = [ProtocolCode.GET_BASIC_INPUT, ProtocolCode.GET_DIGITAL_INPUT]
@@ -406,28 +474,38 @@
         elif cmd_id in unique_data:
             if arm == 12:
                 data_pos = header_i + 6
             else:
                 data_pos = header_i + 5
             data_len -= 1
         else:
-            if arm in [6, 7, 14]:
+            if arm in [6, 7, 14, 8]:
                 data_pos = header_i + 4
             elif arm == 12:
                 data_pos = header_i + 5
         valid_data = data[data_pos : data_pos + data_len]
 
         # process valid data
         res = []
         # if genre in [ProtocolCode.GET_SERVO_VOLTAGES, ProtocolCode.GET_SERVO_STATUS, ProtocolCode.GET_SERVO_TEMPS, ProtocolCode.GO_ZERO]:
         #     for i in valid_data:
         #         res.append(i)
         #     return res    
         if data_len in [6, 8, 12, 14, 16, 24, 26, 60]:
-            if data_len == 8 and arm == 14 and cmd_id == ProtocolCode.IS_INIT_CALIBRATION:
+            ignor_t = (
+                ProtocolCode.GET_SERVO_CURRENTS,
+                ProtocolCode.GET_SERVO_TEMPS,
+                ProtocolCode.GET_SERVO_VOLTAGES,
+                ProtocolCode.GET_SERVO_STATUS,
+                ProtocolCode.IS_ALL_SERVO_ENABLE
+            )
+            if data_len == 8 and (
+                    (arm == 14 and cmd_id == ProtocolCode.IS_INIT_CALIBRATION) or
+                    (arm == 8 and cmd_id in ignor_t)
+            ):
                 for v in valid_data:
                     res.append(v)
                 return res
             elif data_len == 8 and arm == 14 and cmd_id == ProtocolCode.GET_DOWN_ENCODERS:
                 i = 0
                 while i < data_len:
                     byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
@@ -494,14 +572,26 @@
                     res.append(valid_data[i])
                     i+=1
                 elif i < 23:
                     one = valid_data[i : i + 2]
                     res.append(self._decode_int16(one))
                     i+=2
             return res
+        elif data_len == 38:
+            i = 0
+            res = []
+            while i < data_len:
+                if i < 10 or i >= 30:
+                    res.append(valid_data[i])
+                    i+=1
+                elif i < 38:
+                    one = valid_data[i : i + 2]
+                    res.append(self._decode_int16(one))
+                    i+=2
+            return res
         else:
             if genre in [
                 ProtocolCode.GET_SERVO_VOLTAGES,
                 ProtocolCode.GET_SERVO_STATUS,
                 ProtocolCode.GET_SERVO_TEMPS,
             ]:
                 for i in range(data_len):
@@ -556,29 +646,30 @@
         for i in command:
             command_log += hex(i)[2:] + " "
         self.log.debug("_write: {}".format(command_log))
         self._serial_port.write(command)
         self._serial_port.flush()
 
 
-def read(self, genre, method=None, command=None, _class=None):
+def read(self, genre, method=None, command=None, _class=None, timeout=None):
     datas = b""
     data_len = -1
     k = 0
     pre = 0
     t = time.time()
     wait_time = 0.1   
     if method is not None:
          wait_time = 0.3
-    if genre == ProtocolCode.GO_ZERO:
-        wait_time = 120
+    if timeout is not None:
+        wait_time = timeout
     if _class in ["Mercury", "MercurySocket"]:
         if genre == ProtocolCode.POWER_ON:
             wait_time = 8
-        elif genre in [ProtocolCode.POWER_OFF, ProtocolCode.RELEASE_ALL_SERVOS, ProtocolCode.FOCUS_ALL_SERVOS, ProtocolCode.RELEASE_SERVO, ProtocolCode.FOCUS_SERVO, ProtocolCode.STOP]:
+        elif genre in [ProtocolCode.POWER_OFF, ProtocolCode.RELEASE_ALL_SERVOS, ProtocolCode.FOCUS_ALL_SERVOS,
+                       ProtocolCode.RELEASE_SERVO, ProtocolCode.FOCUS_SERVO, ProtocolCode.STOP]:
             wait_time = 3
     if method is not None:
         if genre == 177:
             while True:
                 data = self.sock.recv(1024)
                 if b"password" in data:
                     break
@@ -661,8 +752,8 @@
             self.log.debug("_read : {}".format(command_log))
         else:
             command_log = ""
             for d in datas:
                 command_log += hex(d)[2:] + " "
             self.log.debug("_read : {}".format(command_log))
             
-        return datas
+        return datas
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymycobot-3.4.5/pymycobot/elephantrobot.py` & `pymycobot-3.4.6b1/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/error.py` & `pymycobot-3.4.6b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/generate.py` & `pymycobot-3.4.6b1/pymycobot/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,73 +90,32 @@
         """
         self._version = sys.version_info[:2][0]
         self.debug = debug
         setup_logging(self.debug)
         self.log = logging.getLogger(__name__)
         self.calibration_parameters = calibration_parameters
 
-    def _mesg(self, genre, *args, **kwargs):
-        """
-        Args:
-            genre: command type (Command)
-            *args: other data.
-                   It is converted to octal by default.
-                   If the data needs to be encapsulated into hexadecimal,
-                   the array is used to include them. (Data cannot be nested)
-            **kwargs: support `has_reply`
-                has_reply: Whether there is a return value to accept.
-        """
-        command_data = self._process_data_command(genre, self.__class__.__name__, args)
-
-        if genre == 178:
-            # 修改wifi端口
-            command_data = self._encode_int16(command_data)
-            
-        elif genre in [76, 77]:
-            command_data = [command_data[0]] + self._encode_int16(command_data[1]*10)
-        elif genre == 115:
-            command_data = [command_data[1],command_data[3]]
-        LEN = len(command_data) + 2
-        
-        command = [
-                ProtocolCode.HEADER,
-                ProtocolCode.HEADER,
-                LEN,
-                genre,
-            ]
-        if command_data:
-            command.extend(command_data)
-        if self.__class__.__name__ in ["Mercury", "MercurySocket"]:
-            command[2] += 1
-            command.extend(self.crc_check(command))
-        else:
-            command.append(ProtocolCode.FOOTER)
-
-        real_command = self._flatten(command)
-        has_reply = kwargs.get("has_reply", False)
-        return real_command, has_reply
-
     # System status
     def get_robot_version(self):  # TODO: test method <2021-03-11, yourname> #
         """Get cobot version
 
         Return:
             mycobot   : 1
             mycobotPro: 101
         """
         return self._mesg(ProtocolCode.ROBOT_VERSION, has_reply=True)
-    
+
     def get_system_version(self):
         """get system version"""
-        return self._mesg(ProtocolCode.SOFTWARE_VERSION, has_reply = True)
+        return self._mesg(ProtocolCode.SOFTWARE_VERSION, has_reply=True)
 
     def get_robot_id(self):
         """get robot id"""
-        return self._mesg(ProtocolCode.GET_ROBOT_ID, has_reply = True)
-    
+        return self._mesg(ProtocolCode.GET_ROBOT_ID, has_reply=True)
+
     def set_robot_id(self, id):
         """set robot id
         
         Args:
             id(int): 0 ~ 255
         """
         return self._mesg(ProtocolCode.SET_ROBOT_ID, id)
@@ -445,15 +404,16 @@
                 for mycobot / mecharm: Joint id 1 - 6
                 for mypalletizer: Joint id 1 - 4
                 for mycobot gripper: Joint id 7
                 for myArm: Joint id 1 - 7.
             encoder: The value of the set encoder.
             speed : 1 - 100
         """
-        self.calibration_parameters(class_name = self.__class__.__name__, encode_id = joint_id, encoder = encoder, speed=speed)
+        self.calibration_parameters(class_name=self.__class__.__name__, encode_id=joint_id, encoder=encoder,
+                                    speed=speed)
         return self._mesg(ProtocolCode.SET_ENCODER, joint_id, [encoder], speed)
 
     def get_encoder(self, joint_id):
         """Obtain the specified joint potential value.
 
         Args:
             joint_id: (int)
@@ -581,15 +541,16 @@
             value: 0 - 4096
             mode: 0 - indicates that value is one byte(default), 1 - 1 represents a value of two bytes.
         """
         if mode is None:
             self.calibration_parameters(class_name = self.__class__.__name__, id=servo_id, address=data_id, value=value)
             return self._mesg(ProtocolCode.SET_SERVO_DATA, servo_id, data_id, value)
         else:
-            self.calibration_parameters(class_name = self.__class__.__name__, id=servo_id, address=data_id, value=value, mode=mode)
+            self.calibration_parameters(class_name=self.__class__.__name__, id=servo_id, address=data_id, value=value,
+                                        mode=mode)
             return self._mesg(ProtocolCode.SET_SERVO_DATA, servo_id, data_id, [value], mode)
 
     def get_servo_data(self, servo_id, data_id, mode=None):
         """Read the data parameter of the specified address of the steering gear.
 
         Args:
             servo_id: Serial number of articulated steering gear.
@@ -766,15 +727,16 @@
             speed (int): 1 ~ 100
             gripper_type (int): default 1
                 1: Adaptive gripper
                 3: Parallel gripper, this parameter can be omitted
                 4: Flexible gripper
         """
         if gripper_type is not None:
-            self.calibration_parameters(class_name = self.__class__.__name__, gripper_value=gripper_value, speed=speed, gripper_type=gripper_type)
+            self.calibration_parameters(class_name=self.__class__.__name__, gripper_value=gripper_value, speed=speed,
+                                        gripper_type=gripper_type)
             return self._mesg(ProtocolCode.SET_GRIPPER_VALUE, gripper_value, speed, gripper_type)
         else:
             return self._mesg(ProtocolCode.SET_GRIPPER_VALUE, gripper_value, speed)
             
 
     def set_gripper_calibration(self):
         """Set the current position to zero, set current position value is `2048`."""
```

### Comparing `pymycobot-3.4.5/pymycobot/log.py` & `pymycobot-3.4.6b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mecharmsocket.py` & `pymycobot-3.4.6b1/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mercury.py` & `pymycobot-3.4.6b1/pymycobot/mercury.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,25 +139,37 @@
                             for i in range(1, len(res)):
                                 if res[i] == 1:
                                     r.append(i)
                     return r
                 elif genre in [ProtocolCode.COBOTX_GET_ANGLE, ProtocolCode.COBOTX_GET_SOLUTION_ANGLES]:
                         return self._int2angle(res[0])
                 elif genre == ProtocolCode.MERCURY_ROBOT_STATUS:
-                    i = 9
-                    for i in range(9, len(res)):
-                        if res[i] != 0:
-                            data = bin(res[i])[2:]
-                            res[i] = []
-                            while len(data) != 16:
-                                data = "0"+data
-                            for j in range(16):
-                                if data[j] != "0":
-                                    res[i].append(15-j)
-                    return res
+                    if self._serial_port.port == "/dev/ttyTHS0":
+                        i = 9
+                        for i in range(9, len(res)):
+                            if res[i] != 0:
+                                data = bin(res[i])[2:]
+                                res[i] = []
+                                while len(data) != 16:
+                                    data = "0"+data
+                                for j in range(16):
+                                    if data[j] != "0":
+                                        res[i].append(15-j)
+                        return res
+                    else:
+                        for i in range(10, len(res)):
+                            if res[i] != 0:
+                                data = bin(res[i])[2:]
+                                res[i] = []
+                                while len(data) != 16:
+                                    data = "0"+data
+                                for j in range(16):
+                                    if data[j] != "0":
+                                        res[i].append(15-j)
+                        return res
                 else:
                     return res
             return None
     
     def open(self):
         self._serial_port.open()
```

### Comparing `pymycobot-3.4.5/pymycobot/mercury_api.py` & `pymycobot-3.4.6b1/pymycobot/mercury_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mercurychassis.py` & `pymycobot-3.4.6b1/pymycobot/mercurychassis.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mercurychassisocket.py` & `pymycobot-3.4.6b1/pymycobot/mercurychassisocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mercurysocket.py` & `pymycobot-3.4.6b1/pymycobot/mercurysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/myagv.py` & `pymycobot-3.4.6b1/pymycobot/myagv.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/myarm.py` & `pymycobot-3.4.6b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/myarmsocket.py` & `pymycobot-3.4.6b1/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mybuddy.py` & `pymycobot-3.4.6b1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mybuddybluetooth.py` & `pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mybuddyemoticon.py` & `pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mybuddysocket.py` & `pymycobot-3.4.6b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mycobot.py` & `pymycobot-3.4.6b1/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mycobotpro630.py` & `pymycobot-3.4.6b1/pymycobot/mycobotpro630.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,56 +5,61 @@
 import platform
 import time
 import math
 from enum import Enum
 import subprocess
 import logging
 import os
-import can
+
 from pymycobot.log import setup_logging
 
 
 def is_debian_os():
     try:
         # 执行 lsb_release -a 命令，并捕获输出
-        result = subprocess.run(['lsb_release', '-a'], capture_output=True, text=True, check=True)
+        result = subprocess.run(
+            ["lsb_release", "-a"], capture_output=True, text=True, check=True
+        )
 
         # 解析输出，获取 Distributor ID 的信息
-        lines = result.stdout.split('\n')
+        lines = result.stdout.split("\n")
         for line in lines:
-            if line.startswith('Distributor ID:'):
-                distributor_id = line.split(':', 1)[1].strip()
+            if line.startswith("Distributor ID:"):
+                distributor_id = line.split(":", 1)[1].strip()
                 if distributor_id != "Debian":
                     return False
                 return True
 
     except subprocess.CalledProcessError as e:
         print("Error executing lsb_release -a: {}".format(e))
         return False
 
     return None
 
 
 if platform.system() == "Linux" and platform.machine() == "aarch64" and is_debian_os():
     import linuxcnc as elerob
     import hal
-
+    import can
 
     class JogMode(Enum):
         JOG_JOINT = elerob.ANGULAR - 1
         JOG_TELEOP = elerob.LINEAR - 1
+
+
 from time import sleep
 
 try:
     from gpiozero import CPUTemperature
 except ImportError:
 
     def CPUTemperature():
         return 0
 
+
 COORDS_EPSILON = 0.50
 MAX_JOINTS = 6
 MAX_CARTE = 3
 jog_velocity = 1.0  # 100.0/60.0
 angular_jog_velocity = 3600 / 60
 MAX_PINS = 64
 MAX_ANGULAR_SPEED = 6930
@@ -74,15 +79,14 @@
     JOG_JOINT_STATE = 1
     JOG_AXIS_STATE = 2
     MOVE_AXIS_STATE = 3
     MOVE_JOINT_STATE = 4
     RUN_PROGRAM_STATE = 5
 
 
-
 class JogDirection(Enum):
     POSITIVE = 1
     NEGATIVE = -1
 
 
 class Axis(Enum):
     X = 0
@@ -1471,23 +1475,23 @@
         """
         if not self.set_jog_mode(jog_mode):
             return False
         self.s.poll()
         if self.s.task_state != elerob.STATE_ON:
             return False
         if (
-                (jog_mode == JogMode.JOG_JOINT)
-                and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_JOINT)
+            and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
         ) or (
-                (jog_mode == JogMode.JOG_TELEOP)
-                and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_TELEOP)
+            and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
         ):
             return False
         if (jog_mode == JogMode.JOG_JOINT) and (
-                joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
+            joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
         ):
             return False
         if (jog_mode == JogMode.JOG_TELEOP) and (joint_or_axis.value < 0):
             return False
         if jog_id != self.command_id:
             print("_jog_continuous cancelled: some delay: jog_id != command_id")
             return False
@@ -1539,23 +1543,23 @@
         """
         if not self.set_jog_mode(jog_mode):
             return False
         self.s.poll()
         if self.s.task_state != elerob.STATE_ON:
             return False
         if (
-                (jog_mode == JogMode.JOG_JOINT)
-                and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_JOINT)
+            and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
         ) or (
-                (jog_mode == JogMode.JOG_TELEOP)
-                and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_TELEOP)
+            and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
         ):
             return False
         if (jog_mode == JogMode.JOG_JOINT) and (
-                joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
+            joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
         ):
             return False
         if (jog_mode == JogMode.JOG_TELEOP) and (joint_or_axis.value < 0):
             return False
         direction = 1 if incr >= 0 else -1
         self.c.jog(
             elerob.JOG_INCREMENT,
@@ -1606,23 +1610,23 @@
         """
         if not self.set_jog_mode(jog_mode):
             return False
         self.s.poll()
         if self.s.task_state != elerob.STATE_ON:
             return False
         if (
-                (jog_mode == JogMode.JOG_JOINT)
-                and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_JOINT)
+            and (self.s.motion_mode == elerob.TRAJ_MODE_TELEOP)
         ) or (
-                (jog_mode == JogMode.JOG_TELEOP)
-                and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
+            (jog_mode == JogMode.JOG_TELEOP)
+            and (self.s.motion_mode != elerob.TRAJ_MODE_TELEOP)
         ):
             return False
         if (jog_mode == JogMode.JOG_JOINT) and (
-                joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
+            joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
         ):
             return False
         if (jog_mode == JogMode.JOG_TELEOP) and (joint_or_axis.value < 0):
             return False
         if jog_mode == JogMode.JOG_JOINT:
             self.set_angle(joint_or_axis, pos, speed)
             return True
@@ -1641,15 +1645,15 @@
                                 JogMode.JOG_JOINT (joint (1))
             joint_or_axis (Joint | Axis): Joint.J1 ~ Joint.J6 or Axis.X ~ Axis.RZ
 
         Returns:
             bool: True if jog stopped successfully, False otherwise
         """
         if (jog_mode == JogMode.JOG_JOINT) and (
-                joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
+            joint_or_axis.value < 0 or joint_or_axis.value >= MAX_JOINTS
         ):
             return False
         if (jog_mode == JogMode.JOG_TELEOP) and (joint_or_axis.value < 0):
             return False
         self.c.jog(elerob.JOG_STOP, jog_mode.value, joint_or_axis.value)
         return True
 
@@ -1848,16 +1852,16 @@
 
         Returns:
             bool: True if robot is executing a program, False otherwise
         """
         if do_poll:
             self.s.poll()
         return (
-                self.s.task_mode == elerob.MODE_AUTO
-                and self.s.interp_state != elerob.INTERP_IDLE
+            self.s.task_mode == elerob.MODE_AUTO
+            and self.s.interp_state != elerob.INTERP_IDLE
         )
 
     def manual_ok(self, do_poll=True):
         """Returns True if robot state is elerob.STATE_ON and g-code interpreter
         state is elerob.INTERP_IDLE.
 
         Args:
@@ -1927,16 +1931,16 @@
         """Returns current executing line of g-code file.
 
         Returns:
             int: current executing line
         """
         self.s.poll()
         if self.s.task_mode != elerob.MODE_AUTO or self.s.interp_state not in (
-                elerob.INTERP_READING,
-                elerob.INTERP_WAITING,
+            elerob.INTERP_READING,
+            elerob.INTERP_WAITING,
         ):
             return -1
         self.ensure_mode(TaskMode.AUTO)
         return int(self.s.current_line)
 
     def get_current_gcodes(self):
         """Get current execution G-code.
@@ -1961,16 +1965,16 @@
         """Get G-Code interpreter read line.
 
         Returns:
             int: line interpreter is currently reading
         """
         self.s.poll()
         if self.s.task_mode != elerob.MODE_AUTO or self.s.interp_state not in (
-                elerob.INTERP_READING,
-                elerob.INTERP_WAITING,
+            elerob.INTERP_READING,
+            elerob.INTERP_WAITING,
         ):
             return -1
         self.ensure_mode(TaskMode.AUTO)
         return self.s.read_line
 
     def prog_exec_status(self):
         """Returns G-Code interpreter's current state.
@@ -2008,16 +2012,16 @@
         self.ensure_mode(TaskMode.AUTO, TaskMode.MDI)
         self.c.auto(elerob.AUTO_RESUME)
 
     def program_pause(self):
         """Pause currently running program."""
         self.s.poll()
         if self.s.task_mode != elerob.MODE_AUTO or self.s.interp_state not in (
-                elerob.INTERP_READING,
-                elerob.INTERP_WAITING,
+            elerob.INTERP_READING,
+            elerob.INTERP_WAITING,
         ):
             return
         self.ensure_mode(TaskMode.AUTO)
         self.c.auto(elerob.AUTO_PAUSE)
 
     def program_resume(self):
         """Resume program after pause."""
@@ -2038,17 +2042,17 @@
         self.c.abort()
         self.c.wait_complete()
         if not self.is_task_idle():
             self.c.abort()
             self.c.wait_complete()
             self.s.poll()
             print(
-                "Warning: Failed Task abort: task_mode={}, exec_status={}, interp_state={}".format(self.s.task_mode,
-                                                                                                   self.s.exec_state,
-                                                                                                   self.s.interp_state)
+                "Warning: Failed Task abort: task_mode={}, exec_status={}, interp_state={}".format(
+                    self.s.task_mode, self.s.exec_state, self.s.interp_state
+                )
             )
 
     def task_stop_async(self):
         """Stop robot without waiting for stop to complete."""
         self.c.abort()
 
     def get_digital_in(self, pin_number):
@@ -2408,17 +2412,17 @@
                                 angular (JogMode.JOG_JOINT) jog mode
 
         Returns:
             bool: True if change state was successful, False otherwise
         """
         self.s.poll()
         if (
-                self.s.estop
-                or not self.s.enabled
-                or (self.s.interp_state != elerob.INTERP_IDLE)
+            self.s.estop
+            or not self.s.enabled
+            or (self.s.interp_state != elerob.INTERP_IDLE)
         ):
             return False
         if self.s.task_mode != elerob.MODE_MANUAL:
             self.c.mode(elerob.MODE_MANUAL)
             self.c.wait_complete()
             time.sleep(0.2)
         self.s.poll()
@@ -2490,26 +2494,26 @@
         Args:
             coords (list[float | str]): list of coordinate values
 
         Returns:
             str: gcode string to move to given coords
         """
         return (
-                "X"
-                + str(coords[0])
-                + "Y"
-                + str(coords[1])
-                + "Z"
-                + str(coords[2])
-                + "A"
-                + str(coords[3])
-                + "B"
-                + str(coords[4])
-                + "C"
-                + str(coords[5])
+            "X"
+            + str(coords[0])
+            + "Y"
+            + str(coords[1])
+            + "Z"
+            + str(coords[2])
+            + "A"
+            + str(coords[3])
+            + "B"
+            + str(coords[4])
+            + "C"
+            + str(coords[5])
         )
 
     def angles_to_gcode(self, angles):
         """Returns gcode string to move to given joint angles
 
         Args:
             coords (list[float | str]): list of joint angles values
@@ -2540,39 +2544,39 @@
             coords_1 (list): first coords to compare
             coords_2 (list): second coords to compare
 
         Returns:
             bool: True if coords are equal, False otherwise.
         """
         return (
-                self.float_equal(coords_1[Axis.X.value], coords_2[Axis.X.value])
-                and self.float_equal(coords_1[Axis.Y.value], coords_2[Axis.Y.value])
-                and self.float_equal(coords_1[Axis.Z.value], coords_2[Axis.Z.value])
-                and self.float_equal(coords_1[Axis.RX.value], coords_2[Axis.RX.value])
-                and self.float_equal(coords_1[Axis.RY.value], coords_2[Axis.RY.value])
-                and self.float_equal(coords_1[Axis.RZ.value], coords_2[Axis.RZ.value])
+            self.float_equal(coords_1[Axis.X.value], coords_2[Axis.X.value])
+            and self.float_equal(coords_1[Axis.Y.value], coords_2[Axis.Y.value])
+            and self.float_equal(coords_1[Axis.Z.value], coords_2[Axis.Z.value])
+            and self.float_equal(coords_1[Axis.RX.value], coords_2[Axis.RX.value])
+            and self.float_equal(coords_1[Axis.RY.value], coords_2[Axis.RY.value])
+            and self.float_equal(coords_1[Axis.RZ.value], coords_2[Axis.RZ.value])
         )
 
     def angles_equal(self, angles_1, angles_2):
         """Checks if specified angles are equal.
 
         Args:
             angles_1 (list): first angles to compare
             angles_2 (list): second angles to compare
 
         Returns:
             bool: True if angles are equal, False otherwise.
         """
         return (
-                self.float_equal(angles_1[Axis.X.value], angles_2[Axis.X.value])
-                and self.float_equal(angles_1[Axis.Y.value], angles_2[Axis.Y.value])
-                and self.float_equal(angles_1[Axis.Z.value], angles_2[Axis.Z.value])
-                and self.float_equal(angles_1[Axis.RX.value], angles_2[Axis.RX.value])
-                and self.float_equal(angles_1[Axis.RY.value], angles_2[Axis.RY.value])
-                and self.float_equal(angles_1[Axis.RZ.value], angles_2[Axis.RZ.value])
+            self.float_equal(angles_1[Axis.X.value], angles_2[Axis.X.value])
+            and self.float_equal(angles_1[Axis.Y.value], angles_2[Axis.Y.value])
+            and self.float_equal(angles_1[Axis.Z.value], angles_2[Axis.Z.value])
+            and self.float_equal(angles_1[Axis.RX.value], angles_2[Axis.RX.value])
+            and self.float_equal(angles_1[Axis.RY.value], angles_2[Axis.RY.value])
+            and self.float_equal(angles_1[Axis.RZ.value], angles_2[Axis.RZ.value])
         )
 
     def tool_get_firmware_version(self):
         """Returns ESP32 Pico firmware version.
 
         Returns:
             float: firmware version
@@ -2595,19 +2599,23 @@
     def tool_get_digital_in(self, pin_no):
         """Returns digital input pin's value.
 
         Args:
             pin_no (int): pin number
 
         Returns:
-            int : pin value
+            int: pin value
         """
         self.send_can(data=[0x02, 0x62, pin_no])
-        msg = self.receive_can()
-        pin_state = msg.data[2]
+        pin_state = -1
+        for _ in range(100):
+            msg = self.receive_can()
+            if msg.data[0] == 0x03 and msg.data[1] == 0x62 and msg.data[2] == pin_no:
+                pin_state = msg.data[3]
+                break
         return pin_state
 
     def tool_set_led_color(self, r, g, b):
         """Sets RGB color of ESP32 LED.
 
         Args:
             r (int): red color value (0-255)
@@ -2642,16 +2650,15 @@
         Args:
             value (int): value
             speed (int): speed
         """
         self.send_can([0x03, 0x67, value, speed])
 
     def tool_set_gripper_calibrate(self):
-        """Set the current position of the gripper to zero
-        """
+        """Set the current position of the gripper to zero"""
         self.send_can([0x01, 0x68])
 
     def tool_set_gripper_enabled(self, enabled):
         """Enables or disables gripper.
 
         Args:
             enabled (bool): True if enable, False if disable
@@ -2719,15 +2726,15 @@
         Returns:
             int: how many bytes were actually written
         """
         CHUNK_SIZE = 5
         num_chunks = int(len(bytes) / CHUNK_SIZE + 1)
         # print("num_chunks = " + str(num_chunks))
         for i in range(0, len(bytes), CHUNK_SIZE):
-            chunk = bytes[i: i + CHUNK_SIZE]
+            chunk = bytes[i : i + CHUNK_SIZE]
             # print("num_chunks = " + str(num_chunks) + ", i = " + str(i))
             msg_bytes = [0x2 + len(chunk), 0xB5, num_chunks - int(i / CHUNK_SIZE)]
             msg_bytes.extend(list(chunk))
             # print("msg_bytes = " + str(list(msg_bytes)))
             self.send_can(msg_bytes)
         msg = self.receive_can()
         return msg.data[2]
```

### Comparing `pymycobot-3.4.5/pymycobot/mycobotsocket.py` & `pymycobot-3.4.6b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mypalletizer.py` & `pymycobot-3.4.6b1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/mypalletizersocket.py` & `pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/public.py` & `pymycobot-3.4.6b1/pymycobot/public.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/robot_limit.json` & `pymycobot-3.4.6b1/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/ultraArm.py` & `pymycobot-3.4.6b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot/utils.py` & `pymycobot-3.4.6b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.5
+Version: 3.4.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.5/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 pymycobot/mercury.py
 pymycobot/mercury_api.py
 pymycobot/mercurychassis.py
 pymycobot/mercurychassisocket.py
 pymycobot/mercurysocket.py
 pymycobot/myagv.py
 pymycobot/myarm.py
+pymycobot/myarm_api.py
+pymycobot/myarmc.py
+pymycobot/myarmm.py
 pymycobot/myarmsocket.py
 pymycobot/mybuddy.py
 pymycobot/mybuddybluetooth.py
 pymycobot/mybuddyemoticon.py
 pymycobot/mybuddysocket.py
 pymycobot/mycobot.py
 pymycobot/mycobotpro630.py
```

### Comparing `pymycobot-3.4.5/setup.py` & `pymycobot-3.4.6b1/setup.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/tests/test_api.py` & `pymycobot-3.4.6b1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/tests/test_generator.py` & `pymycobot-3.4.6b1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.5/tests/test_socket.py` & `pymycobot-3.4.6b1/tests/test_socket.py`

 * *Files identical despite different names*

