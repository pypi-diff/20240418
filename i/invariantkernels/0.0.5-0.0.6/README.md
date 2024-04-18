# Comparing `tmp/invariantkernels-0.0.5.tar.gz` & `tmp/invariantkernels-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invariantkernels-0.0.5.tar", last modified: Tue Mar 26 12:05:11 2024, max compression
+gzip compressed data, was "invariantkernels-0.0.6.tar", last modified: Thu Apr 18 14:06:46 2024, max compression
```

## Comparing `invariantkernels-0.0.5.tar` & `invariantkernels-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-03-26 12:05:11.538928 invariantkernels-0.0.5/
--rw-rw-r--   0 theo      (1000) theo      (1000)     1071 2024-03-01 12:02:46.000000 invariantkernels-0.0.5/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)      915 2024-03-26 12:05:11.538928 invariantkernels-0.0.5/PKG-INFO
--rw-rw-r--   0 theo      (1000) theo      (1000)      417 2024-03-04 10:58:14.000000 invariantkernels-0.0.5/README.md
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-03-26 12:05:11.534928 invariantkernels-0.0.5/invariantkernels/
--rw-rw-r--   0 theo      (1000) theo      (1000)      135 2024-03-04 11:09:36.000000 invariantkernels-0.0.5/invariantkernels/__init__.py
--rw-rw-r--   0 theo      (1000) theo      (1000)     2299 2024-03-08 12:17:41.000000 invariantkernels-0.0.5/invariantkernels/group_invariant_kernel.py
--rw-rw-r--   0 theo      (1000) theo      (1000)     2908 2024-03-26 12:01:46.000000 invariantkernels-0.0.5/invariantkernels/transformation_groups.py
-drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-03-26 12:05:11.534928 invariantkernels-0.0.5/invariantkernels.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)      915 2024-03-26 12:05:11.000000 invariantkernels-0.0.5/invariantkernels.egg-info/PKG-INFO
--rw-rw-r--   0 theo      (1000) theo      (1000)      345 2024-03-26 12:05:11.000000 invariantkernels-0.0.5/invariantkernels.egg-info/SOURCES.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)        1 2024-03-26 12:05:11.000000 invariantkernels-0.0.5/invariantkernels.egg-info/dependency_links.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)        9 2024-03-26 12:05:11.000000 invariantkernels-0.0.5/invariantkernels.egg-info/requires.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)       17 2024-03-26 12:05:11.000000 invariantkernels-0.0.5/invariantkernels.egg-info/top_level.txt
--rw-rw-r--   0 theo      (1000) theo      (1000)      637 2024-03-26 12:03:50.000000 invariantkernels-0.0.5/pyproject.toml
--rw-rw-r--   0 theo      (1000) theo      (1000)       38 2024-03-26 12:05:11.538928 invariantkernels-0.0.5/setup.cfg
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-18 14:06:46.114905 invariantkernels-0.0.6/
+-rw-rw-r--   0 theo      (1000) theo      (1000)     1071 2024-03-01 12:02:46.000000 invariantkernels-0.0.6/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-18 14:06:46.114905 invariantkernels-0.0.6/PKG-INFO
+-rw-rw-r--   0 theo      (1000) theo      (1000)      582 2024-03-26 12:05:25.000000 invariantkernels-0.0.6/README.md
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-18 14:06:46.114905 invariantkernels-0.0.6/invariantkernels/
+-rw-rw-r--   0 theo      (1000) theo      (1000)      135 2024-03-04 11:09:36.000000 invariantkernels-0.0.6/invariantkernels/__init__.py
+-rw-rw-r--   0 theo      (1000) theo      (1000)     2299 2024-03-08 12:17:41.000000 invariantkernels-0.0.6/invariantkernels/group_invariant_kernel.py
+-rw-rw-r--   0 theo      (1000) theo      (1000)     2911 2024-04-18 13:58:55.000000 invariantkernels-0.0.6/invariantkernels/transformation_groups.py
+drwxrwxr-x   0 theo      (1000) theo      (1000)        0 2024-04-18 14:06:46.114905 invariantkernels-0.0.6/invariantkernels.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1081 2024-04-18 14:06:46.000000 invariantkernels-0.0.6/invariantkernels.egg-info/PKG-INFO
+-rw-rw-r--   0 theo      (1000) theo      (1000)      345 2024-04-18 14:06:46.000000 invariantkernels-0.0.6/invariantkernels.egg-info/SOURCES.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)        1 2024-04-18 14:06:46.000000 invariantkernels-0.0.6/invariantkernels.egg-info/dependency_links.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)        9 2024-04-18 14:06:46.000000 invariantkernels-0.0.6/invariantkernels.egg-info/requires.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)       17 2024-04-18 14:06:46.000000 invariantkernels-0.0.6/invariantkernels.egg-info/top_level.txt
+-rw-rw-r--   0 theo      (1000) theo      (1000)      637 2024-04-18 14:06:03.000000 invariantkernels-0.0.6/pyproject.toml
+-rw-rw-r--   0 theo      (1000) theo      (1000)       38 2024-04-18 14:06:46.114905 invariantkernels-0.0.6/setup.cfg
```

### Comparing `invariantkernels-0.0.5/LICENSE` & `invariantkernels-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `invariantkernels-0.0.5/PKG-INFO` & `invariantkernels-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invariantkernels
-Version: 0.0.5
+Version: 0.0.6
 Summary: Transformation-invariant kernels in GPyTorch
 Author-email: Theodore Brown <theo.brown.uk@gmail.com>
 Project-URL: Homepage, https://github.com/theo-brown/invariantkernels
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -14,7 +14,13 @@
 
 # invariantkernels
 *Transformation-invariant kernels in GPyTorch*
 
 This package provides kernels for Gaussian processes that are invariant to transformations.
 The core class is `GroupInvariantKernel`, which can be composed with other GPyTorch kernels to make them invariant to a group of transformations.
 Example groups are in [`invariant_kernels/transformation_groups`](./invariantkernels/transformation_groups.py).
+
+## Build notes 
+1. Update the version in `pyproject.toml`
+2. Remove the old versions from `build/` and `dist/`
+3. Run `python -m` build
+4. Run `twine upload dist/*`
```

### Comparing `invariantkernels-0.0.5/invariantkernels/group_invariant_kernel.py` & `invariantkernels-0.0.6/invariantkernels/group_invariant_kernel.py`

 * *Files identical despite different names*

### Comparing `invariantkernels-0.0.5/invariantkernels/transformation_groups.py` & `invariantkernels-0.0.6/invariantkernels/transformation_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         Input data. Shape is ``(n, d)`` or ``(b, n, d), where ``b`` is the batch size, ``n`` is the number of data points and ``d`` is the number of input dimensions.
 
     Returns
     -------
     torch.tensor
         All permutations of the last dimension of x. Shape is ``(G, n, d)``, where ``G`` is the number of permutations of the last dimension of x.
     """
-    indices = range(x.size(-1))  # x is of shape n x d or b x n x d
+    indices = range(x.shape[-1])  # x is of shape n x d or b x n x d
     permuted_indices = [list(p) for p in itertools.permutations(indices)]
     if x.dim() == 2:
         x_orbits = x[:, permuted_indices]  # Shape is n x G x d
         return x_orbits.permute(1, 0, 2)  # Reorder the dimensions to G x n x d
     elif x.dim() == 3:
         x_orbits = x[:, :, permuted_indices]  # Shape is b x n x G x d
         return x_orbits.permute(2, 0, 1, 3)  # Reorder the dimensions to G x b x n x d
@@ -41,18 +41,18 @@
         Size of the blocks to permute. Must be a divisor of the last dimension of x.
 
     Returns
     -------
     torch.tensor
         All block-permutations of the last dimension of x. Shape is ``(G, n, d)``, where ``G`` is the number of block-permutations of the last dimension of x.
     """
-    if x.size(-1) % block_size != 0:
+    if x.shape[-1] % block_size != 0:
         raise ValueError(
             "Last dimension of x must be a multiple of block size"
-            f" (got {x.size(-1)} and {block_size} respectively)."
+            f" (got {x.shape[-1]} and {block_size} respectively)."
         )
 
     block_indices = [range(i, i + block_size) for i in range(0, x.size(-1), block_size)]
     # Use itertools.chain to flatten the list of lists generated by the permutation
     permuted_indices = [
         list(itertools.chain.from_iterable(p))
         for p in itertools.permutations(block_indices)
```

### Comparing `invariantkernels-0.0.5/invariantkernels.egg-info/PKG-INFO` & `invariantkernels-0.0.6/invariantkernels.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invariantkernels
-Version: 0.0.5
+Version: 0.0.6
 Summary: Transformation-invariant kernels in GPyTorch
 Author-email: Theodore Brown <theo.brown.uk@gmail.com>
 Project-URL: Homepage, https://github.com/theo-brown/invariantkernels
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -14,7 +14,13 @@
 
 # invariantkernels
 *Transformation-invariant kernels in GPyTorch*
 
 This package provides kernels for Gaussian processes that are invariant to transformations.
 The core class is `GroupInvariantKernel`, which can be composed with other GPyTorch kernels to make them invariant to a group of transformations.
 Example groups are in [`invariant_kernels/transformation_groups`](./invariantkernels/transformation_groups.py).
+
+## Build notes 
+1. Update the version in `pyproject.toml`
+2. Remove the old versions from `build/` and `dist/`
+3. Run `python -m` build
+4. Run `twine upload dist/*`
```

### Comparing `invariantkernels-0.0.5/pyproject.toml` & `invariantkernels-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invariantkernels"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
   "gpytorch"
 ]
 description = "Transformation-invariant kernels in GPyTorch"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
```

