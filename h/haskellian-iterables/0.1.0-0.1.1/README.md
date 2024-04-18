# Comparing `tmp/haskellian-iterables-0.1.0.tar.gz` & `tmp/haskellian_iterables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-iterables-0.1.0.tar", last modified: Tue Apr  2 05:25:11 2024, max compression
+gzip compressed data, was "haskellian_iterables-0.1.1.tar", last modified: Thu Apr 18 12:59:14 2024, max compression
```

## Comparing `haskellian-iterables-0.1.0.tar` & `haskellian_iterables-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:25:11.571954 haskellian-iterables-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      285 2024-04-02 05:25:11.571954 haskellian-iterables-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-02 05:05:53.000000 haskellian-iterables-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-02 05:05:53.000000 haskellian-iterables-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-02 05:25:11.571954 haskellian-iterables-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:25:11.561954 haskellian-iterables-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:25:11.561954 haskellian-iterables-0.1.0/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:25:11.561954 haskellian-iterables-0.1.0/src/haskellian/iterables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-04-02 05:24:46.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-04-02 05:22:28.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/basics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      611 2024-04-02 05:23:22.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/batching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1449 2024-04-02 05:22:17.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/curried.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      657 2024-04-02 05:20:03.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/generators.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      303 2024-04-02 05:23:54.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/misc.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3523 2024-04-02 05:23:01.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/nested.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      884 2024-04-02 05:21:22.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/slicing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      842 2024-04-02 05:20:37.000000 haskellian-iterables-0.1.0/src/haskellian/iterables/zipping.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:25:11.571954 haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      285 2024-04-02 05:25:11.000000 haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-04-02 05:25:11.000000 haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-02 05:25:11.000000 haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-02 05:25:11.000000 haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      306 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-02 05:05:53.000000 haskellian_iterables-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-04-18 12:59:12.000000 haskellian_iterables-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/src/haskellian/iterables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-16 09:07:04.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-04-02 05:22:28.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/basics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      611 2024-04-02 05:23:22.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/batching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1772 2024-04-16 07:36:12.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/curried.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      657 2024-04-02 05:20:03.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/generators.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      303 2024-04-02 05:23:54.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/misc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4178 2024-04-16 09:06:56.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/nested.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      884 2024-04-02 05:21:22.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/slicing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      872 2024-04-10 07:17:07.000000 haskellian_iterables-0.1.1/src/haskellian/iterables/zipping.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 12:59:14.618395 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      306 2024-04-18 12:59:14.000000 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      587 2024-04-18 12:59:14.000000 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 12:59:14.000000 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-18 12:59:14.000000 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-18 12:59:14.000000 haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/top_level.txt
```

### Comparing `haskellian-iterables-0.1.0/pyproject.toml` & `haskellian_iterables-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-iterables"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "FP-style functions for generators"
 dependencies = [
-  
+  "ramda"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 # [project.urls]
 # repo = "<GIT_REPO_URL>"
```

### Comparing `haskellian-iterables-0.1.0/src/haskellian/iterables/basics.py` & `haskellian_iterables-0.1.1/src/haskellian/iterables/basics.py`

 * *Files identical despite different names*

### Comparing `haskellian-iterables-0.1.0/src/haskellian/iterables/batching.py` & `haskellian_iterables-0.1.1/src/haskellian/iterables/batching.py`

 * *Files identical despite different names*

### Comparing `haskellian-iterables-0.1.0/src/haskellian/iterables/generators.py` & `haskellian_iterables-0.1.1/src/haskellian/iterables/generators.py`

 * *Files identical despite different names*

### Comparing `haskellian-iterables-0.1.0/src/haskellian/iterables/nested.py` & `haskellian_iterables-0.1.1/src/haskellian/iterables/nested.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Iterable, TypeVar, Callable
+from itertools import zip_longest
 import ramda as R
 from .basics import isiterable
 
 A = TypeVar('A')
 B = TypeVar('B')
 
 @R.curry
@@ -100,10 +101,45 @@
             yield from _auto_ndflat(xs)
             
 @R.curry
 def ndflat(xxs: Iterable[Iterable[A]], depth: int | None = None) -> Iterable[Iterable[A]]:
     """`ndflat([[x1, x2], [x3, [x4]]]) = [x1, x2, x3, x4]`"""
     return _auto_ndflat(xxs) if depth is None else _fixed_ndflat(xxs, depth)
 
-def transpose(xs: Iterable[Iterable[A]]) -> Iterable[Iterable[A]]:
-    """`transpose([[1, 2], [3, 4], [5, 6]]) = [[1, 2, 3], [4, 5, 6]]`"""
-    return zip(*xs)
+def transpose(xs: Iterable[Iterable[A]]) -> list[list[A]]:
+    """Transpose a 2d list, cropping to the shortest row. E.g:
+    ```
+    transpose([
+        [1, 2],
+        [3, 4],
+        [5, 6]
+    ]) == [
+        [1, 3, 5],
+        [2, 4, 6]
+    ]
+    ```
+    but
+    ```
+    transpose([
+        [1, 2],
+        [3, 4],
+        [5]
+    ]) == [
+        [1, 2, 3],
+    ]
+    ```
+    """
+    return list(zip(*xs))
+
+def transpose_ragged(xs: Iterable[Iterable[A]]) -> list[list[A]]:
+    """Like `transpose`, but resulting rows can be ragged (i.e. have different lengths). E.g:
+    ```
+    transpose([
+        [1, 2],
+        [3, 4],
+        [5]
+    ]) == [
+        [1, 3, 5],
+        [2, 4]
+    ]
+    ```"""
+    return [[x for x in cols if x is not None] for cols in zip_longest(*xs)]
```

### Comparing `haskellian-iterables-0.1.0/src/haskellian/iterables/slicing.py` & `haskellian_iterables-0.1.1/src/haskellian/iterables/slicing.py`

 * *Files identical despite different names*

### Comparing `haskellian-iterables-0.1.0/src/haskellian_iterables.egg-info/SOURCES.txt` & `haskellian_iterables-0.1.1/src/haskellian_iterables.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/haskellian/iterables/misc.py
 src/haskellian/iterables/nested.py
 src/haskellian/iterables/slicing.py
 src/haskellian/iterables/zipping.py
 src/haskellian_iterables.egg-info/PKG-INFO
 src/haskellian_iterables.egg-info/SOURCES.txt
 src/haskellian_iterables.egg-info/dependency_links.txt
+src/haskellian_iterables.egg-info/requires.txt
 src/haskellian_iterables.egg-info/top_level.txt
```

