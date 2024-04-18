# Comparing `tmp/moval-0.3.0.tar.gz` & `tmp/moval-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-pezhdkot/moval-0.3.0.tar", last modified: Wed Apr 17 16:32:33 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-6icvosnx/moval-0.3.1.tar", last modified: Thu Apr 18 18:39:13 2024, max compression
```

## Comparing `moval-0.3.0.tar` & `moval-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.647933 moval-0.3.0/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-17 16:32:33.647867 moval-0.3.0/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.0/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.641573 moval-0.3.0/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-17 16:31:59.000000 moval-0.3.0/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.642856 moval-0.3.0/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.0/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.643589 moval-0.3.0/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.0/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.0/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.645971 moval-0.3.0/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.0/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.0/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.0/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.0/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10841 2024-04-17 16:31:30.000000 moval-0.3.0/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.0/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.647308 moval-0.3.0/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.0/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.0/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    28535 2024-04-17 02:17:24.000000 moval-0.3.0/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.0/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-17 16:32:33.647606 moval-0.3.0/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-17 16:32:33.000000 moval-0.3.0/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-17 16:32:33.000000 moval-0.3.0/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-17 16:32:33.000000 moval-0.3.0/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-17 16:32:33.000000 moval-0.3.0/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-17 16:32:33.000000 moval-0.3.0/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.0/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-17 16:32:33.648288 moval-0.3.0/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002766 moval-0.3.1/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-18 18:39:13.002702 moval-0.3.1/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.1/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:12.999312 moval-0.3.1/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-18 18:38:14.000000 moval-0.3.1/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.000112 moval-0.3.1/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.1/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.000406 moval-0.3.1/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.1/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.1/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.001464 moval-0.3.1/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.1/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.1/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.1/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.1/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10841 2024-04-17 16:31:30.000000 moval-0.3.1/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.1/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002199 moval-0.3.1/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.1/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.1/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    28961 2024-04-18 18:36:48.000000 moval-0.3.1/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.1/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002428 moval-0.3.1/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.1/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-18 18:39:13.003157 moval-0.3.1/setup.cfg
```

### Comparing `moval-0.3.0/PKG-INFO` & `moval-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.0
+Version: 0.3.1
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.0 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.1 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.0/README.md` & `moval-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/__init__.py` & `moval-0.3.1/moval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.3.0/moval/integrations/sklearn/moval.py` & `moval-0.3.1/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/models/confidences.py` & `moval-0.3.1/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/models/model.py` & `moval-0.3.1/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/models/solver_temperature.py` & `moval-0.3.1/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/models/utils.py` & `moval-0.3.1/moval/models/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/registry.py` & `moval-0.3.1/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/solvers/criterions.py` & `moval-0.3.1/moval/solvers/criterions.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval/solvers/solver.py` & `moval-0.3.1/moval/solvers/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,26 +309,28 @@
                         # change the initial state, if we are not satisfied with the optimization results.
                         print(f"Not satisfied with initial optimization results of param for class {opt_kcls}, trying more initial states...")
                         if self.model.estim_algorithm == "atc-model":
                             score = self.model.conf(inp)
                             if self.model.conf.normalization:
                                 score = self.model._normalize(score)
                             if self.model.mode == "classification":
-                                score_ = score[np.argmax(inp, axis = 1) == kcls]
+                                for kcls in range(self.batch * opt_kcls, np.min((self.batch * (opt_kcls + 1), self.model.num_class))):
+                                    score_.append(score[np.argmax(inp, axis = 1) == kcls])
+                                score_ = np.concatenate(score_)
                                 initial_conditions = [np.array([np.percentile(score_, 20)]), 
                                                       np.array([np.percentile(score_, 40)]), 
                                                       np.array([np.percentile(score_, 50)]), 
                                                       np.array([np.percentile(score_, 60)]), 
                                                       np.array([np.percentile(score_, 80)])]
                             else:
                                 score_ = []
                                 for n_case in range(len(inp)):
                                     score_flatten = score[n_case].flatten() # ``n``
                                     pred_flatten = np.argmax(inp[n_case], axis = 0).flatten()
-                                    score_.append(score_flatten[pred_flatten == kcls])
+                                    score_.append(score_flatten[pred_flatten == opt_kcls])
                                 score_ = np.concatenate(score_)
                                 initial_conditions = [np.array([np.percentile(score_, 20)]), 
                                                       np.array([np.percentile(score_, 50)])]
                         results = []
                         results.append((optimization_result.fun, optimization_result.x[0]))
                         cnt_guess = 0
                         for initial_guess in initial_conditions:
@@ -441,26 +443,28 @@
                         if optimization_result.fun > search_threshold:
                             # change the initial state, if we are not satisfied with the optimization results.
                             print(f"Not satisfied with initial optimization results of param_ext for class {opt_kcls}, trying more initial states...")
                             # change atc to be consistent with the range of confidence score
                             # get the max and min value here.
                             score = self.model.calibrate(inp, midstage = True)
                             if self.model.mode == "classification":
-                                score_ = score[np.argmax(inp, axis = 1) == kcls]
+                                for kcls in range(self.batch * opt_kcls, np.min((self.batch * (opt_kcls + 1), self.model.num_class))):
+                                    score_.append(score[np.argmax(inp, axis = 1) == kcls])
+                                score_ = np.concatenate(score_)
                                 initial_conditions_atc = [np.array([np.percentile(score_, 20)]), 
                                                             np.array([np.percentile(score_, 40)]), 
                                                             np.array([np.percentile(score_, 50)]), 
                                                             np.array([np.percentile(score_, 60)]), 
                                                             np.array([np.percentile(score_, 80)])]
                             else:
                                 score_ = []
                                 for n_case in range(len(inp)):
                                     score_flatten = score[n_case].flatten() # ``n``
                                     pred_flatten = np.argmax(inp[n_case], axis = 0).flatten()
-                                    score_.append(score_flatten[pred_flatten == kcls])
+                                    score_.append(score_flatten[pred_flatten == opt_kcls])
                                 score_ = np.concatenate(score_)
                                 initial_conditions_atc = [np.array([np.percentile(score_, 20)]), 
                                                             np.array([np.percentile(score_, 50)])]
                             results = []
                             results.append((optimization_result.fun, optimization_result.x[0]))
                             cnt_guess = 0
                             for initial_guess in initial_conditions_atc:
```

### Comparing `moval-0.3.0/moval/solvers/utils.py` & `moval-0.3.1/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/moval.egg-info/PKG-INFO` & `moval-0.3.1/moval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.0
+Version: 0.3.1
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.0 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.1 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.0/moval.egg-info/SOURCES.txt` & `moval-0.3.1/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/pyproject.toml` & `moval-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.3.0/setup.cfg` & `moval-0.3.1/setup.cfg`

 * *Files identical despite different names*

