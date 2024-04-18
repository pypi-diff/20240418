# Comparing `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar.gz` & `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar", last modified: Thu Apr 18 21:38:55 2024, max compression
+gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b7.tar", last modified: Thu Apr 18 21:42:48 2024, max compression
```

## Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.532055 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.524056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:42:48.532055 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.524056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.524056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.524056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.524056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:42:48.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 21:42:48.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:42:48.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 21:42:48.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 21:42:48.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:48.528056 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 21:42:44.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/python-publish.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.gitignore` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.pre-commit-config.yaml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/LICENSE` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/Basic Usage.ipynb` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/base.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/pyproject.toml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,22 +346,22 @@
         'completion_code_action': "AUTOMATICALLY_APPROVE"
     }
     # packages function parameters into dictionary
     #_json = locals()
 
     #_json["completion_code_action"] = "AUTOMATICALLY_APPROVE"
 
-    __save_post(
+    data = __save_post(
         "https://api.prolific.co/api/v1/studies/",
         headers={"Authorization": f"Token {prolific_token}"},
         _json=_json,
     )
     keys_to_include = ["id", "maximum_allowed_time"]
     study_dict = dict(
-        (key, value) for key, value in study.json().items() if key in keys_to_include
+        (key, value) for key, value in data.items() if key in keys_to_include
     )
 
     # save to temp_file
     if temp_file != '':
         if not str.endswith(temp_file, '.json'):
             raise ValueError(f"Error: File '{temp_file}' is not in the correct JSON format.")
         with open(temp_file, 'w') as file:
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b7/tests/README.md`

 * *Files identical despite different names*

