# Comparing `tmp/empulse-0.1.2.tar.gz` & `tmp/empulse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empulse-0.1.2.tar", last modified: Wed Feb 28 15:03:44 2024, max compression
+gzip compressed data, was "empulse-0.2.0.tar", last modified: Wed Apr 17 20:35:42 2024, max compression
```

## Comparing `empulse-0.1.2.tar` & `empulse-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:44.098391 empulse-0.1.2/
--rw-rw-rw-   0        0        0     2807 2024-02-28 07:01:42.000000 empulse-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6974 2024-02-28 15:03:44.096535 empulse-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2024-02-28 07:01:42.000000 empulse-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:43.708451 empulse-0.1.2/empulse/
--rw-rw-rw-   0        0        0       23 2024-02-28 14:22:21.000000 empulse-0.1.2/empulse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:43.841278 empulse-0.1.2/empulse/metrics/
--rw-rw-rw-   0        0        0      417 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/_convex_hull.py
--rw-rw-rw-   0        0        0     2516 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/_validation.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:43.903766 empulse-0.1.2/empulse/metrics/acquisition/
--rw-rw-rw-   0        0        0      333 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/acquisition/__init__.py
--rw-rw-rw-   0        0        0     1950 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/acquisition/_validation.py
--rw-rw-rw-   0        0        0     6659 2024-02-28 14:04:45.000000 empulse-0.1.2/empulse/metrics/acquisition/cost.py
--rw-rw-rw-   0        0        0     7776 2024-02-28 13:38:29.000000 empulse-0.1.2/empulse/metrics/acquisition/deterministic.py
--rw-rw-rw-   0        0        0    10466 2024-02-28 13:38:29.000000 empulse-0.1.2/empulse/metrics/acquisition/stochastic.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:43.962086 empulse-0.1.2/empulse/metrics/churn/
--rw-rw-rw-   0        0        0      355 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/churn/__init__.py
--rw-rw-rw-   0        0        0     3008 2024-02-28 14:29:23.000000 empulse-0.1.2/empulse/metrics/churn/_validation.py
--rw-rw-rw-   0        0        0     7013 2024-02-28 14:04:45.000000 empulse-0.1.2/empulse/metrics/churn/cost.py
--rw-rw-rw-   0        0        0     9176 2024-02-28 12:52:46.000000 empulse-0.1.2/empulse/metrics/churn/deterministic.py
--rw-rw-rw-   0        0        0    18722 2024-02-28 13:30:12.000000 empulse-0.1.2/empulse/metrics/churn/stochastic.py
--rw-rw-rw-   0        0        0     4371 2024-01-19 17:22:55.000000 empulse-0.1.2/empulse/metrics/common.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:44.020686 empulse-0.1.2/empulse/metrics/credit_scoring/
--rw-rw-rw-   0        0        0      232 2023-06-15 15:14:06.000000 empulse-0.1.2/empulse/metrics/credit_scoring/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-01-18 17:24:36.000000 empulse-0.1.2/empulse/metrics/credit_scoring/_validation.py
--rw-rw-rw-   0        0        0     6437 2024-02-28 13:14:32.000000 empulse-0.1.2/empulse/metrics/credit_scoring/deterministic.py
--rw-rw-rw-   0        0        0     9399 2024-02-28 13:14:32.000000 empulse-0.1.2/empulse/metrics/credit_scoring/stochastic.py
--rw-rw-rw-   0        0        0    13798 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/emp.py
--rw-rw-rw-   0        0        0     1717 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/lift.py
--rw-rw-rw-   0        0        0     5270 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/metrics/mp.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:44.062382 empulse-0.1.2/empulse/models/
--rw-rw-rw-   0        0        0       84 2024-01-20 23:07:55.000000 empulse-0.1.2/empulse/models/__init__.py
--rw-rw-rw-   0        0        0     9374 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/models/b2boost.py
--rw-rw-rw-   0        0        0    10872 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/models/proflogit.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:44.093536 empulse-0.1.2/empulse/optimizers/
--rw-rw-rw-   0        0        0       70 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/optimizers/__init__.py
--rw-rw-rw-   0        0        0    12791 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/optimizers/generation.py
--rw-rw-rw-   0        0        0      225 2024-02-28 07:01:42.000000 empulse-0.1.2/empulse/optimizers/optimizer.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:03:43.750072 empulse-0.1.2/empulse.egg-info/
--rw-rw-rw-   0        0        0     6974 2024-02-28 15:03:43.000000 empulse-0.1.2/empulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2024-02-28 15:03:43.000000 empulse-0.1.2/empulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 15:03:43.000000 empulse-0.1.2/empulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2024-02-28 15:03:43.000000 empulse-0.1.2/empulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-28 15:03:43.000000 empulse-0.1.2/empulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1969 2024-02-28 14:22:21.000000 empulse-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 15:03:44.098391 empulse-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-02-28 07:01:42.000000 empulse-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.567930 empulse-0.2.0/
+-rw-rw-rw-   0        0        0     2807 2024-04-17 13:09:41.000000 empulse-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6974 2024-04-17 20:35:42.566930 empulse-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2024-04-17 13:09:41.000000 empulse-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.327876 empulse-0.2.0/empulse/
+-rw-rw-rw-   0        0        0       23 2024-04-17 13:33:13.000000 empulse-0.2.0/empulse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.406893 empulse-0.2.0/empulse/metrics/
+-rw-rw-rw-   0        0        0      417 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/_convex_hull.py
+-rw-rw-rw-   0        0        0     2516 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.448903 empulse-0.2.0/empulse/metrics/acquisition/
+-rw-rw-rw-   0        0        0      333 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/acquisition/__init__.py
+-rw-rw-rw-   0        0        0     1950 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/acquisition/_validation.py
+-rw-rw-rw-   0        0        0     6659 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/acquisition/cost.py
+-rw-rw-rw-   0        0        0     7776 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/acquisition/deterministic.py
+-rw-rw-rw-   0        0        0    10466 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/acquisition/stochastic.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.489913 empulse-0.2.0/empulse/metrics/churn/
+-rw-rw-rw-   0        0        0      355 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/churn/__init__.py
+-rw-rw-rw-   0        0        0     3606 2024-04-17 14:49:30.000000 empulse-0.2.0/empulse/metrics/churn/_validation.py
+-rw-rw-rw-   0        0        0     7393 2024-04-17 14:52:30.000000 empulse-0.2.0/empulse/metrics/churn/cost.py
+-rw-rw-rw-   0        0        0     9176 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/churn/deterministic.py
+-rw-rw-rw-   0        0        0    18722 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/churn/stochastic.py
+-rw-rw-rw-   0        0        0     4371 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/common.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.519919 empulse-0.2.0/empulse/metrics/credit_scoring/
+-rw-rw-rw-   0        0        0      232 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/credit_scoring/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/credit_scoring/_validation.py
+-rw-rw-rw-   0        0        0     6437 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/credit_scoring/deterministic.py
+-rw-rw-rw-   0        0        0     9399 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/credit_scoring/stochastic.py
+-rw-rw-rw-   0        0        0    13798 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/emp.py
+-rw-rw-rw-   0        0        0     1717 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/lift.py
+-rw-rw-rw-   0        0        0     5270 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/metrics/mp.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.540926 empulse-0.2.0/empulse/models/
+-rw-rw-rw-   0        0        0       84 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/models/__init__.py
+-rw-rw-rw-   0        0        0     9645 2024-04-17 13:54:10.000000 empulse-0.2.0/empulse/models/b2boost.py
+-rw-rw-rw-   0        0        0    10872 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/models/proflogit.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.562930 empulse-0.2.0/empulse/optimizers/
+-rw-rw-rw-   0        0        0       70 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/optimizers/__init__.py
+-rw-rw-rw-   0        0        0    12791 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/optimizers/generation.py
+-rw-rw-rw-   0        0        0      225 2024-04-17 13:09:41.000000 empulse-0.2.0/empulse/optimizers/optimizer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:35:42.355882 empulse-0.2.0/empulse.egg-info/
+-rw-rw-rw-   0        0        0     6974 2024-04-17 20:35:42.000000 empulse-0.2.0/empulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-04-17 20:35:42.000000 empulse-0.2.0/empulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:35:42.000000 empulse-0.2.0/empulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2024-04-17 20:35:42.000000 empulse-0.2.0/empulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 20:35:42.000000 empulse-0.2.0/empulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1969 2024-04-17 20:32:54.000000 empulse-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:35:42.567930 empulse-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-04-17 13:09:41.000000 empulse-0.2.0/setup.py
```

### Comparing `empulse-0.1.2/LICENSE` & `empulse-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/PKG-INFO` & `empulse-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empulse
-Version: 0.1.2
+Version: 0.2.0
 Summary: Value-driven metrics and models for scikit-learn
 Author-email: Shimanto Rahman <shimanto.rahman@ugent.be>
 License: MIT License
         
         Copyright (c) 2023 Shimanto Rahman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `empulse-0.1.2/README.md` & `empulse-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/_convex_hull.py` & `empulse-0.2.0/empulse/metrics/_convex_hull.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/_validation.py` & `empulse-0.2.0/empulse/metrics/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/acquisition/_validation.py` & `empulse-0.2.0/empulse/metrics/acquisition/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/acquisition/cost.py` & `empulse-0.2.0/empulse/metrics/acquisition/cost.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/acquisition/deterministic.py` & `empulse-0.2.0/empulse/metrics/acquisition/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/acquisition/stochastic.py` & `empulse-0.2.0/empulse/metrics/acquisition/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/churn/_validation.py` & `empulse-0.2.0/empulse/metrics/churn/_validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,14 +77,33 @@
         d: float,
         f: float
 ) -> tuple[np.ndarray, np.ndarray, Union[np.ndarray, float]]:
     _check_fraction(gamma, 'gamma')
     return _validate_input(y_true, y_pred, clv, d, f)
 
 
+def _validate_input_mpc(
+        y_true: ArrayLike,
+        y_pred: ArrayLike,
+        clv: ArrayLike,
+        accept_rate: float,
+        incentive_fraction: float,
+        contact_cost: float
+) -> tuple[np.ndarray, np.ndarray, Union[np.ndarray, float]]:
+    y_true = _check_y_true(y_true)
+    y_pred = _check_y_pred(y_pred)
+    _check_shape(y_true, y_pred)
+    clv = np.asarray(clv)
+    _check_fraction(accept_rate, 'accept_rate')
+    _check_fraction(incentive_fraction, 'incentive_fraction')
+    _check_positive(contact_cost, 'contact_cost')
+
+    return y_true, y_pred, clv
+
+
 def _validate_input_empb(
         y_true: ArrayLike,
         y_pred: ArrayLike,
         clv: ArrayLike,
         alpha: float,
         beta: float,
         incentive_fraction: float,
```

### Comparing `empulse-0.1.2/empulse/metrics/churn/cost.py` & `empulse-0.2.0/empulse/metrics/churn/cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from functools import partial
 from typing import Callable, Union
 
 import numpy as np
 import xgboost as xgb
 from numpy.typing import ArrayLike
 
-from empulse.metrics.churn._validation import _validate_input_mp
+from empulse.metrics.churn._validation import _validate_input_mpc
 
 
 def make_objective_churn(
         accept_rate: float = 0.3,
         clv: Union[float, ArrayLike] = 200,
-        incentive_cost: Union[float, ArrayLike] = 10,
-        contact_cost: float = 1,
+        incentive_fraction: Union[float, ArrayLike] = 0.05,
+        contact_cost: float = 15,
 ) -> Callable[[np.ndarray, xgb.DMatrix], tuple[np.ndarray, np.ndarray]]:
     """
     Create an objective function for the :class:`xgboost:xgboost.XGBClassifier` for customer churn
 
     The objective function presumes a situation where identified churners are
     contacted and offered an incentive to remain customers.
     Only a fraction of churners accepts the incentive offer.
@@ -31,16 +31,17 @@
         Probability of a customer responding to the retention offer (``0 < accept_rate < 1``).
 
     clv : float or 1D array-like, shape=(n_samples), default=200
         If ``float``: constant customer lifetime value per retained customer (``clv > incentive_cost``).
         If ``array``: individualized customer lifetime value of each customer when retained
         (``mean(clv) > incentive_cost``).
 
-    incentive_cost : float, default=10
-        Constant cost of retention offer (``incentive_cost > 0``).
+    incentive_fraction : float, default=0.05
+        Cost of incentive offered to a customer, as a fraction of customer lifetime value
+        (``0 < incentive_fraction < 1``).
 
     contact_cost : float, default=1
         Constant cost of contact (``contact_cost > 0``).
 
     Returns
     -------
     objective : Callable
@@ -62,25 +63,25 @@
         Annals of Operations Research, 1-27.
 
     """
     return partial(
         _objective,
         accept_rate=accept_rate,
         clv=clv,
-        incentive_cost=incentive_cost,
+        incentive_fraction=incentive_fraction,
         contact_cost=contact_cost,
     )
 
 
 def _objective(
         y_pred: np.ndarray,
         dtrain: Union[xgb.DMatrix, np.ndarray],
         accept_rate: float = 0.3,
         clv: Union[float, ArrayLike] = 200,
-        incentive_cost: Union[float, ArrayLike] = 10,
+        incentive_fraction: Union[float, ArrayLike] = 0.05,
         contact_cost: float = 1,
 ) -> tuple[np.ndarray, np.ndarray]:
     """
     Objective function for XGBoost to maximize the profit of a churn model.
 
     Parameters
     ----------
@@ -102,29 +103,30 @@
         y_true = dtrain
     elif isinstance(dtrain, xgb.DMatrix):
         y_true = dtrain.get_label()
     else:
         raise TypeError(f"Expected dtrain to be of type np.ndarray or xgb.DMatrix, got {type(dtrain)} instead.")
     y_pred = 1 / (1 + np.exp(-y_pred))
 
+    incentive_cost = incentive_fraction * clv
     profits = contact_cost + incentive_cost + y_true * (
             accept_rate * incentive_cost - incentive_cost - clv * accept_rate
     )
     gradient = y_pred * (1 - y_pred) * profits
     hessian = np.abs((1 - 2 * y_pred) * gradient)
     return gradient, hessian
 
 
 def mpc_cost_score(
         y_true: ArrayLike,
         y_pred: ArrayLike,
         *,
         accept_rate: float = 0.3,
         clv: Union[float, ArrayLike] = 200,
-        incentive_cost: Union[float, ArrayLike] = 10,
+        incentive_fraction: Union[float, ArrayLike] = 0.05,
         contact_cost: float = 1,
 ) -> float:
     """
     Profit-driven cost function for customer churn
 
     The cost function presumes a situation where identified churners are
     contacted and offered an incentive to remain customers.
@@ -144,16 +146,17 @@
         Probability of a customer responding to the retention offer (``0 < accept_rate < 1``).
 
     clv : float or 1D array-like, shape=(n_samples), default=200
         If ``float``: constant customer lifetime value per retained customer (``clv` > incentive_cost``).
         If ``array``: individualized customer lifetime value of each customer when retained
         (``mean(clv) > incentive_cost``).
 
-    incentive_cost : float, default=10
-        Constant cost of retention offer (``incentive_cost > 0``).
+    incentive_fraction : float, default=0.05
+        Cost of incentive offered to a customer, as a fraction of customer lifetime value
+        (``0 < incentive_fraction < 1``).
 
     contact_cost : float, default=1
         Constant cost of contact (``contact_cost > 0``).
 
     Returns
     -------
     empc_cost : float
@@ -189,13 +192,21 @@
     References
     ----------
     .. [1] Janssens, B., Bogaert, M., Bagué, A., & Van den Poel, D. (2022).
         B2Boost: Instance-dependent profit-driven modelling of B2B churn.
         Annals of Operations Research, 1-27.
 
     """
-    y_true, y_pred, clv = _validate_input_mp(y_true, y_pred, accept_rate, clv, incentive_cost, contact_cost)
+    y_true, y_pred, clv = _validate_input_mpc(
+        y_true,
+        y_pred,
+        clv=clv,
+        accept_rate=accept_rate,
+        incentive_fraction=incentive_fraction,
+        contact_cost=contact_cost
+    )
 
+    incentive_cost = incentive_fraction * clv
     profits = y_pred * (contact_cost + incentive_cost + y_true * (
             accept_rate * incentive_cost - incentive_cost - clv * accept_rate
     ))
     return float(np.mean(profits))
```

### Comparing `empulse-0.1.2/empulse/metrics/churn/deterministic.py` & `empulse-0.2.0/empulse/metrics/churn/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/churn/stochastic.py` & `empulse-0.2.0/empulse/metrics/churn/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/common.py` & `empulse-0.2.0/empulse/metrics/common.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/credit_scoring/_validation.py` & `empulse-0.2.0/empulse/metrics/credit_scoring/_validation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/credit_scoring/deterministic.py` & `empulse-0.2.0/empulse/metrics/credit_scoring/deterministic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/credit_scoring/stochastic.py` & `empulse-0.2.0/empulse/metrics/credit_scoring/stochastic.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/emp.py` & `empulse-0.2.0/empulse/metrics/emp.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/lift.py` & `empulse-0.2.0/empulse/metrics/lift.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/metrics/mp.py` & `empulse-0.2.0/empulse/metrics/mp.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/models/b2boost.py` & `empulse-0.2.0/empulse/models/b2boost.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,17 @@
         Probability of a customer responding to the retention offer (0 < `accept_rate` < 1).
 
     clv : float or 1D array-like, shape=(n_samples), default=200
         If ``float``: constant customer lifetime value per retained customer (``clv > incentive_cost``).
         If ``array``: individualized customer lifetime value of each customer when retained
         (``mean(clv) > incentive_cost``).
 
-    incentive_cost : float, default=10
-        Constant cost of retention offer (``incentive_cost > 0``).
+    incentive_fraction : float, default=0.05
+        Cost of incentive offered to a customer, as a fraction of customer lifetime value
+        (``0 < incentive_fraction < 1``).
 
     contact_cost : float, default=1
         Constant cost of contact (``contact_cost > 0``).
 
     params : dict[str, Any], default=None
         Other parameters passed to :class:`xgboost:xgboost.XGBClassifier` initializer.
 
@@ -55,21 +56,21 @@
         Annals of Operations Research, 1-27.
     """
     def __init__(
             self,
             *,
             accept_rate: float = 0.3,
             clv: Union[float, ArrayLike] = 200,
-            incentive_cost: float = 10,
-            contact_cost: float = 1,
+            incentive_fraction: float = 0.05,
+            contact_cost: float = 15,
             params: Optional[dict[str, Any]] = None,
             **kwargs,
     ) -> None:
         self.clv = clv
-        self.incentive_cost = incentive_cost
+        self.incentive_fraction = incentive_fraction
         self.contact_cost = contact_cost
         self.accept_rate = accept_rate
 
         # necessary to have params because sklearn.clone does not clone **kwargs
         if params is None:
             params = {}
         if kwargs:
@@ -133,15 +134,15 @@
                 valid_params[key] = value
 
         for key, sub_params in nested_params.items():
             valid_params[key].set_params(**sub_params)
 
         return self
 
-    def fit(self, X, y, sample_weights=None, accept_rate=None, clv=None, incentive_cost=None, contact_cost=None):
+    def fit(self, X, y, sample_weights=None, accept_rate=None, clv=None, incentive_fraction=None, contact_cost=None):
         """
         Fit the model.
 
         Parameters
         ----------
         X : 2D numpy.ndarray, shape=(n_samples, n_dim)
             Training data.
@@ -156,28 +157,29 @@
             Probability of a customer responding to the retention offer (``0 < accept_rate < 1``).
 
         clv : float or 1D array-like, shape=(n_samples), default=200
             If ``float``: constant customer lifetime value per retained customer (``clv > incentive_cost``).
             If ``array``: individualized customer lifetime value of each customer when retained
             (``mean(clv) > incentive_cost``).
 
-        incentive_cost : float, default=10
-            Constant cost of retention offer (``incentive_cost > 0``).
+        incentive_fraction : float, default=10
+            Cost of incentive offered to a customer, as a fraction of customer lifetime value
+            (``0 < incentive_fraction < 1``).
 
         contact_cost : float, default=1
             Constant cost of contact (``contact_cost > 0``).
 
         Returns
         -------
         self : B2BoostClassifier
             Fitted B2Boost model.
         """
         objective = make_objective_churn(
             clv=self.clv if clv is None else clv,
-            incentive_cost=self.incentive_cost if incentive_cost is None else incentive_cost,
+            incentive_fraction=self.incentive_fraction if incentive_fraction is None else incentive_fraction,
             contact_cost=self.contact_cost if contact_cost is None else contact_cost,
             accept_rate=self.accept_rate if accept_rate is None else accept_rate,
         )
         self.model = XGBClassifier(objective=objective, **self.params)
         self.model.fit(X, y, sample_weight=sample_weights)
         return self
 
@@ -213,15 +215,15 @@
 
     def score(
             self,
             X: ArrayLike,
             y: ArrayLike,
             accept_rate: float = None,
             clv=None,
-            incentive_cost=None,
+            incentive_fraction=None,
             contact_cost=None
     ) -> float:
         """
         Compute EMPB score.
 
         Parameters
         ----------
@@ -234,16 +236,17 @@
             Probability of a customer responding to the retention offer (``0 < accept_rate < 1``).
 
         clv : float or 1D array-like, shape=(n_samples), default=self.clv
             If ``float``: constant customer lifetime value per retained customer (``clv > incentive_cost``).
             If ``array``: individualized customer lifetime value of each customer when retained
             (``mean(clv) > incentive_cost```).
 
-        incentive_cost : float, default=self.incentive_cost
-            Constant cost of retention offer (``incentive_cost > 0``).
+        incentive_fraction : float, default=self.incentive_cost
+            Cost of incentive offered to a customer, as a fraction of customer lifetime value
+            (``0 < incentive_fraction < 1``).
 
         contact_cost : float, default=self.contact_cost
             Constant cost of contact (``contact_cost > 0``).
 
         Returns
         -------
         score : float
@@ -251,10 +254,10 @@
         """
         X, y = check_X_y(X, y)
         return mpc_cost_score(
             y,
             self.predict_proba(X)[:, 1],
             accept_rate=accept_rate or self.accept_rate,
             clv=clv or self.clv,
-            incentive_cost=incentive_cost or self.incentive_cost,
+            incentive_fraction=incentive_fraction or self.incentive_fraction,
             contact_cost=contact_cost or self.contact_cost,
         )
```

### Comparing `empulse-0.1.2/empulse/models/proflogit.py` & `empulse-0.2.0/empulse/models/proflogit.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse/optimizers/generation.py` & `empulse-0.2.0/empulse/optimizers/generation.py`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/empulse.egg-info/PKG-INFO` & `empulse-0.2.0/empulse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empulse
-Version: 0.1.2
+Version: 0.2.0
 Summary: Value-driven metrics and models for scikit-learn
 Author-email: Shimanto Rahman <shimanto.rahman@ugent.be>
 License: MIT License
         
         Copyright (c) 2023 Shimanto Rahman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `empulse-0.1.2/empulse.egg-info/SOURCES.txt` & `empulse-0.2.0/empulse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `empulse-0.1.2/pyproject.toml` & `empulse-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "empulse"
-version = "0.1.2"
+version = "0.2.0"
 description = "Value-driven metrics and models for scikit-learn"
 readme = "README.md"
 authors = [
     { name = "Shimanto Rahman", email = "shimanto.rahman@ugent.be" },
 ]
 license = { file = "LICENSE" }
```

