# Comparing `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0b3.tar.gz` & `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0b3.tar", last modified: Sun Mar 31 12:19:57 2024, max compression
+gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar", last modified: Thu Apr 18 19:30:26 2024, max compression
```

## Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3.tar` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.335276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.327276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 12:19:57.335276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.327276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.327276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.327276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.327276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-31 12:19:57.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-31 12:19:57.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 12:19:57.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 12:19:57.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 12:19:57.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:57.331276 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 12:19:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.github/workflows/python-publish.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.gitignore` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/.pre-commit-config.yaml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/LICENSE` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/docs/Basic Usage.ipynb` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/mkdocs/base.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/pyproject.toml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,19 +160,30 @@
     return study.status_code < 400
 
 
 def _retrieve_study(study_id: str, prolific_token: str):
     """
     Retrieves information about study given its ID.
     """
-    study = requests.get(
-        f"https://api.prolific.co/api/v1/studies/{study_id}/",
-        headers={"Authorization": f"Token {prolific_token}"},
-    )
-    return study.json()
+    while True:
+        tries = 0
+        while tries < RETRIES:
+            tries += 1
+            try:
+                study = requests.get(
+                    f"https://api.prolific.co/api/v1/studies/{study_id}/",
+                    headers={"Authorization": f"Token {prolific_token}"},
+                )
+                return study.json()
+            except Exception as e:
+                print(
+                    f'Warning: Did not succed to retrieve study.\n'
+                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                    f'Error: {e}')
+                time.sleep(20)
 
 
 def check_prolific_status(study_id: str, prolific_token: str) -> dict:
     """
     Check the status of a study
     Args:
         study_id: id of the study
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0b3/tests/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/README.md`

 * *Files identical despite different names*

