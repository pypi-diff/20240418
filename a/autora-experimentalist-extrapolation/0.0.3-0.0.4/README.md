# Comparing `tmp/autora_experimentalist_extrapolation-0.0.3.tar.gz` & `tmp/autora_experimentalist_extrapolation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experimentalist_extrapolation-0.0.3.tar", last modified: Wed Apr 17 11:23:30 2024, max compression
+gzip compressed data, was "autora_experimentalist_extrapolation-0.0.4.tar", last modified: Thu Apr 18 08:52:50 2024, max compression
```

## Comparing `autora_experimentalist_extrapolation-0.0.3.tar` & `autora_experimentalist_extrapolation-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.idea/autora-experimentalist-extrapolation.iml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/tests/test_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.idea/autora-experimentalist-extrapolation.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:52:50.517059 autora_experimentalist_extrapolation-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.509059 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 08:52:50.000000 autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:52:50.513059 autora_experimentalist_extrapolation-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 08:52:41.000000 autora_experimentalist_extrapolation-0.0.4/tests/test_extrapolation.py
```

### Comparing `autora_experimentalist_extrapolation-0.0.3/.github/pull_request_template.md` & `autora_experimentalist_extrapolation-0.0.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/.github/workflows/python-publish.yml` & `autora_experimentalist_extrapolation-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/.gitignore` & `autora_experimentalist_extrapolation-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/LICENSE` & `autora_experimentalist_extrapolation-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.3
+Version: 0.0.4
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.3/README.md` & `autora_experimentalist_extrapolation-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/docs/Basic Usage.ipynb` & `autora_experimentalist_extrapolation-0.0.4/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/docs/index.md` & `autora_experimentalist_extrapolation-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/mkdocs/base.yml` & `autora_experimentalist_extrapolation-0.0.4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/pyproject.toml` & `autora_experimentalist_extrapolation-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/__init__.py` & `autora_experimentalist_extrapolation-0.0.4/src/autora/experimentalist/extrapolation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 
 def sample(
     conditions: pd.DataFrame,
     experiment_data: pd.DataFrame,
     variables: VariableCollection,
     models,
     num_samples=1,
-    threshold=0.01,
+    threshold_y=0.001,
+    threshold_x=0.001,
     metric: AllowedMetrics = "euclidean",
     estimation_method: Union[AllowedEstimationMethods, None] = "mean",
     seed=None,
 ):
     """
 
     Args:
@@ -58,15 +59,16 @@
         experiment_data: The data that has already been collected
             Attention: `conditions` is a field of the standard state
         variables: The variable definitions used in the experiment
             Attention: `conditions` is a field of the standard state
         models: The models used to predict data on novel conditions
             Attention: `conditions` is a field of the standard state
         num_samples: Number of experimental conditions to select
-        threshold: A threshold bellow that distances are considered equal
+        threshold_y: A threshold bellow that distances are considered equal for y values
+        threshold_x: A threshold bellow that distances are considered equal for x values
         metric: distance measure. Options: 'euclidean', 'manhattan', 'chebyshev',
             'minkowski', 'wminkowski', 'seuclidean', 'mahalanobis', 'haversine',
             'hamming', 'canberra', 'braycurtis', 'matching', 'jaccard', 'dice',
             'kulsinski', 'rogerstanimoto', 'russellrao', 'sokalmichener',
             'sokalsneath', 'yule'.
         estimation_method: The method to estimate the value if conditions occure
             multiple times in the experiment_data
@@ -179,17 +181,19 @@
             or np.isnan(y_c).any()
             or np.isinf(y_r).any()
             or np.isinf(y_c).any()
         ):
             d_y = 0
         else:
             d_y = dist.pairwise([y_r], [[y_c]])[0]
-            if d_y < threshold:
+            if d_y < threshold_y:
                 d_y = 0
         d_x = dist.pairwise([x_r], [x_c])[0]
+        if d_x < threshold_x:
+            d_x = 0
 
         score_1 = 0
         if d_y != 0 and d_x != 0:
             score_1 = d_y / d_x
 
         score_2 = 0
         if d_y == 0:
```

### Comparing `autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.3
+Version: 0.0.4
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt` & `autora_experimentalist_extrapolation-0.0.4/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.3/tests/README.md` & `autora_experimentalist_extrapolation-0.0.4/tests/README.md`

 * *Files identical despite different names*

