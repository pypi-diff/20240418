# Comparing `tmp/augmented_matrix-0.5.tar.gz` & `tmp/augmented_matrix-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix-0.5.tar", last modified: Tue Apr 16 20:14:26 2024, max compression
+gzip compressed data, was "augmented_matrix-0.6.tar", last modified: Thu Apr 18 17:24:57 2024, max compression
```

## Comparing `augmented_matrix-0.5.tar` & `augmented_matrix-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848850 augmented_matrix-0.5/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.5/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 20:14:26.848667 augmented_matrix-0.5/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.5/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.846768 augmented_matrix-0.5/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.5/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     4742 2024-04-16 20:10:39.000000 augmented_matrix-0.5/augmented_matrix/augmented_matrix.py
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848462 augmented_matrix-0.5/augmented_matrix.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-16 19:08:09.000000 augmented_matrix-0.5/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-16 20:14:26.849003 augmented_matrix-0.5/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848064 augmented_matrix-0.5/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.5/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-18 17:24:57.420142 augmented_matrix-0.6/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.6/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-18 17:24:57.419937 augmented_matrix-0.6/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.6/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-18 17:24:57.418242 augmented_matrix-0.6/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.6/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     5050 2024-04-18 17:22:43.000000 augmented_matrix-0.6/augmented_matrix/augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-18 17:24:57.419712 augmented_matrix-0.6/augmented_matrix.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-18 17:24:57.000000 augmented_matrix-0.6/augmented_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-18 17:24:57.000000 augmented_matrix-0.6/augmented_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-18 17:24:57.000000 augmented_matrix-0.6/augmented_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-18 17:24:57.000000 augmented_matrix-0.6/augmented_matrix.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-18 17:24:57.000000 augmented_matrix-0.6/augmented_matrix.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-18 17:24:55.000000 augmented_matrix-0.6/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-18 17:24:57.420179 augmented_matrix-0.6/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-18 17:24:57.419328 augmented_matrix-0.6/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.6/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix-0.5/LICENSE` & `augmented_matrix-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix-0.5/PKG-INFO` & `augmented_matrix-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.5
+Version: 0.6
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.5/augmented_matrix/augmented_matrix.py` & `augmented_matrix-0.6/augmented_matrix/augmented_matrix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import numpy as np
+from fractions import Fraction
 
 
 class NoSolutionError(Exception):
     pass
 
 
 class AugmentedMatrix:
+    """
+    A class that represents an augmented matrix
+    """
     def __init__(self, matrix, constraint=None, /, **kwargs):
-        if constraint is not None:
-            constraint = np.asarray(constraint, **kwargs)
-            matrix = np.append(matrix, [[i] for i in constraint], axis=1)
+        def _to_fraction(original):
+            return [[Fraction(j).limit_denominator() for j in i] for i in original]
+
+        self._matrix = np.asarray(_to_fraction(matrix), **kwargs)
 
-        self._matrix = np.asarray(matrix, **kwargs)
+        if constraint is not None:
+            constraint = np.asarray(_to_fraction(constraint), **kwargs)
+            self._matrix = np.append(self._matrix, [[i] for i in constraint], axis=1)
 
     @property
     def matrix(self) -> np.ndarray:
         """
         :return: the augmented matrix
         """
         return self._matrix
@@ -75,14 +82,15 @@
                     if leading_value == 0:
                         continue
                     factor = -1 * pivot / leading_value
                     matrix[i] = factor * matrix[i] + matrix[row]
 
             column += 1
             row = column
+            print(matrix)
 
         self._matrix = matrix
         return matrix
 
     def simplify_echelon(self) -> np.ndarray:
         """
         Simplifies the upper triangular form so that the pivots are 1
@@ -126,14 +134,15 @@
                     leading = matrix[i][pivot_coord[1]]
                     if leading == 0:
                         continue
 
                     pivot = matrix[pivot_coord[0]][pivot_coord[1]]
                     factor = -1 * leading / pivot
                     matrix[i] = factor * matrix[pivot_coord[0]] + matrix[i]
+            print(matrix)
 
         self._matrix = matrix
         return matrix
 
     def solve(self) -> np.ndarray:
         """
         Solves the augmented matrix
```

### Comparing `augmented_matrix-0.5/augmented_matrix.egg-info/PKG-INFO` & `augmented_matrix-0.6/augmented_matrix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.5
+Version: 0.6
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.5/pyproject.toml` & `augmented_matrix-0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "augmented-matrix"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies= ['numpy']
```

### Comparing `augmented_matrix-0.5/test/test_augmented_matrix.py` & `augmented_matrix-0.6/test/test_augmented_matrix.py`

 * *Files identical despite different names*

