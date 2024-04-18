# Comparing `tmp/clidoro-0.1.0.tar.gz` & `tmp/clidoro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidoro-0.1.0.tar", last modified: Thu Apr 18 08:15:25 2024, max compression
+gzip compressed data, was "clidoro-0.1.1.tar", last modified: Thu Apr 18 08:21:03 2024, max compression
```

## Comparing `clidoro-0.1.0.tar` & `clidoro-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.715319 clidoro-0.1.0/
--rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.0/LICENSE.MD
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:15:25.715319 clidoro-0.1.0/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.0/README.md
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.711319 clidoro-0.1.0/clidoro/
--rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.0/clidoro/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.0/clidoro/_utils.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.1.0/clidoro/chart.py
--rw-------   0 juno      (1000) juno      (1000)     3716 2024-04-18 08:12:17.000000 clidoro-0.1.0/clidoro/clidoro.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.0/clidoro/data.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.711319 clidoro-0.1.0/clidoro/termgraph/
--rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.0/clidoro/termgraph/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.0/clidoro/termgraph/_termgraph.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.0/clidoro/termgraph/module.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.0/clidoro/termgraph/utils.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:15:25.715319 clidoro-0.1.0/clidoro.egg-info/
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)      464 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/SOURCES.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/dependency_links.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/entry_points.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.0/clidoro.egg-info/not-zip-safe
--rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/requires.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 08:15:25.000000 clidoro-0.1.0/clidoro.egg-info/top_level.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 08:15:25.715319 clidoro-0.1.0/setup.cfg
--rw-rw-r--   0 juno      (1000) juno      (1000)     1831 2024-04-18 08:14:51.000000 clidoro-0.1.0/setup.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:21:03.830848 clidoro-0.1.1/
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.1/LICENSE.MD
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:21:03.830848 clidoro-0.1.1/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.1/README.md
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:21:03.826848 clidoro-0.1.1/clidoro/
+-rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.1/clidoro/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.1/clidoro/_utils.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.1.1/clidoro/chart.py
+-rw-------   0 juno      (1000) juno      (1000)     3716 2024-04-18 08:12:17.000000 clidoro-0.1.1/clidoro/clidoro.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.1/clidoro/data.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:21:03.830848 clidoro-0.1.1/clidoro/termgraph/
+-rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.1/clidoro/termgraph/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.1/clidoro/termgraph/_termgraph.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.1/clidoro/termgraph/module.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.1/clidoro/termgraph/utils.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:21:03.830848 clidoro-0.1.1/clidoro.egg-info/
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)      464 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/SOURCES.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/dependency_links.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/entry_points.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.1/clidoro.egg-info/not-zip-safe
+-rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/requires.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 08:21:03.000000 clidoro-0.1.1/clidoro.egg-info/top_level.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 08:21:03.830848 clidoro-0.1.1/setup.cfg
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1946 2024-04-18 08:19:35.000000 clidoro-0.1.1/setup.py
```

### Comparing `clidoro-0.1.0/LICENSE.MD` & `clidoro-0.1.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/PKG-INFO` & `clidoro-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.0
+Version: 0.1.1
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.0/README.md` & `clidoro-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/_utils.py` & `clidoro-0.1.1/clidoro/_utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/chart.py` & `clidoro-0.1.1/clidoro/chart.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/clidoro.py` & `clidoro-0.1.1/clidoro/clidoro.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/data.py` & `clidoro-0.1.1/clidoro/data.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/termgraph/_termgraph.py` & `clidoro-0.1.1/clidoro/termgraph/_termgraph.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/termgraph/module.py` & `clidoro-0.1.1/clidoro/termgraph/module.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro/termgraph/utils.py` & `clidoro-0.1.1/clidoro/termgraph/utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.0/clidoro.egg-info/PKG-INFO` & `clidoro-0.1.1/clidoro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.0
+Version: 0.1.1
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.0/setup.py` & `clidoro-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "1"
-MICRO_VERSION = "0"
+MICRO_VERSION = "1"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 
 setup(
     name="clidoro",
     packages=find_packages(exclude=["docs", "tests*", "examples"]),
     version=VERSION,
@@ -47,8 +47,12 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: System :: Software Distribution",
         "Topic :: System :: Systems Administration",
         "Topic :: Utilities",
     ],
+    package_data={
+        # Include all .jpg files under the clidoro package
+        "clidoro": ["*.jpg"],
+    },
 )
```

