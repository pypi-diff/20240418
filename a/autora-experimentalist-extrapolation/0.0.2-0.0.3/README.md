# Comparing `tmp/autora_experimentalist_extrapolation-0.0.2.tar.gz` & `tmp/autora_experimentalist_extrapolation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experimentalist_extrapolation-0.0.2.tar", last modified: Wed Apr 17 10:56:48 2024, max compression
+gzip compressed data, was "autora_experimentalist_extrapolation-0.0.3.tar", last modified: Wed Apr 17 11:23:30 2024, max compression
```

## Comparing `autora_experimentalist_extrapolation-0.0.2.tar` & `autora_experimentalist_extrapolation-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.731880 autora_experimentalist_extrapolation-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/.idea/autora-experimentalist-extrapolation.iml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 10:56:48.731880 autora_experimentalist_extrapolation-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:56:48.731880 autora_experimentalist_extrapolation-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.727880 autora_experimentalist_extrapolation-0.0.2/src/autora/experimentalist/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/src/autora/experimentalist/extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.731880 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 10:56:48.000000 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 10:56:48.000000 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:56:48.000000 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 10:56:48.000000 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 10:56:48.000000 autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:56:48.731880 autora_experimentalist_extrapolation-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-17 10:56:35.000000 autora_experimentalist_extrapolation-0.0.2/tests/test_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.idea/autora-experimentalist-extrapolation.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.531636 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 11:23:30.000000 autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:30.535636 autora_experimentalist_extrapolation-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-17 11:23:11.000000 autora_experimentalist_extrapolation-0.0.3/tests/test_extrapolation.py
```

### Comparing `autora_experimentalist_extrapolation-0.0.2/.github/pull_request_template.md` & `autora_experimentalist_extrapolation-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/.github/workflows/python-publish.yml` & `autora_experimentalist_extrapolation-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/.gitignore` & `autora_experimentalist_extrapolation-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/LICENSE` & `autora_experimentalist_extrapolation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.2
+Version: 0.0.3
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.2/README.md` & `autora_experimentalist_extrapolation-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/docs/Basic Usage.ipynb` & `autora_experimentalist_extrapolation-0.0.3/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/docs/index.md` & `autora_experimentalist_extrapolation-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/mkdocs/base.yml` & `autora_experimentalist_extrapolation-0.0.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/pyproject.toml` & `autora_experimentalist_extrapolation-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/src/autora/experimentalist/extrapolation/__init__.py` & `autora_experimentalist_extrapolation-0.0.3/src/autora/experimentalist/extrapolation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,22 +170,31 @@
         b_index = closest_b_for_each_a[idx]
         x_r = _r[b_index]
         y_r = np.array(_e_data[dvs])[b_index]
 
         x_c = a_vector
         y_c = _y_c[idx]
 
-        d_y = dist.pairwise([y_r], [[y_c]])[0]
-        if d_y < threshold:
+        if (
+            np.isnan(y_r).any()
+            or np.isnan(y_c).any()
+            or np.isinf(y_r).any()
+            or np.isinf(y_c).any()
+        ):
             d_y = 0
+        else:
+            d_y = dist.pairwise([y_r], [[y_c]])[0]
+            if d_y < threshold:
+                d_y = 0
         d_x = dist.pairwise([x_r], [x_c])[0]
 
         score_1 = 0
         if d_y != 0 and d_x != 0:
             score_1 = d_y / d_x
+
         score_2 = 0
         if d_y == 0:
             score_2 = d_x
         if d_x == 0:
             score_2 = d_y
 
         _a.append([a_vector, score_1, score_2, _random.random()])
```

### Comparing `autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.2
+Version: 0.0.3
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.2/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt` & `autora_experimentalist_extrapolation-0.0.3/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.2/tests/README.md` & `autora_experimentalist_extrapolation-0.0.3/tests/README.md`

 * *Files identical despite different names*

