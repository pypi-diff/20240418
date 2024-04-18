# Comparing `tmp/interlinked-0.3.zip` & `tmp/interlinked-0.3.1.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 11713 bytes, number of entries: 24
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:48 interlinked-0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:48 interlinked-0.3/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:48 interlinked-0.3/interlinked/
--rw-r--r--  2.0 unx      129 b- defN 24-Apr-18 16:48 interlinked-0.3/PKG-INFO
--rw-r--r--  2.0 unx      276 b- defN 24-Apr-18 16:47 interlinked-0.3/pyproject.toml
--rw-r--r--  2.0 unx     2551 b- defN 23-Jun-19 17:12 interlinked-0.3/README.md
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-19 17:12 interlinked-0.3/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 16:48 interlinked-0.3/setup.cfg
--rw-r--r--  2.0 unx      129 b- defN 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      433 b- defN 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 16:48 interlinked-0.3/interlinked.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      447 b- defN 24-Apr-18 12:11 interlinked-0.3/tests/test_mutate.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-19 17:12 interlinked-0.3/tests/test_loop.py
--rw-r--r--  2.0 unx     1124 b- defN 24-Apr-18 16:29 interlinked-0.3/tests/test_workflow.py
--rw-r--r--  2.0 unx      981 b- defN 24-Apr-18 12:08 interlinked-0.3/tests/test_route.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 17:12 interlinked-0.3/interlinked/__init__.py
--rw-r--r--  2.0 unx     3854 b- defN 24-Apr-18 16:45 interlinked-0.3/interlinked/cli.py
--rw-r--r--  2.0 unx      213 b- defN 23-Jun-19 17:12 interlinked-0.3/interlinked/exceptions.py
--rw-r--r--  2.0 unx     8050 b- defN 24-Apr-18 16:30 interlinked-0.3/interlinked/workflow.py
--rw-r--r--  2.0 unx     2242 b- defN 24-Apr-18 16:28 interlinked-0.3/interlinked/router.py
--rw-r--r--  2.0 unx       71 b- defN 24-Apr-11 16:44 interlinked-0.3/interlinked/__main__.py
-24 files, 21894 bytes uncompressed, 8155 bytes compressed:  62.8%
+Zip file size: 11789 bytes, number of entries: 24
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:50 interlinked-0.3.1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:50 interlinked-0.3.1/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:50 interlinked-0.3.1/interlinked/
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-18 16:50 interlinked-0.3.1/PKG-INFO
+-rw-r--r--  2.0 unx      278 b- defN 24-Apr-18 16:50 interlinked-0.3.1/pyproject.toml
+-rw-r--r--  2.0 unx     2551 b- defN 23-Jun-19 17:12 interlinked-0.3.1/README.md
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-19 17:12 interlinked-0.3.1/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 16:50 interlinked-0.3.1/setup.cfg
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      433 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      447 b- defN 24-Apr-18 16:50 interlinked-0.3.1/tests/test_mutate.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-19 17:12 interlinked-0.3.1/tests/test_loop.py
+-rw-r--r--  2.0 unx     1124 b- defN 24-Apr-18 16:50 interlinked-0.3.1/tests/test_workflow.py
+-rw-r--r--  2.0 unx      981 b- defN 24-Apr-18 16:50 interlinked-0.3.1/tests/test_route.py
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 17:12 interlinked-0.3.1/interlinked/__init__.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked/cli.py
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-19 17:12 interlinked-0.3.1/interlinked/exceptions.py
+-rw-r--r--  2.0 unx     8050 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked/workflow.py
+-rw-r--r--  2.0 unx     2242 b- defN 24-Apr-18 16:50 interlinked-0.3.1/interlinked/router.py
+-rw-r--r--  2.0 unx       71 b- defN 24-Apr-11 16:44 interlinked-0.3.1/interlinked/__main__.py
+24 files, 21812 bytes uncompressed, 8135 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,73 +1,73 @@
-Filename: interlinked-0.3/
+Filename: interlinked-0.3.1/
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/
+Filename: interlinked-0.3.1/interlinked.egg-info/
 Comment: 
 
-Filename: interlinked-0.3/tests/
+Filename: interlinked-0.3.1/tests/
 Comment: 
 
-Filename: interlinked-0.3/interlinked/
+Filename: interlinked-0.3.1/interlinked/
 Comment: 
 
-Filename: interlinked-0.3/PKG-INFO
+Filename: interlinked-0.3.1/PKG-INFO
 Comment: 
 
-Filename: interlinked-0.3/pyproject.toml
+Filename: interlinked-0.3.1/pyproject.toml
 Comment: 
 
-Filename: interlinked-0.3/README.md
+Filename: interlinked-0.3.1/README.md
 Comment: 
 
-Filename: interlinked-0.3/setup.py
+Filename: interlinked-0.3.1/setup.py
 Comment: 
 
-Filename: interlinked-0.3/setup.cfg
+Filename: interlinked-0.3.1/setup.cfg
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/PKG-INFO
+Filename: interlinked-0.3.1/interlinked.egg-info/PKG-INFO
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/SOURCES.txt
+Filename: interlinked-0.3.1/interlinked.egg-info/SOURCES.txt
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/entry_points.txt
+Filename: interlinked-0.3.1/interlinked.egg-info/entry_points.txt
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/top_level.txt
+Filename: interlinked-0.3.1/interlinked.egg-info/top_level.txt
 Comment: 
 
-Filename: interlinked-0.3/interlinked.egg-info/dependency_links.txt
+Filename: interlinked-0.3.1/interlinked.egg-info/dependency_links.txt
 Comment: 
 
-Filename: interlinked-0.3/tests/test_mutate.py
+Filename: interlinked-0.3.1/tests/test_mutate.py
 Comment: 
 
-Filename: interlinked-0.3/tests/test_loop.py
+Filename: interlinked-0.3.1/tests/test_loop.py
 Comment: 
 
-Filename: interlinked-0.3/tests/test_workflow.py
+Filename: interlinked-0.3.1/tests/test_workflow.py
 Comment: 
 
-Filename: interlinked-0.3/tests/test_route.py
+Filename: interlinked-0.3.1/tests/test_route.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/__init__.py
+Filename: interlinked-0.3.1/interlinked/__init__.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/cli.py
+Filename: interlinked-0.3.1/interlinked/cli.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/exceptions.py
+Filename: interlinked-0.3.1/interlinked/exceptions.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/workflow.py
+Filename: interlinked-0.3.1/interlinked/workflow.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/router.py
+Filename: interlinked-0.3.1/interlinked/router.py
 Comment: 
 
-Filename: interlinked-0.3/interlinked/__main__.py
+Filename: interlinked-0.3.1/interlinked/__main__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `interlinked-0.3/README.md` & `interlinked-0.3.1/README.md`

 * *Files identical despite different names*

## Comparing `interlinked-0.3/tests/test_loop.py` & `interlinked-0.3.1/tests/test_loop.py`

 * *Files identical despite different names*

## Comparing `interlinked-0.3/tests/test_workflow.py` & `interlinked-0.3.1/tests/test_workflow.py`

 * *Files identical despite different names*

## Comparing `interlinked-0.3/tests/test_route.py` & `interlinked-0.3.1/tests/test_route.py`

 * *Files identical despite different names*

## Comparing `interlinked-0.3/interlinked/cli.py` & `interlinked-0.3.1/interlinked/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import logging
-import json
 from importlib.machinery import SourceFileLoader
 
 from .exceptions import InterlinkedException
 from .workflow import Workflow
 
 try:
     import rich
@@ -31,19 +30,16 @@
             print(res)
 
 
 def load_conf(path):
     if path.endswith(".toml"):
         import toml
         return toml.load(path)
-    elif path.endswith(".json"):
-        return json.load(open(path))
     else:
-        raise ValueError("File type not supported (should be json or toml)")
-
+        raise ValueError("File type not supported (only toml for now)")
 
 def find_workflow(args):
     src = args.source
     wkf_variable = None
     if ":" in src:
         src, wkf_variable = src.split(":", 1)
         assert isinstance(wkf_variable, Workflow)
```

## Comparing `interlinked-0.3/interlinked/workflow.py` & `interlinked-0.3.1/interlinked/workflow.py`

 * *Files identical despite different names*

## Comparing `interlinked-0.3/interlinked/router.py` & `interlinked-0.3.1/interlinked/router.py`

 * *Files identical despite different names*

