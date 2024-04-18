# Comparing `tmp/antelope_background-0.2.3.tar.gz` & `tmp/antelope_background-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_background-0.2.3.tar", last modified: Thu Mar 21 22:47:52 2024, max compression
+gzip compressed data, was "antelope_background-0.2.4.tar", last modified: Thu Apr 18 21:41:33 2024, max compression
```

## Comparing `antelope_background-0.2.3.tar` & `antelope_background-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.3/LICENSE
--rw-r--r--   0 b          (500) b          (506)     3732 2024-03-21 22:47:52.321039 antelope_background-0.2.3/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.3/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background/
--rw-r--r--   0 b          (500) b          (506)     2127 2024-03-13 21:49:28.000000 antelope_background-0.2.3/antelope_background/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background/background/
--rw-r--r--   0 b          (500) b          (506)      112 2024-03-13 21:49:28.000000 antelope_background-0.2.3/antelope_background/background/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24828 2023-12-16 05:38:33.000000 antelope_background-0.2.3/antelope_background/background/flat_background.py
--rw-r--r--   0 b          (500) b          (506)    10748 2023-12-16 06:13:57.000000 antelope_background-0.2.3/antelope_background/background/implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background/background/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.3/antelope_background/background/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.3/antelope_background/background/tests/test_flat_background.py
--rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.3/antelope_background/background/tests/test_implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background/engine/
--rw-r--r--   0 b          (500) b          (506)      346 2024-03-13 21:47:33.000000 antelope_background-0.2.3/antelope_background/engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)    29785 2024-03-15 22:38:06.000000 antelope_background-0.2.3/antelope_background/engine/background_engine.py
--rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.3/antelope_background/engine/emission.py
--rw-r--r--   0 b          (500) b          (506)     4612 2024-03-13 00:24:04.000000 antelope_background-0.2.3/antelope_background/engine/product_flow.py
--rw-r--r--   0 b          (500) b          (506)    10150 2018-07-20 18:48:36.000000 antelope_background-0.2.3/antelope_background/engine/tarjan_stack.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background/providers/
--rw-r--r--   0 b          (500) b          (506)      178 2024-03-13 21:49:57.000000 antelope_background-0.2.3/antelope_background/providers/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3075 2024-03-13 22:07:13.000000 antelope_background-0.2.3/antelope_background/providers/bm_static.py
--rw-r--r--   0 b          (500) b          (506)     1102 2024-03-14 00:30:16.000000 antelope_background-0.2.3/antelope_background/providers/check_terms.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:47:52.321039 antelope_background-0.2.3/antelope_background.egg-info/
--rw-r--r--   0 b          (500) b          (506)     3732 2024-03-21 22:47:52.000000 antelope_background-0.2.3/antelope_background.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      926 2024-03-21 22:47:52.000000 antelope_background-0.2.3/antelope_background.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-03-21 22:47:52.000000 antelope_background-0.2.3/antelope_background.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       44 2024-03-21 22:47:52.000000 antelope_background-0.2.3/antelope_background.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       20 2024-03-21 22:47:52.000000 antelope_background-0.2.3/antelope_background.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2024-03-21 22:47:52.321039 antelope_background-0.2.3/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     1598 2024-03-21 22:47:27.000000 antelope_background-0.2.3/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.4/LICENSE
+-rw-r--r--   0 b          (500) b          (506)     3821 2024-04-18 21:41:33.234599 antelope_background-0.2.4/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.4/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/
+-rw-r--r--   0 b          (500) b          (506)     2127 2024-03-13 21:49:28.000000 antelope_background-0.2.4/antelope_background/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/background/
+-rw-r--r--   0 b          (500) b          (506)      112 2024-03-13 21:49:28.000000 antelope_background-0.2.4/antelope_background/background/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24828 2023-12-16 05:38:33.000000 antelope_background-0.2.4/antelope_background/background/flat_background.py
+-rw-r--r--   0 b          (500) b          (506)    10778 2024-04-17 22:48:03.000000 antelope_background-0.2.4/antelope_background/background/implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/background/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.4/antelope_background/background/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.4/antelope_background/background/tests/test_flat_background.py
+-rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.4/antelope_background/background/tests/test_implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background/engine/
+-rw-r--r--   0 b          (500) b          (506)      346 2024-03-13 21:47:33.000000 antelope_background-0.2.4/antelope_background/engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    29785 2024-03-15 22:38:06.000000 antelope_background-0.2.4/antelope_background/engine/background_engine.py
+-rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.4/antelope_background/engine/emission.py
+-rw-r--r--   0 b          (500) b          (506)     4612 2024-03-13 00:24:04.000000 antelope_background-0.2.4/antelope_background/engine/product_flow.py
+-rw-r--r--   0 b          (500) b          (506)    10150 2018-07-20 18:48:36.000000 antelope_background-0.2.4/antelope_background/engine/tarjan_stack.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background/providers/
+-rw-r--r--   0 b          (500) b          (506)      178 2024-03-13 21:49:57.000000 antelope_background-0.2.4/antelope_background/providers/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     3075 2024-03-13 22:07:13.000000 antelope_background-0.2.4/antelope_background/providers/bm_static.py
+-rw-r--r--   0 b          (500) b          (506)     1102 2024-03-14 00:30:16.000000 antelope_background-0.2.4/antelope_background/providers/check_terms.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     3821 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)      926 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       44 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       20 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 21:41:33.234599 antelope_background-0.2.4/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     1690 2024-04-17 22:51:41.000000 antelope_background-0.2.4/setup.py
```

### Comparing `antelope_background-0.2.3/LICENSE` & `antelope_background-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/PKG-INFO` & `antelope_background-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: antelope_background
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: antelope_core>=0.2.4
+Requires-Dist: scipy>=1.5
+Requires-Dist: numpy>=1.19
 
 # background
 Background LCI implementation including Tarjan Ordering.
 
 This is kept as a separate repo because it is the only place `numpy/scipy` is required.  The 
 idea is to enable people to run LCI/A computations without having the background data on their 
 machine or having to perform matrix construction and inversion (i.e. only using foreground
```

### Comparing `antelope_background-0.2.3/README.md` & `antelope_background-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/__init__.py` & `antelope_background-0.2.4/antelope_background/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/background/flat_background.py` & `antelope_background-0.2.4/antelope_background/background/flat_background.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/background/implementation.py` & `antelope_background-0.2.4/antelope_background/background/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from antelope_core.implementations import BackgroundImplementation, CoreConfigureImplementation
-from antelope import ExteriorFlow, check_direction, comp_dir
+from antelope import check_direction, comp_dir
+from antelope.models import ExteriorFlow
 from antelope_core.exchanges import ExchangeValue  # these should be ExchangeRefs?
 from antelope_core.contexts import Context
 
 from .flat_background import FlatBackground
 
 
 class InvalidRefFlow(Exception):
@@ -139,15 +140,15 @@
             yield self._exchange_from_term_ref(bg)
 
     def exterior_flows(self, search=None, **kwargs):
         self.check_bg()
         for ex in self._flat.ex:
             c = ex.term_ref
             f = self[ex.flow_ref]
-            yield ExteriorFlow(self.origin, f, comp_dir(ex.direction), c)  # serialization is opposite sense from API spec
+            yield ExteriorFlow.from_background(f, comp_dir(ex.direction), c)  # serialization is opposite sense from API spec
 
     def is_in_scc(self, process, ref_flow=None, **kwargs):
         process, ref_flow = self._check_ref(process, ref_flow)
         return self._flat.is_in_scc(process, ref_flow)
 
     def is_in_background(self, process, ref_flow=None, **kwargs):
         process, ref_flow = self._check_ref(process, ref_flow)
```

### Comparing `antelope_background-0.2.3/antelope_background/background/tests/test_flat_background.py` & `antelope_background-0.2.4/antelope_background/background/tests/test_flat_background.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/engine/background_engine.py` & `antelope_background-0.2.4/antelope_background/engine/background_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/engine/emission.py` & `antelope_background-0.2.4/antelope_background/engine/emission.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/engine/product_flow.py` & `antelope_background-0.2.4/antelope_background/engine/product_flow.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/engine/tarjan_stack.py` & `antelope_background-0.2.4/antelope_background/engine/tarjan_stack.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/providers/bm_static.py` & `antelope_background-0.2.4/antelope_background/providers/bm_static.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background/providers/check_terms.py` & `antelope_background-0.2.4/antelope_background/providers/check_terms.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/antelope_background.egg-info/PKG-INFO` & `antelope_background-0.2.4/antelope_background.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
-Name: antelope-background
-Version: 0.2.3
+Name: antelope_background
+Version: 0.2.4
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: antelope_core>=0.2.4
+Requires-Dist: scipy>=1.5
+Requires-Dist: numpy>=1.19
 
 # background
 Background LCI implementation including Tarjan Ordering.
 
 This is kept as a separate repo because it is the only place `numpy/scipy` is required.  The 
 idea is to enable people to run LCI/A computations without having the background data on their 
 machine or having to perform matrix construction and inversion (i.e. only using foreground
```

### Comparing `antelope_background-0.2.3/antelope_background.egg-info/SOURCES.txt` & `antelope_background-0.2.4/antelope_background.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.3/setup.py` & `antelope_background-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 requires = [
-    "antelope_core>=0.2.3",
+    "antelope_core>=0.2.4",
     "scipy>=1.5",
     "numpy>=1.19"
 ]
 
 """
 Change Log
+0.2.4 - 2024-04-17 - Remove antelope.ExteriorFlow in favor of antelope.models.ExteriorFlow
+
 0.2.3 - 2024-03-21 - Correct dependencies
 
 0.2.2 - 2024-03-12 - termination test; changed some exceptions
 
 0.2.1 - 2023-04-10 - xdb passes benchmarks.
                      sys_lci running both locally and remotely.
 
@@ -28,15 +30,15 @@
 0.1.5 - 2021-02-05 - bump version to keep pace with antelope_core 
 0.1.4 - 2021-01-29 - bugfixes to get CI passing.  match consistent versions with other packages.
 
 0.1.0 - 2021-01-06 - first published release
 """
 
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 
 setup(
     name="antelope_background",
     version=VERSION,
     author="Brandon Kuczenski",
     author_email="bkuczenski@ucsb.edu",
     license="BSD 3-clause",
```

