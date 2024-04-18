# Comparing `tmp/coppyr-0.9.3.tar.gz` & `tmp/coppyr-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coppyr-0.9.3.tar", last modified: Mon May  1 18:02:45 2023, max compression
+gzip compressed data, was "coppyr-0.9.4.tar", last modified: Thu Apr 18 20:36:11 2024, max compression
```

## Comparing `coppyr-0.9.3.tar` & `coppyr-0.9.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       58 2023-04-28 19:06:54.000000 coppyr-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4983 2023-05-01 18:02:45.258540 coppyr-0.9.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.254540 coppyr-0.9.3/coppyr/
--rw-rw-r--   0 root         (0) root         (0)      437 2023-05-01 18:01:28.000000 coppyr-0.9.3/coppyr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/collections/
--rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/collections/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/collections/cycle.py
--rw-rw-r--   0 root         (0) root         (0)      856 2023-04-28 16:36:15.000000 coppyr-0.9.3/coppyr/collections/dotdict.py
--rw-rw-r--   0 root         (0) root         (0)     1871 2023-04-28 22:23:32.000000 coppyr-0.9.3/coppyr/config.py
--rw-rw-r--   0 root         (0) root         (0)     4362 2023-05-01 18:00:33.000000 coppyr-0.9.3/coppyr/context.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.3/coppyr/daemon.py
--rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.3/coppyr/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/extensions/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/extensions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.3/coppyr/extensions/load.py
--rw-rw-r--   0 root         (0) root         (0)     4735 2023-05-01 00:53:09.000000 coppyr-0.9.3/coppyr/logger.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.3/coppyr/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/process/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-27 19:30:48.000000 coppyr-0.9.3/coppyr/process/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.3/coppyr/process/concurrent.py
--rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.3/coppyr/process/parallel.py
--rw-rw-r--   0 root         (0) root         (0)     3881 2023-04-28 22:09:04.000000 coppyr-0.9.3/coppyr/process/subp.py
--rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/types/
--rw-rw-r--   0 root         (0) root         (0)      179 2023-04-27 21:29:25.000000 coppyr-0.9.3/coppyr/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3569 2023-04-27 23:05:32.000000 coppyr-0.9.3/coppyr/types/differ.py
--rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/types/lazyproperty.py
--rw-rw-r--   0 root         (0) root         (0)     1187 2023-04-27 19:30:58.000000 coppyr-0.9.3/coppyr/types/singleton.py
--rw-rw-r--   0 root         (0) root         (0)      763 2023-04-27 19:56:36.000000 coppyr-0.9.3/coppyr/types/slot.py
--rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.3/coppyr/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4983 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      152 2023-04-28 22:20:08.000000 coppyr-0.9.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 18:02:45.258540 coppyr-0.9.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.3/setup.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/
+-rw-r--r--   0      503 dialout     (20)     1072 2024-04-18 16:30:23.000000 coppyr-0.9.4/LICENSE
+-rw-r--r--   0      503 dialout     (20)       58 2024-04-18 16:30:23.000000 coppyr-0.9.4/MANIFEST.in
+-rw-r--r--   0      503 dialout     (20)     5551 2024-04-18 20:36:11.000000 coppyr-0.9.4/PKG-INFO
+-rw-r--r--   0      503 dialout     (20)     4266 2024-04-18 16:30:23.000000 coppyr-0.9.4/README.rst
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr/
+-rw-r--r--   0      503 dialout     (20)      437 2024-04-18 20:17:27.000000 coppyr-0.9.4/coppyr/__init__.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr/collections/
+-rw-r--r--   0      503 dialout     (20)       78 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/collections/__init__.py
+-rw-r--r--   0      503 dialout     (20)     1091 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/collections/cycle.py
+-rw-r--r--   0      503 dialout     (20)      856 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/collections/dotdict.py
+-rw-r--r--   0      503 dialout     (20)     1967 2024-04-18 20:13:09.000000 coppyr-0.9.4/coppyr/config.py
+-rw-r--r--   0      503 dialout     (20)     4568 2024-04-18 20:12:09.000000 coppyr-0.9.4/coppyr/context.py
+-rw-r--r--   0      503 dialout     (20)     2316 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/daemon.py
+-rw-r--r--   0      503 dialout     (20)     1645 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/error.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr/extensions/
+-rw-r--r--   0      503 dialout     (20)       24 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/extensions/__init__.py
+-rw-r--r--   0      503 dialout     (20)     3152 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/extensions/load.py
+-rw-r--r--   0      503 dialout     (20)     4735 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/logger.py
+-rw-r--r--   0      503 dialout     (20)     2428 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/package.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr/process/
+-rw-r--r--   0      503 dialout     (20)       24 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/process/__init__.py
+-rw-r--r--   0      503 dialout     (20)     1431 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/process/concurrent.py
+-rw-r--r--   0      503 dialout     (20)    10918 2024-04-18 20:05:53.000000 coppyr-0.9.4/coppyr/process/parallel.py
+-rw-r--r--   0      503 dialout     (20)     3881 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/process/subp.py
+-rw-r--r--   0      503 dialout     (20)      389 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/testing.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr/types/
+-rw-r--r--   0      503 dialout     (20)      179 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/types/__init__.py
+-rw-r--r--   0      503 dialout     (20)     3569 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/types/differ.py
+-rw-r--r--   0      503 dialout     (20)      351 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/types/lazyproperty.py
+-rw-r--r--   0      503 dialout     (20)     1187 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/types/singleton.py
+-rw-r--r--   0      503 dialout     (20)      763 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/types/slot.py
+-rw-r--r--   0      503 dialout     (20)     1028 2024-04-18 16:30:23.000000 coppyr-0.9.4/coppyr/web.py
+drwxr-xr-x   0      503 dialout     (20)        0 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/
+-rw-r--r--   0      503 dialout     (20)     5551 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/PKG-INFO
+-rw-r--r--   0      503 dialout     (20)      732 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/SOURCES.txt
+-rw-r--r--   0      503 dialout     (20)        1 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/dependency_links.txt
+-rw-r--r--   0      503 dialout     (20)      166 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/requires.txt
+-rw-r--r--   0      503 dialout     (20)        7 2024-04-18 20:36:11.000000 coppyr-0.9.4/coppyr.egg-info/top_level.txt
+-rw-r--r--   0      503 dialout     (20)      152 2024-04-18 16:30:23.000000 coppyr-0.9.4/pyproject.toml
+-rw-r--r--   0      503 dialout     (20)       38 2024-04-18 20:36:11.000000 coppyr-0.9.4/setup.cfg
+-rw-r--r--   0      503 dialout     (20)     1285 2024-04-18 16:30:23.000000 coppyr-0.9.4/setup.py
```

### Comparing `coppyr-0.9.3/LICENSE` & `coppyr-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/PKG-INFO` & `coppyr-0.9.4/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: coppyr
-Version: 0.9.3
-Summary: A collection of boilerplate for Python applications.
-Home-page: https://github.com/gshulegaard/coppyr
-Author: Grant Hulegaard
-Author-email: loki.labrys@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: config
-Provides-Extra: daemon
-Provides-Extra: dev
-Provides-Extra: pkg
-Provides-Extra: all
-License-File: LICENSE
-
-
 ======
 Coppyr
 ======
 
 Coppyr (Copp-**er**) is a collecton of useful Python boilerplate that I find
 myself reusing frequently between projects.
```

### Comparing `coppyr-0.9.3/README.rst` & `coppyr-0.9.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: coppyr
+Version: 0.9.4
+Summary: A collection of boilerplate for Python applications.
+Home-page: https://github.com/gshulegaard/coppyr
+Author: Grant Hulegaard
+Author-email: loki.labrys@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
+Provides-Extra: config
+Requires-Dist: PyYAML; extra == "config"
+Requires-Dist: toml; extra == "config"
+Provides-Extra: daemon
+Requires-Dist: python-daemon==2.3.2; extra == "daemon"
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: semver; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: pkg
+Requires-Dist: pip>=10; extra == "pkg"
+Provides-Extra: all
+Requires-Dist: PyYAML; extra == "all"
+Requires-Dist: toml; extra == "all"
+Requires-Dist: python-daemon==2.3.2; extra == "all"
+Requires-Dist: pip>=10; extra == "all"
+
+
 ======
 Coppyr
 ======
 
 Coppyr (Copp-**er**) is a collecton of useful Python boilerplate that I find
 myself reusing frequently between projects.
```

### Comparing `coppyr-0.9.3/coppyr/collections/cycle.py` & `coppyr-0.9.4/coppyr/collections/cycle.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/collections/dotdict.py` & `coppyr-0.9.4/coppyr/collections/dotdict.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/config.py` & `coppyr-0.9.4/coppyr/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 # errors
 
 
 class CoppyrConfigIOError(CoppyrError):
     description = "Error opening the config file."
 
 
-class CoppyrConfigYAMLError(CoppyrError):
+class CoppyrConfigYamlError(CoppyrError):
     description = "Couldn't load YAML."
 
 
+class CoppyrConfigTomlError(CoppyrError):
+    description = "Couldn't load TOML."
+
+
 # objects
 
 
 class AbstractConfig(DotDict):
     def __init__(self, file_path: str=None):
         """
         :param file_path: String
@@ -32,50 +36,51 @@
             )
 
         self.__file_path__ = file_path
 
         # Load KV arguments into DotDict
         super().__init__(**self.load(file_path))
 
-    @abc.abstractstaticmethod
+    @staticmethod
+    @abc.abstractmethod
     def load(file_path: str) -> Dict:
         return {}
 
 
-class YAMLConfig(AbstractConfig):
+class YamlConfig(AbstractConfig):
     @staticmethod
     def load(file_path: str):
         import yaml
 
         try:
             with open(file_path, "r") as f:
                 raw = yaml.load(f, Loader=yaml.CLoader)
         except IOError as e:
             raise CoppyrConfigIOError(
                 f"Failed to load file path \"{file_path}\".",
                 caught=e
             )
         except Exception as e:
-            raise CoppyrConfigYAMLError(caught=e)
+            raise CoppyrConfigYamlError(caught=e)
 
         return raw
 
 
-class TOMLConfig(AbstractConfig):
+class TomlConfig(AbstractConfig):
     @staticmethod
     def load(file_path: str):
         import toml
 
         try:
             raw = toml.load(file_path)
         except IOError as e:
             raise CoppyrConfigIOError(
                 f"Failed to load file path \"{file_path}\".",
                 caught=e
             )
         except Exception as e:
-            raise CoppyrConfigYAMLError(caught=e)
+            raise CoppyrConfigTomlError(caught=e)
 
         return raw
 
 
 # TODO: Add an environment lookup for the configuration bit.
```

### Comparing `coppyr-0.9.3/coppyr/context.py` & `coppyr-0.9.4/coppyr/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,16 +131,21 @@
     def fqdn(self):
         import socket
         return socket.getfqdn()
 
     @lazyproperty
     def config(self):
         if self.config_path:
-            from coppyr.config import YAMLConfig
-            return YAMLConfig(self.config_path)
+            import coppyr.config as cfg
+
+            # Try to load config as toml, if that fails to parse, try to load as yaml.
+            try:
+                return cfg.TomlConfig(self.config_path)
+            except cfg.CoppyrConfigTomlError:
+                return cfg.YamlConfig(self.config_path)
         else:
             return DotDict()
 
     @lazyproperty
     def log(self):
         from coppyr import logger
```

### Comparing `coppyr-0.9.3/coppyr/daemon.py` & `coppyr-0.9.4/coppyr/daemon.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/error.py` & `coppyr-0.9.4/coppyr/error.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/extensions/load.py` & `coppyr-0.9.4/coppyr/extensions/load.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/logger.py` & `coppyr-0.9.4/coppyr/logger.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/package.py` & `coppyr-0.9.4/coppyr/package.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/process/concurrent.py` & `coppyr-0.9.4/coppyr/process/concurrent.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/process/parallel.py` & `coppyr-0.9.4/coppyr/process/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import multiprocessing as mp
 import queue as q
 import sys
 import uuid
 
-from coppyr.singleton import Singleton
+from coppyr.types.singleton import Singleton
 
 
 class Worker(object):
     """
     This is a utility wrapper for taking a function and converting it into a
     callable that accepts Queue pipes from Parent process rather than direct
     inputs.
```

### Comparing `coppyr-0.9.3/coppyr/process/subp.py` & `coppyr-0.9.4/coppyr/process/subp.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/types/differ.py` & `coppyr-0.9.4/coppyr/types/differ.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/types/singleton.py` & `coppyr-0.9.4/coppyr/types/singleton.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/types/slot.py` & `coppyr-0.9.4/coppyr/types/slot.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr/web.py` & `coppyr-0.9.4/coppyr/web.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/coppyr.egg-info/PKG-INFO` & `coppyr-0.9.4/coppyr.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.3
+Version: 0.9.4
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
 Provides-Extra: config
+Requires-Dist: PyYAML; extra == "config"
+Requires-Dist: toml; extra == "config"
 Provides-Extra: daemon
+Requires-Dist: python-daemon==2.3.2; extra == "daemon"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: semver; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Provides-Extra: pkg
+Requires-Dist: pip>=10; extra == "pkg"
 Provides-Extra: all
-License-File: LICENSE
+Requires-Dist: PyYAML; extra == "all"
+Requires-Dist: toml; extra == "all"
+Requires-Dist: python-daemon==2.3.2; extra == "all"
+Requires-Dist: pip>=10; extra == "all"
 
 
 ======
 Coppyr
 ======
 
 Coppyr (Copp-**er**) is a collecton of useful Python boilerplate that I find
```

### Comparing `coppyr-0.9.3/coppyr.egg-info/SOURCES.txt` & `coppyr-0.9.4/coppyr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.3/setup.py` & `coppyr-0.9.4/setup.py`

 * *Files identical despite different names*

