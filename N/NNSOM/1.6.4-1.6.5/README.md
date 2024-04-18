# Comparing `tmp/nnsom-1.6.4.tar.gz` & `tmp/nnsom-1.6.5.tar.gz`

## Comparing `nnsom-1.6.4.tar` & `nnsom-1.6.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/som.py
--rw-r--r--   0        0        0    23705 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.6.4/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.4/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.4/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.4/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nnsom-1.6.5/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.5/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.5/src/NNSOM/som.py
+-rw-r--r--   0        0        0    23705 2020-02-02 00:00:00.000000 nnsom-1.6.5/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.6.5/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.5/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.5/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.5/PKG-INFO
```

### Comparing `nnsom-1.6.4/src/NNSOM/plots.py` & `nnsom-1.6.5/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.4/src/NNSOM/som.py` & `nnsom-1.6.5/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.4/src/NNSOM/som_gpu.py` & `nnsom-1.6.5/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.4/src/NNSOM/utils.py` & `nnsom-1.6.5/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.4/.gitignore` & `nnsom-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.4/pyproject.toml` & `nnsom-1.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.6.4"
+version = "1.6.5"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.6.4/PKG-INFO` & `nnsom-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.6.4
+Version: 1.6.5
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

