# Comparing `tmp/talklib-1.2.0.tar.gz` & `tmp/talklib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talklib-1.2.0.tar", last modified: Fri Apr  5 20:24:09 2024, max compression
+gzip compressed data, was "talklib-1.2.1.tar", last modified: Thu Apr 18 19:27:28 2024, max compression
```

## Comparing `talklib-1.2.0.tar` & `talklib-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:24:09.049886 talklib-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-05 20:24:03.000000 talklib-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-05 20:24:09.049886 talklib-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-05 20:24:03.000000 talklib-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-05 20:24:03.000000 talklib-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 20:24:03.000000 talklib-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:24:09.049886 talklib-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:24:09.045886 talklib-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:24:09.049886 talklib-1.2.0/src/talklib/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/ev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-05 20:24:03.000000 talklib-1.2.0/src/talklib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:24:09.049886 talklib-1.2.0/src/talklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-05 20:24:09.000000 talklib-1.2.0/src/talklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 20:24:09.000000 talklib-1.2.0/src/talklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:24:09.000000 talklib-1.2.0/src/talklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 20:24:09.000000 talklib-1.2.0/src/talklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 20:24:09.000000 talklib-1.2.0/src/talklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 19:27:22.000000 talklib-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 19:27:28.707447 talklib-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-18 19:27:22.000000 talklib-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-18 19:27:22.000000 talklib-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 19:27:22.000000 talklib-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:27:28.707447 talklib-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.703447 talklib-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/src/talklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/src/talklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/top_level.txt
```

### Comparing `talklib-1.2.0/LICENSE.txt` & `talklib-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/PKG-INFO` & `talklib-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.0/README.md` & `talklib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/pyproject.toml` & `talklib-1.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "talklib"
-version = "1.2.0"
+version = "1.2.1"
 description = "A package to automate processing of shows/segments airing on the TL"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 maintainers = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `talklib-1.2.0/requirements.txt` & `talklib-1.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib/ev.py` & `talklib-1.2.1/src/talklib/ev.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib/ffmpeg.py` & `talklib-1.2.1/src/talklib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib/notify.py` & `talklib-1.2.1/src/talklib/notify.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib/show.py` & `talklib-1.2.1/src/talklib/show.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib/utils.py` & `talklib-1.2.1/src/talklib/utils.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.0/src/talklib.egg-info/PKG-INFO` & `talklib-1.2.1/src/talklib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.0/src/talklib.egg-info/requires.txt` & `talklib-1.2.1/src/talklib.egg-info/requires.txt`

 * *Files identical despite different names*

