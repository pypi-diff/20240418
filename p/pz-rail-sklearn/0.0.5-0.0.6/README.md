# Comparing `tmp/pz-rail-sklearn-0.0.5.tar.gz` & `tmp/pz_rail_sklearn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-sklearn-0.0.5.tar", last modified: Wed Nov  1 01:54:03 2023, max compression
+gzip compressed data, was "pz_rail_sklearn-0.0.6.tar", last modified: Wed Apr 17 23:58:01 2024, max compression
```

## Comparing `pz-rail-sklearn-0.0.5.tar` & `pz_rail_sklearn-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/src/rail/estimation/algos/k_nearneigh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12518 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/src/rail/estimation/algos/nz_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/src/rail/estimation/algos/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/src/rail/estimation/algos/sklearn_neurnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/src/rail/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/src/rail/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-01 01:54:03.000000 pz-rail-sklearn-0.0.5/src/rail/sklearn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.675998 pz-rail-sklearn-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:54:03.679998 pz-rail-sklearn-0.0.5/tests/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2023-11-01 01:53:48.000000 pz-rail-sklearn-0.0.5/tests/sklearn/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.528747 pz_rail_sklearn-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:58:01.528747 pz_rail_sklearn-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/k_nearneigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12447 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/nz_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/sklearn_neurnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/rail/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/rail/sklearn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/tests/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/tests/sklearn/test_algos.py
```

### Comparing `pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/pull_request_template.md` & `pz_rail_sklearn-0.0.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/workflows/linting.yml` & `pz_rail_sklearn-0.0.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/workflows/publish-to-pypi.yml` & `pz_rail_sklearn-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/workflows/smoke-test.yml` & `pz_rail_sklearn-0.0.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.github/workflows/testing-and-coverage.yml` & `pz_rail_sklearn-0.0.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.gitignore` & `pz_rail_sklearn-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/.pre-commit-config.yaml` & `pz_rail_sklearn-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/LICENSE` & `pz_rail_sklearn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/PKG-INFO` & `pz_rail_sklearn-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-sklearn-0.0.5/README.md` & `pz_rail_sklearn-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/pyproject.toml` & `pz_rail_sklearn-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/PKG-INFO` & `pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-sklearn-0.0.5/src/pz_rail_sklearn.egg-info/SOURCES.txt` & `pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/src/rail/estimation/algos/k_nearneigh.py` & `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/k_nearneigh.py`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/src/rail/estimation/algos/nz_dir.py` & `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/nz_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,18 @@
         if self.comm is not None:  # pragma: no cover
             bootstrap_matrix = self.comm.bcast(bootstrap_matrix, root = 0)
 
         iterator = self.input_iterator('input')
         first = True
         self._initialize_run()
         self._output_handle = None
-        total_chunks = int(np.ceil(self._input_length/self.config.chunk_size))
         for s, e, test_data in iterator:
             print(f"Process {self.rank} running estimator on chunk {s} - {e}")
-
-            total_chunks = int(np.ceil(self._input_length/self.config.chunk_size))
+            if first:
+                total_chunks = int(np.ceil(self._input_length/(e-s)))
             chunk_number = s//self.config.chunk_size
             self._process_chunk(first, total_chunks, chunk_number, test_data, bootstrap_matrix)
             first = False
         self._single_handle.finalize_write()
         self._sample_handle.finalize_write()
         if self.comm is not None:  # pragma: no cover
             self.comm.Barrier()
```

### Comparing `pz-rail-sklearn-0.0.5/src/rail/estimation/algos/random_forest.py` & `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/random_forest.py`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/src/rail/estimation/algos/sklearn_neurnet.py` & `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/sklearn_neurnet.py`

 * *Files identical despite different names*

### Comparing `pz-rail-sklearn-0.0.5/tests/sklearn/test_algos.py` & `pz_rail_sklearn-0.0.6/tests/sklearn/test_algos.py`

 * *Files identical despite different names*

