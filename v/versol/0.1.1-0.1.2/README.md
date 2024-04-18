# Comparing `tmp/versol-0.1.1.tar.gz` & `tmp/versol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versol-0.1.1.tar", max compression
+gzip compressed data, was "versol-0.1.2.tar", max compression
```

## Comparing `versol-0.1.1.tar` & `versol-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1095 2024-04-16 07:48:57.398658 versol-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      499 2024-04-16 06:43:10.808571 versol-0.1.1/README.md
--rw-r--r--   0        0        0      932 2024-04-16 07:48:48.051960 versol-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 22:49:12.751357 versol-0.1.1/src/versol/__init__.py
--rw-r--r--   0        0        0     9736 2024-04-16 06:39:43.124480 versol-0.1.1/src/versol/_solution.py
--rw-r--r--   0        0        0     2311 2024-04-16 06:04:31.409859 versol-0.1.1/src/versol/incompatibility.py
--rw-r--r--   0        0        0     2687 2024-04-16 06:04:10.419782 versol-0.1.1/src/versol/interfaces.py
--rw-r--r--   0        0        0    13947 2024-04-16 06:04:36.113209 versol-0.1.1/src/versol/iset.py
--rw-r--r--   0        0        0     2353 2024-04-15 03:22:50.516828 versol-0.1.1/src/versol/iset_test.py
--rw-r--r--   0        0        0        0 2024-04-16 07:47:00.044925 versol-0.1.1/src/versol/py.typed
--rw-r--r--   0        0        0     7406 2024-04-16 06:42:29.975089 versol-0.1.1/src/versol/report.py
--rw-r--r--   0        0        0     7741 2024-04-16 06:39:53.834519 versol-0.1.1/src/versol/solve.py
--rw-r--r--   0        0        0     9622 2024-04-16 06:33:19.773070 versol-0.1.1/src/versol/solve_test.py
--rw-r--r--   0        0        0     4349 2024-04-16 05:44:28.191537 versol-0.1.1/src/versol/term.py
--rw-r--r--   0        0        0     2521 2024-04-16 06:23:40.614203 versol-0.1.1/src/versol/util.py
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 versol-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-16 07:48:57.398658 versol-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      499 2024-04-16 06:43:10.808571 versol-0.1.2/README.md
+-rw-r--r--   0        0        0      932 2024-04-18 01:24:11.435590 versol-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 22:49:12.751357 versol-0.1.2/src/versol/__init__.py
+-rw-r--r--   0        0        0     9736 2024-04-16 06:39:43.124480 versol-0.1.2/src/versol/_solution.py
+-rw-r--r--   0        0        0     2311 2024-04-16 06:04:31.409859 versol-0.1.2/src/versol/incompatibility.py
+-rw-r--r--   0        0        0     2687 2024-04-16 06:04:10.419782 versol-0.1.2/src/versol/interfaces.py
+-rw-r--r--   0        0        0    14180 2024-04-18 01:22:43.278510 versol-0.1.2/src/versol/iset.py
+-rw-r--r--   0        0        0     2968 2024-04-18 01:19:09.424172 versol-0.1.2/src/versol/iset_test.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:47:00.044925 versol-0.1.2/src/versol/py.typed
+-rw-r--r--   0        0        0     7406 2024-04-16 06:42:29.975089 versol-0.1.2/src/versol/report.py
+-rw-r--r--   0        0        0     7741 2024-04-16 06:39:53.834519 versol-0.1.2/src/versol/solve.py
+-rw-r--r--   0        0        0     9622 2024-04-16 06:33:19.773070 versol-0.1.2/src/versol/solve_test.py
+-rw-r--r--   0        0        0     4349 2024-04-16 05:44:28.191537 versol-0.1.2/src/versol/term.py
+-rw-r--r--   0        0        0     2521 2024-04-16 06:23:40.614203 versol-0.1.2/src/versol/util.py
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 versol-0.1.2/PKG-INFO
```

### Comparing `versol-0.1.1/LICENSE.txt` & `versol-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/pyproject.toml` & `versol-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "versol"
-version = "0.1.1"
+version = "0.1.2"
 description = "A generic library for dependency solving, based on the pubgrub algorithm"
 authors = ["vector-of-bool <vectorofbool@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "versol", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `versol-0.1.1/src/versol/_solution.py` & `versol-0.1.2/src/versol/_solution.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/incompatibility.py` & `versol-0.1.2/src/versol/incompatibility.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/interfaces.py` & `versol-0.1.2/src/versol/interfaces.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/iset.py` & `versol-0.1.2/src/versol/iset.py`

 * *Files 7% similar despite different names*

```diff
@@ -212,30 +212,37 @@
 
     def __remove(self, iv: _Interval[PointT]) -> None:
         """
         Remove all points within ``iv`` from the set. This function is only used
         for calculating `.difference()`.
         """
         low, high = iv
-        left = self.__n_points_before_or_at(low)
-        right = self.__n_points_before(high)
+        left = self.__n_points_before(low)
+        right = self.__n_points_before_or_at(high)
         if left % 2:  # Starts within the set?
             if right % 2:  # Ends within the set?
                 self.__points[left:right] = (low, high)
             else:
                 self.__points[left:right] = (low,)
         elif right % 2:  # Ends within the set?
             self.__points[left:right] = (high,)
         else:
             self.__points[left:right] = ()
 
     def __repr__(self) -> str:
         pairs = (f"[{lo!r}, {hi!r})" for lo, hi in self.intervals)
         return f'<HalfOpenIntervalSet ⟨{", ".join(pairs)}⟩>'
 
+    def __str__(self) -> str:
+        if self.empty:
+            return "HalfOpenIntervalSet()"
+        else:
+            ivs = " ∪ ".join(f"⟨≥{low},<{high}⟩" for low, high in self.intervals)
+            return f"{{{ivs}}}"
+
     def __eq__(self, other: object) -> bool:
         """
         Compare two sets for equality. The two sets are equivalent if it is
         defined by the same boundary points and the sets use the same key
         function.
 
         This will compare the point objects using the default ``==`` operator.
```

### Comparing `versol-0.1.1/src/versol/iset_test.py` & `versol-0.1.2/src/versol/iset_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,30 @@
     assert iv.contains(2)
     assert not iv.contains(7)
     assert iv.contains(1)
     assert iv.contains(3)
     assert iv.contains(4)
     assert iv == mod.HalfOpenIntervalSet[int]([(1, 7)])
 
+    iv = mod.HalfOpenIntervalSet[int]([(1, 10), (1, 15)])
+    assert list(iv.intervals) == [(1, 15)]
+
+    iv = mod.HalfOpenIntervalSet[int]([(1, 10), (5, 10)])
+    assert list(iv.intervals) == [(1, 10)]
+
+    iv = mod.HalfOpenIntervalSet[int]([(5, 10), (1, 10)])
+    assert list(iv.intervals) == [(1, 10)]
+
+
+def test_self_union():
+    iv = mod.HalfOpenIntervalSet[int]([(1, 10)])
+    un = iv | iv
+    assert un == iv
+    assert list(un.intervals) == [(1, 10)]
+
 
 def test_disjoint_union():
     iv = mod.HalfOpenIntervalSet[int]([(1, 4), (6, 9)])
     assert iv.contains(1)
     assert not iv.contains(4)
     assert iv.contains(6)
     assert not iv.contains(9)
@@ -67,14 +83,21 @@
     iv2 = mod.HalfOpenIntervalSet[int]([(5, 15)])
     diff = iv.difference(iv2)
     assert diff == mod.HalfOpenIntervalSet[int]([(1, 5)])
     diff2 = iv2 - iv
     assert diff != diff2
 
 
+def test_difference_same():
+    iv = mod.HalfOpenIntervalSet[int]([(1, 10)])
+    nil = iv - iv
+    assert nil.empty
+    assert list(nil.intervals) == []
+
+
 def _many_pairs(base: int, n: int, width: int, stride: int) -> Iterator[tuple[int, int]]:
     for x in range(n):
         x = base + x * stride
         yield (x, x + width)
 
 
 def test_huge():
```

### Comparing `versol-0.1.1/src/versol/report.py` & `versol-0.1.2/src/versol/report.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/solve.py` & `versol-0.1.2/src/versol/solve.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/solve_test.py` & `versol-0.1.2/src/versol/solve_test.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/term.py` & `versol-0.1.2/src/versol/term.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/src/versol/util.py` & `versol-0.1.2/src/versol/util.py`

 * *Files identical despite different names*

### Comparing `versol-0.1.1/PKG-INFO` & `versol-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versol
-Version: 0.1.1
+Version: 0.1.2
 Summary: A generic library for dependency solving, based on the pubgrub algorithm
 Home-page: https://github.com/vector-of-bool/versol
 License: MIT
 Author: vector-of-bool
 Author-email: vectorofbool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

