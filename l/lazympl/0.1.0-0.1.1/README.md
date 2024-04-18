# Comparing `tmp/lazympl-0.1.0.tar.gz` & `tmp/lazympl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazympl-0.1.0.tar", last modified: Thu Apr 18 10:40:17 2024, max compression
+gzip compressed data, was "lazympl-0.1.1.tar", last modified: Thu Apr 18 10:49:12 2024, max compression
```

## Comparing `lazympl-0.1.0.tar` & `lazympl-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.752365 lazympl-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.748365 lazympl-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.748365 lazympl-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 10:40:13.000000 lazympl-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 10:40:13.000000 lazympl-0.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 10:40:13.000000 lazympl-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 10:40:13.000000 lazympl-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:40:17.752365 lazympl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 10:40:13.000000 lazympl-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-18 10:40:13.000000 lazympl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:40:17.752365 lazympl-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.748365 lazympl-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.752365 lazympl-0.1.0/src/lazympl/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 10:40:13.000000 lazympl-0.1.0/src/lazympl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-18 10:40:13.000000 lazympl-0.1.0/src/lazympl/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-18 10:40:13.000000 lazympl-0.1.0/src/lazympl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:13.000000 lazympl-0.1.0/src/lazympl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:40:17.752365 lazympl-0.1.0/src/lazympl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 10:40:17.000000 lazympl-0.1.0/src/lazympl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 10:40:13.000000 lazympl-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 10:49:07.000000 lazympl-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 10:49:07.000000 lazympl-0.1.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 10:49:07.000000 lazympl-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 10:49:07.000000 lazympl-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:49:12.784703 lazympl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 10:49:07.000000 lazympl-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-18 10:49:07.000000 lazympl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:49:12.784703 lazympl-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.780703 lazympl-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/src/lazympl/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:07.000000 lazympl-0.1.1/src/lazympl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:49:12.784703 lazympl-0.1.1/src/lazympl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 10:49:12.000000 lazympl-0.1.1/src/lazympl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 10:49:07.000000 lazympl-0.1.1/tox.ini
```

### Comparing `lazympl-0.1.0/.github/workflows/release.yml` & `lazympl-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.0/.github/workflows/tox.yml` & `lazympl-0.1.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.0/LICENSE` & `lazympl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.0/PKG-INFO` & `lazympl-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazympl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lazy wrappers around matplotlib
 Author: Thomas Guillet
 Author-email: Adrien Morison <adrien.morison@gmail.com>
 Maintainer-email: Adrien Morison <adrien.morison@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Adrien Morison, Thomas Guillet
```

### Comparing `lazympl-0.1.0/pyproject.toml` & `lazympl-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.0/src/lazympl/figure.py` & `lazympl-0.1.1/src/lazympl/figure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
+import matplotlib.figure as mplf
+
 if TYPE_CHECKING:
     from os import PathLike
     from typing import Any, Sequence, Union
 
-    import matplotlib.figure as mplf
-
     from .plot import Plot
 
 
 class Figure(ABC):
     @abstractmethod
     def figure(self) -> mplf.Figure:
         """Build the matplotlib figure"""
```

### Comparing `lazympl-0.1.0/src/lazympl/plot.py` & `lazympl-0.1.1/src/lazympl/plot.py`

 * *Files identical despite different names*

### Comparing `lazympl-0.1.0/src/lazympl.egg-info/PKG-INFO` & `lazympl-0.1.1/src/lazympl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazympl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lazy wrappers around matplotlib
 Author: Thomas Guillet
 Author-email: Adrien Morison <adrien.morison@gmail.com>
 Maintainer-email: Adrien Morison <adrien.morison@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Adrien Morison, Thomas Guillet
```

