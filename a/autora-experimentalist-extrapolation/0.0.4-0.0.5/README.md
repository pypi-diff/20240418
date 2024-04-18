# Comparing `tmp/autora_experimentalist_extrapolation-0.0.4.tar.gz` & `tmp/autora_experimentalist_extrapolation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experimentalist_extrapolation-0.0.4.tar", last modified: Thu Apr 18 08:52:50 2024, max compression
+gzip compressed data, was "autora_experimentalist_extrapolation-0.0.5.tar", last modified: Thu Apr 18 11:47:22 2024, max compression
```

## Comparing `autora_experimentalist_extrapolation-0.0.4.tar` & `autora_experimentalist_extrapolation-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.idea/autora-experimentalist-extrapolation.iml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:52:50.517059 autora_experimentalist_extrapolation-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/tests/test_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.idea/autora-experimentalist-extrapolation.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/tests/test_extrapolation.py
```

### Comparing `autora_experimentalist_extrapolation-0.0.4/.github/pull_request_template.md` & `autora_experimentalist_extrapolation-0.0.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/.github/workflows/python-publish.yml` & `autora_experimentalist_extrapolation-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/.gitignore` & `autora_experimentalist_extrapolation-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/LICENSE` & `autora_experimentalist_extrapolation-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.4
+Version: 0.0.5
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.4/README.md` & `autora_experimentalist_extrapolation-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/docs/Basic Usage.ipynb` & `autora_experimentalist_extrapolation-0.0.5/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/docs/index.md` & `autora_experimentalist_extrapolation-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/mkdocs/base.yml` & `autora_experimentalist_extrapolation-0.0.5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/pyproject.toml` & `autora_experimentalist_extrapolation-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/__init__.py` & `autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Example Experimentalist
 """
+import copy
 import random as _random
 from typing import Literal, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import DistanceMetric
 
@@ -45,14 +46,15 @@
     variables: VariableCollection,
     models,
     num_samples=1,
     threshold_y=0.001,
     threshold_x=0.001,
     metric: AllowedMetrics = "euclidean",
     estimation_method: Union[AllowedEstimationMethods, None] = "mean",
+    check_influence=True,
     seed=None,
 ):
     """
 
     Args:
         conditions: The pool to sample from.
             Attention: `conditions` is a field of the standard state
@@ -68,14 +70,16 @@
         metric: distance measure. Options: 'euclidean', 'manhattan', 'chebyshev',
             'minkowski', 'wminkowski', 'seuclidean', 'mahalanobis', 'haversine',
             'hamming', 'canberra', 'braycurtis', 'matching', 'jaccard', 'dice',
             'kulsinski', 'rogerstanimoto', 'russellrao', 'sokalmichener',
             'sokalsneath', 'yule'.
         estimation_method: The method to estimate the value if conditions occure
             multiple times in the experiment_data
+        check_influence: Test if features of conditions are infleuncial in the prediction, if
+            not randomize them
         seed: A random seed that makes results reproducible
 
     Returns:
         Sampled pool of experimental conditions
 
     Examples:
         First, we describe an experiment with one independent and one dependent variable:
@@ -202,10 +206,48 @@
             score_2 = d_y
 
         _a.append([a_vector, score_1, score_2, _random.random()])
 
     _sorted_a = sorted(_a, key=lambda x: (x[1], x[2], x[3]), reverse=True)
 
     a_np = np.array([x[0] for x in _sorted_a])
+
+    n_features = _c.shape[1]
+
+    # Initialize a list to store the influence of each feature
+    feature_influence = []
+
+    for i in range(n_features):
+        # Create a copy of the original data
+        modified_c = copy.deepcopy(_c)
+        # Set the i-th feature to zero
+        modified_c[:, i] = 0
+        # Predict with the modified data
+        modified_predictions = models[-1].predict(modified_c)
+        # Check if predictions change
+        if np.array_equal(_y_c, modified_predictions):
+            feature_influence.append(False)
+        else:
+            feature_influence.append(True)
+
+    if any(feature_influence) and not all(feature_influence) and check_influence:
+        a_np = _replace_with_conditional_matching(_c, a_np, np.array(feature_influence))
+
     new_conditions = pd.DataFrame(a_np, columns=conditions.columns)
 
     return new_conditions[:num_samples]
+
+
+def _replace_with_conditional_matching(pool, target, mask):
+    # For each entry in the target array
+    for idx, entry in enumerate(target):
+        # Start with a full pool and filter down based on mask
+        filtered_pool = pool
+        for i, should_match in enumerate(mask):
+            if should_match:  # Apply filter only where mask is True
+                filtered_pool = filtered_pool[filtered_pool[:, i] == entry[i]]
+
+        # If there are matching entries, replace the target entry with a random one from the matches
+        if len(filtered_pool) > 0:
+            target[idx] = filtered_pool[np.random.randint(len(filtered_pool))]
+
+    return target
```

### Comparing `autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.4
+Version: 0.0.5
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt` & `autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.4/tests/README.md` & `autora_experimentalist_extrapolation-0.0.5/tests/README.md`

 * *Files identical despite different names*

