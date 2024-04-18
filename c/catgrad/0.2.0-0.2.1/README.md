# Comparing `tmp/catgrad-0.2.0.tar.gz` & `tmp/catgrad-0.2.1.tar.gz`

## Comparing `catgrad-0.2.0.tar` & `catgrad-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/combinators.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/compile.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/layers.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/signature.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/bidirectional/functor.py
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/bidirectional/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/core/__init__.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/core/operation.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/special/definition.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/special/parameter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/ast.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/special.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/__init__.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/numpy.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/torch.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/array_backend/type.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/__init__.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/codegen.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/definition.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 catgrad-0.2.0/catgrad/target/python/codegen/operation.py
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 catgrad-0.2.0/LICENSE
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 catgrad-0.2.0/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 catgrad-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 catgrad-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/combinators.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/compile.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/layers.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/signature.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/bidirectional/functor.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/bidirectional/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/core/__init__.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/core/operation.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/special/definition.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/special/parameter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/ast.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/special.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/array_backend/__init__.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/array_backend/numpy.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/array_backend/torch.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/array_backend/type.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/codegen/__init__.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/codegen/codegen.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/codegen/definition.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 catgrad-0.2.1/catgrad/target/python/codegen/operation.py
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 catgrad-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 catgrad-0.2.1/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 catgrad-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 catgrad-0.2.1/PKG-INFO
```

### Comparing `catgrad-0.2.0/catgrad/combinators.py` & `catgrad-0.2.1/catgrad/combinators.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/compile.py` & `catgrad-0.2.1/catgrad/compile.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/layers.py` & `catgrad-0.2.1/catgrad/layers.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/signature.py` & `catgrad-0.2.1/catgrad/signature.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/bidirectional/functor.py` & `catgrad-0.2.1/catgrad/bidirectional/functor.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/bidirectional/operation.py` & `catgrad-0.2.1/catgrad/bidirectional/operation.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/core/operation.py` & `catgrad-0.2.1/catgrad/core/operation.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/special/definition.py` & `catgrad-0.2.1/catgrad/special/definition.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/special/parameter.py` & `catgrad-0.2.1/catgrad/special/parameter.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/ast.py` & `catgrad-0.2.1/catgrad/target/ast.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/python/special.py` & `catgrad-0.2.1/catgrad/target/python/special.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/python/array_backend/numpy.py` & `catgrad-0.2.1/catgrad/target/python/array_backend/numpy.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,25 @@
         return np.broadcast_to(x.reshape(x.shape + (1,)*len(shape)), x.shape + shape)
 
     @staticmethod
     def nsplit(x: np.ndarray, k: int) -> List[np.ndarray]:
         if k == 0:
             return None
 
-        result = np.split(x, k, -1)
+        # NOTE: nsplit *removes* final dimension (as if keepdims=False)
+        result = [ x.reshape(x.shape[:-1]) for x in np.split(x, k, -1) ]
         if k == 1:
             return result[0] # unpack list for single values
         return result
 
     @staticmethod
     def nconcatenate(xs: List[np.ndarray], k: int) -> List[np.ndarray]:
         assert len(xs) == k
         if k == 0: return None
+        xs = [np.expand_dims(x, -1) for x in xs]
         return np.concatenate(xs, axis=-1)
 
     @staticmethod
     def nadd(dims: Tuple, x: np.ndarray) -> np.ndarray:
         return x.sum(dims)
 
     @staticmethod
```

### Comparing `catgrad-0.2.0/catgrad/target/python/array_backend/torch.py` & `catgrad-0.2.1/catgrad/target/python/array_backend/torch.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,23 +23,24 @@
     @staticmethod
     def nsplit(x: torch.tensor, k: int) -> List[torch.tensor]:
         if k == 0:
             return None
 
         # NOTE: this interface is subtly different to numpy!
         # You specify the *size* of the chunk, not the number of splits!
-        result = torch.split(x, 1, dim=-1)
+        result = [ a.squeeze(-1) for a in torch.split(x, 1, dim=-1) ]
         if k == 1:
             return result[0] # unpack list for single values
         return result
 
     @staticmethod
     def nconcatenate(xs: List[torch.tensor], k: int) -> List[torch.tensor]:
         assert len(xs) == k
         if k == 0: return None
+        xs = [ a.unsqueeze(-1) for a in xs ]
         return torch.concatenate(xs, axis=-1)
 
     @staticmethod
     def nadd(dims: Tuple, x: torch.tensor) -> torch.tensor:
         return x.sum(dims)
 
     @staticmethod
```

### Comparing `catgrad-0.2.0/catgrad/target/python/array_backend/type.py` & `catgrad-0.2.1/catgrad/target/python/array_backend/type.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/python/codegen/codegen.py` & `catgrad-0.2.1/catgrad/target/python/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/python/codegen/definition.py` & `catgrad-0.2.1/catgrad/target/python/codegen/definition.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/catgrad/target/python/codegen/operation.py` & `catgrad-0.2.1/catgrad/target/python/codegen/operation.py`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/LICENSE` & `catgrad-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catgrad-0.2.0/README.md` & `catgrad-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,9 +67,10 @@
     python3 -m examples.iris (linear|simple|dense|hidden)
 
 # Compilation Targets
 
 Target backends we plan to support soon:
 
 - [x] Python/numpy
+- [x] Python/torch
 - [ ] Python/[tinygrad](https://github.com/tinygrad/tinygrad/)
 - [ ] C++/[GGML](https://github.com/ggerganov/ggml)
```

### Comparing `catgrad-0.2.0/pyproject.toml` & `catgrad-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "catgrad"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "deep learning with reverse derivatives"
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
```

### Comparing `catgrad-0.2.0/PKG-INFO` & `catgrad-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: catgrad
-Version: 0.2.0
+Version: 0.2.1
 Summary: deep learning with reverse derivatives
 Project-URL: Homepage, https://github.com/statusfailed/catgrad/
 Project-URL: Github, https://github.com/statusfailed/catgrad/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -86,9 +86,10 @@
     python3 -m examples.iris (linear|simple|dense|hidden)
 
 # Compilation Targets
 
 Target backends we plan to support soon:
 
 - [x] Python/numpy
+- [x] Python/torch
 - [ ] Python/[tinygrad](https://github.com/tinygrad/tinygrad/)
 - [ ] C++/[GGML](https://github.com/ggerganov/ggml)
```

