# Comparing `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar.gz` & `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar", last modified: Thu Apr 18 20:00:32 2024, max compression
+gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar", last modified: Thu Apr 18 21:38:55 2024, max compression
```

## Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.361049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (127)    20777 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.656823 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 21:38:55.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:55.660822 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 21:38:51.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/python-publish.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.gitignore` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.pre-commit-config.yaml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/LICENSE` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/Basic Usage.ipynb` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/base.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/pyproject.toml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,56 @@
 import string
 from typing import Any, List
 import requests
 import json
 
 RETRIES = 20
 
+
+def __save_get(url, headers):
+    tries = 0
+    while tries < RETRIES:
+        tries += 1
+        response = requests.get(url, headers=headers)
+        if response.status_code < 400:
+            return response.json()
+        print(f'Warning in geting from prolific: {response.status_code}. Retry: {tries}/{RETRIES}')
+        time.sleep(20)
+    raise Exception(f'Error in geting from prolific: {response.status_code}')
+
+
+def __save_post(url, headers, _json):
+    tries = 0
+    while tries < RETRIES:
+        tries += 1
+        response = requests.post(url, headers=headers, json=_json)
+        if response.status_code < 400:
+            return True
+        print(f'Warning in posting to prolific: {response.status_code}. Retry: {tries}/{RETRIES}')
+        time.sleep(20)
+    raise Exception(f'Error in posting to prolific: {response.status_code}')
+
+
+def __save_patch(url, headers, _json):
+    tries = 0
+    while tries < RETRIES:
+        tries += 1
+        response = requests.patch(url, headers=headers, json=_json)
+        if response.status_code < 400:
+            return True
+        print(f'Warning in patching to prolific: {response.status_code}. Retry: {tries}/{RETRIES}')
+        time.sleep(20)
+    raise Exception(f'Error in patching to prolific: {response.status_code}')
+
+
 def __get_request_results(url, headers):
     # Fetch all submissions using pagination
     all_submissions = []
-
     while True:
-        tries = 0
-        while tries < RETRIES:
-            try:
-                tries += 1
-                response = requests.get(url, headers=headers)
-                data = response.json()
-            except Exception as e:
-                print(
-                    f'Warning: Did not get requested response.\n'
-                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                    f'Error: {e}')
-                time.sleep(20)
-
+        data = __save_get(url, headers)
         if "results" in data:
             all_submissions.extend(data["results"])
 
         next_page = data.get("next_page")
         if next_page:
             url = next_page
         else:
@@ -40,29 +64,15 @@
     page = 1  # Start with the first page
     results_per_page = 50  # Specify the number of results per page
 
     # Concatenate all submissions
     all_submissions = []
 
     while True:
-        tries = 0
-        while tries < RETRIES:
-            try:
-                tries += 1
-                response = requests.get(
-                    url,
-                    headers=headers,
-                )
-                data = response.json()
-            except Exception as e:
-                print(
-                    f'Warning: Did not get requested response.\n'
-                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                    f'Error: {e}')
-                time.sleep(20)
+        data = __save_get(url, headers)
         url = data['_links']['next']['href']
         # Concatenate the JSON object from the response
         all_submissions.extend(data.get("results", []))
         # Check if there are no more results
         if url is None:
             break
 
@@ -107,33 +117,19 @@
     for s in incomplete_lst:
         submissions = __get_request_results(
             f'https://api.prolific.com/api/v1/submissions/?study={s["id"]}',
             {"Authorization": f"Token {prolific_token}"},
         )
         for sub in submissions:
             if sub['is_complete'] and sub['status'] == 'AWAITING REVIEW':
-                code = 400
-                retries = 0
-                while code >= 400 and retries < RETRIES:
-                    try:
-                        retries += 1
-                        study = requests.post(
-                            f'https://api.prolific.com/api/v1/submissions/{sub["id"]}/transition/',
-                            headers={"Authorization": f"Token {prolific_token}"},
-                            json={"action": "APPROVE"},
-                        )
-                        code = study.status_code
-                    except Exception as e:
-                        print(
-                            f'Warning: Did not get requested response.\n'
-                            f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                            f'Error: {e}')
-                        time.sleep(20)
-                    if code >= 400:
-                        time.sleep(20)
+                __save_post(
+                    f'https://api.prolific.com/api/v1/submissions/{sub["id"]}/transition/',
+                    headers={"Authorization": f"Token {prolific_token}"},
+                    _json={"action": "APPROVE"}
+                )
 
 
 def _get_study_submissions(study_id: str, prolific_token: str) -> dict:
     study = _retrieve_study(study_id, prolific_token)
     submissions = __get_request_results(
         study['_links']['related']['href'],
         {"Authorization": f"Token {prolific_token}"},
@@ -165,89 +161,48 @@
             if s['study_code'] == 'NOCODE'
             and s['status'] != 'RETURNED'
             and not s['return_requested']]
 
 
 def _request_return(id: str, prolific_token: str):
     data = {"request_return_reasons": ["No completion code.", "Did not finish study."]}
-    code = 400
-    retries = 0
-    while code >= 400 and retries < RETRIES:
-        try:
-            retries += 1
-            study = requests.post(
-                f"https://api.prolific.com/api/v1/submissions/{id}/request-return/",
-                headers={"Authorization": f"Token {prolific_token}"},
-                json=data,
-            )
-            code = study.status_code
-        except Exception as e:
-            print(
-                f'Warning: Did not get requested response.\n'
-                f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                f'Error: {e}')
-            time.sleep(20)
-        if code >= 400:
-            time.sleep(20)
+    __save_post(
+        f"https://api.prolific.com/api/v1/submissions/{id}/request-return/",
+        headers={"Authorization": f"Token {prolific_token}"},
+        _json=data,
+    )
 
 
 def request_return_all(study_id: str, prolific_token: str):
     submissions = _get_submissions_no_code_not_returned(study_id, prolific_token)
     for id in submissions:
         _request_return(id, prolific_token)
 
 
 def _update_study(study_id: str, prolific_token: str, **kwargs) -> bool:
     """
     Updates the parameters of a given study.
     If a study is already published, only internal_name
     and total_available_places can be updated.
     """
-    code = 400
-    retries = 0
-    while code >= 400 and retries < RETRIES:
-        try:
-            retries += 1
-            study = requests.patch(
-                f"https://api.prolific.co/api/v1/studies/{study_id}/",
-                headers={"Authorization": f"Token {prolific_token}"},
-                json=kwargs,
-            )
-            code = study.status_code
-        except Exception as e:
-            print(
-                f'Warning: Did not get requested response.\n'
-                f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                f'Error: {e}')
-            time.sleep(20)
-        if code >= 400:
-            time.sleep(20)
-    return study.status_code < 400
+    return __save_patch(
+        f"https://api.prolific.co/api/v1/studies/{study_id}/",
+        headers={"Authorization": f"Token {prolific_token}"},
+        _json=kwargs,
+    )
 
 
 def _retrieve_study(study_id: str, prolific_token: str):
     """
     Retrieves information about study given its ID.
     """
-    while True:
-        tries = 0
-        while tries < RETRIES:
-            tries += 1
-            try:
-                study = requests.get(
-                    f"https://api.prolific.co/api/v1/studies/{study_id}/",
-                    headers={"Authorization": f"Token {prolific_token}"},
-                )
-                return study.json()
-            except Exception as e:
-                print(
-                    f'Warning: Did not succed to retrieve study.\n'
-                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                    f'Error: {e}')
-                time.sleep(20)
+    return __save_get(
+        f"https://api.prolific.co/api/v1/studies/{study_id}/",
+        headers={"Authorization": f"Token {prolific_token}"},
+    )
 
 
 def check_prolific_status(study_id: str, prolific_token: str) -> dict:
     """
     Check the status of a study
     Args:
         study_id: id of the study
@@ -371,40 +326,39 @@
             random.choices(string.ascii_letters + string.digits, k=6)
         )
     if reward == 0:
         reward = round(20 * estimated_completion_time)  # 12$ per hour / 20¢ per minute
 
     external_study_url = _append_url_variable(external_study_url, 'PROLIFIC_PID={{%PROLIFIC_PID%}}')
 
+    _json = {
+        'name': name,
+        'description': description,
+        'external_study_url': external_study_url,
+        'estimated_completion_time': estimated_completion_time,
+        'reward': reward,
+        'prolific_id_option': prolific_id_option,
+        'completion_code': completion_code,
+        'completion_option': completion_option,
+        'total_available_places': total_available_places,
+        'eligibility_requirements': eligibility_requirements,
+        'device_compatibility': device_compatibility,
+        'peripheral_requirements': peripheral_requirements,
+        'completion_code_action': "AUTOMATICALLY_APPROVE"
+    }
     # packages function parameters into dictionary
-    data = locals()
+    #_json = locals()
+
+    #_json["completion_code_action"] = "AUTOMATICALLY_APPROVE"
 
-    data["completion_code_action"] = "AUTOMATICALLY_APPROVE"
-    code = 400
-    retries = 0
-    while code >= 400 and retries < RETRIES:
-        try:
-            retries += 1
-            study = requests.post(
-                "https://api.prolific.co/api/v1/studies/",
-                headers={"Authorization": f"Token {prolific_token}"},
-                json=data,
-            )
-            code = study.status_code
-        except Exception as e:
-            print(
-                f'Warning: Did not succed to retrieve study.\n'
-                f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                f'Error: {e}')
-            time.sleep(20)
-        if code >= 400:
-            time.sleep(20)
-    # handles request failure
-    if study.status_code >= 400:
-        return False
+    __save_post(
+        "https://api.prolific.co/api/v1/studies/",
+        headers={"Authorization": f"Token {prolific_token}"},
+        _json=_json,
+    )
     keys_to_include = ["id", "maximum_allowed_time"]
     study_dict = dict(
         (key, value) for key, value in study.json().items() if key in keys_to_include
     )
 
     # save to temp_file
     if temp_file != '':
@@ -416,37 +370,19 @@
 
 
 def _update_study_status(study_id: str, action: str, prolific_token: str):
     """
     Performs action on specified study. Default action is to publish
     the study.
     """
-    data = {"action": action}
-    code = 400
-    retries = 0
-    while code >= 400 and retries < RETRIES:
-        try:
-            retries += 1
-            study = requests.post(
-                f"https://api.prolific.co/api/v1/studies/{study_id}/transition/",
-                headers={"Authorization": f"Token {prolific_token}"},
-                json=data,
-            )
-            code = study.status_code
-        except Exception as e:
-            print(
-                f'Warning: Did not succed to retrieve study.\n'
-                f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                f'Error: {e}')
-            time.sleep(20)
-        if code >= 400:
-            time.sleep(20)
-    if study.status_code != 400:
-        return False
-    return True
+    return __save_post(
+        f"https://api.prolific.co/api/v1/studies/{study_id}/transition/",
+        headers={"Authorization": f"Token {prolific_token}"},
+        _json={"action": action},
+    )
 
 
 def pause_study(study_id: str, prolific_token: str):
     """
     Pauses the study
     """
     return _update_study_status(study_id, "PAUSE", prolific_token)
@@ -491,37 +427,19 @@
 
 
 def approve_all(study_id: str, prolific_token: str):
     awaiting_review = get_participants_awaiting_review(study_id, prolific_token)
     data = {"study_id": study_id,
             "participant_ids": awaiting_review
             }
-    code = 400
-    retries = 0
-    while code >= 400 and retries < RETRIES:
-        try:
-            retries += 1
-            study = requests.post(
-                f"https://api.prolific.co/api/v1/submissions/bulk-approve/",
-                headers={"Authorization": f"Token {prolific_token}"},
-                json=data,
-            )
-            code = study.status_code
-        except Exception as e:
-            print(
-                f'Warning: Did not succed to retrieve study.\n'
-                f'Retrying... Trial: {tries}/{RETRIES}.\n'
-                f'Error: {e}')
-            time.sleep(20)
-        if code >= 400:
-            time.sleep(20)
-    if study.status_code != 400:
-        print(study.json())
-        return False
-    return True
+    return __save_postt(
+        f"https://api.prolific.co/api/v1/submissions/bulk-approve/",
+        headers={"Authorization": f"Token {prolific_token}"},
+        _json=data,
+    )
 
 
 class EligibilityOptions:
     @staticmethod
     def age(minimum: int, maximum: int):
         return {
             "_cls": "web.eligibility.models.AgeRangeEligibilityRequirement",
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b6/tests/README.md`

 * *Files identical despite different names*

