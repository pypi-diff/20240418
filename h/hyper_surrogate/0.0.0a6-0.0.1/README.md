# Comparing `tmp/hyper_surrogate-0.0.0a6.tar.gz` & `tmp/hyper_surrogate-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper_surrogate-0.0.0a6.tar", max compression
+gzip compressed data, was "hyper_surrogate-0.0.1.tar", max compression
```

## Comparing `hyper_surrogate-0.0.0a6.tar` & `hyper_surrogate-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/LICENSE
--rw-r--r--   0        0        0     1103 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/README.md
--rw-r--r--   0        0        0        0 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/__init__.py
--rw-r--r--   0        0        0    10696 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/deformation_gradient.py
--rw-r--r--   0        0        0     4505 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/generator.py
--rw-r--r--   0        0        0     4110 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/kinematics.py
--rw-r--r--   0        0        0     2648 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/materials.py
--rw-r--r--   0        0        0     4880 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/reporter.py
--rw-r--r--   0        0        0     6502 2024-04-18 08:10:14.932229 hyper_surrogate-0.0.0a6/hyper_surrogate/symbolic.py
--rw-r--r--   0        0        0     2062 2024-04-18 08:10:34.024319 hyper_surrogate-0.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 hyper_surrogate-0.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2565 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/__init__.py
+-rw-r--r--   0        0        0    10696 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/deformation_gradient.py
+-rw-r--r--   0        0        0     4505 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/generator.py
+-rw-r--r--   0        0        0     4111 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/kinematics.py
+-rw-r--r--   0        0        0     1216 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/materials.py
+-rw-r--r--   0        0        0     6486 2024-03-28 15:57:44.683962 hyper_surrogate-0.0.1/hyper_surrogate/symbolic.py
+-rw-r--r--   0        0        0     1909 2024-03-28 15:58:02.120047 hyper_surrogate-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 hyper_surrogate-0.0.1/PKG-INFO
```

### Comparing `hyper_surrogate-0.0.0a6/LICENSE` & `hyper_surrogate-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_surrogate-0.0.0a6/hyper_surrogate/deformation_gradient.py` & `hyper_surrogate-0.0.1/hyper_surrogate/deformation_gradient.py`

 * *Files identical despite different names*

### Comparing `hyper_surrogate-0.0.0a6/hyper_surrogate/generator.py` & `hyper_surrogate-0.0.1/hyper_surrogate/generator.py`

 * *Files identical despite different names*

### Comparing `hyper_surrogate-0.0.0a6/hyper_surrogate/kinematics.py` & `hyper_surrogate-0.0.1/hyper_surrogate/kinematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def pushforward(f: np.ndarray, tensor2D: np.ndarray) -> Any:
         """
         Forward tensor configuration.
         F*tensor2D*F^T. This is the forward transformation of a 2D tensor.
 
         Args:
             f (np.ndarray): deformation gradient # (N, 3, 3)
-            tensor2D (np.ndarray): The 2D tensor to be mapped # (N, 3, 3)
+            2d_tensor (np.ndarray): The 2D tensor to be mapped # (N, 3, 3)
 
         Returns:
             np.ndarray: The transformed tensor.
         """
         return np.einsum("nik,njl,nkl->nij", f, f, tensor2D)
 
     def principal_stretches(self, f: np.ndarray) -> np.ndarray:
```

### Comparing `hyper_surrogate-0.0.0a6/hyper_surrogate/symbolic.py` & `hyper_surrogate-0.0.1/hyper_surrogate/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         *args: dict,
     ) -> Any:
         """
         Automatically substitute numerical values from a given 3x3 numerical matrix into c_tensor.
 
         Args:
             symbolic_tensor (sym.Matrix): A symbolic tensor to substitute numerical values into.
-            numerical_c_tensor (np.ndarray): A 3x3 numerical matrix to substitute into c_tensor.
+            numerical_matrix (np.ndarray): A 3x3 numerical matrix to substitute into c_tensor.
             args (dict): Additional substitution dictionaries.
 
         Returns:
             sym.Matrix: The symbolic_tensor with numerical values substituted.
 
         Raises:
             ValueError: If numerical_tensor is not a 3x3 matrix.
@@ -142,15 +142,15 @@
         *args: dict,
     ) -> Any:
         """
         Automatically substitute numerical values from a given 3x3 numerical matrix into c_tensor.
 
         Args:
             symbolic_tensor (sym.Matrix): A symbolic tensor to substitute numerical values into.
-            numerical_c_tensors (np.ndarray): N 3x3 numerical matrices to substitute into c_tensor.
+            numerical_matrix (np.ndarray): A 3x3 numerical matrix to substitute into c_tensor.
             args (dict): Additional substitution dictionaries.
 
         Returns:
             sym.Matrix: The symbolic_tensor with numerical values substituted.
 
         Raises:
             ValueError: If numerical_tensor is not a 3x3 matrix.
@@ -159,15 +159,15 @@
             yield self.substitute(symbolic_tensor, numerical_c_tensor, *args)
 
     def lambdify(self, symbolic_tensor: sym.Matrix, *args: Iterable[Any]) -> Any:
         """
         Create a lambdified function from a symbolic tensor that can be used for numerical evaluation.
 
         Args:
-            symbolic_tensor (sym.Expr or sym.Matrix): The symbolic tensor to be lambdified.
+            tensor (sym.Expr or sym.Matrix): The symbolic tensor to be lambdified.
             args (dict): Additional substitution lists of symbols.
         Returns:
             function: A function that can be used to numerically evaluate the tensor with specific values.
         """
 
         return sym.lambdify((self.c_symbols(), *args), symbolic_tensor, modules="numpy")
```

### Comparing `hyper_surrogate-0.0.0a6/pyproject.toml` & `hyper_surrogate-0.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 [tool.poetry]
 name = "hyper_surrogate"
-version = "v0.0.0-alpha.6"
+version = "0.0.1"
 description = "Hyperelastic Surrogates"
 authors = ["Joao Ferreira <fj.ferreira@fe.up.pt>"]
 repository = "https://github.com/jpsferreira/hyper-surrogate"
 documentation = "https://jpsferreira.github.io/hyper-surrogate/"
 readme = "README.md"
 packages = [
   {include = "hyper_surrogate"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 numpy = "^1.26.4"
 sympy = "^1.12"
-matplotlib = "^3.8.3"
-seaborn = "^0.13.2"
-tqdm = "^4.66.2"
-pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
 tox = "^4.11.1"
 ipykernel = "^6.29.3"
-types-tqdm = "^4.66.0.20240106"
-types-seaborn = "^0.13.2.20240311"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.2.7"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 
 [build-system]
```

