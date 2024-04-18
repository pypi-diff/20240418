# Comparing `tmp/ikpls-1.1.3.tar.gz` & `tmp/ikpls-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikpls-1.1.3.tar", max compression
+gzip compressed data, was "ikpls-1.2.0.tar", max compression
```

## Comparing `ikpls-1.1.3.tar` & `ikpls-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-10 17:54:41.941952 ikpls-1.1.3/LICENSE
--rw-r--r--   0        0        0     8047 2024-03-10 17:54:41.941952 ikpls-1.1.3/README.rst
--rw-r--r--   0        0        0       21 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/fast_cross_validation/__init__.py
--rw-r--r--   0        0        0    20401 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/fast_cross_validation/numpy_ikpls.py
--rw-r--r--   0        0        0    14861 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/jax_ikpls_alg_1.py
--rw-r--r--   0        0        0    12992 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/jax_ikpls_alg_2.py
--rw-r--r--   0        0        0    39561 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/jax_ikpls_base.py
--rw-r--r--   0        0        0     9091 2024-03-10 17:54:41.941952 ikpls-1.1.3/ikpls/numpy_ikpls.py
--rw-r--r--   0        0        0      553 2024-03-10 17:54:41.945952 ikpls-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     8966 1970-01-01 00:00:00.000000 ikpls-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11433 2024-04-18 15:45:10.087361 ikpls-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8767 2024-04-18 15:45:10.087361 ikpls-1.2.0/README.rst
+-rw-r--r--   0        0        0       22 2024-04-18 15:45:10.087361 ikpls-1.2.0/ikpls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:45:10.087361 ikpls-1.2.0/ikpls/fast_cross_validation/__init__.py
+-rw-r--r--   0        0        0    23705 2024-04-18 15:45:10.087361 ikpls-1.2.0/ikpls/fast_cross_validation/numpy_ikpls.py
+-rw-r--r--   0        0        0    15583 2024-04-18 15:45:10.087361 ikpls-1.2.0/ikpls/jax_ikpls_alg_1.py
+-rw-r--r--   0        0        0    13495 2024-04-18 15:45:10.087361 ikpls-1.2.0/ikpls/jax_ikpls_alg_2.py
+-rw-r--r--   0        0        0    41664 2024-04-18 15:45:10.091361 ikpls-1.2.0/ikpls/jax_ikpls_base.py
+-rw-r--r--   0        0        0    10170 2024-04-18 15:45:10.091361 ikpls-1.2.0/ikpls/numpy_ikpls.py
+-rw-r--r--   0        0        0      553 2024-04-18 15:45:10.091361 ikpls-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9686 1970-01-01 00:00:00.000000 ikpls-1.2.0/PKG-INFO
```

### Comparing `ikpls-1.1.3/LICENSE` & `ikpls-1.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Ole-Christian Galbo Engstrøm, Erik Schou Dreier, Birthe Møller Jespersen, and Kim Steenstrup Pedersen
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/README.rst` & `ikpls-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
 =======================================================================
 
 .. image:: https://img.shields.io/pypi/v/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: PyPI Version
+.. image:: https://img.shields.io/pypi/dm/ikpls
+   :target: https://pypi.python.org/pypi/ikpls/
+   :alt: PyPI - Downloads
 .. image:: https://img.shields.io/pypi/pyversions/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: Python Versions
 .. image:: https://img.shields.io/pypi/l/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: License
 .. image:: https://readthedocs.org/projects/ikpls/badge/?version=latest
@@ -36,21 +39,23 @@
 .. _Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 11(1), 73-85: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?
 .. _Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720: https://doi.org/10.1007/s00362-009-0251-7
 .. _Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 23(10), 518-529: https://doi.org/10.1002/cem.1248
 .. _NumPy: https://numpy.org/
 .. _scikit-learn: https://scikit-learn.org/stable/
 .. _JAX: https://jax.readthedocs.io/en/latest/
 
-Extremely Fast Cross-Validation
+Fast Cross-Validation
 -------------------------------
 In addition to the implementations mentioned above, this package contains the novel, fast cross-validation algorithms mentioned in [7]_ using both IKPLS algorithms.
 The fast cross-validation algorithms benefit both IKPLS Algorithms and especially Algorithm #2.
 The fast cross-validation algorithms are mathematically equivalent to the classical cross-validation algorithm. Still, they are much quicker if cross-validation splits exceed 3.
 The fast cross-validation algorithms correctly handle (column-wise) centering and scaling of the X and Y input matrices using training set means and standard deviations to avoid data leakage from the validation set.
 This centering and scaling can be enabled by setting the center parameter to True and the scale parameter to True, respectively.
+The fast cross-validation algorithms correctly handle row-wise preprocessing such as (row-wise) centering and scaling of the X and Y input matrices, convolution, or other preprocessing.
+Row-wise preprocessing can safely be applied before passing the data to the fast cross-validation algorithms.
 
 .. [7] `Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments`_.
 
 .. _Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation\: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments: https://arxiv.org/abs/2401.13185
 
 Pre-requisites
 --------------
@@ -76,41 +81,62 @@
 Quick Start
 -----------
 Use the ikpls package for PLS modeling
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~   
 
   .. code:: python
 
-    import numpy as np
+   import numpy as np
+
+   from ikpls.numpy_ikpls import PLS
 
-    from ikpls.numpy_ikpls import PLS
 
     N = 100  # Number of samples.
     K = 50  # Number of features.
     M = 10  # Number of targets.
     A = 20  # Number of latent variables (PLS components).
 
+    # Using float64 is important for numerical stability.
     X = np.random.uniform(size=(N, K)).astype(np.float64)
     Y = np.random.uniform(size=(N, M)).astype(np.float64)
 
-    # The other PLS algorithms and implementations, except for NpPLS_FastCV, have the same interface for fit() and predict().
+    # The other PLS algorithms and implementations have the same interface for fit()
+    # and predict(). The fast cross-validation implementation with IKPLS has a
+    # different interface.
     np_ikpls_alg_1 = PLS(algorithm=1)
     np_ikpls_alg_1.fit(X, Y, A)
 
-    y_pred = np_ikpls_alg_1.predict(X) # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible numbers of components up to and including A.
-    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20) # Has shape (N, M) = (100, 10).
-    (y_pred_20_components == y_pred[19]).all() # True
+    # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
+    # numbers of components up to and including A.
+    y_pred = np_ikpls_alg_1.predict(X)
+
+    # Has shape (N, M) = (100, 10).
+    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
+    (y_pred_20_components == y_pred[19]).all()  # True
 
     # The internal model parameters can be accessed as follows:
-    np_ikpls_alg_1.B  # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
-    np_ikpls_alg_1.W  # X weights matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.P  # X loadings matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.Q  # Y loadings matrix of shape (M, A) = (10, 20).
-    np_ikpls_alg_1.R  # X rotations matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.T  # X scores matrix of shape (N, A) = (100, 20). This is only computed for IKPLS Algorithm #1.
+
+    # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
+    np_ikpls_alg_1.B
+
+    # X weights matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.W
+
+    # X loadings matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.P
+
+    # Y loadings matrix of shape (M, A) = (10, 20).
+    np_ikpls_alg_1.Q
+
+    # X rotations matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.R
+
+    # X scores matrix of shape (N, A) = (100, 20).
+    # This is only computed for IKPLS Algorithm #1.
+    np_ikpls_alg_1.T
 
 Examples
 ~~~~~~~~
 
 In `examples <https://github.com/Sm00thix/IKPLS/tree/main/examples>`_ you will find:
 
 - `Fit and Predict with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py>`_
@@ -121,7 +147,11 @@
 
 - `Cross-validate with NumPy and fast cross-validation. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py>`_
 
 - `Cross-validate with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py>`_
 
 - `Compute the gradient of a preprocessing convolution filter with respect to the RMSE between the target value and the value predicted by PLS after fitting with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py>`_
 
+Contribute
+----------
+
+To contribute, please read the `Contribution Guidelines <https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.rst>`_.
```

### Comparing `ikpls-1.1.3/ikpls/fast_cross_validation/numpy_ikpls.py` & `ikpls-1.2.0/ikpls/fast_cross_validation/numpy_ikpls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,63 @@
+"""
+Contains the PLS class which implements fast cross-validation with partial
+least-squares regression using Improved Kernel PLS by Dayal and MacGregor:
+https://arxiv.org/abs/2401.13185
+https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+
+The implementation is written using NumPy and allows for parallelization of the
+cross-validation process using joblib.
+
+Author: Ole-Christian Galbo Engstrøm
+E-mail: ole.e@di.ku.dk
+"""
+
 import warnings
-from typing import Any, Callable, Union
+from collections import defaultdict
+from typing import Any, Callable, Hashable, Iterable, Union
 
 import joblib
 import numpy as np
 import numpy.linalg as la
 import numpy.typing as npt
 from joblib import Parallel, delayed
 
 
 class PLS:
     """
-    Implements fast cross-validation with partial least-squares regression using Improved Kernel PLS by Dayal and MacGregor: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+    Implements fast cross-validation with partial least-squares regression using
+    Improved Kernel PLS by Dayal and MacGregor:
+    https://arxiv.org/abs/2401.13185
+    https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
     center : bool, optional default=False
-            Whether to center `X` and `Y` before fitting by subtracting a mean row from each. The centering is computed on the training set for each fold to avoid data leakage. The centering is undone before returning predictions. Setting this to True while using multiple jobs will increase the memory consumption as each job will then have to keep its own copy of the data with its specific centering.
+            Whether to center `X` and `Y` before fitting by subtracting a mean row from
+            each. The centering is computed on the training set for each fold to avoid
+            data leakage. The centering is undone before returning predictions. Setting
+            this to True while using multiple jobs will increase the memory consumption
+            as each job will then have to keep its own copy of the data with its
+            specific centering.
 
     scale : bool, optional default=False, only used if `center` is True
-        Whether to scale `X` and `Y` before fitting by dividing each row by its standard deviation. The scaling is computed on the training set for each fold to avoid data leakage. The scaling is undone before returning predictions. Setting this to True while using multiple jobs will increase the memory consumption as each job will then have to keep its own copy of the data with its specific scaling.
+        Whether to scale `X` and `Y` before fitting by dividing each row by its
+        standard deviation. The scaling is computed on the training set for each fold
+        to avoid data leakage. The scaling is undone before returning predictions.
+        Setting this to True while using multiple jobs will increase the memory
+        consumption as each job will then have to keep its own copy of the data with
+        its specific scaling.
 
     algorithm : int, default=1
         Whether to use Improved Kernel PLS Algorithm #1 or #2.
 
     dtype : numpy.float, default=numpy.float64
-        The float datatype to use in computation of the PLS algorithm. Using a lower precision than float64 will yield significantly worse results when using an increasing number of components due to propagation of numerical errors.
+        The float datatype to use in computation of the PLS algorithm. Using a lower
+        precision than float64 will yield significantly worse results when using an
+        increasing number of components due to propagation of numerical errors.
 
     Raises
     ------
     ValueError
         If `algorithm` is not 1 or 2.
     """
 
@@ -44,18 +73,53 @@
         self.algorithm = algorithm
         self.dtype = dtype
         self.name = f"Improved Kernel PLS Algorithm #{algorithm}"
         if self.algorithm not in [1, 2]:
             raise ValueError(
                 f"Invalid algorithm: {self.algorithm}. Algorithm must be 1 or 2."
             )
+        self.X = None
+        self.Y = None
+        self.A = None
+        self.N = None
+        self.K = None
+        self.M = None
+        self.X_mean = None
+        self.Y_mean = None
+        self.sum_X = None
+        self.sum_Y = None
+        self.sum_sq_X = None
+        self.sum_sq_Y = None
+        self.XTX = None
+        self.XTY = None
+        if self.algorithm == 1:
+            self.all_indices = None
+
+    def _weight_warning(self, i: int) -> None:
+        """
+        Raises a warning if the weight is close to zero.
+
+        Parameters
+        ----------
+        norm : float
+            The norm of the weight vector.
+
+        i : int
+            The current number of components.
+        """
+        with warnings.catch_warnings():
+            warnings.simplefilter("always", UserWarning)
+            warnings.warn(
+                f"Weight is close to zero. Results with A = {i} component(s) or higher"
+                " may be unstable."
+            )
 
     def _stateless_fit(
         self,
-        validation_indices: npt.ArrayLike,
+        validation_indices: npt.NDArray[np.int_],
     ) -> Union[
         tuple[
             npt.NDArray[np.float_],
             npt.NDArray[np.float_],
             npt.NDArray[np.float_],
             npt.NDArray[np.float_],
             npt.NDArray[np.float_],
@@ -78,16 +142,17 @@
         ],
     ]:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
 
         Parameters
         ----------
-        validation_indices : Array of shape (N,)
-            Boolean array defining indices into X and Y corresponding to validation samples.
+        validation_indices : Array of shape (N_val,)
+            Integer array defining indices into X and Y corresponding to validation
+            samples.
 
         Returns
         -------
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         W : Array of shape (A, K)
@@ -98,55 +163,61 @@
 
         Q : Array of shape (A, M)
             PLS Loadings matrix for Y.
 
         R : Array of shape (A, K)
             PLS weights matrix to compute scores T directly from original X.
 
-        T : Array of shape (A, N)
+        T : Array of shape (A, N_train)
             PLS scores matrix of X. Only Returned for Improved Kernel PLS Algorithm #1.
 
         training_X_mean : Array of shape (1, K)
-            Mean row of training X. Will be an array of zeros if `self.center` is False.
+            Mean row of training X. Will be an array of zeros if `self.center` is
+            False.
 
         training_Y_mean : Array of shape (1, M)
-            Mean row of training Y. Will be an array of zeros if `self.center` is False.
+            Mean row of training Y. Will be an array of zeros if `self.center` is
+            False.
 
         training_X_std : Array of shape (1, K)
-            Sample standard deviation row of training X. Will be an array of ones if `self.scale` is False. Any zero standard deviations will be replaced with ones.
+            Sample standard deviation row of training X. Will be an array of ones if
+            `self.scale` is False. Any zero standard deviations will be replaced with
+            ones.
 
         training_Y_std : Array of shape (1, M)
-            Sample standard deviation row of training Y. Will be an array of ones if `self.scale` is False. Any zero standard deviations will be replaced with ones.
+            Sample standard deviation row of training Y. Will be an array of ones if
+            `self.scale` is False. Any zero standard deviations will be replaced with
+            ones.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
         """
 
         B = np.zeros(shape=(self.A, self.K, self.M), dtype=self.dtype)
         WT = np.zeros(shape=(self.A, self.K), dtype=self.dtype)
         PT = np.zeros(shape=(self.A, self.K), dtype=self.dtype)
         QT = np.zeros(shape=(self.A, self.M), dtype=self.dtype)
         RT = np.zeros(shape=(self.A, self.K), dtype=self.dtype)
         W = WT.T
         P = PT.T
         Q = QT.T
         R = RT.T
+
+        validation_size = validation_indices.size
         if self.algorithm == 1:
-            TT = np.zeros(
-                shape=(self.A, self.N - np.sum(validation_indices)), dtype=self.dtype
-            )
+            TT = np.zeros(shape=(self.A, self.N - validation_size), dtype=self.dtype)
             T = TT.T
 
         # Extract training XTY
         validation_X = self.X[validation_indices]
         validation_Y = self.Y[validation_indices]
         if self.center:
-            validation_size = np.einsum("i->", validation_indices, dtype=int)
             training_size = self.N - validation_size
             N_total_over_N_train = self.N / training_size
             N_val_over_N_train = validation_size / training_size
             training_X_mean = (
                 N_total_over_N_train * self.X_mean
                 - N_val_over_N_train * np.mean(validation_X, axis=0, keepdims=True)
             )
@@ -196,15 +267,18 @@
             training_XTY = training_XTY - training_size * (
                 training_X_mean.T @ training_Y_mean
             )
             if self.scale:
                 # Apply the training set scaling
                 training_XTY = training_XTY / (training_X_std.T @ training_Y_std)
         if self.algorithm == 1:
-            training_X = self.X[~validation_indices]
+            training_indices = np.setdiff1d(self.all_indices,
+                                            validation_indices,
+                                            assume_unique=True)
+            training_X = self.X[training_indices]
             if self.center:
                 # Apply the training set centering
                 training_X = training_X - training_X_mean
                 if self.scale:
                     # Apply the training set scaling
                     training_X = training_X / training_X_std
         else:
@@ -221,40 +295,34 @@
                     training_XTX = training_XTX / (training_X_std.T @ training_X_std)
 
         for i in range(self.A):
             # Step 2
             if self.M == 1:
                 norm = la.norm(training_XTY, ord=2)
                 if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                    warnings.warn(
-                        f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                    )
+                    self._weight_warning(i)
                     break
                 w = training_XTY / norm
             else:
                 if self.M < self.K:
                     training_XTYTtraining_XTY = training_XTY.T @ training_XTY
                     eig_vals, eig_vecs = la.eigh(training_XTYTtraining_XTY)
                     q = eig_vecs[:, -1:]
                     w = training_XTY @ q
                     norm = la.norm(w)
                     if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                        warnings.warn(
-                            f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                        )
+                        self._weight_warning(i)
                         break
                     w = w / norm
                 else:
                     training_XTYYTX = training_XTY @ training_XTY.T
                     eig_vals, eig_vecs = la.eigh(training_XTYYTX)
                     norm = eig_vals[-1]
                     if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                        warnings.warn(
-                            f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                        )
+                        self._weight_warning(i)
                         break
                     w = eig_vecs[:, -1:]
             WT[i] = w.squeeze()
 
             # Step 3
             r = np.copy(w)
             for j in range(i):
@@ -295,95 +363,113 @@
                 R,
                 T,
                 training_X_mean,
                 training_Y_mean,
                 training_X_std,
                 training_Y_std,
             )
-        else:
-            return (
-                B,
-                W,
-                P,
-                Q,
-                R,
-                training_X_mean,
-                training_Y_mean,
-                training_X_std,
-                training_Y_std,
-            )
+        return (
+            B,
+            W,
+            P,
+            Q,
+            R,
+            training_X_mean,
+            training_Y_mean,
+            training_X_std,
+            training_Y_std,
+        )
 
     def _stateless_predict(
         self,
-        indices: npt.NDArray[np.float_],
+        indices: npt.NDArray[np.int_],
         B: npt.NDArray[np.float_],
         training_X_mean: npt.NDArray[np.float_],
         training_Y_mean: npt.NDArray[np.float_],
         training_X_std: npt.NDArray[np.float_],
         training_Y_std: npt.NDArray[np.float_],
         n_components: Union[None, int] = None,
     ) -> npt.NDArray[np.float_]:
         """
-        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using `n_components` components. If `n_components` is None, then predictions are returned for all number of components.
+        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using
+        `n_components` components. If `n_components` is None, then predictions are
+        returned for all number of components.
 
         Parameters
         ----------
-        indices : Array of shape (N,)
-            Boolean array defining indices into X and Y corresponding to samples on which to predict.
+        indices : Array of shape (N_val,)
+            Integer array defining indices into X and Y corresponding to samples on
+            which to predict.
 
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         training_X_mean : Array of shape (1, K)
-            Mean row of training X. If self.center is False, then this should be an array of zeros.
+            Mean row of training X. If self.center is False, then this should be an
+            array of zeros.
 
         training_Y_mean : Array of shape (1, M)
-            Mean row of training Y. If self.center is False, then this should be an array of zeros.
+            Mean row of training Y. If self.center is False, then this should be an
+            array of zeros.
 
         training_X_std : Array of shape (1, K)
-            Sample standard deviation row of training X. If self.scale is False, then this should be an array of ones. Any zero standard deviations should be replaced with ones.
+            Sample standard deviation row of training X. If self.scale is False, then
+            this should be an array of ones. Any zero standard deviations should be
+            replaced with ones.
 
         training_Y_std : Array of shape (1, M)
-            Sample standard deviation row of training Y. If self.scale is False, then this should be an array of ones. Any zero standard deviations should be replaced with ones.
+            Sample standard deviation row of training Y. If self.scale is False, then
+            this should be an array of ones. Any zero standard deviations should be
+            replaced with ones.
 
         n_components : int or None, optional
-            Number of components in the PLS model. If None, then all number of components are used.
+            Number of components in the PLS model. If None, then all number of
+            components are used.
 
         Returns
         -------
         Y_pred : Array of shape (N_pred, M) or (A, N_pred, M)
-            If `n_components` is an int, then an array of shape (N_pred, M) with the predictions for that specific number of components is used. If `n_components` is None, returns a prediction for each number of components up to `A`.
+            If `n_components` is an int, then an array of shape (N_pred, M) with the
+            predictions for that specific number of components is used. If
+            `n_components` is None, returns a prediction for each number of components
+            up to `A`.
         """
 
         predictor_variables = self.X[indices]
         # Apply the potential training set centering
         predictor_variables = (predictor_variables - training_X_mean) / training_X_std
         if n_components is None:
             Y_pred = predictor_variables @ B
         else:
             Y_pred = predictor_variables @ B[n_components - 1]
         # Add the potential training set bias
         return Y_pred * training_Y_std + training_Y_mean
 
     def _stateless_fit_predict_eval(
         self,
-        validation_indices: npt.NDArray[np.float_],
+        validation_indices: npt.NDArray[np.int_],
         metric_function: Callable[
             [npt.NDArray[np.float_], npt.NDArray[np.float_]], Any
         ],
     ) -> Any:
         """
-        Fits Improved Kernel PLS Algorithm #1 or #2 on `X` or `XTX`, `XTY` and `Y` using `A` components, predicts on `X` and evaluates predictions using `metric_function`. The fit is performed on the training set defined by `validation_indices`. The prediction is performed on the validation set defined by `validation_indices`.
+        Fits Improved Kernel PLS Algorithm #1 or #2 on `X` or `XTX`, `XTY` and `Y`
+        using `A` components, predicts on `X` and evaluates predictions using
+        `metric_function`. The fit is performed on the training set defined by
+        all samples not in `validation_indices`. The prediction is performed on the
+        validation set defined by all samples in `validation_indices`.
 
         Parameters
         ----------
-        validation_indices : Array of shape (N,)
-            Boolean array defining indices into X and Y corresponding to validation samples.
+        validation_indices : Array of shape (N_val,)
+            Integer array defining indices into X and Y corresponding to validation
+            samples.
 
-        metric_function : Callable receiving arrays `Y_true` and `Y_pred` and returning Any
+        metric_function : Callable receiving arrays `Y_true` and `Y_pred` and returning
+        Any
 
         Returns
         -------
         metric : Any
             The result of evaluating `metric_function` on the validation set.
         """
         matrices = self._stateless_fit(validation_indices)
@@ -398,77 +484,120 @@
             training_X_mean,
             training_Y_mean,
             training_X_std,
             training_Y_std,
         )
         return metric_function(self.Y[validation_indices], Y_pred)
 
+    def _generate_validation_indices_list(
+        self, cv_splits: Iterable[Hashable]
+    ) -> list[npt.NDArray[np.int_]]:
+        """
+        Generates a list of validation indices for each fold in `cv_splits`.
+
+        Parameters
+        ----------
+        cv_splits : Iterable of Hashable with N elements
+            An iterable defining cross-validation splits. Each unique value in
+            `cv_splits` corresponds to a different fold.
+
+        Returns
+        -------
+        validation_indices_list : list of array of int
+            A list of validation indices for each fold.
+        """
+        index_dict = defaultdict(list)
+        for i, num in enumerate(cv_splits):
+            index_dict[num].append(i)
+        validation_indices_list = list(index_dict.values())
+        return [np.asarray(indices) for indices in validation_indices_list]
+
     def cross_validate(
         self,
         X: npt.ArrayLike,
         Y: npt.ArrayLike,
         A: int,
-        cv_splits: npt.ArrayLike,
+        cv_splits: Iterable[Hashable],
         metric_function: Callable[[npt.ArrayLike, npt.ArrayLike], Any],
         n_jobs=-1,
         verbose=10,
     ) -> list[Any]:
         """
-        Cross-validates the PLS model using `cv_splits` splits on `X` and `Y` with `n_components` components evaluating results with `metric_function`.
+        Cross-validates the PLS model using `cv_splits` splits on `X` and `Y` with
+        `n_components` components evaluating results with `metric_function`.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         Y : Array of shape (N, M) or (N,)
             Target variables.
 
         A : int
             Number of components in the PLS model.
 
-        cv_splits : Array of shape (N,)
-            An array defining cross-validation splits. Each unique value in `cv_splits` corresponds to a different fold.
-
-        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning Any
-            Computes a metric based on true values `Y_test` and predicted values `Y_pred`. `Y_pred` contains a prediction for all `A` components.
+        cv_splits : Iterable of Hashable with N elements
+            An iterable defining cross-validation splits. Each unique value in
+            `cv_splits` corresponds to a different fold.
+
+        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning
+        Any
+            Computes a metric based on true values `Y_test` and predicted values
+            `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
         mean_centering : bool, optional default=True
-            Whether to mean X and Y across the sample axis before fitting. The mean is subtracted from X and Y before fitting and added back to the predictions. This implementation ensures that no data leakage occurs between training and validation sets.
+            Whether to mean X and Y across the sample axis before fitting. The mean is
+            subtracted from X and Y before fitting and added back to the predictions.
+            This implementation ensures that no data leakage occurs between training
+            and validation sets.
 
         n_jobs : int, optional default=-1
-            Number of parallel jobs to use. A value of -1 will use the minimum of all available cores and the number of unique values in `cv_splits`.
+            Number of parallel jobs to use. A value of -1 will use the minimum of all
+            available cores and the number of unique values in `cv_splits`.
 
         verbose : int, optional default=10
             Controls verbosity of parallel jobs.
 
         Returns
         -------
         metrics : list of Any
             A list of the results of evaluating `metric_function` on each fold.
+
+        Notes:
+        ------
+        The order of cross-validation folds is determined by the order of the unique
+        values in `cv_splits`. `metrics` will be sorted in the same order.
         """
 
         self.X = np.asarray(X, dtype=self.dtype)
         self.Y = np.asarray(Y, dtype=self.dtype)
         if self.Y.ndim == 1:
             self.Y = self.Y.reshape(-1, 1)
         self.A = A
         self.N, self.K = X.shape
         self.M = self.Y.shape[1]
-        unique_splits = np.unique(cv_splits)
+        validation_indices_list = self._generate_validation_indices_list(cv_splits)
+        num_splits = len(validation_indices_list)
+
+        if self.algorithm == 1:
+            self.all_indices = np.arange(self.N, dtype=int)
 
         if n_jobs == -1:
-            n_jobs = min(joblib.cpu_count(), unique_splits.size)
+            n_jobs = min(joblib.cpu_count(), num_splits)
 
         print(
-            f"Cross-validating Improved Kernel PLS Algorithm {self.algorithm} with {A} components on {len(unique_splits)} unique splits using {n_jobs} parallel processes."
+            f"Cross-validating Improved Kernel PLS Algorithm {self.algorithm} with {A}"
+            f" components on {num_splits} unique splits using {n_jobs} "
+            f"parallel processes."
         )
 
         if self.center:
-            # We can compute these once for the entire dataset and subtract the validation parts during cross-validation.
+            # We can compute these once for the entire dataset and subtract the
+            # validation parts during cross-validation.
             self.X_mean = np.mean(self.X, axis=0, keepdims=True)
             self.Y_mean = np.mean(self.Y, axis=0, keepdims=True)
             if self.scale:
                 self.sum_X = np.expand_dims(np.einsum("ij->j", self.X), axis=0)
                 self.sum_Y = np.expand_dims(np.einsum("ij->j", self.Y), axis=0)
                 self.sum_sq_X = np.expand_dims(
                     np.einsum("ij,ij->j", self.X, self.X), axis=0
@@ -485,16 +614,21 @@
         if self.algorithm == 2:
             if verbose > 0:
                 print("Computing total XTX...")
             self.XTX = self.X.T @ self.X
             if verbose > 0:
                 print("Done!")
 
-        def worker(split):
-            validation_indices = cv_splits == split
-            return self._stateless_fit_predict_eval(validation_indices, metric_function)
+        def worker(validation_indices: npt.NDArray[np.int_],
+                   metric_function: Callable[[npt.ArrayLike, npt.ArrayLike], Any]
+                   ) -> Any:
+            return self._stateless_fit_predict_eval(
+                    validation_indices,
+                    metric_function
+                   )
 
         metrics = Parallel(n_jobs=n_jobs, verbose=verbose)(
-            delayed(worker)(split) for split in unique_splits
+            delayed(worker)(validation_indices, metric_function)
+            for validation_indices in validation_indices_list
         )
 
         return metrics
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/ikpls/jax_ikpls_alg_1.py` & `ikpls-1.2.0/ikpls/jax_ikpls_alg_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,67 @@
+"""
+Contains the PLS Class which implements partial least-squares regression using Improved
+Kernel PLS Algorithm #1 by Dayal and MacGregor:
+https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+
+The class is implemented using JAX for end-to-end differentiability. Additionally, JAX
+allows CPU, GPU, and TPU execution.
+
+Author: Ole-Christian Galbo Engstrøm
+E-mail: ole.e@di.ku.dk
+"""
+
 from functools import partial
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
-from jax.experimental import host_callback
 from jax.typing import ArrayLike, DTypeLike
 
 from ikpls.jax_ikpls_base import PLSBase
 
 
 class PLS(PLSBase):
     """
-    Implements partial least-squares regression using Improved Kernel PLS Algorithm #1 by Dayal and MacGregor: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23.
+    Implements partial least-squares regression using Improved Kernel PLS Algorithm #1
+    by Dayal and MacGregor:
+    https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
     center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+        Whether to center the data before fitting. If True, then the mean of the
+        training data is subtracted from the data. If False, then the data is assumed
+        to be already centered.
 
     scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+        Whether to scale the data before fitting. If True, then the data is scaled
+        using Bessel's correction for the unbiased estimate of the sample standard
+        deviation. If False, then the data is assumed to be already scaled.
 
     copy : bool, optional, default=True
-        Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+        Whether to copy `X` and `Y` in fit before potentially applying centering and
+        scaling. If True, then the data is copied before fitting. If False, and `dtype`
+        matches the type of `X` and `Y`, then centering and scaling is done inplace,
+        modifying both arrays.
 
     dtype : DTypeLike, optional, default=jnp.float64
-        The float datatype to use in computation of the PLS algorithm. Using a lower precision than float64 will yield significantly worse results when using an increasing number of components due to propagation of numerical errors.
+        The float datatype to use in computation of the PLS algorithm. Using a lower
+        precision than float64 will yield significantly worse results when using an
+        increasing number of components due to propagation of numerical errors.
 
     reverse_differentiable: bool, optional, default=False
-        Whether to make the implementation end-to-end differentiable. The differentiable version is slightly slower. Results among the two versions are identical.
+        Whether to make the implementation end-to-end differentiable. The
+        differentiable version is slightly slower. Results among the two versions are
+        identical.
 
     verbose : bool, optional, default=False
-        If True, each sub-function will print when it will be JIT compiled. This can be useful to track if recompilation is triggered due to passing inputs with different shapes.
+        If True, each sub-function will print when it will be JIT compiled. This can be
+        useful to track if recompilation is triggered due to passing inputs with
+        different shapes.
     """
 
     def __init__(
         self,
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
@@ -48,21 +74,24 @@
             center=center,
             scale=scale,
             copy=copy,
             dtype=dtype,
             reverse_differentiable=reverse_differentiable,
             verbose=verbose,
         )
+        self.name += " #1"
+        self.T = None
 
     @partial(jax.jit, static_argnums=(0, 1, 2, 3, 4))
     def _get_initial_matrices(
         self, A: int, K: int, M: int, N: int
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Initialize the matrices and arrays needed for the PLS algorithm. This method is part of the PLS fitting process.
+        Initialize the matrices and arrays needed for the PLS algorithm. This method is
+        part of the PLS fitting process.
 
         Parameters
         ----------
         A : int
             Number of components in the PLS model.
 
         K : int
@@ -175,15 +204,16 @@
         M: int,
         K: int,
         P: jax.Array,
         R: jax.Array,
         reverse_differentiable: bool,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Execute the main loop body of Improved Kernel PLS Algorithm #1. This function performs various steps of the PLS algorithm for each component.
+        Execute the main loop body of Improved Kernel PLS Algorithm #1. This function
+        performs various steps of the PLS algorithm for each component.
 
         Parameters
         ----------
         A : int
             Number of components in the PLS model.
 
         i : int
@@ -230,21 +260,22 @@
         t : Array of shape (N, 1)
             Updated intermediate result used in the PLS algorithm.
 
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
         """
         if self.verbose:
             print(f"_main_loop_body for {self.name} will be JIT compiled...")
         # step 2
         w, norm = self._step_2(XTY, M, K)
-        host_callback.id_tap(self._weight_warning, [i, norm])
+        jax.debug.callback(self._weight_warning, (i, norm))
         # step 3
         if reverse_differentiable:
             r = self._step_3(A, w, P, R)
         else:
             r = self._step_3(i, w, P, R)
         # step 4
         tTt, p, q, t = self._step_4(X, XTY, r)
@@ -302,19 +333,21 @@
         Returns
         -------
         None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        stateless_fit : Performs the same operation but returns the output matrices instead of storing them in the class instance.
+        stateless_fit : Performs the same operation but returns the output matrices
+        instead of storing them in the class instance.
         """
         self.B, W, P, Q, R, T, self.X_mean, self.Y_mean, self.X_std, self.Y_std = (
             self.stateless_fit(X, Y, A, self.center, self.scale, self.copy)
         )
         self.W = W.T
         self.P = P.T
         self.Q = Q.T
@@ -328,35 +361,45 @@
         Y: ArrayLike,
         A: int,
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components. Returns the internal matrices instead of storing them in the class instance.
+        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
+        Returns the internal matrices instead of storing them in the class instance.
 
         Parameters
         ----------
         X : Array of shape (N, K)
-            Predictor variables. Its dtype will be converted to float64 for reliable results.
+            Predictor variables. Its dtype will be converted to float64 for reliable
+            results.
 
         Y : Array of shape (N, M) or (N,)
-            Response variables. Its dtype will be converted to float64 for reliable results.
+            Response variables. Its dtype will be converted to float64 for reliable
+            results.
 
         A : int
             Number of components in the PLS model.
 
         center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+            Whether to center the data before fitting. If True, then the mean of the
+            training data is subtracted from the data. If False, then the data is
+            assumed to be already centered.
 
         scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+            Whether to scale the data before fitting. If True, then the data is scaled
+            using Bessel's correction for the unbiased estimate of the sample standard
+            deviation. If False, then the data is assumed to be already scaled.
 
         copy : bool, optional, default=True
-            Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+            Whether to copy `X` and `Y` in fit before potentially applying centering
+            and scaling. If True, then the data is copied before fitting. If False, and
+            `dtype` matches the type of `X` and `Y`, then centering and scaling is done
+            inplace, modifying both arrays.
 
         Returns
         -------
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         W : Array of shape (A, K)
@@ -385,23 +428,26 @@
 
         Y_std : Array of shape (1, M) or None
             Sample standard deviation of Y. If scaling is not performed, this is None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        fit : Performs the same operation but stores the output matrices in the class instance instead of returning them.
+        fit : Performs the same operation but stores the output matrices in the class
+        instance instead of returning them.
 
         Notes
         -----
-        For optimization purposes, the internal representation of all matrices (except B) is transposed from the usual representation.
+        For optimization purposes, the internal representation of all matrices
+        (except B) is transposed from the usual representation.
         """
 
         if self.verbose:
             print(f"stateless_fit for {self.name} will be JIT compiled...")
 
         X, Y = self._initialize_input_matrices(X, Y)
         X, Y, X_mean, Y_mean, X_std, Y_std = self._center_scale_input_matrices(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/ikpls/jax_ikpls_alg_2.py` & `ikpls-1.2.0/ikpls/jax_ikpls_alg_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,82 +1,106 @@
+"""
+Contains the PLS Class which implements partial least-squares regression using Improved
+Kernel PLS Algorithm #2 by Dayal and MacGregor:
+https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+
+The class is implemented using JAX for end-to-end differentiability. Additionally, JAX
+allows CPU, GPU, and TPU execution.
+
+Author: Ole-Christian Galbo Engstrøm
+E-mail: ole.e@di.ku.dk
+"""
+
 from functools import partial
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
-from jax.experimental import host_callback
 from jax.typing import ArrayLike, DTypeLike
 
 from ikpls.jax_ikpls_base import PLSBase
 
 
 class PLS(PLSBase):
     """
-    Implements partial least-squares regression using Improved Kernel PLS Algorithm #2 by Dayal and MacGregor: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23.
+    Implements partial least-squares regression using Improved Kernel PLS Algorithm #2
+    by Dayal and MacGregor:
+    https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23.
 
     Parameters
     ----------
     center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+        Whether to center the data before fitting. If True, then the mean of the
+        training data is subtracted from the data. If False, then the data is assumed
+        to be already centered.
 
     scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+        Whether to scale the data before fitting. If True, then the data is scaled
+        using Bessel's correction for the unbiased estimate of the sample standard
+        deviation. If False, then the data is assumed to be already scaled.
 
     copy : bool, optional, default=True
-        Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+        Whether to copy `X` and `Y` in fit before potentially applying centering and
+        scaling. If True, then the data is copied before fitting. If False, and `dtype`
+        matches the type of `X` and `Y`, then centering and scaling is done inplace,
+        modifying both arrays.
 
     dtype : DTypeLike, optional, default=jnp.float64
-        The float datatype to use in computation of the PLS algorithm. Using a lower precision than float64 will yield significantly worse results when using an increasing number of components due to propagation of numerical errors.
+        The float datatype to use in computation of the PLS algorithm. Using a lower
+        precision than float64 will yield significantly worse results when using an
+        increasing number of components due to propagation of numerical errors.
 
     reverse_differentiable: bool, optional, default=False
-        Whether to make the implementation end-to-end differentiable. The differentiable version is slightly slower. Results among the two versions are identical.
+        Whether to make the implementation end-to-end differentiable. The
+        differentiable version is slightly slower. Results among the two versions are
+        identical.
 
     verbose : bool, optional, default=False
-        If True, each sub-function will print when it will be JIT compiled. This can be useful to track if recompilation is triggered due to passing inputs with different shapes.
+        If True, each sub-function will print when it will be JIT compiled. This can be
+        useful to track if recompilation is triggered due to passing inputs with
+        different shapes.
     """
 
     def __init__(
         self,
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
         dtype: DTypeLike = jnp.float64,
         reverse_differentiable: bool = False,
         verbose: bool = False,
     ) -> None:
-        self.name = "Improved Kernel PLS Algorithm #2"
         super().__init__(
             center=center,
             scale=scale,
             copy=copy,
             dtype=dtype,
             reverse_differentiable=reverse_differentiable,
             verbose=verbose,
         )
+        self.name += " #2"
 
     def _get_initial_matrices(
-        self, X: ArrayLike, Y: ArrayLike, A: int
+        self, A: int, K: int, M: int
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Initialize the matrices and arrays needed for the PLS algorithm. This method is part of the PLS fitting process.
+        Initialize the matrices and arrays needed for the PLS algorithm. This method is
+        part of the PLS fitting process.
 
         Parameters
         ----------
         A : int
             Number of components in the PLS model.
 
         K : int
             Number of predictor variables.
 
         M : int
             Number of response variables.
 
-        N : int
-            Number of samples.
-
         Returns
         -------
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         W : Array of shape (A, K)
             PLS weights matrix for X.
@@ -88,15 +112,15 @@
             PLS Loadings matrix for Y.
 
         R : Array of shape (A, K)
             PLS weights matrix to compute scores T directly from original X.
         """
         if self.verbose:
             print(f"_get_initial_matrices for {self.name} will be JIT compiled...")
-        return super()._get_initial_matrices(X, Y, A)
+        return super()._get_initial_matrices(A, K, M)
 
     @partial(jax.jit, static_argnums=(0,))
     def _step_1(self, X: ArrayLike, Y: ArrayLike) -> Tuple[jax.Array, jax.Array]:
         """
         Perform the first step of Improved Kernel PLS Algorithm #2.
 
         Parameters
@@ -109,15 +133,16 @@
 
         Returns
         -------
         XTX : Array of shape (K, K)
             Product of transposed predictor variables and predictor variables.
 
         XTY : Array of shape (K, M)
-            Initial cross-covariance matrix of the predictor variables and the response variables.
+            Initial cross-covariance matrix of the predictor variables and the response
+            variables.
         """
         if self.verbose:
             print(f"_step_1 for {self.name} will be JIT compiled...")
         XT = self._compute_XT(X)
         XTX = self._compute_XTX(XT, X)
         XTY = self._compute_initial_XTY(XT, Y)
         return XTX, XTY
@@ -169,15 +194,16 @@
         M: int,
         K: int,
         P: jax.Array,
         R: jax.Array,
         reverse_differentiable: bool,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Execute the main loop body of Improved Kernel PLS Algorithm #2. This function performs various steps of the PLS algorithm for each component.
+        Execute the main loop body of Improved Kernel PLS Algorithm #2. This function
+        performs various steps of the PLS algorithm for each component.
 
         Parameters
         ----------
         A : int
             Number of components in the PLS model.
 
         i : int
@@ -221,15 +247,15 @@
         r : Array of shape (K, K)
             PLS weight vector.
         """
         if self.verbose:
             print(f"_main_loop_body for {self.name} will be JIT compiled...")
         # step 2
         w, norm = self._step_2(XTY, M, K)
-        host_callback.id_tap(self._weight_warning, [i, norm])
+        jax.debug.callback(self._weight_warning, (i, norm))
         # step 3
         if reverse_differentiable:
             r = self._step_3(A, w, P, R)
         else:
             r = self._step_3(i, w, P, R)
         # step 4
         tTt, p, q = self._step_4(XTX, XTY, r)
@@ -284,19 +310,21 @@
         Returns
         -------
         None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        stateless_fit : Performs the same operation but returns the output matrices instead of storing them in the class instance.
+        stateless_fit : Performs the same operation but returns the output matrices
+        instead of storing them in the class instance.
         """
         self.B, W, P, Q, R, self.X_mean, self.Y_mean, self.X_std, self.Y_std = (
             self.stateless_fit(X, Y, A, self.center, self.scale, self.copy)
         )
         self.W = W.T
         self.P = P.T
         self.Q = Q.T
@@ -309,23 +337,26 @@
         Y: ArrayLike,
         A: int,
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components. Returns the internal matrices instead of storing them in the class instance.
+        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
+        Returns the internal matrices instead of storing them in the class instance.
 
         Parameters
         ----------
         X : Array of shape (N, K)
-            Predictor variables. Its dtype will be converted to float64 for reliable results.
+            Predictor variables. Its dtype will be converted to float64 for reliable
+            results.
 
         Y : Array of shape (N, M) or (N,)
-            Response variables. Its dtype will be converted to float64 for reliable results.
+            Response variables. Its dtype will be converted to float64 for reliable
+            results.
 
         A : int
             Number of components in the PLS model.
 
         Returns
         -------
         B : Array of shape (A, K, M)
@@ -354,34 +385,37 @@
 
         Y_std : Array of shape (1, M) or None
             Sample standard deviation of Y. If scaling is not performed, this is None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        fit : Performs the same operation but stores the output matrices in the class instance instead of returning them.
+        fit : Performs the same operation but stores the output matrices in the class
+        instance instead of returning them.
 
         Notes
         -----
-        For optimization purposes, the internal representation of all matrices (except B) is transposed from the usual representation.
+        For optimization purposes, the internal representation of all matrices
+        (except B) is transposed from the usual representation.
         """
         if self.verbose:
             print(f"stateless_fit for {self.name} will be JIT compiled...")
 
         X, Y = self._initialize_input_matrices(X, Y)
         X, Y, X_mean, Y_mean, X_std, Y_std = self._center_scale_input_matrices(
             X, Y, center, scale, copy
         )
 
         # Get shapes
-        N, K = X.shape
+        _N, K = X.shape
         M = Y.shape[1]
 
         # Initialize matrices
         B, W, P, Q, R = self._get_initial_matrices(A, K, M)
 
         # step 1
         XTX, XTY = self._step_1(X, Y)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/ikpls/jax_ikpls_base.py` & `ikpls-1.2.0/ikpls/jax_ikpls_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,77 @@
+"""
+Implements an abstract class for partial least-squares regression using Improved Kernel
+PLS by Dayal and MacGregor.
+
+Implementations of concrete classes exist for both Improved Kernel PLS Algorithm #1
+and Improved Kernel PLS Algorithm #2.
+
+For more details, refer to the paper: 
+"Improved Kernel Partial Least Squares Regression" by Dayal and MacGregor.
+
+Author: Ole-Christian Galbo Engstrøm
+E-mail: ole.e@di.ku.dk
+"""
+
 import abc
 import warnings
 from collections.abc import Callable
 from functools import partial
 from typing import Any, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax.numpy.linalg as jla
 import numpy as np
 from jax.typing import ArrayLike, DTypeLike
+from numpy import typing as npt
 from tqdm import tqdm
 
 
 class PLSBase(abc.ABC):
     """
-    Implements an abstract class for partial least-squares regression using Improved Kernel PLS by Dayal and MacGregor: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23.
+    Implements an abstract class for partial least-squares regression using Improved
+    Kernel PLS by Dayal and MacGregor:
+    https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
-    Implementations of concrete classes exist for both Improved Kernel PLS Algorithm #1 and Improved Kernel PLS Algorithm #2.
+    Implementations of concrete classes exist for both Improved Kernel PLS Algorithm #1
+    and Improved Kernel PLS Algorithm #2.
 
     Parameters
     ----------
     center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+        Whether to center the data before fitting. If True, then the mean of the
+        training data is subtracted from the data. If False, then the data is assumed
+        to be already centered.
 
     scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+        Whether to scale the data before fitting. If True, then the data is scaled
+        using Bessel's correction for the unbiased estimate of the sample standard
+        deviation. If False, then the data is assumed to be already scaled.
 
     copy : bool, optional, default=True
-        Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+        Whether to copy `X` and `Y` in fit before potentially applying centering and
+        scaling. If True, then the data is copied before fitting. If False, and `dtype`
+        matches the type of `X` and `Y`, then centering and scaling is done inplace,
+        modifying both arrays.
 
     dtype : jnp.float, optional, default=jnp.float64
-        The float datatype to use in computation of the PLS algorithm. Using a lower precision than float64 will yield significantly worse results when using an increasing number of components due to propagation of numerical errors.
+        The float datatype to use in computation of the PLS algorithm. Using a lower
+        precision than float64 will yield significantly worse results when using an
+        increasing number of components due to propagation of numerical errors.
 
     reverse_differentiable: bool, optional, default=False
-        Whether to make the implementation end-to-end differentiable. The differentiable version is slightly slower. Results among the two versions are identical.
+        Whether to make the implementation end-to-end differentiable. The
+        differentiable version is slightly slower. Results among the two versions are
+        identical.
 
     verbose : bool, optional, default=False
-        If True, each sub-function will print when it will be JIT compiled. This can be useful to track if recompilation is triggered due to passing inputs with different shapes.
+        If True, each sub-function will print when it will be JIT compiled. This can be
+        useful to track if recompilation is triggered due to passing inputs with
+        different shapes.
     """
 
     def __init__(
         self,
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
@@ -50,41 +81,54 @@
     ) -> None:
         self.center = center
         self.scale = scale
         self.copy = copy
         self.dtype = dtype
         self.reverse_differentiable = reverse_differentiable
         self.verbose = verbose
+        self.name = "Improved Kernel PLS Algorithm"
+        self.B = None
+        self.W = None
+        self.P = None
+        self.Q = None
+        self.R = None
+        self.X_mean = None
+        self.Y_mean = None
+        self.X_std = None
+        self.Y_std = None
 
-    def _weight_warning(self, arg, *args):
+    def _weight_warning(self, arg: Tuple[npt.NDArray[np.int_], npt.NDArray[np.float_]]):
         """
         Display a warning message if the weight is close to zero.
 
         Parameters
         ----------
         arg : tuple
             A tuple containing the component index and the weight norm.
 
-        *args : Any
-            Placeholder for unused arguments.
-
         Warns
         -----
         UserWarning.
-            If the weight norm is below machine epsilon, a warning message is displayed.
+            If the weight norm is below machine epsilon, a warning message is
+            displayed.
 
         Notes
         -----
-        This method issues a warning if the weight becomes close to zero during the PLS algorithm. It provides a hint about potential instability in results with a higher number of components.
+        This method issues a warning if the weight becomes close to zero during the PLS
+        algorithm. It provides a hint about potential instability in results with a
+        higher number of components.
         """
         i, norm = arg
         if np.isclose(norm, 0, atol=np.finfo(self.dtype).eps, rtol=0):
-            warnings.warn(
-                f"Weight is close to zero. Results with A = {i} component(s) or higher may be unstable."
-            )
+            with warnings.catch_warnings():
+                warnings.simplefilter("always", UserWarning)
+                warnings.warn(
+                    f"Weight is close to zero. Results with A = {i} component(s) or "
+                    "higher may be unstable."
+                )
 
     @partial(jax.jit, static_argnums=0)
     def _compute_regression_coefficients(
         self, b_last: jax.Array, r: jax.Array, q: jax.Array
     ) -> jax.Array:
         """
         Compute the regression coefficients in the PLS algorithm.
@@ -103,15 +147,17 @@
         Returns
         -------
         b : Array of shape (K, M)
             The updated regression coefficient matrix for the current component.
 
         Notes
         -----
-        This method computes the regression coefficients matrix for the current component in the PLS algorithm, incorporating the orthogonal weight vector and loadings vector.
+        This method computes the regression coefficients matrix for the current
+        component in the PLS algorithm, incorporating the orthogonal weight vector and
+        loadings vector.
         """
         b = b_last + r @ q.T
         return b
 
     @partial(jax.jit, static_argnums=0)
     def _initialize_input_matrices(self, X: jax.Array, Y: jax.Array):
         """
@@ -279,15 +325,17 @@
             PLS Loadings matrix for Y.
 
         R : Array of shape (A, K)
             PLS weights matrix to compute scores T directly from the original X.
 
         Notes
         -----
-        This abstract method is responsible for initializing various matrices used in the PLS algorithm, including regression coefficients, weights, loadings, and orthogonal weights.
+        This abstract method is responsible for initializing various matrices used in
+        the PLS algorithm, including regression coefficients, weights, loadings, and
+        orthogonal weights.
         """
         B = jnp.zeros(shape=(A, K, M), dtype=self.dtype)
         W = jnp.zeros(shape=(A, K), dtype=self.dtype)
         P = jnp.zeros(shape=(A, K), dtype=self.dtype)
         Q = jnp.zeros(shape=(A, M), dtype=self.dtype)
         R = jnp.zeros(shape=(A, K), dtype=self.dtype)
         return B, W, P, Q, R
@@ -305,46 +353,51 @@
         Returns
         -------
         XT : Array of shape (K, N)
             Transposed predictor variables matrix.
 
         Notes
         -----
-        This method calculates the transposed predictor variables matrix from the original predictor variables matrix.
+        This method calculates the transposed predictor variables matrix from the
+        original predictor variables matrix.
         """
         return X.T
 
     @partial(jax.jit, static_argnums=0)
     def _compute_initial_XTY(self, XT: jax.Array, Y: jax.Array) -> jax.Array:
         """
-        Compute the initial cross-covariance matrix of the predictor variables and the response variables.
+        Compute the initial cross-covariance matrix of the predictor variables and the
+        response variables.
 
         Parameters
         ----------
         XT : Array of shape (K, N)
             Transposed predictor variables matrix.
 
         Y : Array of shape (N, M)
             Response variables matrix.
 
         Returns
         -------
         XTY : Array of shape (K, M)
-            Initial cross-covariance matrix of the predictor variables and the response variables.
+            Initial cross-covariance matrix of the predictor variables and the response
+            variables.
 
         Notes
         -----
-        This method calculates the initial cross-covariance matrix of the predictor variables and the response variables.
+        This method calculates the initial cross-covariance matrix of the predictor
+        variables and the response variables.
         """
         return XT @ Y
 
     @partial(jax.jit, static_argnums=0)
     def _compute_XTX(self, XT: jax.Array, X: jax.Array) -> jax.Array:
         """
-        Compute the product of the transposed predictor variables matrix and the predictor variables matrix.
+        Compute the product of the transposed predictor variables matrix and the
+        predictor variables matrix.
 
         Parameters
         ----------
         XT : Array of shape (K, N)
             Transposed predictor variables matrix.
 
         X : Array of shape (N, K)
@@ -353,48 +406,53 @@
         Returns
         -------
         XTX : Array of shape (K, K)
             Product of transposed predictor variables and predictor variables.
 
         Notes
         -----
-        This method calculates the product of the transposed predictor variables matrix and the predictor variables matrix.
+        This method calculates the product of the transposed predictor variables matrix
+        and the predictor variables matrix.
         """
         return XT @ X
 
     @abc.abstractmethod
     @partial(jax.jit, static_argnums=0)
-    def _step_1(self):
+    def _step_1(self, X: jax.Array, Y: jax.Array):
         """
-        Abstract method representing the first step in the PLS algorithm. This step should be implemented in concrete PLS classes.
+        Abstract method representing the first step in the PLS algorithm. This step
+        should be implemented in concrete PLS classes.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         Notes
         -----
-        This method represents the first step of the PLS algorithm and should be implemented in concrete PLS classes.
+        This method represents the first step of the PLS algorithm and should be
+        implemented in concrete PLS classes.
         """
 
     @partial(jax.jit, static_argnums=(0, 2, 3))
     def _step_2(
         self, XTY: jax.Array, M: jax.Array, K: jax.Array
     ) -> Tuple[jax.Array, DTypeLike]:
         """
-        The second step of the PLS algorithm. Computes the next weight vector and the associated norm.
+        The second step of the PLS algorithm. Computes the next weight vector and the
+        associated norm.
 
         Parameters
         ----------
         XTY : Array of shape (K, M)
-            The cross-covariance matrix of the predictor variables and the response variables.
+            The cross-covariance matrix of the predictor variables and the response
+            variables.
 
         M : int
             Number of response variables.
 
         K : int
             Number of predictor variables.
 
@@ -404,15 +462,16 @@
             The next weight vector for the PLS algorithm.
 
         norm : float
             The l2 norm of the weight vector `w`.
 
         Notes
         -----
-        This method computes the next weight vector `w` for the PLS algorithm and its associated norm. It is an essential step in the PLS algorithm.
+        This method computes the next weight vector `w` for the PLS algorithm and its
+        associated norm. It is an essential step in the PLS algorithm.
         """
         if self.verbose:
             print(f"_step_2 for {self.name} will be JIT compiled...")
         if M == 1:
             norm = jla.norm(XTY)
             w = XTY / norm
         else:
@@ -444,37 +503,41 @@
         w : Array of shape (K, 1)
             The current weight vector.
 
         P : Array of shape (A, K)
             The loadings matrix for the predictor variables.
 
         R : Array of shape (A, K)
-            The weights matrix to compute scores `T` directly from the original predictor variables.
+            The weights matrix to compute scores `T` directly from the original
+            predictor variables.
 
         Returns
         -------
         r : Array of shape (K, 1)
             The orthogonal weight vector for the current component.
 
         Notes
         -----
-        This method computes the orthogonal weight vector `r` for the current component in the PLS algorithm. It is a key step for calculating the loadings and weights matrices.
+        This method computes the orthogonal weight vector `r` for the current component
+        in the PLS algorithm. It is a key step for calculating the loadings and weights
+        matrices.
         """
         if self.verbose:
             print(f"_step_3 for {self.name} will be JIT compiled...")
         r = jnp.copy(w)
         r, P, w, R = jax.lax.fori_loop(0, i, self._step_3_body, (r, P, w, R))
         return r
 
     @partial(jax.jit, static_argnums=0)
     def _step_3_body(
         self, j: int, carry: Tuple[jax.Array, jax.Array, jax.Array, jax.Array]
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array]:
         """
-        The body of the third step of the PLS algorithm. Iteratively computes orthogonal weight vectors.
+        The body of the third step of the PLS algorithm. Iteratively computes
+        orthogonal weight vectors.
 
         Parameters
         ----------
         j : int
             The current iteration index.
 
         carry : Tuple of arrays
@@ -483,66 +546,71 @@
         Returns
         -------
         carry : Tuple of arrays
             Updated weight vectors and matrices used in the PLS algorithm.
 
         Notes
         -----
-        This method is the body of the third step of the PLS algorithm and iteratively computes orthogonal weight vectors used in the PLS algorithm.
+        This method is the body of the third step of the PLS algorithm and iteratively
+        computes orthogonal weight vectors used in the PLS algorithm.
         """
         if self.verbose:
             print(f"_step_3_body for {self.name} will be JIT compiled...")
         r, P, w, R = carry
         r = r - P[j].reshape(-1, 1).T @ w * R[j].reshape(-1, 1)
         return r, P, w, R
 
     @abc.abstractmethod
     @partial(jax.jit, static_argnums=0)
     def _step_4(self):
         """
-        Abstract method representing the fourth step in the PLS algorithm. This step should be implemented in concrete PLS classes.
+        Abstract method representing the fourth step in the PLS algorithm. This step
+        should be implemented in concrete PLS classes.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         Notes
         -----
-        This method represents the fourth step of the PLS algorithm and should be implemented in concrete PLS classes.
+        This method represents the fourth step of the PLS algorithm and should be
+        implemented in concrete PLS classes.
         """
 
     @partial(jax.jit, static_argnums=0)
     def _step_5(
         self, XTY: jax.Array, p: jax.Array, q: jax.Array, tTt: jax.Array
     ) -> jax.Array:
         if self.verbose:
             print(f"_step_5 for {self.name} will be JIT compiled...")
         return XTY - (p @ q.T) * tTt
 
     @abc.abstractmethod
     @partial(jax.jit, static_argnums=0)
     def _main_loop_body(self):
         """
-        Abstract method representing the main loop body in the PLS algorithm. This method should be implemented in concrete PLS classes.
+        Abstract method representing the main loop body in the PLS algorithm. This
+        method should be implemented in concrete PLS classes.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         Notes
         -----
-        This method represents the main loop body of the PLS algorithm and should be implemented in concrete PLS classes.
+        This method represents the main loop body of the PLS algorithm and should be
+        implemented in concrete PLS classes.
         """
 
     @abc.abstractmethod
     @partial(jax.jit, static_argnums=(0, 3))
     def stateless_fit(
         self,
         X: ArrayLike,
@@ -552,35 +620,43 @@
         scale: bool = True,
         copy: bool = True,
     ) -> Union[
         Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array],
         Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array],
     ]:
         """
-        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components. Returns the internal matrices instead of storing them in the class instance.
+        Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
+        Returns the internal matrices instead of storing them in the class instance.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         Y : Array of shape (N, M) or (N,)
             Response variables.
 
         A : int
             Number of components in the PLS model.
 
         center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+            Whether to center the data before fitting. If True, then the mean of the
+            training data is subtracted from the data. If False, then the data is
+            assumed to be already centered.
 
         scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+            Whether to scale the data before fitting. If True, then the data is scaled
+            using Bessel's correction for the unbiased estimate of the sample standard
+            deviation. If False, then the data is assumed to be already scaled.
 
         copy : bool, optional, default=True
-            Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+            Whether to copy `X` and `Y` in fit before potentially applying centering
+            and scaling. If True, then the data is copied before fitting. If False, and
+            `dtype` matches the type of `X` and `Y`, then centering and scaling is done
+            inplace, modifying both arrays.
 
         Returns
         -------
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         W : Array of shape (A, K)
@@ -601,31 +677,36 @@
         X_mean : Array of shape (1, K) or None
             Mean of the predictor variables `center` is True, otherwise None.
 
         Y_mean : Array of shape (1, M) or None
             Mean of the response variables `center` is True, otherwise None.
 
         X_std : Array of shape (1, K) or None
-            Sample standard deviation of the predictor variables `scale` is True, otherwise None.
+            Sample standard deviation of the predictor variables `scale` is True,
+            otherwise None.
 
         Y_std : Array of shape (1, M) or None
-            Sample standard deviation of the response variables `scale` is True, otherwise None.
+            Sample standard deviation of the response variables `scale` is True,
+            otherwise None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        fit : Performs the same operation but stores the output matrices in the class instance instead of returning them.
+        fit : Performs the same operation but stores the output matrices in the class
+        instance instead of returning them.
 
         Notes
         -----
-        For optimization purposes, the internal representation of all matrices (except B) is transposed from the usual representation.
+        For optimization purposes, the internal representation of all matrices
+        (except B) is transposed from the usual representation.
         """
 
     @abc.abstractmethod
     def fit(self, X: ArrayLike, Y: ArrayLike, A: int) -> None:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
 
@@ -663,66 +744,80 @@
         Returns
         -------
         None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine epsilon.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine epsilon.
 
         See Also
         --------
-        stateless_fit : Performs the same operation but returns the output matrices instead of storing them in the class instance.
+        stateless_fit : Performs the same operation but returns the output matrices
+        instead of storing them in the class instance.
         """
 
     @partial(jax.jit, static_argnums=(0, 3))
     def stateless_predict(
         self,
         X: ArrayLike,
         B: jax.Array,
         n_components: Union[None, int] = None,
         X_mean: Union[None, jax.Array] = None,
         X_std: Union[None, jax.Array] = None,
         Y_mean: Union[None, jax.Array] = None,
         Y_std: Union[None, jax.Array] = None,
     ) -> jax.Array:
         """
-        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using `n_components` components. If `n_components` is None, then predictions are returned for all number of components.
+        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using
+        `n_components` components. If `n_components` is None, then predictions are
+        returned for all number of components.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         n_components : int or None, optional
-            Number of components in the PLS model. If None, then all number of components are used.
+            Number of components in the PLS model. If None, then all number of
+            components are used.
 
         X_mean : Array of shape (1, K) or None, optional, default=None
-            Mean of the predictor variables. If None, then no mean is subtracted from the predictor variables.
+            Mean of the predictor variables. If None, then no mean is subtracted from
+            the predictor variables.
 
         X_std : Array of shape (1, K) or None, optional, default=None
-            Sample standard deviation of the predictor variables. If None, then no scaling is applied to the predictor variables.
+            Sample standard deviation of the predictor variables. If None, then no
+            scaling is applied to the predictor variables.
 
         Y_mean : Array of shape (1, M) or None, optional, default=None
-            Mean of the response variables. If None, then no mean is subtracted from the response variables.
+            Mean of the response variables. If None, then no mean is subtracted from
+            the response variables.
 
         Y_std : Array of shape (1, M) or None, optional, default=None
-            Sample standard deviation of the response variables. If None, then no scaling is applied to the response variables.
+            Sample standard deviation of the response variables. If None, then no
+            scaling is applied to the response variables.
 
         Returns
         -------
         Y_pred : Array of shape (N, M) or (A, N, M)
-            If `n_components` is an int, then an array of shape (N, M) with the predictions for that specific number of components is used. If `n_components` is None, returns a prediction for each number of components up to `A`.
+            If `n_components` is an int, then an array of shape (N, M) with the
+            predictions for that specific number of components is used. If
+            `n_components` is None, returns a prediction for each number of components
+            up to `A`.
 
         See Also
         --------
-        predict : Performs the same operation but uses the class instances of `B`, `X_mean`, `X_std`, `Y_mean`, and `Y_std` instead of the ones passed as arguments.
+        predict : Performs the same operation but uses the class instances of `B`,
+        `X_mean`, `X_std`, `Y_mean`, and `Y_std` instead of the ones passed as
+        arguments.
         """
         X = jnp.asarray(X, dtype=self.dtype)
         if self.verbose:
             print(f"stateless_predict for {self.name} will be JIT compiled...")
 
         if X_mean is not None:
             X = X - X_mean
@@ -738,32 +833,40 @@
             Y_pred = Y_pred * Y_std
         if Y_mean is not None:
             Y_pred = Y_pred + Y_mean
         return Y_pred
 
     def predict(self, X: ArrayLike, n_components: Union[None, int] = None) -> jax.Array:
         """
-        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using `n_components` components. If `n_components` is None, then predictions are returned for all number of components.
+        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using
+        `n_components` components. If `n_components` is None, then predictions are
+        returned for all number of components.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         n_components : int or None, optional
-            Number of components in the PLS model. If None, then all number of components are used.
+            Number of components in the PLS model. If None, then all number of
+            components are used.
 
         Returns
         -------
         Y_pred : Array of shape (N, M) or (A, N, M)
-            If `n_components` is an int, then an array of shape (N, M) with the predictions for that specific number of components is used. If `n_components` is None, returns a prediction for each number of components up to `A`.
+            If `n_components` is an int, then an array of shape (N, M) with the
+            predictions for that specific number of components is used. If
+            `n_components` is None, returns a prediction for each number of components
+            up to `A`.
 
         See Also
         --------
-        stateless_predict : Performs the same operation but uses inputs `B`, `X_mean`, `X_std`, `Y_mean`, and `Y_std` instead of the ones stored in the class instance.
+        stateless_predict : Performs the same operation but uses inputs `B`, `X_mean`,
+        `X_std`, `Y_mean`, and `Y_std` instead of the ones stored in the class
+        instance.
         """
         return self.stateless_predict(
             X, self.B, n_components, self.X_mean, self.X_std, self.Y_mean, self.Y_std
         )
 
     @partial(jax.jit, static_argnums=(0, 3, 6, 7, 8, 9))
     def stateless_fit_predict_eval(
@@ -775,15 +878,17 @@
         Y_test: ArrayLike,
         metric_function: Callable[[jax.Array, jax.Array], Any],
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
     ) -> Any:
         """
-        Computes `B` with `stateless_fit`. Then computes `Y_pred` with `stateless_predict`. `Y_pred` is an array of shape (A, N, M). Then evaluates and returns the result of `metric_function(Y_test, Y_pred)`.
+        Computes `B` with `stateless_fit`. Then computes `Y_pred` with
+        `stateless_predict`. `Y_pred` is an array of shape (A, N, M). Then evaluates
+        and returns the result of `metric_function(Y_test, Y_pred)`.
 
         Parameters
         ----------
         X_train : Array of shape (N_train, K)
             Predictor variables.
 
         Y_train : Array of shape (N_train, M) or (N_train,)
@@ -794,35 +899,47 @@
 
         X_test : Array of shape (N_test, K)
             Predictor variables.
 
         Y_test : Array of shape (N_test, M) or (N_test,)
             Response variables.
 
-        metric_function : Callable receiving arrays `Y_test` of shape (N, M) and `Y_pred` (A, N, M) and returns Any
-            Computes a metric based on true values `Y_test` and predicted values `Y_pred`. `Y_pred` contains a prediction for all `A` components.
+        metric_function : Callable receiving arrays `Y_test` of shape (N, M) and
+        `Y_pred` (A, N, M) and returns Any
+            Computes a metric based on true values `Y_test` and predicted values
+            `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
         center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+            Whether to center the data before fitting. If True, then the mean of the
+            training data is subtracted from the data. If False, then the data is
+            assumed to be already centered.
 
         scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+            Whether to scale the data before fitting. If True, then the data is scaled
+            using Bessel's correction for the unbiased estimate of the sample standard
+            deviation. If False, then the data is assumed to be already scaled.
 
         copy : bool, optional, default=True
-            Whether to copy `X_train` and `Y_train` in stateless_fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+            Whether to copy `X_train` and `Y_train` in stateless_fit before potentially
+            applying centering and scaling. If True, then the data is copied before
+            fitting. If False, and `dtype` matches the type of `X` and `Y`, then
+            centering and scaling is done inplace, modifying both arrays.
 
         Returns
         -------
         metric_function(Y_test, Y_pred) : Any.
 
         See Also
         --------
-        stateless_fit : Fits on `X_train` and `Y_train` using `A` components while optionally performing centering and scaling. Then returns the internal matrices instead of storing them in the class instance.
+        stateless_fit : Fits on `X_train` and `Y_train` using `A` components while
+        optionally performing centering and scaling. Then returns the internal matrices
+        instead of storing them in the class instance.
 
-        stateless_predict : Computes `Y_pred` given predictor variables `X` and regression tensor `B` and optionally `A` components.
+        stateless_predict : Computes `Y_pred` given predictor variables `X` and
+        regression tensor `B` and optionally `A` components.
         """
         if self.verbose:
             print(f"stateless_fit_predict_eval for {self.name} will be JIT compiled...")
 
         X_train, Y_train = self._initialize_input_matrices(X=X_train, Y=Y_train)
         X_test, Y_test = self._initialize_input_matrices(X=X_test, Y=Y_test)
 
@@ -847,60 +964,77 @@
             Tuple[jax.Array, jax.Array, jax.Array, jax.Array],
         ],
         metric_function: Callable[[jax.Array, jax.Array], Any],
         metric_names: list[str],
         show_progress=True,
     ) -> dict[str, Any]:
         """
-        Performs cross-validation for the Partial Least-Squares (PLS) model on given data. `preprocessing_function` will be applied before any potential centering and scaling as determined by `self.center` and `self.scale`. Any such potential centering and scaling is applied for each split using training set statistics to avoid data leakage from the validation set.
+        Performs cross-validation for the Partial Least-Squares (PLS) model on given
+        data. `preprocessing_function` will be applied before any potential centering
+        and scaling as determined by `self.center` and `self.scale`. Any such potential
+        centering and scaling is applied for each split using training set statistics
+        to avoid data leakage from the validation set.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         Y : Array of shape (N, M) or (N,)
             Response variables.
 
         A : int
             Number of components in the PLS model.
 
         cv_splits : Array of shape (N,)
-            An array defining cross-validation splits. Each unique value in `cv_splits` corresponds to a different fold.
-
-        preprocessing_function : Callable receiving arrays `X_train`, `Y_train`, `X_val`, and `Y_val`
-            A function that preprocesses the training and validation data for each fold. It should return preprocessed arrays for `X_train`, `Y_train`, `X_val`, and `Y_val`.
+            An array defining cross-validation splits. Each unique value in `cv_splits`
+            corresponds to a different fold.
 
-        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning Any
-            Computes a metric based on true values `Y_test` and predicted values `Y_pred`. `Y_pred` contains a prediction for all `A` components.
+        preprocessing_function : Callable receiving arrays `X_train`, `Y_train`,
+        `X_val`, and `Y_val`
+            A function that preprocesses the training and validation data for each
+            fold. It should return preprocessed arrays for `X_train`, `Y_train`,
+            `X_val`, and `Y_val`.
+
+        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning
+        Any
+            Computes a metric based on true values `Y_test` and predicted values
+            `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
         metric_names : list of str
             A list of names for the metrics used for evaluation.
 
         show_progress : bool, optional, default=True
             If True, displays a progress bar for the cross-validation.
 
         Returns
         -------
         metrics : dict[str, Any]
-            A dictionary containing evaluation metrics for each metric specified in `metric_names`. The keys are metric names, and the values are lists of metric values for each cross-validation fold.
+            A dictionary containing evaluation metrics for each metric specified in
+            `metric_names`. The keys are metric names, and the values are lists of
+            metric values for each cross-validation fold.
 
         See Also
         --------
-        _inner_cv : Performs cross-validation for a single fold and computes evaluation metrics.
+        _inner_cv : Performs cross-validation for a single fold and computes evaluation
+        metrics.
 
-        _update_metric_value_lists : Updates lists of metric values for each metric and fold.
+        _update_metric_value_lists : Updates lists of metric values for each metric and
+        fold.
 
-        _finalize_metric_values : Organizes and finalizes the metric values into a dictionary for the specified metric names.
+        _finalize_metric_values : Organizes and finalizes the metric values into a
+        dictionary for the specified metric names.
 
-        stateless_fit_predict_eval : Fits the PLS model, makes predictions, and evaluates metrics for a given fold.
+        stateless_fit_predict_eval : Fits the PLS model, makes predictions, and
+        evaluates metrics for a given fold.
 
         Notes
         -----
-        This method is used to perform cross-validation on the PLS model with different data splits and evaluate its performance using user-defined metrics.
+        This method is used to perform cross-validation on the PLS model with different
+        data splits and evaluate its performance using user-defined metrics.
         """
         X = jnp.asarray(X, dtype=self.dtype)
         Y = jnp.asarray(Y, dtype=self.dtype)
         cv_splits = jnp.asarray(cv_splits, dtype=jnp.int64)
         metric_value_lists = [[] for _ in metric_names]
         unique_splits = jnp.unique(cv_splits)
         for split in tqdm(unique_splits, disable=not show_progress):
@@ -937,15 +1071,16 @@
         ],
         metric_function: Callable[[jax.Array, jax.Array], Any],
         center: bool = True,
         scale: bool = True,
         copy: bool = True,
     ):
         """
-        Performs cross-validation for a single fold of the data and computes evaluation metrics.
+        Performs cross-validation for a single fold of the data and computes evaluation
+        metrics.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         Y : Array of shape (N, M)
@@ -956,37 +1091,50 @@
 
         val_idxs : Array of shape (N_val,)
             Indices of data points in the validation set.
 
         A : int
             Number of components in the PLS model.
 
-        preprocessing_function : Callable receiving arrays `X_train`, `Y_train`, `X_val`, and `Y_val`
-            A function that preprocesses the training and validation data for each fold. It should return preprocessed arrays for `X_train`, `Y_train`, `X_val`, and `Y_val`.
-
-        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning Any
-            Computes a metric based on true values `Y_test` and predicted values `Y_pred`. `Y_pred` contains a prediction for all `A` components.
+        preprocessing_function : Callable receiving arrays `X_train`, `Y_train`,
+        `X_val`, and `Y_val`
+            A function that preprocesses the training and validation data for each
+            fold. It should return preprocessed arrays for `X_train`, `Y_train`,
+            `X_val`, and `Y_val`.
+
+        metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning
+        Any
+            Computes a metric based on true values `Y_test` and predicted values
+            `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
         center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+            Whether to center the data before fitting. If True, then the mean of the
+            training data is subtracted from the data. If False, then the data is
+            assumed to be already centered.
 
         scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+            Whether to scale the data before fitting. If True, then the data is scaled
+            using Bessel's correction for the unbiased estimate of the sample standard
+            deviation. If False, then the data is assumed to be already scaled.
 
         copy : bool, optional, default=True
-            Whether to copy `X_train` and `Y_train` in stateless_fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+            Whether to copy `X_train` and `Y_train` in stateless_fit before potentially
+            applying centering and scaling. If True, then the data is copied before
+            fitting. If False, and `dtype` matches the type of `X` and `Y`, then
+            centering and scaling is done inplace, modifying both arrays.
 
         Returns
         -------
         metric_values : Any
             metric values based on the true and predicted values for a single fold.
 
         Notes
         -----
-        This method performs cross-validation for a single fold of the data, including preprocessing, fitting, predicting, and evaluating the PLS model.
+        This method performs cross-validation for a single fold of the data, including
+        preprocessing, fitting, predicting, and evaluating the PLS model.
         """
         if self.verbose:
             print(f"_inner_cv for {self.name} will be JIT compiled...")
 
         X_train = jnp.take(X, train_idxs, axis=0)
         Y_train = jnp.take(Y, train_idxs, axis=0)
 
@@ -1011,15 +1159,16 @@
     def _update_metric_value_lists(
         self,
         metric_value_lists: list[list[Any]],
         metric_names: list[str],
         metric_values: Any,
     ):
         """
-        Updates lists of metric values for each metric and fold during cross-validation.
+        Updates lists of metric values for each metric and fold during
+        cross-validation.
 
         Parameters
         ----------
         metric_value_lists : list of list of Any
             Lists of metric values for each metric and fold.
 
         metric_values : list of Any
@@ -1028,45 +1177,50 @@
         Returns
         -------
         metric_value_lists : list of list of Any
             Updated lists of metric values for each metric and fold.
 
         Notes
         -----
-        This method updates the lists of metric values for each metric and fold during cross-validation.
+        This method updates the lists of metric values for each metric and fold during
+        cross-validation.
         """
         if len(metric_names) == 1:
             metric_value_lists[0].append(metric_values)
         else:
             for i in range(len(metric_names)):
                 metric_value_lists[i].append(metric_values[i])
         return metric_value_lists
 
     def _finalize_metric_values(
         self, metrics_results: list[list[Any]], metric_names: list[str]
     ):
         """
-        Organizes and finalizes the metric values into a dictionary for the specified metric names.
+        Organizes and finalizes the metric values into a dictionary for the specified
+        metric names.
 
         Parameters
         ----------
         metrics_results : list of list of Any
             Lists of metric values for each metric and fold.
 
         metric_names : list of str
             A list of names for the metrics used for evaluation.
 
         Returns
         -------
         metrics : dict[str, list[Any]]
-            A dictionary containing evaluation metrics for each metric specified in `metric_names`. The keys are metric names, and the values are lists of metric values for each cross-validation fold.
+            A dictionary containing evaluation metrics for each metric specified in
+            `metric_names`. The keys are metric names, and the values are lists of
+            metric values for each cross-validation fold.
 
         Notes
         -----
-        This method organizes and finalizes the metric values into a dictionary for the specified metric names, making it easy to analyze the cross-validation results.
+        This method organizes and finalizes the metric values into a dictionary for the
+        specified metric names, making it easy to analyze the cross-validation results.
         """
         metrics = {}
         for name, lst_of_metric_value_for_each_split in zip(
             metric_names, metrics_results
         ):
             metrics[name] = lst_of_metric_value_for_each_split
         return metrics
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/ikpls/numpy_ikpls.py` & `ikpls-1.2.0/ikpls/numpy_ikpls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,59 @@
+"""
+Contains the PLS Class which implements partial least-squares regression using Improved
+Kernel PLS by Dayal and MacGregor:
+https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+
+The PLS class subclasses scikit-learn's BaseEstimator to ensure compatibility with e.g.
+scikit-learn's cross_validate. It is written using NumPy.
+
+Author: Ole-Christian Galbo Engstrøm
+E-mail: ole.e@di.ku.dk
+"""
+
 import warnings
 from typing import Union
 
 import numpy as np
 import numpy.linalg as la
 import numpy.typing as npt
 from sklearn.base import BaseEstimator
 
 
 class PLS(BaseEstimator):
     """
-    Implements partial least-squares regression using Improved Kernel PLS by Dayal and MacGregor: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
+    Implements partial least-squares regression using Improved Kernel PLS by Dayal and
+    MacGregor:
+    https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
     algorithm : int, default=1
         Whether to use Improved Kernel PLS Algorithm #1 or #2.
 
     center : bool, default=True
-        Whether to center the data before fitting. If True, then the mean of the training data is subtracted from the data. If False, then the data is assumed to be already centered.
+        Whether to center the data before fitting. If True, then the mean of the
+        training data is subtracted from the data. If False, then the data is assumed
+        to be already centered.
 
     scale : bool, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled using Bessel's correction for the unbiased estimate of the sample standard deviation. If False, then the data is assumed to be already scaled.
+        Whether to scale the data before fitting. If True, then the data is scaled
+        using Bessel's correction for the unbiased estimate of the sample standard
+        deviation. If False, then the data is assumed to be already scaled.
 
     copy : bool, default=True
-        Whether to copy `X` and `Y` in fit before potentially applying centering and scaling. If True, then the data is copied before fitting. If False, and `dtype` matches the type of `X` and `Y`, then centering and scaling is done inplace, modifying both arrays.
+        Whether to copy `X` and `Y` in fit before potentially applying centering and
+        scaling. If True, then the data is copied before fitting. If False, and `dtype`
+        matches the type of `X` and `Y`, then centering and scaling is done inplace,
+        modifying both arrays.
 
     dtype : numpy.float, default=numpy.float64
-        The float datatype to use in computation of the PLS algorithm. Using a lower precision than float64 will yield significantly worse results when using an increasing number of components due to propagation of numerical errors.
+        The float datatype to use in computation of the PLS algorithm. Using a lower
+        precision than float64 will yield significantly worse results when using an
+        increasing number of components due to propagation of numerical errors.
 
     Raises
     ------
     ValueError
         If `algorithm` is not 1 or 2.
     """
 
@@ -48,14 +71,48 @@
         self.copy = copy
         self.dtype = dtype
         self.name = f"Improved Kernel PLS Algorithm #{algorithm}"
         if self.algorithm not in [1, 2]:
             raise ValueError(
                 f"Invalid algorithm: {self.algorithm}. Algorithm must be 1 or 2."
             )
+        self.A = None
+        self.N = None
+        self.K = None
+        self.M = None
+        self.B = None
+        self.W = None
+        self.P = None
+        self.Q = None
+        self.R = None
+        self.T = None
+        self.X_mean = None
+        self.Y_mean = None
+        self.X_std = None
+        self.Y_std = None
+
+    def _weight_warning(self, i: int) -> None:
+        """
+        Warns the user that the weight is close to zero.
+
+        Parameters
+        ----------
+        i : int
+            Number of components.
+
+        Returns
+        -------
+        None.
+        """
+        with warnings.catch_warnings():
+            warnings.simplefilter("always", UserWarning)
+            warnings.warn(
+                f"Weight is close to zero. Results with A = {i} component(s) or higher"
+                " may be unstable."
+            )
 
     def fit(self, X: npt.ArrayLike, Y: npt.ArrayLike, A: int) -> None:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
 
         Parameters
         ----------
@@ -83,15 +140,15 @@
             PLS Loadings matrix for Y.
 
         R : Array of shape (K, A)
             PLS weights matrix to compute scores T directly from original X.
 
         T : Array of shape (N, A)
             PLS scores matrix of X. Only assigned for Improved Kernel PLS Algorithm #1.
-        
+
         X_mean : Array of shape (1, K) or None
             Mean of X. If centering is not performed, this is None.
 
         Y_mean : Array of shape (1, M) or None
             Mean of Y. If centering is not performed, this is None.
 
         X_std : Array of shape (1, K) or None
@@ -103,15 +160,16 @@
         Returns
         -------
         None.
 
         Warns
         -----
         UserWarning.
-            If at any point during iteration over the number of components `A`, the residual goes below machine precision for jnp.float64.
+            If at any point during iteration over the number of components `A`, the
+            residual goes below machine precision for np.float64.
         """
         X = np.asarray(X, dtype=self.dtype)
         Y = np.asarray(Y, dtype=self.dtype)
 
         if Y.ndim == 1:
             Y = Y.reshape(-1, 1)
 
@@ -161,40 +219,34 @@
             XTX = X.T @ X
 
         for i in range(A):
             # Step 2
             if M == 1:
                 norm = la.norm(XTY, ord=2)
                 if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                    warnings.warn(
-                        f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                    )
+                    self._weight_warning(i)
                     break
                 w = XTY / norm
             else:
                 if M < K:
                     XTYTXTY = XTY.T @ XTY
                     eig_vals, eig_vecs = la.eigh(XTYTXTY)
                     q = eig_vecs[:, -1:]
                     w = XTY @ q
                     norm = la.norm(w)
                     if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                        warnings.warn(
-                            f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                        )
+                        self._weight_warning(i)
                         break
                     w = w / norm
                 else:
                     XTYYTX = XTY @ XTY.T
                     eig_vals, eig_vecs = la.eigh(XTYYTX)
                     norm = eig_vals[-1]
                     if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
-                        warnings.warn(
-                            f"Weight is close to zero. Stopping fitting after A = {i} component(s)."
-                        )
+                        self._weight_warning(i)
                         break
                     w = eig_vecs[:, -1:]
             W[i] = w.squeeze()
 
             # Step 3
             r = np.copy(w)
             for j in range(i):
@@ -221,28 +273,34 @@
             # Compute regression coefficients
             self.B[i] = self.B[i - 1] + r @ q.T
 
     def predict(
         self, X: npt.ArrayLike, n_components: Union[None, int] = None
     ) -> npt.NDArray[np.float_]:
         """
-        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using `n_components` components. If `n_components` is None, then predictions are returned for all number of components.
+        Predicts with Improved Kernel PLS Algorithm #1 on `X` with `B` using
+        `n_components` components. If `n_components` is None, then predictions are
+        returned for all number of components.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         n_components : int or None, optional, default=None.
-            Number of components in the PLS model. If None, then all number of components are used.
+            Number of components in the PLS model. If None, then all number of
+            components are used.
 
         Returns
         -------
         Y_pred : Array of shape (N, M) or (A, N, M)
-            If `n_components` is an int, then an array of shape (N, M) with the predictions for that specific number of components is used. If `n_components` is None, returns a prediction for each number of components up to `A`.
+            If `n_components` is an int, then an array of shape (N, M) with the
+            predictions for that specific number of components is used. If
+            `n_components` is None, returns a prediction for each number of components
+            up to `A`.
         """
         X = np.asarray(X, dtype=self.dtype)
         if self.center:
             X = X - self.X_mean
         if self.scale:
             X = X / self.X_std
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ikpls-1.1.3/pyproject.toml` & `ikpls-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ikpls"
-version = "1.1.3"
+version = "1.2.0"
 description = ""
 authors = ["Sm00thix <oleemail@icloud.com>"]
 maintainers = ["Sm00thix <oleemail@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://ikpls.readthedocs.io/en/latest/"
 repository = "https://github.com/Sm00thix/IKPLS"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
-numpy = "^1.26.1"
-jax = "^0.4.19"
-jaxlib = "^0.4.19"
-scikit-learn = "^1.3.2"
+numpy = "^1.26.3"
+jax = "^0.4.20"
+jaxlib = "^0.4.20"
+scikit-learn = "^1.4.1"
 tqdm = "^4.66.1"
 joblib = "^1.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ikpls-1.1.3/PKG-INFO` & `ikpls-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: ikpls
-Version: 1.1.3
+Version: 1.2.0
 Summary: 
 Home-page: https://ikpls.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Sm00thix
 Author-email: oleemail@icloud.com
 Maintainer: Sm00thix
 Maintainer-email: oleemail@icloud.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: jax (>=0.4.19,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.19,<0.5.0)
+Requires-Dist: jax (>=0.4.20,<0.5.0)
+Requires-Dist: jaxlib (>=0.4.20,<0.5.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
-Requires-Dist: numpy (>=1.26.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
+Requires-Dist: numpy (>=1.26.3,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.1,<2.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/Sm00thix/IKPLS
 Description-Content-Type: text/x-rst
 
 Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
 =======================================================================
 
 .. image:: https://img.shields.io/pypi/v/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: PyPI Version
+.. image:: https://img.shields.io/pypi/dm/ikpls
+   :target: https://pypi.python.org/pypi/ikpls/
+   :alt: PyPI - Downloads
 .. image:: https://img.shields.io/pypi/pyversions/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: Python Versions
 .. image:: https://img.shields.io/pypi/l/ikpls.svg
    :target: https://pypi.python.org/pypi/ikpls/
    :alt: License
 .. image:: https://readthedocs.org/projects/ikpls/badge/?version=latest
@@ -62,21 +65,23 @@
 .. _Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 11(1), 73-85: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?
 .. _Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720: https://doi.org/10.1007/s00362-009-0251-7
 .. _Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 23(10), 518-529: https://doi.org/10.1002/cem.1248
 .. _NumPy: https://numpy.org/
 .. _scikit-learn: https://scikit-learn.org/stable/
 .. _JAX: https://jax.readthedocs.io/en/latest/
 
-Extremely Fast Cross-Validation
+Fast Cross-Validation
 -------------------------------
 In addition to the implementations mentioned above, this package contains the novel, fast cross-validation algorithms mentioned in [7]_ using both IKPLS algorithms.
 The fast cross-validation algorithms benefit both IKPLS Algorithms and especially Algorithm #2.
 The fast cross-validation algorithms are mathematically equivalent to the classical cross-validation algorithm. Still, they are much quicker if cross-validation splits exceed 3.
 The fast cross-validation algorithms correctly handle (column-wise) centering and scaling of the X and Y input matrices using training set means and standard deviations to avoid data leakage from the validation set.
 This centering and scaling can be enabled by setting the center parameter to True and the scale parameter to True, respectively.
+The fast cross-validation algorithms correctly handle row-wise preprocessing such as (row-wise) centering and scaling of the X and Y input matrices, convolution, or other preprocessing.
+Row-wise preprocessing can safely be applied before passing the data to the fast cross-validation algorithms.
 
 .. [7] `Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments`_.
 
 .. _Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation\: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments: https://arxiv.org/abs/2401.13185
 
 Pre-requisites
 --------------
@@ -102,41 +107,62 @@
 Quick Start
 -----------
 Use the ikpls package for PLS modeling
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~   
 
   .. code:: python
 
-    import numpy as np
+   import numpy as np
+
+   from ikpls.numpy_ikpls import PLS
 
-    from ikpls.numpy_ikpls import PLS
 
     N = 100  # Number of samples.
     K = 50  # Number of features.
     M = 10  # Number of targets.
     A = 20  # Number of latent variables (PLS components).
 
+    # Using float64 is important for numerical stability.
     X = np.random.uniform(size=(N, K)).astype(np.float64)
     Y = np.random.uniform(size=(N, M)).astype(np.float64)
 
-    # The other PLS algorithms and implementations, except for NpPLS_FastCV, have the same interface for fit() and predict().
+    # The other PLS algorithms and implementations have the same interface for fit()
+    # and predict(). The fast cross-validation implementation with IKPLS has a
+    # different interface.
     np_ikpls_alg_1 = PLS(algorithm=1)
     np_ikpls_alg_1.fit(X, Y, A)
 
-    y_pred = np_ikpls_alg_1.predict(X) # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible numbers of components up to and including A.
-    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20) # Has shape (N, M) = (100, 10).
-    (y_pred_20_components == y_pred[19]).all() # True
+    # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
+    # numbers of components up to and including A.
+    y_pred = np_ikpls_alg_1.predict(X)
+
+    # Has shape (N, M) = (100, 10).
+    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
+    (y_pred_20_components == y_pred[19]).all()  # True
 
     # The internal model parameters can be accessed as follows:
-    np_ikpls_alg_1.B  # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
-    np_ikpls_alg_1.W  # X weights matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.P  # X loadings matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.Q  # Y loadings matrix of shape (M, A) = (10, 20).
-    np_ikpls_alg_1.R  # X rotations matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.T  # X scores matrix of shape (N, A) = (100, 20). This is only computed for IKPLS Algorithm #1.
+
+    # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
+    np_ikpls_alg_1.B
+
+    # X weights matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.W
+
+    # X loadings matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.P
+
+    # Y loadings matrix of shape (M, A) = (10, 20).
+    np_ikpls_alg_1.Q
+
+    # X rotations matrix of shape (K, A) = (50, 20).
+    np_ikpls_alg_1.R
+
+    # X scores matrix of shape (N, A) = (100, 20).
+    # This is only computed for IKPLS Algorithm #1.
+    np_ikpls_alg_1.T
 
 Examples
 ~~~~~~~~
 
 In `examples <https://github.com/Sm00thix/IKPLS/tree/main/examples>`_ you will find:
 
 - `Fit and Predict with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py>`_
@@ -147,8 +173,11 @@
 
 - `Cross-validate with NumPy and fast cross-validation. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py>`_
 
 - `Cross-validate with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py>`_
 
 - `Compute the gradient of a preprocessing convolution filter with respect to the RMSE between the target value and the value predicted by PLS after fitting with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py>`_
 
+Contribute
+----------
 
+To contribute, please read the `Contribution Guidelines <https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.rst>`_.
```

