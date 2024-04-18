# Comparing `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar.gz` & `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar", last modified: Thu Apr 18 19:30:26 2024, max compression
+gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar", last modified: Thu Apr 18 20:00:32 2024, max compression
```

## Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4.tar` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.443090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 19:30:26.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:26.447090 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 19:30:21.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.361049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:00:32.369049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)    20777 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 20:00:32.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:32.365049 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 20:00:27.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.github/workflows/python-publish.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.gitignore` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/.pre-commit-config.yaml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/LICENSE` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/docs/Basic Usage.ipynb` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/mkdocs/base.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/pyproject.toml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import time
 import random
 import string
 from typing import Any, List
 import requests
 import json
 
+RETRIES = 20
 
 def __get_request_results(url, headers):
     # Fetch all submissions using pagination
     all_submissions = []
 
     while True:
-        response = requests.get(url, headers=headers)
-        data = response.json()
+        tries = 0
+        while tries < RETRIES:
+            try:
+                tries += 1
+                response = requests.get(url, headers=headers)
+                data = response.json()
+            except Exception as e:
+                print(
+                    f'Warning: Did not get requested response.\n'
+                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                    f'Error: {e}')
+                time.sleep(20)
 
         if "results" in data:
             all_submissions.extend(data["results"])
 
         next_page = data.get("next_page")
         if next_page:
             url = next_page
@@ -29,20 +40,29 @@
     page = 1  # Start with the first page
     results_per_page = 50  # Specify the number of results per page
 
     # Concatenate all submissions
     all_submissions = []
 
     while True:
-        response = requests.get(
-            url,
-            headers=headers,
-
-        )
-        data = response.json()
+        tries = 0
+        while tries < RETRIES:
+            try:
+                tries += 1
+                response = requests.get(
+                    url,
+                    headers=headers,
+                )
+                data = response.json()
+            except Exception as e:
+                print(
+                    f'Warning: Did not get requested response.\n'
+                    f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                    f'Error: {e}')
+                time.sleep(20)
         url = data['_links']['next']['href']
         # Concatenate the JSON object from the response
         all_submissions.extend(data.get("results", []))
         # Check if there are no more results
         if url is None:
             break
 
@@ -87,19 +107,33 @@
     for s in incomplete_lst:
         submissions = __get_request_results(
             f'https://api.prolific.com/api/v1/submissions/?study={s["id"]}',
             {"Authorization": f"Token {prolific_token}"},
         )
         for sub in submissions:
             if sub['is_complete'] and sub['status'] == 'AWAITING REVIEW':
-                study = requests.post(
-                    f'https://api.prolific.com/api/v1/submissions/{sub["id"]}/transition/',
-                    headers={"Authorization": f"Token {prolific_token}"},
-                    json={"action": "APPROVE"},
-                )
+                code = 400
+                retries = 0
+                while code >= 400 and retries < RETRIES:
+                    try:
+                        retries += 1
+                        study = requests.post(
+                            f'https://api.prolific.com/api/v1/submissions/{sub["id"]}/transition/',
+                            headers={"Authorization": f"Token {prolific_token}"},
+                            json={"action": "APPROVE"},
+                        )
+                        code = study.status_code
+                    except Exception as e:
+                        print(
+                            f'Warning: Did not get requested response.\n'
+                            f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                            f'Error: {e}')
+                        time.sleep(20)
+                    if code >= 400:
+                        time.sleep(20)
 
 
 def _get_study_submissions(study_id: str, prolific_token: str) -> dict:
     study = _retrieve_study(study_id, prolific_token)
     submissions = __get_request_results(
         study['_links']['related']['href'],
         {"Authorization": f"Token {prolific_token}"},
@@ -115,52 +149,82 @@
 def _get_submissions_returned(study_id: str, prolific_token: str):
     return _get_submissions_type(study_id, prolific_token, 'RETURNED')
 
 
 def _get_submissions_timed_out(study_id: str, prolific_token: str):
     return _get_submissions_type(study_id, prolific_token, 'TIMED-OUT')
 
-def get_submissions_incompleted(study_id:str, prolific_token: str):
+
+def get_submissions_incompleted(study_id: str, prolific_token: str):
     return _get_submissions_returned(study_id, prolific_token) + \
         _get_submissions_type(study_id, prolific_token, 'TIMED-OUT')
 
 
 def _get_submissions_no_code_not_returned(study_id: str, prolific_token: str):
     submissions = _get_study_submissions(study_id, prolific_token)
     return [s['id'] for s in submissions
             if s['study_code'] == 'NOCODE'
             and s['status'] != 'RETURNED'
             and not s['return_requested']]
 
 
 def _request_return(id: str, prolific_token: str):
     data = {"request_return_reasons": ["No completion code.", "Did not finish study."]}
-    study = requests.post(
-        f"https://api.prolific.com/api/v1/submissions/{id}/request-return/",
-        headers={"Authorization": f"Token {prolific_token}"},
-        json=data,
-    )
+    code = 400
+    retries = 0
+    while code >= 400 and retries < RETRIES:
+        try:
+            retries += 1
+            study = requests.post(
+                f"https://api.prolific.com/api/v1/submissions/{id}/request-return/",
+                headers={"Authorization": f"Token {prolific_token}"},
+                json=data,
+            )
+            code = study.status_code
+        except Exception as e:
+            print(
+                f'Warning: Did not get requested response.\n'
+                f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                f'Error: {e}')
+            time.sleep(20)
+        if code >= 400:
+            time.sleep(20)
+
 
 def request_return_all(study_id: str, prolific_token: str):
     submissions = _get_submissions_no_code_not_returned(study_id, prolific_token)
     for id in submissions:
         _request_return(id, prolific_token)
-    
+
 
 def _update_study(study_id: str, prolific_token: str, **kwargs) -> bool:
     """
     Updates the parameters of a given study.
     If a study is already published, only internal_name
     and total_available_places can be updated.
     """
-    study = requests.patch(
-        f"https://api.prolific.co/api/v1/studies/{study_id}/",
-        headers={"Authorization": f"Token {prolific_token}"},
-        json=kwargs,
-    )
+    code = 400
+    retries = 0
+    while code >= 400 and retries < RETRIES:
+        try:
+            retries += 1
+            study = requests.patch(
+                f"https://api.prolific.co/api/v1/studies/{study_id}/",
+                headers={"Authorization": f"Token {prolific_token}"},
+                json=kwargs,
+            )
+            code = study.status_code
+        except Exception as e:
+            print(
+                f'Warning: Did not get requested response.\n'
+                f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                f'Error: {e}')
+            time.sleep(20)
+        if code >= 400:
+            time.sleep(20)
     return study.status_code < 400
 
 
 def _retrieve_study(study_id: str, prolific_token: str):
     """
     Retrieves information about study given its ID.
     """
@@ -311,23 +375,35 @@
 
     external_study_url = _append_url_variable(external_study_url, 'PROLIFIC_PID={{%PROLIFIC_PID%}}')
 
     # packages function parameters into dictionary
     data = locals()
 
     data["completion_code_action"] = "AUTOMATICALLY_APPROVE"
-
-    study = requests.post(
-        "https://api.prolific.co/api/v1/studies/",
-        headers={"Authorization": f"Token {prolific_token}"},
-        json=data,
-    )
+    code = 400
+    retries = 0
+    while code >= 400 and retries < RETRIES:
+        try:
+            retries += 1
+            study = requests.post(
+                "https://api.prolific.co/api/v1/studies/",
+                headers={"Authorization": f"Token {prolific_token}"},
+                json=data,
+            )
+            code = study.status_code
+        except Exception as e:
+            print(
+                f'Warning: Did not succed to retrieve study.\n'
+                f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                f'Error: {e}')
+            time.sleep(20)
+        if code >= 400:
+            time.sleep(20)
     # handles request failure
     if study.status_code >= 400:
-        print(study.json())
         return False
     keys_to_include = ["id", "maximum_allowed_time"]
     study_dict = dict(
         (key, value) for key, value in study.json().items() if key in keys_to_include
     )
 
     # save to temp_file
@@ -341,21 +417,34 @@
 
 def _update_study_status(study_id: str, action: str, prolific_token: str):
     """
     Performs action on specified study. Default action is to publish
     the study.
     """
     data = {"action": action}
-    study = requests.post(
-        f"https://api.prolific.co/api/v1/studies/{study_id}/transition/",
-        headers={"Authorization": f"Token {prolific_token}"},
-        json=data,
-    )
+    code = 400
+    retries = 0
+    while code >= 400 and retries < RETRIES:
+        try:
+            retries += 1
+            study = requests.post(
+                f"https://api.prolific.co/api/v1/studies/{study_id}/transition/",
+                headers={"Authorization": f"Token {prolific_token}"},
+                json=data,
+            )
+            code = study.status_code
+        except Exception as e:
+            print(
+                f'Warning: Did not succed to retrieve study.\n'
+                f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                f'Error: {e}')
+            time.sleep(20)
+        if code >= 400:
+            time.sleep(20)
     if study.status_code != 400:
-        print(study.json())
         return False
     return True
 
 
 def pause_study(study_id: str, prolific_token: str):
     """
     Pauses the study
@@ -402,19 +491,33 @@
 
 
 def approve_all(study_id: str, prolific_token: str):
     awaiting_review = get_participants_awaiting_review(study_id, prolific_token)
     data = {"study_id": study_id,
             "participant_ids": awaiting_review
             }
-    study = requests.post(
-        f"https://api.prolific.co/api/v1/submissions/bulk-approve/",
-        headers={"Authorization": f"Token {prolific_token}"},
-        json=data,
-    )
+    code = 400
+    retries = 0
+    while code >= 400 and retries < RETRIES:
+        try:
+            retries += 1
+            study = requests.post(
+                f"https://api.prolific.co/api/v1/submissions/bulk-approve/",
+                headers={"Authorization": f"Token {prolific_token}"},
+                json=data,
+            )
+            code = study.status_code
+        except Exception as e:
+            print(
+                f'Warning: Did not succed to retrieve study.\n'
+                f'Retrying... Trial: {tries}/{RETRIES}.\n'
+                f'Error: {e}')
+            time.sleep(20)
+        if code >= 400:
+            time.sleep(20)
     if study.status_code != 400:
         print(study.json())
         return False
     return True
 
 
 class EligibilityOptions:
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b4/tests/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b5/tests/README.md`

 * *Files identical despite different names*

