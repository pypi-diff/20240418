# Comparing `tmp/pldag-0.6.4.tar.gz` & `tmp/pldag-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.6.4.tar", max compression
+gzip compressed data, was "pldag-0.6.5.tar", max compression
```

## Comparing `pldag-0.6.4.tar` & `pldag-0.6.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.4/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.6.4/README.md
--rw-r--r--   0        0        0    23735 2024-04-15 13:28:56.625033 pldag-0.6.4/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.4/pldag/solver/__init__.py
--rw-r--r--   0        0        0      837 2024-04-15 12:41:50.577849 pldag-0.6.4/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-15 13:46:35.024484 pldag-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 pldag-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.6.5/README.md
+-rw-r--r--   0        0        0    26911 2024-04-18 13:22:37.287060 pldag-0.6.5/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.5/pldag/solver/__init__.py
+-rw-r--r--   0        0        0      837 2024-04-15 12:41:50.577849 pldag-0.6.5/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-18 13:33:16.090714 pldag-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 pldag-0.6.5/PKG-INFO
```

### Comparing `pldag-0.6.4/LICENSE` & `pldag-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.6.4/README.md` & `pldag-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.6.4/pldag/__init__.py` & `pldag-0.6.5/pldag/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from hashlib import sha1
 from itertools import groupby, repeat
-from functools import partial
-from typing import Dict, List, Set
+from functools import partial, lru_cache
+from typing import Dict, List, Set, Optional
 from graphlib import TopologicalSorter
 
 from enum import Enum
 from importlib import import_module
 
 class Solver(Enum):
     GLPK = "glpk"
@@ -35,14 +35,22 @@
         self._dvec = np.zeros((0, ),    dtype=complex)
         # Bias vector
         self._bvec = np.zeros((0, ),    dtype=complex)
         # Boolean vector indicating if the node is a composition
         self._cvec = np.zeros((0, ),    dtype=bool)
         # Maps id's to index
         self._imap = {}
+        # Alias to id mapping
+        self._amap = {}
+
+    def __hash__(self) -> int:
+        return hash(self.sha1())
+    
+    def sha1(self) -> str:
+        return sha1("".join(self._imap.keys()).encode()).hexdigest()
 
     @property
     def bounds(self) -> np.ndarray:
         """Get the bounds of all aliases"""
         return self._dvec
     
     @property
@@ -73,14 +81,27 @@
         return self._col_vars[~self._cvec]
     
     @property
     def composites(self) -> np.ndarray:
         return self._col_vars[self._cvec]
     
     @property
+    def columns(self) -> np.ndarray:
+        return self._col_vars
+    
+    @property
+    def rows(self) -> np.ndarray:
+        return self.composites
+    
+    @property
+    def adjacency_matrix(self) -> np.ndarray:
+        """Get the adjacency matrix"""
+        return np.vstack((np.zeros((self._amat.shape[1]-self._amat.shape[0], self._amat.shape[1])), self._amat))
+    
+    @property
     def _revimap(self) -> dict:
         """Get the reverse map"""
         return dict(map(lambda x: (x[1], x[0]), self._imap.items()))
     
     @property
     def _col_vars(self) -> np.ndarray:
         return np.array(list(self._imap.keys()))
@@ -109,28 +130,31 @@
     
     def _row(self, id: str) -> int:
         """
             Returns the row index of the given ID.
         """
         return self._col(id) - (~self._cvec).sum()
     
-    def _set_gelineq(self, children: list, bias: int, negate: bool = False) -> str:
+    def _set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of at least `value`.
         """
         _id = self._composite_id(children, bias, negate)
         if not _id in self._imap:
             self._amat = np.pad(self._amat, ((0, 1), (0, 1)), mode='constant')
             self._amat[-1, [self._col(child) for child in children]] = 1
             self._dvec = np.append(self._dvec, complex(0, 1))
             self._bvec = np.append(self._bvec, complex(*repeat(bias * (1-negate) + (bias + 1) * negate * -1, 2)))
             self._nvec = np.append(self._nvec, negate)
             self._cvec = np.append(self._cvec, True)
             self._imap[_id] = self._amat.shape[1] - 1
 
+        if alias:
+            self._amap[alias] = _id
+
         return _id
     
     @staticmethod
     def _prop_algo(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, F: np.ndarray, forced: np.ndarray, max_iterations: int = 100):
 
         """
             Propagation algorithm.
@@ -161,14 +185,30 @@
             new_D = forced * D + ~forced * prop(previous_D)
             if (new_D == previous_D).all():
                 return new_D
             previous_D = new_D
         
         raise Exception(f"Maximum iterations ({max_iterations}) reached without convergence.")
     
+    def id_from_alias(self, alias: str) -> Optional[str]:
+        """Get the ID of the given alias"""
+        return self._amap.get(alias, None)
+    
+    def alias_to_ids(self, id: str) -> List[str]:
+        """Get the aliases of the given ID"""
+        return list(
+            map(
+                lambda x: x[0],
+                filter(
+                    lambda x: x[1] == id,
+                    self._amap.items(),
+                )
+            )
+        )
+    
     def get(self, *id: str) -> np.ndarray:
         """Get the bounds of the given ID(s)"""
         return self._dvec[list(map(self._col, id))]
     
     def exists(self, id: str) -> bool:
         """Check if the given id exists"""
         return (id in self._imap)
@@ -330,15 +370,15 @@
             List[str]
                 The IDs of the primitive variables.
         """
         for id in ids:
             self.set_primitive(id, bound)
         return ids
     
-    def set_atleast(self, references: List[str], value: int) -> str:
+    def set_atleast(self, references: List[str], value: int, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of at least `value`.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -355,17 +395,17 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self._set_gelineq(references, -1 * value, False)
+        return self._set_gelineq(references, -1 * value, False, alias)
     
-    def set_atmost(self, references: List[str], value: int) -> str:
+    def set_atmost(self, references: List[str], value: int, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of at most `value`.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -382,17 +422,17 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self._set_gelineq(references, -1 * (value + 1), True)
+        return self._set_gelineq(references, -1 * (value + 1), True, alias)
     
-    def set_or(self, references: List[str]) -> str:
+    def set_or(self, references: List[str], alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an OR operation.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -406,17 +446,17 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self.set_atleast(references, 1)
+        return self.set_atleast(references, 1, alias)
     
-    def set_and(self, references: List[str]) -> str:
+    def set_and(self, references: List[str], alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an AND operation.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -430,17 +470,17 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self.set_atleast(references, len(references))
+        return self.set_atleast(references, len(references), alias)
     
-    def set_not(self, references: List[str]) -> str:
+    def set_not(self, references: List[str], alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of a NOT operation.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -454,17 +494,17 @@
             0j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self.set_atmost(references, 0)
+        return self.set_atmost(references, 0, alias)
     
-    def set_xor(self, references: List[str]) -> str:
+    def set_xor(self, references: List[str], alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an XOR operation.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -481,17 +521,17 @@
             -------
             str
                 The ID of the composite constraint.
         """
         return self.set_and([
             self.set_atleast(references, 1),
             self.set_atmost(references, 1),
-        ])
+        ], alias)
     
-    def set_imply(self, condition: str, consequence: str) -> str:
+    def set_imply(self, condition: str, consequence: str, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an IMPLY operation.
 
             Parameters
             ----------
             condition : str
                 The reference to the condition.
@@ -514,17 +554,48 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self.set_or([self.set_not([condition]), consequence])
+        return self.set_or([self.set_not([condition]), consequence], alias)
+
+    def set_equal(self, references: List[str], alias: Optional[str] = None) -> str:
+        """
+            Add a composite constraint of an EQUAL operation.
 
-    def to_polyhedron(self, fix: Dict[str, int] = {}) -> tuple:
+            Parameters
+            ----------
+            references : List[str]
+                The references to composite constraints or primitive variables.
+
+            Examples
+            --------
+            >>> model = PLDAG()
+            >>> model.set_primitives("xy")
+            >>> a = model.set_equal("x", "y")
+            >>> model.test({"x": 1j, "y": 1j}).get(a)
+            1j
+
+            >>> model.test({"x": 1+1j, "y": 0j}).get(a)
+            0j
+
+            Returns
+            -------
+            str
+                The ID of the composite constraint.
+        """
+        return self.set_xor([
+            self.set_and(references),
+            self.set_not(references),
+        ], alias)
+    
+    @lru_cache
+    def to_polyhedron(self, **fix) -> tuple:
 
         """
             Constructs a polyhedron of matrix A and bias vector b,
             such that A.dot(x) >= b, where x is the vector of variables.
             Every composite variable A is its own column in the matrix where
             A -> (A's composite proposition) is true. 
 
@@ -583,14 +654,33 @@
                 _b = a.sum() * i
             else:
                 _b = 0
 
             A = np.vstack([A, a])
             b = np.append(b, _b)
 
+        # Set bounds for integer variables
+        int_vars = list(set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
+
+        # Declare new constraints for upper and lower bound for integer variables
+        A_int = np.zeros((len(int_vars) * 2, A.shape[1]), dtype=np.int64)
+        b_int = np.zeros((len(int_vars) * 2, ), dtype=np.int64)
+        
+        # Lower bound for integers..
+        A_int[np.arange(len(int_vars) * 2, step=2), int_vars] = 1
+        b_int[np.arange(len(int_vars) * 2, step=2)] = self._dvec[int_vars].real
+        
+        # Upper bound for integers..
+        A_int[np.arange(len(int_vars) * 2, step=2) + 1, int_vars] = -1
+        b_int[np.arange(len(int_vars) * 2, step=2) + 1] = -1 * self._dvec[int_vars].imag
+
+        # Add them onto polyhedron
+        A = np.vstack([A, A_int])
+        b = np.append(b, b_int)
+
         # Reverse index map
         rimap = dict(map(lambda x: (x[1], x[0]), self._imap.items()))
 
         # Create the variable list
         variables = np.array(
             list(
                 map(
@@ -709,15 +799,15 @@
             [{'x': 0, 'y': 1, 'z': 0}]
 
             Returns
             -------
             List[Dict[str, int]]
                 The solutions for the objectives.
         """
-        A, b, variables = self.to_polyhedron(fix)
+        A, b, variables = self.to_polyhedron(**fix)
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
             solutions = solve_lp(A, b, obj_mat, set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
```

### Comparing `pldag-0.6.4/pldag/solver/glpk_solver.py` & `pldag-0.6.5/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.6.4/PKG-INFO` & `pldag-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

