# Comparing `tmp/cellworld_game-0.0.15.tar.gz` & `tmp/cellworld_game-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.15.tar", last modified: Wed Apr 17 18:32:48 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.16.tar", last modified: Thu Apr 18 16:24:34 2024, max compression
```

## Comparing `cellworld_game-0.0.15.tar` & `cellworld_game-0.0.16.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 18:32:48.097074 cellworld_game-0.0.15/
--rw-rw-rw-   0        0        0       36 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/MANIFEST.in
--rw-rw-rw-   0        0        0      429 2024-04-17 18:32:48.096074 cellworld_game-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 18:32:48.066882 cellworld_game-0.0.15/cellworld_game/
--rw-rw-rw-   0        0        0       40 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game/README.md
--rw-rw-rw-   0        0        0      399 2024-04-17 15:15:42.000000 cellworld_game-0.0.15/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:32:48.089975 cellworld_game-0.0.15/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      700 2024-04-17 16:19:33.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     9842 2024-04-17 17:55:17.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     8588 2024-04-16 17:26:10.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     7484 2024-04-17 18:10:32.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     2666 2024-04-10 15:31:18.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     4654 2024-04-17 18:08:23.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6071 2024-03-31 20:09:24.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      934 2024-04-17 14:24:14.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     1245 2024-04-12 16:59:11.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/reward.cpython-312.pyc
--rw-rw-rw-   0        0        0     3344 2024-04-16 17:23:22.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-10 15:31:18.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     9429 2024-04-17 18:13:18.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.15/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     5912 2024-04-17 17:55:01.000000 cellworld_game-0.0.15/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.15/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:32:48.092975 cellworld_game-0.0.15/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.15/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.15/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.15/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.15/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     6818 2024-04-16 17:26:07.000000 cellworld_game-0.0.15/cellworld_game/model.py
--rw-rw-rw-   0        0        0     4842 2024-04-17 18:10:29.000000 cellworld_game-0.0.15/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1775 2024-04-10 15:24:24.000000 cellworld_game-0.0.15/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     3242 2024-04-17 18:01:31.000000 cellworld_game-0.0.15/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4973 2024-03-31 20:08:15.000000 cellworld_game-0.0.15/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      269 2024-04-17 14:24:07.000000 cellworld_game-0.0.15/cellworld_game/resources.py
--rw-rw-rw-   0        0        0      619 2024-04-12 16:56:53.000000 cellworld_game-0.0.15/cellworld_game/reward.py
--rw-rw-rw-   0        0        0     1905 2024-04-16 17:23:15.000000 cellworld_game-0.0.15/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game/setup.cfg
--rw-rw-rw-   0        0        0     7908 2024-04-10 15:24:24.000000 cellworld_game-0.0.15/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6402 2024-04-17 18:29:02.000000 cellworld_game-0.0.15/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.15/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:32:48.095050 cellworld_game-0.0.15/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      429 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 18:32:48.097074 cellworld_game-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-04-17 18:32:47.000000 cellworld_game-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:24:34.368235 cellworld_game-0.0.16/
+-rw-rw-rw-   0        0        0       36 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/MANIFEST.in
+-rw-rw-rw-   0        0        0      429 2024-04-18 16:24:34.367246 cellworld_game-0.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 16:24:34.335126 cellworld_game-0.0.16/cellworld_game/
+-rw-rw-rw-   0        0        0       40 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      381 2024-04-18 16:24:24.000000 cellworld_game-0.0.16/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:24:34.361234 cellworld_game-0.0.16/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      700 2024-04-17 16:19:33.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9842 2024-04-17 17:55:17.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8588 2024-04-16 17:26:10.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7484 2024-04-17 18:10:32.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2666 2024-04-10 15:31:18.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4654 2024-04-17 18:08:23.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6071 2024-03-31 20:09:24.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      934 2024-04-17 14:24:14.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1245 2024-04-12 16:59:11.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/reward.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3344 2024-04-16 17:23:22.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-10 15:31:18.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9429 2024-04-17 18:13:18.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.16/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5912 2024-04-17 17:55:01.000000 cellworld_game-0.0.16/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.16/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:24:34.364237 cellworld_game-0.0.16/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.16/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.16/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.16/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.16/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     6818 2024-04-16 17:26:07.000000 cellworld_game-0.0.16/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     4237 2024-04-18 16:24:24.000000 cellworld_game-0.0.16/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1775 2024-04-10 15:24:24.000000 cellworld_game-0.0.16/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     3242 2024-04-17 18:01:31.000000 cellworld_game-0.0.16/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4973 2024-03-31 20:08:15.000000 cellworld_game-0.0.16/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      269 2024-04-17 14:24:07.000000 cellworld_game-0.0.16/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0      619 2024-04-12 16:56:53.000000 cellworld_game-0.0.16/cellworld_game/reward.py
+-rw-rw-rw-   0        0        0     1905 2024-04-16 17:23:15.000000 cellworld_game-0.0.16/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/cellworld_game/setup.cfg
+-rw-rw-rw-   0        0        0     7908 2024-04-10 15:24:24.000000 cellworld_game-0.0.16/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6402 2024-04-17 18:29:02.000000 cellworld_game-0.0.16/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.16/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:24:34.366244 cellworld_game-0.0.16/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      429 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-18 16:24:34.000000 cellworld_game-0.0.16/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 16:24:34.368235 cellworld_game-0.0.16/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-04-18 16:24:33.000000 cellworld_game-0.0.16/setup.py
```

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/mouse.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/resources.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/resources.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/reward.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/reward.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/view.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.16/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/agent.py` & `cellworld_game-0.0.16/cellworld_game/agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.16/cellworld_game/cellworld_loader.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/files/agent.png` & `cellworld_game-0.0.16/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/files/predator.png` & `cellworld_game-0.0.16/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/files/prey.png` & `cellworld_game-0.0.16/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/license.txt` & `cellworld_game-0.0.16/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/model.py` & `cellworld_game-0.0.16/cellworld_game/model.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/mouse.py` & `cellworld_game-0.0.16/cellworld_game/mouse.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,17 @@
 
 import pygame
 from .agent import AgentState, Agent
 from .navigation import Navigation
 from .navigation_agent import NavigationAgent
 from .resources import Resources
 import shapely as sp
-from enum import Enum
 from .util import distance
 
 
-class MouseObservation(typing.List[float]):
-    class Field(Enum):
-        prey_x = 0
-        prey_y = 1
-        prey_direction = 2
-        predator_x = 3
-        predator_y = 4
-        predator_direction = 5
-        goal_distance = 6
-        predator_distance = 7
-        puffed = 8
-        puff_cooled_down = 9
-        finished = 10
-
-    def __init__(self):
-        super().__init__()
-        for i in MouseObservation.Field:
-            self.append(0.0)
-
-    def __setitem__(self, field: Field, value):
-        list.__setitem__(self, field.value, value)
-
-
 class Mouse(NavigationAgent):
     def __init__(self,
                  start_state: AgentState,
                  actions: typing.List[typing.Tuple[float, float]],
                  goal_location: typing.Tuple[float, float],
                  goal_threshold: float,
                  puff_threshold: float,
```

### Comparing `cellworld_game-0.0.15/cellworld_game/navigation.py` & `cellworld_game-0.0.16/cellworld_game/navigation.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.16/cellworld_game/navigation_agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.16/cellworld_game/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/reward.py` & `cellworld_game-0.0.16/cellworld_game/reward.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/robot.py` & `cellworld_game-0.0.16/cellworld_game/robot.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/util.py` & `cellworld_game-0.0.16/cellworld_game/util.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/view.py` & `cellworld_game-0.0.16/cellworld_game/view.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game/visibility.py` & `cellworld_game-0.0.16/cellworld_game/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.16/cellworld_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.15/setup.py` & `cellworld_game-0.0.16/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_game/README.md').read(),
       long_description_content_type='text/markdown',
       packages=['cellworld_game'],
       install_requires=['cellworld', 'pygame', 'shapely'],
       license='MIT',
       include_package_data=True,
-      version='0.0.15',
+      version='0.0.16',
       zip_safe=False)
```

