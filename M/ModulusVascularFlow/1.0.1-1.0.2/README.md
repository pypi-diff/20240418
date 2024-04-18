# Comparing `tmp/modulusvascularflow-1.0.1.tar.gz` & `tmp/modulusvascularflow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modulusvascularflow-1.0.1.tar", last modified: Thu Apr 18 15:05:11 2024, max compression
+gzip compressed data, was "modulusvascularflow-1.0.2.tar", last modified: Thu Apr 18 15:09:05 2024, max compression
```

## Comparing `modulusvascularflow-1.0.1.tar` & `modulusvascularflow-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.673510 modulusvascularflow-1.0.1/
--rw-rw-rw-   0        0        0     1067 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.673510 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/
--rw-rw-rw-   0        0        0     3664 2024-04-18 15:05:11.000000 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2024-04-18 15:05:11.000000 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 15:05:11.000000 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-18 15:05:11.000000 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 15:05:11.000000 modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3664 2024-04-18 15:05:11.673510 modulusvascularflow-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.610964 modulusvascularflow-1.0.1/modulusDL/
--rw-rw-rw-   0        0        0      108 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.1/modulusDL/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.610964 modulusvascularflow-1.0.1/modulusDL/eq/
--rw-rw-rw-   0        0        0       17 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.1/modulusDL/eq/__init__.py
--rw-rw-rw-   0        0        0    11264 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/eq/coordinate_transformed_pde.py
--rw-rw-rw-   0        0        0    35946 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/eq/pde.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.626608 modulusvascularflow-1.0.1/modulusDL/geometry/
--rw-rw-rw-   0        0        0       51 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/geometry/__init__.py
--rw-rw-rw-   0        0        0    50663 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/geometry/geometry.py
--rw-rw-rw-   0        0        0     3766 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/geometry/ideal_encoding.py
--rw-rw-rw-   0        0        0     8213 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/geometry/ideal_warping.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.642234 modulusvascularflow-1.0.1/modulusDL/loss/
--rw-rw-rw-   0        0        0       18 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/loss/__init__.py
--rw-rw-rw-   0        0        0     2584 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/loss/loss.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.657859 modulusvascularflow-1.0.1/modulusDL/models/
--rw-rw-rw-   0        0        0       65 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/models/__init__.py
--rw-rw-rw-   0        0        0   158960 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/models/arch.py
--rw-rw-rw-   0        0        0    11477 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/models/archCombi.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.657859 modulusvascularflow-1.0.1/modulusDL/models/layers/
--rw-rw-rw-   0        0        0      145 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/models/layers/__init__.py
--rw-rw-rw-   0        0        0    11737 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/models/layers/inherited.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:05:11.673510 modulusvascularflow-1.0.1/modulusDL/solver/
--rw-rw-rw-   0        0        0       20 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/solver/__init__.py
--rw-rw-rw-   0        0        0    20695 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.1/modulusDL/solver/solver.py
--rw-rw-rw-   0        0        0     1075 2024-04-18 15:03:17.000000 modulusvascularflow-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 15:05:11.673510 modulusvascularflow-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.950310 modulusvascularflow-1.0.2/
+-rw-rw-rw-   0        0        0     1067 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.928574 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/
+-rw-rw-rw-   0        0        0     3664 2024-04-18 15:09:05.000000 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2024-04-18 15:09:05.000000 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:09:05.000000 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-18 15:09:05.000000 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 15:09:05.000000 modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3664 2024-04-18 15:09:05.948694 modulusvascularflow-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.860508 modulusvascularflow-1.0.2/modulusDL/
+-rw-rw-rw-   0        0        0       84 2024-04-18 15:08:21.000000 modulusvascularflow-1.0.2/modulusDL/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.876169 modulusvascularflow-1.0.2/modulusDL/eq/
+-rw-rw-rw-   0        0        0       17 2024-04-18 13:00:42.000000 modulusvascularflow-1.0.2/modulusDL/eq/__init__.py
+-rw-rw-rw-   0        0        0    11264 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/eq/coordinate_transformed_pde.py
+-rw-rw-rw-   0        0        0    35946 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/eq/pde.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.881685 modulusvascularflow-1.0.2/modulusDL/geometry/
+-rw-rw-rw-   0        0        0       51 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/geometry/__init__.py
+-rw-rw-rw-   0        0        0    50663 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/geometry/geometry.py
+-rw-rw-rw-   0        0        0     3766 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/geometry/ideal_encoding.py
+-rw-rw-rw-   0        0        0     8213 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/geometry/ideal_warping.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.897323 modulusvascularflow-1.0.2/modulusDL/loss/
+-rw-rw-rw-   0        0        0       18 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/loss/__init__.py
+-rw-rw-rw-   0        0        0     2584 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/loss/loss.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.912948 modulusvascularflow-1.0.2/modulusDL/models/
+-rw-rw-rw-   0        0        0       65 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/models/__init__.py
+-rw-rw-rw-   0        0        0   158960 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/models/arch.py
+-rw-rw-rw-   0        0        0    11477 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/models/archCombi.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.912948 modulusvascularflow-1.0.2/modulusDL/models/layers/
+-rw-rw-rw-   0        0        0      145 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/models/layers/__init__.py
+-rw-rw-rw-   0        0        0    11737 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/models/layers/inherited.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:09:05.928574 modulusvascularflow-1.0.2/modulusDL/solver/
+-rw-rw-rw-   0        0        0       20 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/solver/__init__.py
+-rw-rw-rw-   0        0        0    20695 2024-04-18 13:00:43.000000 modulusvascularflow-1.0.2/modulusDL/solver/solver.py
+-rw-rw-rw-   0        0        0     1075 2024-04-18 15:08:54.000000 modulusvascularflow-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:09:05.950885 modulusvascularflow-1.0.2/setup.cfg
```

### Comparing `modulusvascularflow-1.0.1/LICENSE` & `modulusvascularflow-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/PKG-INFO` & `modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModulusVascularFlow
-Version: 1.0.1
+Version: 1.0.2
 Summary: Codes extention from NVIDIA Modulus.
 Author-email: Wei Xuan Chan <w.x.chan1986@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 W. X. Chan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `modulusvascularflow-1.0.1/ModulusVascularFlow.egg-info/SOURCES.txt` & `modulusvascularflow-1.0.2/ModulusVascularFlow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/PKG-INFO` & `modulusvascularflow-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModulusVascularFlow
-Version: 1.0.1
+Version: 1.0.2
 Summary: Codes extention from NVIDIA Modulus.
 Author-email: Wei Xuan Chan <w.x.chan1986@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 W. X. Chan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `modulusvascularflow-1.0.1/README.md` & `modulusvascularflow-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/eq/coordinate_transformed_pde.py` & `modulusvascularflow-1.0.2/modulusDL/eq/coordinate_transformed_pde.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/eq/pde.py` & `modulusvascularflow-1.0.2/modulusDL/eq/pde.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/geometry/geometry.py` & `modulusvascularflow-1.0.2/modulusDL/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/geometry/ideal_encoding.py` & `modulusvascularflow-1.0.2/modulusDL/geometry/ideal_encoding.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/geometry/ideal_warping.py` & `modulusvascularflow-1.0.2/modulusDL/geometry/ideal_warping.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/loss/loss.py` & `modulusvascularflow-1.0.2/modulusDL/loss/loss.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/models/arch.py` & `modulusvascularflow-1.0.2/modulusDL/models/arch.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/models/archCombi.py` & `modulusvascularflow-1.0.2/modulusDL/models/archCombi.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/models/layers/inherited.py` & `modulusvascularflow-1.0.2/modulusDL/models/layers/inherited.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/modulusDL/solver/solver.py` & `modulusvascularflow-1.0.2/modulusDL/solver/solver.py`

 * *Files identical despite different names*

### Comparing `modulusvascularflow-1.0.1/pyproject.toml` & `modulusvascularflow-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ModulusVascularFlow"
-version = "1.0.1"
+version = "1.0.2"
 description = "Codes extention from NVIDIA Modulus."
 readme = "README.md"
 authors = [{ name = "Wei Xuan Chan", email = "w.x.chan1986@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

