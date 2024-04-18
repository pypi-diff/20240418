# Comparing `tmp/antakia_core-0.3.8.tar.gz` & `tmp/antakia_core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antakia_core-0.3.8.tar", max compression
+gzip compressed data, was "antakia_core-0.4.0.tar", max compression
```

## Comparing `antakia_core-0.3.8.tar` & `antakia_core-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.3.8/LICENSE
--rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.3.8/README.md
--rw-r--r--   0        0        0      667 2024-04-04 13:38:04.501132 antakia_core-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.3.8/src/antakia_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.3.8/src/antakia_core/compute/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/__init__.py
--rw-r--r--   0        0        0     5676 2024-03-29 13:03:55.191432 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
--rw-r--r--   0        0        0     7771 2024-03-29 13:03:55.166286 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduction.py
--rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
--rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/__init__.py
--rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/classification_models.py
--rw-r--r--   0        0        0     3713 2024-03-19 14:18:22.611148 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_class.py
--rw-r--r--   0        0        0     7347 2024-03-21 13:48:10.207887 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_interface.py
--rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/regression_models.py
--rw-r--r--   0        0        0     1702 2024-03-19 14:18:22.611529 antakia_core-0.3.8/src/antakia_core/compute/skope_rule/skope_rule.py
--rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.3.8/src/antakia_core/data_handler/__init__.py
--rw-r--r--   0        0        0     3968 2024-03-29 13:03:54.732075 antakia_core-0.3.8/src/antakia_core/data_handler/projected_values.py
--rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.3.8/src/antakia_core/data_handler/region.py
--rw-r--r--   0        0        0     8700 2024-03-21 17:21:13.833477 antakia_core-0.3.8/src/antakia_core/data_handler/region_.py
--rw-r--r--   0        0        0    10471 2024-03-19 15:16:36.155976 antakia_core-0.3.8/src/antakia_core/data_handler/region_set.py
--rw-r--r--   0        0        0     9227 2024-03-19 14:18:22.612332 antakia_core-0.3.8/src/antakia_core/data_handler/rule.py
--rw-r--r--   0        0        0     4176 2024-03-22 13:24:54.198488 antakia_core-0.3.8/src/antakia_core/data_handler/rules.py
--rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.3.8/src/antakia_core/explanation/__init__.py
--rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.3.8/src/antakia_core/explanation/explanation_method.py
--rw-r--r--   0        0        0     4761 2024-03-29 13:03:54.922148 antakia_core-0.3.8/src/antakia_core/explanation/explanations.py
--rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.3.8/src/antakia_core/utils/__init__.py
--rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.3.8/src/antakia_core/utils/long_task.py
--rw-r--r--   0        0        0      548 2024-03-29 13:08:53.274643 antakia_core-0.3.8/src/antakia_core/utils/splittable_callback.py
--rw-r--r--   0        0        0     4325 2024-04-04 10:22:26.379728 antakia_core-0.3.8/src/antakia_core/utils/utils.py
--rw-r--r--   0        0        0     6859 2024-03-29 11:27:00.874984 antakia_core-0.3.8/src/antakia_core/utils/variable.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 antakia_core-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.4.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.4.0/README.md
+-rw-r--r--   0        0        0      667 2024-04-18 15:16:58.819461 antakia_core-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.4.0/src/antakia_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.4.0/src/antakia_core/compute/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/__init__.py
+-rw-r--r--   0        0        0     5731 2024-04-18 12:22:43.032815 antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
+-rw-r--r--   0        0        0     7771 2024-03-29 13:03:55.166286 antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/dim_reduction.py
+-rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
+-rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/classification_models.py
+-rw-r--r--   0        0        0     3733 2024-04-18 12:22:43.034037 antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/model_class.py
+-rw-r--r--   0        0        0     7402 2024-04-18 12:22:43.035572 antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/model_interface.py
+-rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/regression_models.py
+-rw-r--r--   0        0        0     1786 2024-04-18 14:48:12.159906 antakia_core-0.4.0/src/antakia_core/compute/skope_rule/skope_rule.py
+-rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.4.0/src/antakia_core/data_handler/__init__.py
+-rw-r--r--   0        0        0     3968 2024-03-29 13:03:54.732075 antakia_core-0.4.0/src/antakia_core/data_handler/projected_values.py
+-rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.4.0/src/antakia_core/data_handler/region.py
+-rw-r--r--   0        0        0     8700 2024-04-18 12:26:06.291697 antakia_core-0.4.0/src/antakia_core/data_handler/region_.py
+-rw-r--r--   0        0        0    10471 2024-03-19 15:16:36.155976 antakia_core-0.4.0/src/antakia_core/data_handler/region_set.py
+-rw-r--r--   0        0        0     9434 2024-04-18 12:22:43.038824 antakia_core-0.4.0/src/antakia_core/data_handler/rule.py
+-rw-r--r--   0        0        0     4176 2024-03-22 13:24:54.198488 antakia_core-0.4.0/src/antakia_core/data_handler/rules.py
+-rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.4.0/src/antakia_core/explanation/__init__.py
+-rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.4.0/src/antakia_core/explanation/explanation_method.py
+-rw-r--r--   0        0        0     4778 2024-04-18 12:22:43.039449 antakia_core-0.4.0/src/antakia_core/explanation/explanations.py
+-rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.4.0/src/antakia_core/utils/__init__.py
+-rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.4.0/src/antakia_core/utils/long_task.py
+-rw-r--r--   0        0        0      548 2024-03-29 13:08:53.274643 antakia_core-0.4.0/src/antakia_core/utils/splittable_callback.py
+-rw-r--r--   0        0        0     4576 2024-04-18 12:22:43.039960 antakia_core-0.4.0/src/antakia_core/utils/utils.py
+-rw-r--r--   0        0        0    12510 2024-04-18 12:24:16.380195 antakia_core-0.4.0/src/antakia_core/utils/variable.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 antakia_core-0.4.0/PKG-INFO
```

### Comparing `antakia_core-0.3.8/LICENSE` & `antakia_core-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/pyproject.toml` & `antakia_core-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antakia-core"
-version = "0.3.8"
+version = "0.4.0"
 description = "Core modules for AntakIA"
 authors = ["Pierre Hulot <pierre@ai-vidence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pandas = "^2.2.0"
```

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduc_method.py` & `antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/dim_reduc_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         """
         std = X.std()
         std[std == 0] = 1
         from sklearn.feature_selection import mutual_info_regression
         chunck_size = 20
         mutual_info_scores = []
         for i in range(0, len(X.T), chunck_size):
-            chunck_mi = mutual_info_regression(X.iloc[:, i:i + chunck_size], y)
+            chunck_mi = mutual_info_regression(X.iloc[:, i:i + chunck_size],
+                                               y.iloc[:])
             mutual_info_scores.append(
                 pd.Series(chunck_mi, index=X.columns[i:i + chunck_size]))
             if progress_callback is not None:
                 progress_callback(i / len(X.T) * 100)
         mi = pd.concat(mutual_info_scores)
         return (X - X.mean()) / std * mi
```

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduction.py` & `antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/dim_reduction.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py` & `antakia_core-0.4.0/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/classification_models.py` & `antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/classification_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_class.py` & `antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/model_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                 self.feature_importances_ = pd.Series(fi.importances_mean,
                                                       index=X.columns)
 
     def fit_and_compute_fi(self, X_train, y_train, X_test, y_test, score,
                            score_type):
         self.fit(X_train, y_train)
         self.compute_feature_importances(X_test, y_test, score, score_type)
+        return self
 
 
 class AvgRegressionBaseline:
 
     def fit(self, X, y, *args, **kwargs):
         self.mean = y.mean()
```

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_interface.py` & `antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/model_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,21 @@
             score: self.available_scores[score]
             for score in scores_list
         }
         self.scores[self.custom_score_str] = (self.custom_score,
                                               self.score_type)
 
     def _train_models(self, X_train, y_train, X_test, y_test):
-        Parallel(n_jobs=1)(delayed(model.fit_and_compute_fi)
-                           (X_train, y_train, X_test, y_test,
-                            self.custom_score, self.score_type)
-                           for model_name, model in self.models.items()
-                           if not model.fitted)
+        models = Parallel(n_jobs=-1)(delayed(model.fit_and_compute_fi)(
+            X_train, y_train, X_test, y_test, self.custom_score,
+            self.score_type) for model_name, model in self.models.items()
+                                     if not model.fitted)
+
+        for model in models:
+            self.models[pretty_model_name(model.name)] = model
 
     def _compute_score_type(self, customer_model, X: pd.DataFrame,
                             y: pd.Series):
         y_pred = customer_model.predict(X)
         s1 = self.custom_score(y_pred, y)
         s2 = self.custom_score(y.sample(len(y)).values, y.values)
         self.score_type = 'maximize' if s1 > s2 else 'minimize'
```

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/regression_models.py` & `antakia_core-0.4.0/src/antakia_core/compute/model_subtitution/regression_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/compute/skope_rule/skope_rule.py` & `antakia_core-0.4.0/src/antakia_core/compute/skope_rule/skope_rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     precision for SKR binary classifer : defaults to 0.7
     recall for SKR binary classifer : defaults to 0.7
     """
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         # We convert df_indexes in row_indexes
         y_train = df_mask.astype(int)
+        if df_mask.all() or not df_mask.any():
+            return RuleSet(), {}
         if variables is None:
-            variables = DataVariables.guess_variables(base_space_df)
+            variables = DataVariables.build_variables(base_space_df, [])
 
         sk_classifier = SkopeRules(
             feature_names=variables.columns_list(),
             random_state=random_state,
             n_estimators=5,
             recall_min=recall,
             precision_min=precision,
```

### Comparing `antakia_core-0.3.8/src/antakia_core/data_handler/projected_values.py` & `antakia_core-0.4.0/src/antakia_core/data_handler/projected_values.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/data_handler/region_.py` & `antakia_core-0.4.0/src/antakia_core/data_handler/region_.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/data_handler/region_set.py` & `antakia_core-0.4.0/src/antakia_core/data_handler/region_set.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/data_handler/rule.py` & `antakia_core-0.4.0/src/antakia_core/data_handler/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,28 +147,33 @@
 
     @property
     def is_categorical_rule(self):
         return self.categorical_rule
 
     def get_matching_mask(self, X: pd.DataFrame) -> pd.Series:
         col = X.loc[:, self.variable.column_name]
+        return self.get_series_matching_mask(col)
+
+    def get_series_matching_mask(self, x: pd.Series) -> pd.Series:
         if self.rule_type == -1:
-            return boolean_mask(X, True)
+            return boolean_mask(x, True)
         if self.rule_type == 0:
-            return col.isin(self.cat_values)  # type:ignore
+            return x.isin(self.cat_values)  # type:ignore
         if self.rule_type == 4:
-            return col == self.min
+            return x == self.min
         if self.rule_type == 5:
-            return boolean_mask(X, False)
-        return getattr(col, self.operator_max)(self.max) & getattr(
-            col, self.operator_min)(self.min)
+            return boolean_mask(x, False)
+        return getattr(x, self.operator_max)(self.max) & getattr(
+            x, self.operator_min)(self.min)
 
     def __call__(self, value: float | pd.DataFrame) -> bool | pd.Series:
         if isinstance(value, pd.DataFrame):
             return self.get_matching_mask(value)
+        if isinstance(value, pd.Series):
+            return self.get_series_matching_mask(value)
         if self.rule_type == -1:
             return True
         if self.rule_type == 0:
             return value in self.cat_values  # type:ignore
         if self.rule_type == 4:
             return value == self.min
         if self.rule_type == 5:
```

### Comparing `antakia_core-0.3.8/src/antakia_core/data_handler/rules.py` & `antakia_core-0.4.0/src/antakia_core/data_handler/rules.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/explanation/explanation_method.py` & `antakia_core-0.4.0/src/antakia_core/explanation/explanation_method.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/explanation/explanations.py` & `antakia_core-0.4.0/src/antakia_core/explanation/explanations.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     SHAP computation class.
     """
 
     def __init__(self,
                  X: pd.DataFrame,
                  model,
-                 task_type,
+                 task_type: ProblemCategory,
                  progress_updated: ProgressCallback | None = None):
         super().__init__(ExplanationMethod.SHAP, X, model, task_type,
                          progress_updated)
 
     @property
     def link(self):
         if self.task_type == ProblemCategory.regression:
```

### Comparing `antakia_core-0.3.8/src/antakia_core/utils/long_task.py` & `antakia_core-0.4.0/src/antakia_core/utils/long_task.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/utils/splittable_callback.py` & `antakia_core-0.4.0/src/antakia_core/utils/splittable_callback.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.8/src/antakia_core/utils/utils.py` & `antakia_core-0.4.0/src/antakia_core/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 """
 Utils module for the antakia package.
 """
 import math
+import os
 import time
 from enum import EnumMeta, Enum
 from numbers import Number
 
 import numpy as np
 from functools import wraps
 
 import pandas as pd
 from pandas.api.types import is_bool_dtype, is_integer_dtype
 
 
+def timeit(method):
+
+    def timed(*args, **kw):
+        if os.environ.get('ATK_DEV') == 'TRUE':
+            ts = time.time()
+            result = method(*args, **kw)
+            te = time.time()
+            if 'log_time' in kw:
+                name = kw.get('log_name', method.__name__.upper())
+                kw['log_time'][name] = int((te - ts) * 1000)
+            else:
+                if te - ts > 0.001:
+                    print(
+                        f'{method.__module__}.{method.__name__}  {(te - ts) * 1000:2.2f} ms'
+                    )
+            return result
+        return method(*args, **kw)
+
+    return timed
+
+
 def in_index(indexes: list, X: pd.DataFrame) -> bool:
     """
     Checks if a list of indexes is in the index of a DataFrame
     """
     try:
         _ = X.loc[indexes]
         return True
@@ -37,51 +59,36 @@
     """
     Converts DataFrame Index numbers to row numbers
     """
     index = pd.Series(np.arange(len(X)), index=X.index)
     return index.loc[indexes_list].tolist()
 
 
+@timeit
 def mask_to_rows(mask: pd.Series) -> list:
     """
     converts a mask to row indices (i.e. iloc)
     """
     return mask_to_index(mask.reset_index(drop=True))
 
 
 def mask_to_index(mask: pd.Series) -> list:
     """
     converts a mask to indices (i.e. loc)
     """
     return mask[mask].index.tolist()
 
 
-def boolean_mask(X: pd.DataFrame, value: bool = True):
+def boolean_mask(X: pd.DataFrame | pd.Series, value: bool = True):
     """
     builds a constant series indexed on X with value as value
     """
     return pd.Series([value] * len(X), index=X.index)
 
 
-def timeit(method):
-
-    def timed(*args, **kw):
-        ts = time.time()
-        result = method(*args, **kw)
-        te = time.time()
-        if 'log_time' in kw:
-            name = kw.get('log_name', method.__name__.upper())
-            kw['log_time'][name] = int((te - ts) * 1000)
-        else:
-            print('%r  %2.2f ms' % (method.__name__, (te - ts) * 1000))
-        return result
-
-    return timed
-
-
 def debug(func):
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         print(
             f"Calling {func.__name__} with args: {args} and kwargs: {kwargs}")
         result = func(*args, **kwargs)
```

### Comparing `antakia_core-0.3.8/PKG-INFO` & `antakia_core-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antakia-core
-Version: 0.3.8
+Version: 0.4.0
 Summary: Core modules for AntakIA
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

