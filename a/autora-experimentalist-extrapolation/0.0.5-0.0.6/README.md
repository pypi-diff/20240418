# Comparing `tmp/autora_experimentalist_extrapolation-0.0.5.tar.gz` & `tmp/autora_experimentalist_extrapolation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experimentalist_extrapolation-0.0.5.tar", last modified: Thu Apr 18 11:47:22 2024, max compression
+gzip compressed data, was "autora_experimentalist_extrapolation-0.0.6.tar", last modified: Thu Apr 18 12:42:53 2024, max compression
```

## Comparing `autora_experimentalist_extrapolation-0.0.5.tar` & `autora_experimentalist_extrapolation-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.idea/autora-experimentalist-extrapolation.iml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.026992 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:47:22.000000 autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:47:22.030992 autora_experimentalist_extrapolation-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 11:47:15.000000 autora_experimentalist_extrapolation-0.0.5/tests/test_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.447420 autora_experimentalist_extrapolation-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.439420 autora_experimentalist_extrapolation-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/.idea/autora-experimentalist-extrapolation.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 12:42:53.447420 autora_experimentalist_extrapolation-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:42:53.447420 autora_experimentalist_extrapolation-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.439420 autora_experimentalist_extrapolation-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.439420 autora_experimentalist_extrapolation-0.0.6/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.439420 autora_experimentalist_extrapolation-0.0.6/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/src/autora/experimentalist/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/src/autora/experimentalist/extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 12:42:53.000000 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 12:42:53.000000 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:42:53.000000 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 12:42:53.000000 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:42:53.000000 autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:42:53.443420 autora_experimentalist_extrapolation-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 12:42:48.000000 autora_experimentalist_extrapolation-0.0.6/tests/test_extrapolation.py
```

### Comparing `autora_experimentalist_extrapolation-0.0.5/.github/pull_request_template.md` & `autora_experimentalist_extrapolation-0.0.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/.github/workflows/python-publish.yml` & `autora_experimentalist_extrapolation-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/.gitignore` & `autora_experimentalist_extrapolation-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/LICENSE` & `autora_experimentalist_extrapolation-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.5
+Version: 0.0.6
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.5/README.md` & `autora_experimentalist_extrapolation-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/docs/Basic Usage.ipynb` & `autora_experimentalist_extrapolation-0.0.6/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/docs/index.md` & `autora_experimentalist_extrapolation-0.0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/mkdocs/base.yml` & `autora_experimentalist_extrapolation-0.0.6/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/pyproject.toml` & `autora_experimentalist_extrapolation-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/src/autora/experimentalist/extrapolation/__init__.py` & `autora_experimentalist_extrapolation-0.0.6/src/autora/experimentalist/extrapolation/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     conditions: pd.DataFrame,
     experiment_data: pd.DataFrame,
     variables: VariableCollection,
     models,
     num_samples=1,
     threshold_y=0.001,
     threshold_x=0.001,
+    precision=5,
     metric: AllowedMetrics = "euclidean",
     estimation_method: Union[AllowedEstimationMethods, None] = "mean",
     check_influence=True,
     seed=None,
 ):
     """
 
@@ -63,14 +64,15 @@
         variables: The variable definitions used in the experiment
             Attention: `conditions` is a field of the standard state
         models: The models used to predict data on novel conditions
             Attention: `conditions` is a field of the standard state
         num_samples: Number of experimental conditions to select
         threshold_y: A threshold bellow that distances are considered equal for y values
         threshold_x: A threshold bellow that distances are considered equal for x values
+        precision: The precision to round the differences
         metric: distance measure. Options: 'euclidean', 'manhattan', 'chebyshev',
             'minkowski', 'wminkowski', 'seuclidean', 'mahalanobis', 'haversine',
             'hamming', 'canberra', 'braycurtis', 'matching', 'jaccard', 'dice',
             'kulsinski', 'rogerstanimoto', 'russellrao', 'sokalmichener',
             'sokalsneath', 'yule'.
         estimation_method: The method to estimate the value if conditions occure
             multiple times in the experiment_data
@@ -191,25 +193,35 @@
             d_y = dist.pairwise([y_r], [[y_c]])[0]
             if d_y < threshold_y:
                 d_y = 0
         d_x = dist.pairwise([x_r], [x_c])[0]
         if d_x < threshold_x:
             d_x = 0
 
+        d_y = np.round(d_y, precision)
+        d_x = np.round(d_x, precision)
+
         score_1 = 0
         if d_y != 0 and d_x != 0:
             score_1 = d_y / d_x
 
         score_2 = 0
         if d_y == 0:
             score_2 = d_x
         if d_x == 0:
             score_2 = d_y
 
-        _a.append([a_vector, score_1, score_2, _random.random()])
+        _a.append(
+            [
+                a_vector,
+                np.round(score_1, precision),
+                np.round(score_2, precision),
+                _random.random(),
+            ]
+        )
 
     _sorted_a = sorted(_a, key=lambda x: (x[1], x[2], x[3]), reverse=True)
 
     a_np = np.array([x[0] for x in _sorted_a])
 
     n_features = _c.shape[1]
```

### Comparing `autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.5
+Version: 0.0.6
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.5/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt` & `autora_experimentalist_extrapolation-0.0.6/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.5/tests/README.md` & `autora_experimentalist_extrapolation-0.0.6/tests/README.md`

 * *Files identical despite different names*

