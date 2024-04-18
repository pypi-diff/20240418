# Comparing `tmp/clidoro-0.0.2.tar.gz` & `tmp/clidoro-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidoro-0.0.2.tar", last modified: Thu Apr 18 05:45:10 2024, max compression
+gzip compressed data, was "clidoro-0.0.3.tar", last modified: Thu Apr 18 06:40:58 2024, max compression
```

## Comparing `clidoro-0.0.2.tar` & `clidoro-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 05:45:10.149813 clidoro-0.0.2/
--rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.0.2/LICENSE.MD
--rw-r--r--   0 juno      (1000) juno      (1000)     1185 2024-04-18 05:45:10.149813 clidoro-0.0.2/PKG-INFO
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 05:45:10.145813 clidoro-0.0.2/clidoro/
--rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.0.2/clidoro/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2422 2024-04-18 04:51:34.000000 clidoro-0.0.2/clidoro/_utils.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 04:58:08.000000 clidoro-0.0.2/clidoro/chart.py
--rw-------   0 juno      (1000) juno      (1000)     3259 2024-04-18 05:17:27.000000 clidoro-0.0.2/clidoro/clidoro.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      449 2024-04-18 04:56:29.000000 clidoro-0.0.2/clidoro/data.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 05:45:10.145813 clidoro-0.0.2/clidoro/termgraph/
--rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.0.2/clidoro/termgraph/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.0.2/clidoro/termgraph/_termgraph.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.0.2/clidoro/termgraph/module.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.0.2/clidoro/termgraph/utils.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 05:45:10.149813 clidoro-0.0.2/clidoro.egg-info/
--rw-r--r--   0 juno      (1000) juno      (1000)     1185 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)      444 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/SOURCES.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/dependency_links.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/entry_points.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.0.2/clidoro.egg-info/not-zip-safe
--rw-rw-r--   0 juno      (1000) juno      (1000)       42 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/requires.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 05:45:10.000000 clidoro-0.0.2/clidoro.egg-info/top_level.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       38 2024-04-18 05:45:10.149813 clidoro-0.0.2/setup.cfg
--rw-rw-r--   0 juno      (1000) juno      (1000)     1609 2024-04-18 05:44:47.000000 clidoro-0.0.2/setup.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.0.3/LICENSE.MD
+-rw-r--r--   0 juno      (1000) juno      (1000)     2500 2024-04-18 06:40:58.958819 clidoro-0.0.3/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1289 2024-04-18 05:46:55.000000 clidoro-0.0.3/README.md
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.954819 clidoro-0.0.3/clidoro/
+-rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.0.3/clidoro/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2422 2024-04-18 04:51:34.000000 clidoro-0.0.3/clidoro/_utils.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.0.3/clidoro/chart.py
+-rw-------   0 juno      (1000) juno      (1000)     3259 2024-04-18 06:32:04.000000 clidoro-0.0.3/clidoro/clidoro.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      449 2024-04-18 04:56:29.000000 clidoro-0.0.3/clidoro/data.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/clidoro/termgraph/
+-rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.0.3/clidoro/termgraph/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.0.3/clidoro/termgraph/_termgraph.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.0.3/clidoro/termgraph/module.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.0.3/clidoro/termgraph/utils.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 06:40:58.958819 clidoro-0.0.3/clidoro.egg-info/
+-rw-r--r--   0 juno      (1000) juno      (1000)     2500 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)      464 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/SOURCES.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/dependency_links.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/entry_points.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.0.3/clidoro.egg-info/not-zip-safe
+-rw-rw-r--   0 juno      (1000) juno      (1000)       60 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/requires.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 06:40:58.000000 clidoro-0.0.3/clidoro.egg-info/top_level.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 06:40:58.962819 clidoro-0.0.3/setup.cfg
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1811 2024-04-18 06:40:27.000000 clidoro-0.0.3/setup.py
```

### Comparing `clidoro-0.0.2/LICENSE.MD` & `clidoro-0.0.3/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/_utils.py` & `clidoro-0.0.3/clidoro/_utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/chart.py` & `clidoro-0.0.3/clidoro/chart.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/clidoro.py` & `clidoro-0.0.3/clidoro/clidoro.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/termgraph/_termgraph.py` & `clidoro-0.0.3/clidoro/termgraph/_termgraph.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/termgraph/module.py` & `clidoro-0.0.3/clidoro/termgraph/module.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/clidoro/termgraph/utils.py` & `clidoro-0.0.3/clidoro/termgraph/utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.0.2/setup.py` & `clidoro-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from setuptools import find_packages, setup
 
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = "\n" + f.read()
+
 MAJOR_VERSION = "0"
 MINOR_VERSION = "0"
-MICRO_VERSION = "2"
+MICRO_VERSION = "3"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 
 setup(
     name="clidoro",
     packages=find_packages(exclude=["docs", "tests*", "examples"]),
     version=VERSION,
     license="MIT",
     zip_safe=False,
     platforms="Linux",
     description="clidoro: pomodoro in your cli",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kingjuno/clidoro",
     entry_points={"console_scripts": ["clidoro = clidoro.clidoro:main"]},
     keywords=["Productivity", "Pomodoro"],
-    install_requires=["playsound", "alive-progress", "simple-term-menu"],
+    install_requires=[
+        "playsound",
+        "alive-progress",
+        "simple-term-menu",
+        "requests",
+        "colorama",
+    ],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Intended Audience :: System Administrators",
         "Operating System :: Unix",
         # TODO: Add Windows support
         # TODO: Add Mac support
```

