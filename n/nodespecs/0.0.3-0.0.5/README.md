# Comparing `tmp/nodespecs-0.0.3.tar.gz` & `tmp/nodespecs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.3.tar", last modified: Thu Apr 18 20:27:48 2024, max compression
+gzip compressed data, was "nodespecs-0.0.5.tar", last modified: Thu Apr 18 21:08:36 2024, max compression
```

## Comparing `nodespecs-0.0.3.tar` & `nodespecs-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.230646 nodespecs-0.0.3/
--rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5755 2024-04-18 20:27:48.228651 nodespecs-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3874 2024-04-18 20:26:59.000000 nodespecs-0.0.3/README.md
--rw-rw-rw-   0        0        0      899 2024-04-18 20:24:28.000000 nodespecs-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 20:27:48.230646 nodespecs-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.193827 nodespecs-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.227307 nodespecs-0.0.3/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     5755 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.224319 nodespecs-0.0.3/src/specs/
--rw-rw-rw-   0        0        0       91 2024-04-18 20:27:13.000000 nodespecs-0.0.3/src/specs/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.3/src/specs/__main__.py
--rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.3/src/specs/cmd.py
--rw-rw-rw-   0        0        0     1400 2024-04-12 15:15:38.000000 nodespecs-0.0.3/src/specs/cpu-benchmark.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.3/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7189 2024-04-12 22:25:26.000000 nodespecs-0.0.3/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.093700 nodespecs-0.0.5/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5854 2024-04-18 21:08:36.091010 nodespecs-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3973 2024-04-18 20:55:37.000000 nodespecs-0.0.5/README.md
+-rw-rw-rw-   0        0        0      899 2024-04-18 21:07:43.000000 nodespecs-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 21:08:36.094153 nodespecs-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.055012 nodespecs-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.089013 nodespecs-0.0.5/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     5854 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.087014 nodespecs-0.0.5/src/specs/
+-rw-rw-rw-   0        0        0       91 2024-04-18 21:06:53.000000 nodespecs-0.0.5/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.5/src/specs/__main__.py
+-rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.5/src/specs/cmd.py
+-rw-rw-rw-   0        0        0     1400 2024-04-12 15:15:38.000000 nodespecs-0.0.5/src/specs/cpu-benchmark.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.5/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7189 2024-04-12 22:25:26.000000 nodespecs-0.0.5/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.3/LICENSE` & `nodespecs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.3/PKG-INFO` & `nodespecs-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.3
+Version: 0.0.5
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -16,32 +16,39 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.5
-Requires-Dist: tabulate>=0.9.0
+Requires-Dist: tabulate>=0.8.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
 
 
 ### install and use with pip
 
 ```shell
-pip install node-specs
+pip install nodespecs
 python -m specs
 ```
 
+```
+sudo apt install python3-pip
+python3 -m pip install nodespecs && python3 -m specs
+```
+
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
```

### Comparing `nodespecs-0.0.3/README.md` & `nodespecs-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
 
 
 ### install and use with pip
 
 ```shell
-pip install node-specs
+pip install nodespecs
 python -m specs
 ```
 
+```
+sudo apt install python3-pip
+python3 -m pip install nodespecs && python3 -m specs
+```
+
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
```

### Comparing `nodespecs-0.0.3/pyproject.toml` & `nodespecs-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.3"
+version = "0.0.5"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["cpu", "gpu", "benchmark"]
 dependencies = [
     "psutil >= 5.9.5",
-    "tabulate >= 0.9.0",
+    "tabulate >= 0.8.0",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = ["GPUtil","pip-tools"]
```

### Comparing `nodespecs-0.0.3/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.5/src/nodespecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.3
+Version: 0.0.5
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -16,32 +16,39 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.5
-Requires-Dist: tabulate>=0.9.0
+Requires-Dist: tabulate>=0.8.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
 
 
 ### install and use with pip
 
 ```shell
-pip install node-specs
+pip install nodespecs
 python -m specs
 ```
 
+```
+sudo apt install python3-pip
+python3 -m pip install nodespecs && python3 -m specs
+```
+
+
+
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
```

### Comparing `nodespecs-0.0.3/src/specs/cpu-benchmark.py` & `nodespecs-0.0.5/src/specs/cpu-benchmark.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.3/src/specs/cpuinfo.py` & `nodespecs-0.0.5/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.3/src/specs/hardware.py` & `nodespecs-0.0.5/src/specs/hardware.py`

 * *Files identical despite different names*

