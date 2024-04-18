# Comparing `tmp/dsse-1.0.1.tar.gz` & `tmp/dsse-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.0.1.tar", last modified: Thu Apr 18 19:30:10 2024, max compression
+gzip compressed data, was "dsse-1.0.2.tar", last modified: Thu Apr 18 19:39:32 2024, max compression
```

## Comparing `dsse-1.0.1.tar` & `dsse-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.798695 dsse-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.794695 dsse-1.0.1/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.794695 dsse-1.0.1/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/coverage_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/env_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.794695 dsse-1.0.1/DSSE/environment/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/imgs/drone.png
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/imgs/person-swimming.png
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.794695 dsse-1.0.1/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/simulation/particle_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.798695 dsse-1.0.1/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 19:30:02.000000 dsse-1.0.1/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:10.798695 dsse-1.0.1/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:30:10.000000 dsse-1.0.1/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 19:30:10.000000 dsse-1.0.1/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:30:10.000000 dsse-1.0.1/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 19:30:10.000000 dsse-1.0.1/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 19:30:10.000000 dsse-1.0.1/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 19:30:02.000000 dsse-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:30:02.000000 dsse-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:30:10.798695 dsse-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-18 19:30:02.000000 dsse-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:30:10.798695 dsse-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 19:30:10.000000 dsse-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.916237 dsse-1.0.2/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/coverage_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/env_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/imgs/drone.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/imgs/person-swimming.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/particle_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 19:39:25.000000 dsse-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:39:25.000000 dsse-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:39:32.920237 dsse-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-18 19:39:25.000000 dsse-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:39:32.920237 dsse-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 19:39:32.000000 dsse-1.0.2/setup.py
```

### Comparing `dsse-1.0.1/DSSE/environment/coverage_env.py` & `dsse-1.0.2/DSSE/environment/coverage_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/env.py` & `dsse-1.0.2/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/env_base.py` & `dsse-1.0.2/DSSE/environment/env_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 import numpy as np
 from abc import ABC, abstractmethod
 from pettingzoo import ParallelEnv
 from .entities.drone import DroneData
 from .pygame_interface import PygameInterface
 from .simulation.dynamic_probability import ProbabilityMatrix
-from .simulation.dynamic_probability import ProbabilityMatrix
 from .constants import Actions
 from gymnasium.spaces import MultiDiscrete, Discrete, Tuple, Box
 from copy import copy
 
 
 class DroneSwarmSearchBase(ABC, ParallelEnv):
     def __init__(
```

### Comparing `dsse-1.0.1/DSSE/environment/imgs/drone.png` & `dsse-1.0.2/DSSE/environment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/imgs/person-swimming.png` & `dsse-1.0.2/DSSE/environment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/pygame_interface.py` & `dsse-1.0.2/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.0.2/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/simulation/particle_sim.py` & `dsse-1.0.2/DSSE/environment/simulation/particle_sim.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/environment/simulation/time_step.py` & `dsse-1.0.2/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/tests/drone_policy.py` & `dsse-1.0.2/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/tests/test_env.py` & `dsse-1.0.2/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/tests/test_env_coverage.py` & `dsse-1.0.2/DSSE/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE/tests/test_matrix.py` & `dsse-1.0.2/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/DSSE.egg-info/PKG-INFO` & `dsse-1.0.2/DSSE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.0.1
+Version: 1.0.2
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.2.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
 License: MIT
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gymnasium
```

### Comparing `dsse-1.0.1/DSSE.egg-info/SOURCES.txt` & `dsse-1.0.2/DSSE.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 DSSE.egg-info/top_level.txt
 DSSE/environment/__init__.py
 DSSE/environment/constants.py
 DSSE/environment/coverage_env.py
 DSSE/environment/env.py
 DSSE/environment/env_base.py
 DSSE/environment/pygame_interface.py
+DSSE/environment/entities/__init__.py
+DSSE/environment/entities/drone.py
+DSSE/environment/entities/person.py
 DSSE/environment/imgs/drone.png
 DSSE/environment/imgs/person-swimming.png
 DSSE/environment/simulation/__init__.py
 DSSE/environment/simulation/dynamic_probability.py
 DSSE/environment/simulation/particle_sim.py
 DSSE/environment/simulation/time_step.py
 DSSE/tests/__init__.py
```

### Comparing `dsse-1.0.1/LICENSE` & `dsse-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.0.1/PKG-INFO` & `dsse-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.0.1
+Version: 1.0.2
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.2.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
 License: MIT
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gymnasium
```

### Comparing `dsse-1.0.1/README.md` & `dsse-1.0.2/README.md`

 * *Files identical despite different names*

