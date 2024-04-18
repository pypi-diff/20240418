# Comparing `tmp/palma-2024.1.1.tar.gz` & `tmp/palma-2024.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palma-2024.1.1.tar", last modified: Mon Jan 22 12:39:56 2024, max compression
+gzip compressed data, was "palma-2024.1.2.tar", last modified: Thu Apr 18 10:00:51 2024, max compression
```

## Comparing `palma-2024.1.1.tar` & `palma-2024.1.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.004748 palma-2024.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-22 12:39:46.000000 palma-2024.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-22 12:39:46.000000 palma-2024.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-01-22 12:39:56.004748 palma-2024.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-01-22 12:39:46.000000 palma-2024.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:55.996748 palma-2024.1.1/palma/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:55.996748 palma-2024.1.1/palma/base/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/base/splitting_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/palma/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/data_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/data_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    16453 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/components/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/palma/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/palma/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/preprocessing/na_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11376 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/preprocessing/pca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/palma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/utils/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    51350 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/utils/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-01-22 12:39:46.000000 palma-2024.1.1/palma/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/palma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-01-22 12:39:55.000000 palma-2024.1.1/palma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-22 12:39:55.000000 palma-2024.1.1/palma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 12:39:55.000000 palma-2024.1.1/palma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-22 12:39:55.000000 palma-2024.1.1/palma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-22 12:39:55.000000 palma-2024.1.1/palma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-22 12:39:46.000000 palma-2024.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 12:39:56.004748 palma-2024.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:39:56.000748 palma-2024.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-22 12:39:46.000000 palma-2024.1.1/tests/test_utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 10:00:47.000000 palma-2024.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 10:00:47.000000 palma-2024.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 10:00:51.789838 palma-2024.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-18 10:00:47.000000 palma-2024.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.781838 palma-2024.1.2/palma/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/splitting_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/data_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/data_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/na_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11376 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/palma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51350 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/palma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 10:00:47.000000 palma-2024.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 10:00:47.000000 palma-2024.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:00:51.789838 palma-2024.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-18 10:00:47.000000 palma-2024.1.2/tests/test_utils_.py
```

### Comparing `palma-2024.1.1/LICENSE` & `palma-2024.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/PKG-INFO` & `palma-2024.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: palma
-Version: 2024.1.1
-Author-email: Vincent Laurent <vlaurent@eurobios.com>
+Version: 2024.1.2
+Author-email: Vincent Laurent <vlaurent@mews-labs.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seaborn>0.12.0
 Requires-Dist: tabulate>0.8.10
 Requires-Dist: frozendict>2.3.4
 Requires-Dist: flaml[automl]>=2
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: numpy>=1
 Requires-Dist: scikit-learn<1.4,>=1
 Requires-Dist: pandas>=1
-Requires-Dist: shap
+Requires-Dist: shap<0.45,>0.40
 Requires-Dist: llvmlite>=0.39
 Requires-Dist: xgboost>2
 Requires-Dist: pyaml>12
 Requires-Dist: llvmlite
 Requires-Dist: numba
 Provides-Extra: components
 Requires-Dist: deepchecks; extra == "components"
@@ -43,15 +43,15 @@
 Requires-Dist: sphinx-favicon; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: sphinx-autoapi; extra == "doc"
 Requires-Dist: sphinx-version-warning; extra == "doc"
 Requires-Dist: sphinx-prompt; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 
-<img src="./.static/logo.png" width="200"/>
+<img src=".static/logo.png" width="200"/>
 
 ### _Project for Automated Learning MAchine_ 
 
 [![Maintenance](https://img.shields.io/badge/maintained%3F-yes-green.svg)](https://GitHub.com/eurobios-mews-labs/palma/graphs/commit-activity)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![pytest](https://github.com/eurobios-scb/palma/actions/workflows/pytest.yml/badge.svg?event=push)](https://docs.pytest.org)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
```

### Comparing `palma-2024.1.1/README.md` & `palma-2024.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="./.static/logo.png" width="200"/>
+<img src=".static/logo.png" width="200"/>
 
 ### _Project for Automated Learning MAchine_ 
 
 [![Maintenance](https://img.shields.io/badge/maintained%3F-yes-green.svg)](https://GitHub.com/eurobios-mews-labs/palma/graphs/commit-activity)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![pytest](https://github.com/eurobios-scb/palma/actions/workflows/pytest.yml/badge.svg?event=push)](https://docs.pytest.org)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
```

### Comparing `palma-2024.1.1/palma/__init__.py` & `palma-2024.1.2/palma/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/base/__init__.py` & `palma-2024.1.2/palma/base/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/base/engine.py` & `palma-2024.1.2/palma/base/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 from abc import ABCMeta, abstractmethod
 from typing import Dict, Union
 
 import pandas as pd
 from flaml import AutoML
 from sklearn import base
 
+from palma.base.splitting_strategy import ValidationStrategy
+
 try:
     from autosklearn.classification import AutoSklearnClassifier
     from autosklearn.regression import AutoSklearnRegressor
 except ImportError:
     pass
 
 
 class BaseOptimizer(object, metaclass=ABCMeta):
 
     def __init__(self, engine_parameters: dict) -> None:
         self.__engine_parameters = engine_parameters
 
     @abstractmethod
-    def optimize(self, X: pd.DataFrame, y: pd.Series, splitter=None
+    def optimize(self, X: pd.DataFrame, y: pd.Series,
+                 splitter: "ValidationStrategy" = None
                  ) -> None:
         ...
 
     @property
     @abstractmethod
     def optimizer(self) -> None:
         ...
@@ -83,21 +86,21 @@
 
         self.__optimizer.fit(X, y)
         self.__optimizer.refit(X, y)
 
     @property
     def optimizer(self) -> Union[
         'AutoSklearnClassifier',
-            'AutoSklearnRegressor']:
+        'AutoSklearnRegressor']:
         return self.__optimizer
 
     @property
     def estimator_(self) -> Union[
         'AutoSklearnClassifier',
-            'AutoSklearnRegressor']:
+        'AutoSklearnRegressor']:
         return self.__optimizer.get_models_with_weights()
 
     @property
     def transformer_(self):
         ...
 
 
@@ -107,22 +110,28 @@
 
         if "task" in engine_parameters.keys():
             logging.info(
                 f"The problem is already provided through project object ({problem})"
             )
         engine_parameters["task"] = problem
 
-    def optimize(self, X: pd.DataFrame, y: pd.DataFrame, splitter=None
+    def optimize(self, X: pd.DataFrame, y: pd.DataFrame,
+                 splitter: ValidationStrategy = None
                  ) -> None:
+        split_type = None if splitter is None else splitter.splitter
+        groups = None if splitter is None else splitter.groups
+        groups = groups if groups is None else groups[splitter.train_index]
+
         self.allowing_splitter(splitter)
         self.__optimizer = AutoML()
         self.__optimizer.fit(
             X_train=pd.DataFrame(X.values, index=range(len(X))),
             y_train=pd.Series(y.values, index=range(len(X))),
-            split_type=splitter, mlflow_logging=False,
+            split_type=split_type, groups=groups,
+            mlflow_logging=False,
             **self.engine_parameters
         )
 
     @property
     def optimizer(self) -> AutoML:
         return self.__optimizer
```

### Comparing `palma-2024.1.1/palma/base/model.py` & `palma-2024.1.2/palma/base/model.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/base/model_selection.py` & `palma-2024.1.2/palma/base/model_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,19 +43,25 @@
 
         )
 
         logging.disable()
         self.engine_.optimize(
             project.X.iloc[project.validation_strategy.train_index],
             project.y.iloc[project.validation_strategy.train_index],
-            splitter=project.validation_strategy.splitter
+            splitter=project.validation_strategy,
         )
         self.best_model_ = self.engine_.estimator_
         logging.basicConfig(level=logging.DEBUG)
 
         logger.logger.log_artifact(
             self.engine_.estimator_,
             self.__run_id)
+        try:
+            logger.logger.log_metrics(
+                {"best_estimator": str(self.best_model_)}, 'model_selection'
+            )
+        except:
+            pass
 
     @property
     def run_id(self) -> str:
         return self.__run_id
```

### Comparing `palma-2024.1.1/palma/base/project.py` & `palma-2024.1.2/palma/base/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             X_test=None, y_test=None,
             groups=None,
             **kwargs
     ) -> None:
         from palma.utils.checker import ProjectPlanChecker
         from palma import logger
         self.__validation_strategy = ValidationStrategy(splitter)
-        self.__base_index = list(range(len(X)))
         self.__X, self.__y = self.__validation_strategy(
             X=X, y=y, X_test=X_test, y_test=y_test,
             groups=groups)
         ProjectPlanChecker().run_checks(self)
         self.__data_id = blake2b(
             pd.util.hash_pandas_object(
                 pd.concat([self.__X, self.__y], axis=1)
@@ -105,18 +104,14 @@
         self.__is_started = True
 
     def __call_components(self, object_: "Project") -> None:
         for _, component in self.components.items():
             component(object_)
 
     @property
-    def base_index(self) -> List[int]:
-        return self.__base_index
-
-    @property
     def components(self) -> dict:
         return self.__components
 
     @property
     def date(self) -> datetime:
         return self.__date
```

### Comparing `palma-2024.1.1/palma/base/splitting_strategy.py` & `palma-2024.1.2/palma/base/splitting_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             splitter: Union[
                 BaseShuffleSplit,
                 BaseCrossValidator,
                 List[tuple],
                 List[str]],
             **kwargs
     ) -> None:
-
+        self.__groups = None
         self.__splitter = splitter
         if hasattr(self.__splitter, "split"):
             self._splitter_args = self.__splitter.__dict__
         else:
             self._splitter_args = ""
         if hasattr(self.__splitter, "random_state"):
             if getattr(self.__splitter, "random_state") is None:
@@ -94,15 +94,15 @@
         -----------
         - X (pd.DataFrame): The feature data for the project.
         - y (pd.Series): The target variable for the project.
         - X_test (pd.DataFrame): Optional test feature data.
         - y_test (pd.Series): Optional test target variable.
         - groups: Optional grouping information.
         """
-
+        self.__groups = groups
         if X_test is not None and y_test is not None:
             n_train, n_test = len(X), len(X_test)
             X = pd.concat((X, X_test), axis=0)
             y = pd.concat((y, y_test), axis=0)
             self._train_index = np.array(range(n_train))
             self._test_index = np.array(range(n_train, n_train + n_test))
         else:
@@ -162,7 +162,13 @@
     @property
     def id(self):
         return self.__id
 
     @property
     def splitter(self):
         return self.__splitter
+
+    @property
+    def groups(self):
+        if self.__groups is None:
+            return None
+        return np.array(self.__groups)
```

### Comparing `palma-2024.1.1/palma/components/__init__.py` & `palma-2024.1.2/palma/components/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/components/base.py` & `palma-2024.1.2/palma/components/base.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/components/checker.py` & `palma-2024.1.2/palma/components/checker.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/components/dashboard.py` & `palma-2024.1.2/palma/components/dashboard.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/components/data_checker.py` & `palma-2024.1.2/palma/components/data_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             logger.logger.log_artifact(results, f'{results.name}')
 
         list_results = [
             *self.train_test_checks_results.get_not_passed_checks(),
             *self.dataset_checks_results.get_not_passed_checks(),
         ]
         if self.raise_on_fail and len(list_results):
-            line = "="*50
+            line = "=" * 50
             raise ValueError(
                 f"The following tests did not pass :"
                 f"{line}\n"
                 f"{list_results}\n"
                 f"{line}")
 
     def __generate_datasets(self, project: Project, **kwargs) -> None:
@@ -130,15 +130,14 @@
         self.__dataset = Dataset(df, label="target", **kwargs)
 
         self.__train_dataset = self.__dataset.copy(
             df.loc[project.validation_strategy.train_index])
         self.__test_dataset = self.__dataset.copy(
             df.loc[project.validation_strategy.test_index])
 
-
     @staticmethod
     def __generate_suite(
             checks: Union[List[BaseCheck], BaseSuite],
             name: str
     ) -> Suite:
         """
         Generate a Suite of checks from a list of checks or a suite of checks
@@ -166,17 +165,14 @@
             raise TypeError(
                 "checks must be a list of instances of "
                 "class BaseCheck or an instance of class Suite"
             )
 
         return suite
 
-    def __str__(self) -> str:
-        return "DeepCheck"
-
 
 class Leakage(ProjectComponent):
     """
     Class for detecting data leakage in a classification project.
 
     This class implements component that checks for data leakage in a given
     project. It uses the FLAML optimizer for model selection and performs
```

### Comparing `palma-2024.1.1/palma/components/data_profiler.py` & `palma-2024.1.2/palma/components/data_profiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and limitations under the License.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import pandas as pd
 
 from palma.components.base import ProjectComponent
 
 try:
     from pandas_profiling import ProfileReport
```

### Comparing `palma-2024.1.1/palma/components/logger.py` & `palma-2024.1.2/palma/components/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             The metrics to be logged.
         path : str
             The relative path (from the study directory)
             where the metrics JSON file will be saved.
         """
         path = f"{self.path_study}/{path}.json"
         with open(path, 'w') as output_file:
-            _logger.info("Metrics saved in {}".format(path))
+            _logger.info(f"Metrics saved in {path}")
             json.dump(metrics, output_file, indent=4)
 
     def log_artifact(self, obj, path: str) -> None:
         """
         Logs an artifact, handling different types of objects.
 
         Parameters
```

### Comparing `palma-2024.1.1/palma/components/performance.py` & `palma-2024.1.2/palma/components/performance.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,32 +13,38 @@
 from abc import ABCMeta
 
 import matplotlib.pyplot as plot
 import numpy as np
 import pandas as pd
 import shap
 from sklearn import metrics
+from sklearn.metrics import _regression, _ranking
 
 from palma.components.base import ModelComponent
-from palma.utils import plotting, utils
 from palma.components.logger import logger
+from palma.utils import plotting, utils
 
-
-colors = ['r', 'b', '#33cc33', '#ff6600', "darkblue", '#9933ff',
-          '#99cc00', '#3399ff'] * 50
-
-colors_rainbow = [plot.get_cmap("rainbow")(1 - i / 4) for i in range(5)] * 3
+__fpr_sampling__ = np.linspace(0, 1, 200)
 
 
 class Analyser(ModelComponent, metaclass=ABCMeta):
-    metrics = {}
-    _metrics = {}
+    """
+    Analyser class for performing analysis on a model.
+
+    Parameters
+    ----------
+    on : str
+        The type of analysis to perform. Possible values are
+        "indexes_train_test" or "indexes_val".
+    """
 
     def __init__(self, on):
         self.__on = on
+        self.__metrics = {}
+        self._hidden_metrics = {}
 
     def __call__(self, project: "Project", model: "ModelEvaluation"):
         self._add(project, model)
 
     def _add(self, project, model):
 
         if self.__on == "indexes_train_test":
@@ -57,65 +63,141 @@
                 f"'indexes_train_test' or 'indexes_val'")
         self.X = project.X
         self.y = project.y
 
         __tmp = utils._get_processing_pipeline(self.estimators)
         self.preproc_estimators, self.only_estimators = __tmp
         self._is_regression = project.problem == "regression"
+        if project.problem == "regression":
+            for metric in _regression.__ALL__:
+                try:
+                    self.compute_metrics({metric: getattr(_regression, metric)})
+                except ValueError:
+                    pass
+        elif project.problem == "classification":
+            for metric in ["roc_auc_score",
+                           "label_ranking_average_precision_score",
+                           "coverage_error", "label_ranking_loss", "dcg_score"]:
+                try:
+                    self.compute_metrics({metric: getattr(_ranking, metric)})
+                except ValueError:
+                    pass
 
     def variable_importance(self):
+        """
+        Compute the feature importance for each estimator.
+
+        Returns
+        -------
+        feature_importance : pandas.DataFrame
+            DataFrame containing the feature importance values for each estimator.
+        """
         feature_importance = pd.DataFrame(columns=self.X.columns)
         for i, _ in enumerate(self.indexes):
             importance = utils._get_and_check_var_importance(
                 self.estimators[i])
             feature_importance.loc[i, :] = importance
         return feature_importance.T
 
     def compute_metrics(self, metric: dict):
+        """
+        Compute the specified metrics for each estimator.
+
+        Parameters
+        ----------
+        metric : dict
+            Dictionary containing the metric name as key and the metric function as value.
+        """
         from palma import logger
         for name, fun in metric.items():
             self._compute_metric(name, fun)
-        logger.logger.log_metrics(
-            {k: str(v) for k, v in self.get_test_metrics().to_dict().items()},
-            path="metrics")
+
+        for m_name, metric_fold in self.get_test_metrics().to_dict().items():
+            for k, v in metric_fold.items():
+                if isinstance(v, float) or isinstance(v, int):
+                    logger.logger.log_metrics(
+                        {f"{m_name}_fold{k}": v}, path="metrics")
 
     def _compute_metric(self, name: str, fun: typing.Callable):
-        """Compute on specific metric and add it to 'metric' attribute"""
-        self.metrics[name] = {}
+        """
+        Compute a specific metric and add it to the metrics attribute.
+
+        Parameters
+        ----------
+        name : str
+            The name of the metric.
+        fun : callable
+            The function to compute the metric.
+        """
+        self.__metrics[name] = {}
         for i, (train, test) in enumerate(self.indexes):
-            self.metrics[name][i] = dict(
+            self.__metrics[name][i] = dict(
                 train=fun(self.y.iloc[train],
                           self.predictions[i]["train"]),
                 test=fun(self.y.iloc[test],
                          self.predictions[i]["test"])
             )
 
     def get_train_metrics(self) -> pd.DataFrame:
+        """
+        Get the computed metrics for the training set.
+
+        Returns
+        -------
+        pd.DataFrame
+            DataFrame containing the computed metrics for the training set.
+        """
         return self.__get_metrics_helper("train")
 
     def get_test_metrics(self) -> pd.DataFrame:
+        """
+        Get the computed metrics for the test set.
+
+        Returns
+        -------
+        pd.DataFrame
+            DataFrame containing the computed metrics for the test set.
+        """
         return self.__get_metrics_helper("test")
 
     def __get_metrics_helper(self, identifier) -> pd.DataFrame:
-        m = self.metrics
+        m = self.__metrics
         ret = pd.DataFrame(columns=list(m.keys()),
                            index=m[list(m.keys())[0]].keys())
         for k in m.keys():
             for f in m[k].keys():
                 ret.loc[f, k] = m[k][f][identifier]
         return ret
 
     def plot_variable_importance(self, mode="minmax",
                                  color="darkblue",
-                                 cmap="flare"):
+                                 cmap="flare", **kwargs):
+        """
+        Plot the variable importance.
+
+        Parameters
+        ----------
+        mode : str, optional
+            The mode for plotting the variable importance, by default "minmax".
+        color : str, optional
+            The color for the plot, by default "darkblue".
+        cmap : str, optional
+            The colormap for the plot, by default "flare".
+        """
         from palma.utils.plotting import plot_variable_importance
         plot_variable_importance(
-            self.variable_importance(), mode=mode, color=color, cmap=cmap)
+            self.variable_importance(), mode=mode, color=color, cmap=cmap,
+            **kwargs
+        )
         logger.logger.log_artifact(plot.gcf(), "variable_importance")
 
+    @property
+    def metrics(self):
+        return self.__metrics
+
 
 class ShapAnalysis(Analyser):
 
     def __init__(self, on, n_shap, compute_interaction=False):
         super().__init__(on)
         self.n_shap = n_shap
         self.compute_interaction = compute_interaction
@@ -211,47 +293,63 @@
             display_features=self.shap_X
         )
         logger.logger.log_artifact(plot.gcf(), f"shap_interaction_"
                                                f"{feature_x}_{feature_y}")
 
 
 class ScoringAnalysis(Analyser):
-    mean_fpr = np.linspace(0, 1, 100)
+    """
+    The ScoringAnalyser class provides methods for analyzing the performance of
+    a machine learning model.
+    """
+
+    def __init__(self, on):
+        super().__init__(on)
 
     def confusion_matrix(self, in_percentage=False):
+        """
+        Compute the confusion matrix.
 
-        cv = self.indexes.copy()
+        Parameters
+        ----------
+        in_percentage : bool, optional
+            Whether to return the confusion matrix in percentage, by default False
 
-        mat_ = np.array([[0, 0], [0, 0]])
-        for i, (_, val) in enumerate(cv):
+        Returns
+        -------
+        pandas.DataFrame
+            The confusion matrix
+        """
+
+        matrix = np.array([[0, 0], [0, 0]])
+        for i, (_, val) in enumerate(self.indexes):
             proba = self.estimators[i].predict_proba(self.X.iloc[val])[:, -1]
             y_pred = proba > self.threshold
-            mat_ += metrics.confusion_matrix(self.y.iloc[val], y_pred)
-            mat_ = mat_ / len(cv)
+            matrix += metrics.confusion_matrix(self.y.iloc[val], y_pred)
+            matrix = matrix / len(self.indexes)
         columns = ['predicted : 0', 'predicted : 1']
         index = ['real : 0', 'real : 1']
 
-        mat_ = pd.DataFrame(mat_, index=index, columns=columns,
-                            ).round(decimals=1)
+        matrix = pd.DataFrame(matrix, index=index, columns=columns,
+                              ).round(decimals=1)
         if in_percentage:
-            mat_ = mat_ / mat_.sum().sum() * 100
-            mat_ = mat_.round(decimals=1)
-        return mat_
+            matrix = matrix / matrix.sum().sum() * 100
+            matrix = matrix.round(decimals=1)
+        return matrix
 
     def __interpolate_roc(self, _):
-        self._metrics["roc_curve_interp"] = utils.interpolate_roc(
-            self.metrics["roc_curve"], self.mean_fpr)
+        self._hidden_metrics["roc_curve_interp"] = utils.interpolate_roc(
+            self.metrics["roc_curve"], __fpr_sampling__)
 
     def plot_roc_curve(
             self,
             plot_method="mean",
             plot_train: bool = False,
-            c=colors[0],
+            c='C0',
             cmap: str = "inferno",
-            cv_iter=None,
             label: str = "",
             mode: str = "std",
             label_iter: iter = None,
             plot_base: bool = True,
             **kwargs):
         """
         Plot the ROC curve.
@@ -270,116 +368,188 @@
             If True the train ROC curves will be plot, default False.
 
         c: str
             Not used only with plot_method="all". Set the color of ROC curve
 
         cmap: str
 
-        cv_iter
         label
         mode
         label_iter
         plot_base: bool,
             Plot basic ROC curve helper
         kwargs:
             Deprecated
 
         Returns
         -------
 
         """
         self._compute_metric("roc_curve", metrics.roc_curve)
-        self.label = label
-        if cv_iter is not None:
-            cv = list(np.array(self.indexes)[cv_iter])
-        else:
-            cv = self.indexes.copy()
-        self.__interpolate_roc(cv)
-        roc = self._metrics["roc_curve_interp"]
+
+        self.__interpolate_roc(self.indexes)
+        roc = self._hidden_metrics["roc_curve_interp"]
 
         select_i = "train" if plot_train else "test"
-        list_tpr = [roc[i][select_i][1] for i in range(len(cv))]
-        list_fpr = [roc[i][select_i][0] for i in range(len(cv))]
+        list_tpr = [roc[i][select_i][1] for i in range(len(self.indexes))]
+        list_fpr = [roc[i][select_i][0] for i in range(len(self.indexes))]
 
         if plot_method not in ["beam", "all", "mean"]:
             raise ValueError(
                 f"argument plot_method={plot_method} is not recognize")
 
         plot_all: bool = plot_method == "all"
         plot_beam: bool = plot_method == "beam"
         plot_mean: bool = plot_method == "mean"
 
-        plotting.roc_plot_bundle(list_fpr, list_tpr, mean_fpr=self.mean_fpr,
+        plotting.roc_plot_bundle(list_fpr, list_tpr, mean_fpr=__fpr_sampling__,
                                  plot_all=plot_all, plot_beam=plot_beam,
                                  label_iter=label_iter,
                                  cmap=cmap, plot_mean=plot_mean,
-                                 c=c, mode=mode, label=self.label)
+                                 c=c, mode=mode, label=label)
 
         if plot_base:
             plotting.roc_plot_base()
 
         logger.logger.log_artifact(plot.gcf(), "roc_curve")
         return plot
 
     def compute_threshold(
             self,
             method: str = "total_population",
             value: float = 0.5,
             metric: typing.Callable = None):
-        """Compute threshold using various heuristics"""
+        """
+        Compute threshold using various heuristics
+
+        Parameters
+        ----------
+        method : str, optional
+            The method to compute the threshold, by default "total_population"
+
+            - total population : compute threshold so that the percentage of
+            positive prediction is equal to `value`
+            - fpr : compute threshold so that the false positive rate
+            is equal to `value`
+            - optimize_metric : compute threshold so that the metric is optimized
+            `value` parameter is ignored, `metric` parameter must be provided
+
+        value : float, optional
+            The value to use for the threshold computation, by default 0.5
+        metric : typing.Callable, optional
+            The metric function to use for the threshold computation, by default None
+
+        Returns
+        -------
+        float
+            The computed threshold
+        """
         th = []
 
         if method == "total_population":
             for i, _ in enumerate(self.indexes):
                 th.append(np.percentile(self.predictions[i]["test"], value))
         elif method == "fpr":
             if "roc_curve" not in self.metrics.keys():
                 self._compute_metric("roc_curve", metrics.roc_curve)
             self.__interpolate_roc(self.indexes)
             for i, _ in enumerate(self.indexes):
-                roc = self._metrics["roc_curve_interp"][i]["test"]
+                roc = self._hidden_metrics["roc_curve_interp"][i]["test"]
                 idx = np.argmin(np.abs(roc[0] - value))
                 th.append(roc[2][idx])
         elif method == "optimize_metric":
             name = "threshold_criterion"
             if metric is None:
                 raise ValueError("Argument metric must not be not None")
-            self._metrics[name] = {}
+            self._hidden_metrics[name] = {}
             for i, (train, test) in enumerate(self.indexes):
                 ths = np.unique(self.predictions[i]["test"])
                 temp = {}
                 for th_ in ths:
                     temp[th_] = metric(
                         self.y.iloc[test],
                         self.predictions[i]["test"] > th_)
-                self._metrics[name][i] = dict(test=pd.Series(temp).idxmax())
-                th = [self._metrics[name][i]["test"] for i in
-                      self._metrics[name].keys()]
+                self._hidden_metrics[name][i] = dict(
+                    test=pd.Series(temp).idxmax())
+                th = [self._hidden_metrics[name][i]["test"] for i in
+                      self._hidden_metrics[name].keys()]
         else:
             raise ValueError(f"method {method} is not recognized")
         self.__threshold = np.nanmean(th)
         return self.__threshold
 
     def plot_threshold(self, **plot_kwargs):
+        """
+        Plot the threshold on fpr/tpr axes
+
+        Parameters
+        ----------
+        plot_kwargs : dict, optional
+            Additional keyword arguments to pass to the scatter plot function
+
+        Returns
+        -------
+        matplotlib.pyplot
+            The threshold plot
+        """
         fpr = []
         tpr = []
         for i, _ in enumerate(self.indexes):
-            roc = self._metrics["roc_curve_interp"][i]["test"]
+            roc = self._hidden_metrics["roc_curve_interp"][i]["test"]
             idx = np.argmin(np.abs(roc[2] - self.__threshold))
             fpr.append(roc[0][idx])
             tpr.append(roc[1][idx])
         plot.scatter(fpr, tpr, **plot_kwargs)
         logger.logger.log_artifact(plot.gcf(), "roc_threshold")
 
     @property
     def threshold(self):
         return self.__threshold
 
 
 class RegressionAnalysis(Analyser):
+    """
+    Analyser class for performing analysis on a regression model.
+
+    Parameters
+    ----------
+    on : str
+        The type of analysis to perform. Possible values are
+        "indexes_train_test" or "indexes_val".
+
+    Attributes
+    ----------
+    _hidden_metrics : dict
+        Dictionary to store additional metrics that are not displayed.
+
+    Methods
+    -------
+    variable_importance()
+        Compute the feature importance for each estimator.
+    compute_metrics(metric: dict)
+        Compute the specified metrics for each estimator.
+    get_train_metrics() -> pd.DataFrame
+        Get the computed metrics for the training set.
+    get_test_metrics() -> pd.DataFrame
+        Get the computed metrics for the test set.
+    plot_variable_importance(mode="minmax", color="darkblue", cmap="flare")
+        Plot the variable importance.
+    plot_prediction_versus_real
+        Plot prediction versus real values
+    plot_errors_pairgrid
+        Plot pair grid errors
+
+    Properties
+    ----------
+    metrics : dict
+        The computed metrics.
+    """
+
+    def __init__(self, on):
+        super().__init__(on)
 
     def compute_predictions_errors(self, fun=None):
         self.errors = {}
         if fun is None:
             def fun(yt_, yp_):
                 return (yt_ - yp_) ** 2
 
@@ -426,9 +596,7 @@
         g = sns.PairGrid(df_plot, hue="error quartile", palette=palette,
                          x_vars=features, y_vars=features,
                          )
         g.map_diag(sns.histplot, multiple="stack")
         g.map_offdiag(sns.scatterplot, size=df_plot["error"])
         g.add_legend(title="", adjust_subtitles=True)
         logger.logger.log_artifact(plot.gcf(), "pair_grid")
-
-
```

### Comparing `palma-2024.1.1/palma/datasets/__init__.py` & `palma-2024.1.2/palma/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/preprocessing/__init__.py` & `palma-2024.1.2/palma/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/preprocessing/na_encoder.py` & `palma-2024.1.2/palma/preprocessing/na_encoder.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/preprocessing/pca.py` & `palma-2024.1.2/palma/preprocessing/pca.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/utils/__init__.py` & `palma-2024.1.2/palma/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/utils/checker.py` & `palma-2024.1.2/palma/utils/checker.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/utils/names.py` & `palma-2024.1.2/palma/utils/names.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma/utils/plotting.py` & `palma-2024.1.2/palma/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 def plot_variable_importance(
         variable_importance: pd.DataFrame,
         mode="minmax",
         color="darkblue",
         cmap="flare",
-        alpha=0.2,
+        alpha=0.2, **kwargs
 ):
     variable_importance = variable_importance.copy()
     variable_importance.index = variable_importance.index.astype(str)
     m = np.array(variable_importance.mean(axis=1)).ravel()
     variable_importance["mean"] = m
 
     variable_importance = variable_importance.sort_values(
```

### Comparing `palma-2024.1.1/palma/utils/utils.py` & `palma-2024.1.2/palma/utils/utils.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.1/palma.egg-info/PKG-INFO` & `palma-2024.1.2/palma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: palma
-Version: 2024.1.1
-Author-email: Vincent Laurent <vlaurent@eurobios.com>
+Version: 2024.1.2
+Author-email: Vincent Laurent <vlaurent@mews-labs.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seaborn>0.12.0
 Requires-Dist: tabulate>0.8.10
 Requires-Dist: frozendict>2.3.4
 Requires-Dist: flaml[automl]>=2
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: numpy>=1
 Requires-Dist: scikit-learn<1.4,>=1
 Requires-Dist: pandas>=1
-Requires-Dist: shap
+Requires-Dist: shap<0.45,>0.40
 Requires-Dist: llvmlite>=0.39
 Requires-Dist: xgboost>2
 Requires-Dist: pyaml>12
 Requires-Dist: llvmlite
 Requires-Dist: numba
 Provides-Extra: components
 Requires-Dist: deepchecks; extra == "components"
@@ -43,15 +43,15 @@
 Requires-Dist: sphinx-favicon; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: sphinx-autoapi; extra == "doc"
 Requires-Dist: sphinx-version-warning; extra == "doc"
 Requires-Dist: sphinx-prompt; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 
-<img src="./.static/logo.png" width="200"/>
+<img src=".static/logo.png" width="200"/>
 
 ### _Project for Automated Learning MAchine_ 
 
 [![Maintenance](https://img.shields.io/badge/maintained%3F-yes-green.svg)](https://GitHub.com/eurobios-mews-labs/palma/graphs/commit-activity)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![pytest](https://github.com/eurobios-scb/palma/actions/workflows/pytest.yml/badge.svg?event=push)](https://docs.pytest.org)
 [![PyPI version](https://badge.fury.io/py/palma.svg)](https://badge.fury.io/py/palma)
```

### Comparing `palma-2024.1.1/palma.egg-info/SOURCES.txt` & `palma-2024.1.2/palma.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 palma/__init__.py
 palma.egg-info/PKG-INFO
 palma.egg-info/SOURCES.txt
 palma.egg-info/dependency_links.txt
 palma.egg-info/requires.txt
 palma.egg-info/top_level.txt
 palma/base/__init__.py
```

### Comparing `palma-2024.1.1/tests/test_utils_.py` & `palma-2024.1.2/tests/test_utils_.py`

 * *Files identical despite different names*

