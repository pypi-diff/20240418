# Comparing `tmp/github_custom_actions-0.0.2.tar.gz` & `tmp/github_custom_actions-1.0.1.tar.gz`

## Comparing `github_custom_actions-0.0.2.tar` & `github_custom_actions-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,44 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.mypy.ini
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.pylintrc
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/pytest.ini
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/requirements.dev.in
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/requirements.dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/requirements.in
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/requirements.txt
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/tasks.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.github/workflows/static.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/docs/mkdocs.yml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/docs/src/en/index.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/docs/src/en/reference.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/__init__.py
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 github_custom_actions-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.dev.in
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.in
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.txt
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/index.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/quick_start.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/reference.md
+-rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/ru/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/PKG-INFO
```

### Comparing `github_custom_actions-0.0.2/.pre-commit-config.yaml` & `github_custom_actions-1.0.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 exclude: |
     (?x)(
         tests/|
         site/|
         docs/|
         tasks.py|
+        scripts/|
         __about__.py
     )
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
     rev: v0.3.4
     hooks:
```

### Comparing `github_custom_actions-0.0.2/activate.sh` & `github_custom_actions-1.0.1/activate.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env bash
 #
 # "Set-ups or/and activates development environment"
 #
 
 VENV_FOLDER="venv"
-PRIMARY_PYTHON_VERSION="3.12"  # sync with .github/workflows/docs.yml&static.yml
+PRIMARY_PYTHON_VERSION="3.7"  # sync with .github/workflows/docs.yml&static.yml
 
 RED='\033[1;31m'
 GREEN='\033[1;32m'
 CYAN='\033[1;36m'
 NC='\033[0m' # No Color
 
 if ! (return 0 2>/dev/null) ; then
```

### Comparing `github_custom_actions-0.0.2/requirements.dev.txt` & `github_custom_actions-1.0.1/requirements.dev.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,157 +1,194 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements.dev.in --output-file=requirements.dev.txt
 -e .
-astroid==3.0.2
+astroid==2.15.8
     # via pylint
 babel==2.14.0
     # via mkdocs-material
-bracex==2.4
+bracex==2.3.post1
     # via wcmatch
+cached-property==1.5.2
+    # via griffe
 certifi==2023.11.17
     # via requests
-cfgv==3.4.0
+cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
-    # via
-    #   mkdocs
-    #   mkdocstrings
+    # via mkdocs
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
-coverage==7.3.2
+coverage==7.2.7
     # via pytest-cov
 dill==0.3.7
     # via pylint
 distlib==0.3.8
     # via virtualenv
 editables==0.5
     # via hatchling
-filelock==3.13.1
+exceptiongroup==1.2.0
+    # via pytest
+filelock==3.12.2
     # via virtualenv
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.30.1
     # via mkdocstrings-python
-hatchling==1.20.0
-identify==2.5.33
+hatchling==1.17.1
+identify==2.5.24
     # via pre-commit
 idna==3.6
     # via requests
+importlib-metadata==6.7.0
+    # via
+    #   click
+    #   hatchling
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   pluggy
+    #   pre-commit
+    #   pytest
+    #   virtualenv
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
-isort==5.13.2
+isort==5.11.5
     # via pylint
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
-markdown==3.5.1
+lazy-object-proxy==1.9.0
+    # via astroid
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocs
-    #   mkdocs-autorefs
     #   mkdocstrings
 mccabe==0.7.0
     # via pylint
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.5.3
     # via
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-material
     #   mkdocstrings
-mkdocs-autorefs==1.0.1
+mkdocs-autorefs==0.4.1
     # via mkdocstrings
 mkdocs-awesome-pages-plugin==2.9.2
-mkdocs-material==9.5.2
-mkdocs-material-extensions==1.3.1
+mkdocs-material==9.2.7
+mkdocs-material-extensions==1.2
     # via mkdocs-material
-mkdocstrings==0.24.1
+mkdocstrings==0.22.0
     # via mkdocstrings-python
-mkdocstrings-python==1.8.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
-mypy==1.7.1
+mypy==1.4.1
 mypy-extensions==1.0.0
     # via mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
 nodeenv==1.8.0
     # via pre-commit
 packaging==23.2
     # via
     #   hatchling
     #   mkdocs
     #   pytest
 paginate==0.5.6
     # via mkdocs-material
-pathspec==0.12.1
+pathspec==0.11.2
     # via
     #   hatchling
     #   mkdocs
-platformdirs==4.1.0
+platformdirs==4.0.0
     # via
     #   mkdocs
-    #   mkdocstrings
     #   pylint
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.2.0
     # via
     #   hatchling
     #   pytest
-pre-commit==3.6.0
+pre-commit==2.21.0
 pygments==2.17.2
     # via mkdocs-material
-pylint==3.0.3
-pymdown-extensions==10.5
+pylint==2.17.7
+pymdown-extensions==10.2.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pytest==7.4.3
     # via pytest-cov
 pytest-cov==4.1.0
 python-dateutil==2.8.2
     # via ghp-import
+pytz==2024.1
+    # via babel
 pyyaml==6.0.1
     # via
     #   mkdocs
     #   pre-commit
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.10.3
+regex==2022.10.31
     # via mkdocs-material
 requests==2.31.0
     # via mkdocs-material
-setuptools==69.5.1
+setuptools==68.0.0
     # via nodeenv
 six==1.16.0
     # via python-dateutil
 toml==0.10.2
+tomli==2.0.1
+    # via
+    #   coverage
+    #   hatchling
+    #   mypy
+    #   pylint
+    #   pytest
 tomlkit==0.12.3
     # via pylint
 trove-classifiers==2023.11.29
     # via hatchling
-typing-extensions==4.9.0
-    # via mypy
-urllib3==2.1.0
+typed-ast==1.5.5
+    # via
+    #   astroid
+    #   mypy
+typing-extensions==4.7.1
+    # via
+    #   astroid
+    #   importlib-metadata
+    #   mkdocs
+    #   mkdocstrings
+    #   mypy
+    #   platformdirs
+    #   pylint
+urllib3==2.0.7
     # via requests
 virtualenv==20.25.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
-wcmatch==8.5
+wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
+wrapt==1.16.0
+    # via astroid
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `github_custom_actions-0.0.2/tasks.py` & `github_custom_actions-1.0.1/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ALLOWED_DOC_LANGUAGES = get_allowed_doc_languages()
 ALLOWED_VERSION_TYPES = ["release", "bug", "feature"]
 
 
 @task
 def version(c: Context):
     """Show the current version."""
-    with open("src/bitwarden_import_msecure/__about__.py", "r") as f:
+    with open("src/github-custom-actions/__about__.py", "r") as f:
         version_line = f.readline()
         version_num = version_line.split('"')[1]
         print(version_num)
         return version_num
 
 
 def ver_task_factory(version_type: str):
@@ -59,15 +59,15 @@
     c.run("pip install -r requirements.dev.txt")
 
 
 def docs_task_factory(language: str):
     @task
     def docs(c: Context):
         """Docs preview for the language specified."""
-        c.run("open -a 'Google Chrome' http://127.0.0.1:8000/bitwarden-import-msecure/")
+        c.run("open -a 'Google Chrome' http://127.0.0.1:8000/github-custom-actions/")
         c.run(f"scripts/docs-render-config.sh {language}")
         c.run("mkdocs serve -f docs/_mkdocs.yml")
 
     return docs
 
 
 @task
```

### Comparing `github_custom_actions-0.0.2/.github/workflows/ci.yml` & `github_custom_actions-1.0.1/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
   pull_request:
     branches: [ master, main ]
 
 jobs:
   build:
     strategy:
       matrix:
-        python-version: [3.9, "3.10", 3.11, 3.12]
-        platform: [ubuntu-latest, macos-latest, windows-latest]
+        python-version: [3.7, 3.8, 3.9, "3.10", 3.11, 3.12]
+        platform: [ubuntu-latest]
     env:
       PRIMARY_PYTHON_VERSION: '3.12'
       PRIMARY_PLATFORM: 'ubuntu-latest'
       PYTEST_CMD: >
         python -m pytest 
         --junitxml=pytest.xml 
         --cov-report=term-missing:skip-covered
```

### Comparing `github_custom_actions-0.0.2/.github/workflows/docs.yml` & `github_custom_actions-1.0.1/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 permissions:
   contents: write
 
 jobs:
   deploy:
     env:
-      PRIMARY_PYTHON_VERSION: '3.12'
+      PRIMARY_PYTHON_VERSION: '3.8'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PRIMARY_PYTHON_VERSION  }}
       - run: |
```

### Comparing `github_custom_actions-0.0.2/.github/workflows/pip_publish.yml` & `github_custom_actions-1.0.1/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-0.0.2/.github/workflows/static.yml` & `github_custom_actions-1.0.1/.github/workflows/static.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   push:
     branches:
       - main
       - master
 jobs:
   deploy:
     env:
-      PRIMARY_PYTHON_VERSION: '3.12'
+      PRIMARY_PYTHON_VERSION: '3.7'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PRIMARY_PYTHON_VERSION  }}
       - uses: andgineer/uv-venv@v1
```

### Comparing `github_custom_actions-0.0.2/docs/mkdocs.yml` & `github_custom_actions-1.0.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-0.0.2/docs/src/en/index.md` & `github_custom_actions-1.0.1/docs/src/en/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# github-custom-actions
+# Installation
 
-Python package for creating custom GitHub Actions. 
+Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
+
+Supports Python 3.7 and higher for very only self-hosted action runners.
+
+- [Example of usage](https://github.com/andgineer/allure-report)
 
 ## Installation
 
 ## Installing pipx
 [`pipx`](https://pypa.github.io/pipx/) creates isolated environments to avoid conflicts with existing system packages.
 
 === "MacOS"
```

### Comparing `github_custom_actions-0.0.2/docs/src/ru/index.md` & `github_custom_actions-1.0.1/docs/src/ru/index.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # github-custom-actions
 
-Python package for creating custom GitHub Actions.
+Библиотека упрощающая создание
+[custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions).
+
+Поддерживает Python 3.7 и выше для древних self-hosted action runners.
+
+- [Пример использования](https://github.com/andgineer/allure-report)
 
 ## Установка
 
 ## Установка pipx
 [`pipx`](https://pypa.github.io/pipx/) создает изолированные среды, чтобы избежать конфликтов с 
 существующими системными пакетами.
```

### Comparing `github_custom_actions-0.0.2/scripts/include_pyproject_requirements.py` & `github_custom_actions-1.0.1/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-0.0.2/scripts/verup.sh` & `github_custom_actions-1.0.1/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-0.0.2/LICENSE.txt` & `github_custom_actions-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-0.0.2/README.md` & `github_custom_actions-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,55 +23,94 @@
 00000160: 6d2d 6163 7469 6f6e 732f 626c 6f62 2f70  m-actions/blob/p
 00000170: 7974 686f 6e2d 636f 7665 7261 6765 2d63  ython-coverage-c
 00000180: 6f6d 6d65 6e74 2d61 6374 696f 6e2d 6461  omment-action-da
 00000190: 7461 2f68 746d 6c63 6f76 2f69 6e64 6578  ta/htmlcov/index
 000001a0: 2e68 746d 6c29 0a23 2067 6974 6875 622d  .html).# github-
 000001b0: 6375 7374 6f6d 2d61 6374 696f 6e73 0a0a  custom-actions..
 000001c0: 5079 7468 6f6e 2070 6163 6b61 6765 2066  Python package f
-000001d0: 6f72 2063 7265 6174 696e 6720 6375 7374  or creating cust
-000001e0: 6f6d 2047 6974 4875 6220 4163 7469 6f6e  om GitHub Action
-000001f0: 732e 200a 0a23 2044 6f63 756d 656e 7461  s. ..# Documenta
-00000200: 7469 6f6e 0a0a 5b47 6974 6875 6220 4375  tion..[Github Cu
-00000210: 7374 6f6d 2041 6374 696f 6e73 5d28 6874  stom Actions](ht
-00000220: 7470 733a 2f2f 616e 6467 696e 6565 722e  tps://andgineer.
-00000230: 6769 7468 7562 2e69 6f2f 6769 7468 7562  github.io/github
-00000240: 2d63 7573 746f 6d2d 6163 7469 6f6e 732f  -custom-actions/
-00000250: 290a 0a23 2044 6576 656c 6f70 6572 730a  )..# Developers.
-00000260: 0a44 6f20 6e6f 7420 666f 7267 6574 2074  .Do not forget t
-00000270: 6f20 7275 6e20 602e 202e 2f61 6374 6976  o run `. ./activ
-00000280: 6174 652e 7368 602e 0a0a 2320 5363 7269  ate.sh`...# Scri
-00000290: 7074 730a 496e 7374 616c 6c20 5b69 6e76  pts.Install [inv
-000002a0: 6f6b 655d 2868 7474 7073 3a2f 2f64 6f63  oke](https://doc
-000002b0: 732e 7079 696e 766f 6b65 2e6f 7267 2f65  s.pyinvoke.org/e
-000002c0: 6e2f 7374 6162 6c65 2f29 2070 7265 6665  n/stable/) prefe
-000002d0: 7261 626c 7920 7769 7468 205b 7069 7078  rably with [pipx
-000002e0: 5d28 6874 7470 733a 2f2f 7079 7061 2e67  ](https://pypa.g
-000002f0: 6974 6875 622e 696f 2f70 6970 782f 293a  ithub.io/pipx/):
-00000300: 0a0a 2020 2020 7069 7078 2069 6e73 7461  ..    pipx insta
-00000310: 6c6c 2069 6e76 6f6b 650a 0a46 6f72 2061  ll invoke..For a
-00000320: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
-00000330: 6c65 2073 6372 6970 7473 2072 756e 3a0a  le scripts run:.
-00000340: 0a20 2020 2069 6e76 6f6b 6520 2d2d 6c69  .    invoke --li
-00000350: 7374 0a0a 466f 7220 6d6f 7265 2069 6e66  st..For more inf
-00000360: 6f72 6d61 7469 6f6e 2061 626f 7574 2061  ormation about a
-00000370: 2073 6372 6970 7420 7275 6e3a 0a0a 2020   script run:..  
-00000380: 2020 696e 766f 6b65 203c 7363 7269 7074    invoke <script
-00000390: 3e20 2d2d 6865 6c70 0a0a 2323 2043 6f76  > --help..## Cov
-000003a0: 6572 6167 6520 7265 706f 7274 0a2a 205b  erage report.* [
-000003b0: 436f 6465 636f 765d 2868 7474 7073 3a2f  Codecov](https:/
-000003c0: 2f61 7070 2e63 6f64 6563 6f76 2e69 6f2f  /app.codecov.io/
-000003d0: 6768 2f61 6e64 6769 6e65 6572 2f67 6974  gh/andgineer/git
-000003e0: 6875 622d 6375 7374 6f6d 2d61 6374 696f  hub-custom-actio
-000003f0: 6e73 2f74 7265 652f 6d61 696e 2f73 7263  ns/tree/main/src
-00000400: 2532 4667 6974 6875 625f 6375 7374 6f6d  %2Fgithub_custom
-00000410: 5f61 6374 696f 6e73 290a 2a20 5b43 6f76  _actions).* [Cov
-00000420: 6572 616c 6c73 5d28 6874 7470 733a 2f2f  eralls](https://
-00000430: 636f 7665 7261 6c6c 732e 696f 2f67 6974  coveralls.io/git
-00000440: 6875 622f 616e 6467 696e 6565 722f 6769  hub/andgineer/gi
-00000450: 7468 7562 2d63 7573 746f 6d2d 6163 7469  thub-custom-acti
-00000460: 6f6e 7329 0a0a 3e20 4372 6561 7465 6420  ons)..> Created 
-00000470: 7769 7468 2063 6f6f 6b69 6563 7574 7465  with cookiecutte
-00000480: 7220 7573 696e 6720 5b74 656d 706c 6174  r using [templat
-00000490: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-000004a0: 622e 636f 6d2f 616e 6467 696e 6565 722f  b.com/andgineer/
-000004b0: 636f 6f6b 6965 6375 7474 6572 2d70 7974  cookiecutter-pyt
-000004c0: 686f 6e2d 7061 636b 6167 6529            hon-package)
+000001d0: 6f72 2063 7265 6174 696e 6720 5b63 7573  or creating [cus
+000001e0: 746f 6d20 4769 7448 7562 2041 6374 696f  tom GitHub Actio
+000001f0: 6e73 5d28 6874 7470 733a 2f2f 646f 6373  ns](https://docs
+00000200: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
+00000210: 6374 696f 6e73 2f63 7265 6174 696e 672d  ctions/creating-
+00000220: 6163 7469 6f6e 732f 6162 6f75 742d 6375  actions/about-cu
+00000230: 7374 6f6d 2d61 6374 696f 6e73 292e 200a  stom-actions). .
+00000240: 0a23 2323 2320 4578 616d 706c 6520 6f66  .#### Example of
+00000250: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+00000260: 6e0a 6672 6f6d 2067 6974 6875 625f 6375  n.from github_cu
+00000270: 7374 6f6d 5f61 6374 696f 6e73 2069 6d70  stom_actions imp
+00000280: 6f72 7420 4163 7469 6f6e 4261 7365 2c20  ort ActionBase, 
+00000290: 4163 7469 6f6e 496e 7075 7473 0a0a 636c  ActionInputs..cl
+000002a0: 6173 7320 4d79 496e 7075 7473 2841 6374  ass MyInputs(Act
+000002b0: 696f 6e49 6e70 7574 7329 3a0a 2020 2020  ionInputs):.    
+000002c0: 6d79 5f69 6e70 7574 3a20 7374 720a 2020  my_input: str.  
+000002d0: 2020 2222 224d 7920 696e 7075 7420 6465    """My input de
+000002e0: 7363 7269 7074 696f 6e22 2222 0a20 2020  scription""".   
+000002f0: 200a 2020 2020 6d79 5f70 6174 683a 2050   .    my_path: P
+00000300: 6174 680a 2020 2020 2222 224d 7920 7061  ath.    """My pa
+00000310: 7468 2064 6573 6372 6970 7469 6f6e 2222  th description""
+00000320: 220a 0a63 6c61 7373 204d 7941 6374 696f  "..class MyActio
+00000330: 6e28 4163 7469 6f6e 4261 7365 293a 0a20  n(ActionBase):. 
+00000340: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000350: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00000360: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00000370: 696e 7075 7473 3d4d 7949 6e70 7574 7328  inputs=MyInputs(
+00000380: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
+00000390: 6c66 2e69 6e70 7574 732e 6d79 5f70 6174  lf.inputs.my_pat
+000003a0: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+000003b0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000003c0: 7565 4572 726f 7228 226d 795f 7061 7468  ueError("my_path
+000003d0: 2069 7320 7265 7175 6972 6564 2229 0a0a   is required")..
+000003e0: 2020 2020 6465 6620 6d61 696e 2873 656c      def main(sel
+000003f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00000400: 2e69 6e70 7574 732e 6d79 5f70 6174 682e  .inputs.my_path.
+00000410: 6d6b 6469 7228 6578 6973 745f 6f6b 3d54  mkdir(exist_ok=T
+00000420: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
+00000430: 662e 6f75 7470 7574 735b 2252 554e 4e45  f.outputs["RUNNE
+00000440: 525f 4f53 225d 203d 2073 656c 662e 7661  R_OS"] = self.va
+00000450: 7273 2e72 756e 6e65 725f 6f73 0a60 6060  rs.runner_os.```
+00000460: 0a23 2044 6f63 756d 656e 7461 7469 6f6e  .# Documentation
+00000470: 0a0a 5b47 6974 6875 6220 4375 7374 6f6d  ..[Github Custom
+00000480: 2041 6374 696f 6e73 5d28 6874 7470 733a   Actions](https:
+00000490: 2f2f 616e 6467 696e 6565 722e 6769 7468  //andgineer.gith
+000004a0: 7562 2e69 6f2f 6769 7468 7562 2d63 7573  ub.io/github-cus
+000004b0: 746f 6d2d 6163 7469 6f6e 732f 290a 0a23  tom-actions/)..#
+000004c0: 2044 6576 656c 6f70 6572 730a 0a44 6f20   Developers..Do 
+000004d0: 6e6f 7420 666f 7267 6574 2074 6f20 7275  not forget to ru
+000004e0: 6e20 602e 202e 2f61 6374 6976 6174 652e  n `. ./activate.
+000004f0: 7368 602e 0a0a 2320 5363 7269 7074 730a  sh`...# Scripts.
+00000500: 496e 7374 616c 6c20 5b69 6e76 6f6b 655d  Install [invoke]
+00000510: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+00000520: 696e 766f 6b65 2e6f 7267 2f65 6e2f 7374  invoke.org/en/st
+00000530: 6162 6c65 2f29 2070 7265 6665 7261 626c  able/) preferabl
+00000540: 7920 7769 7468 205b 7069 7078 5d28 6874  y with [pipx](ht
+00000550: 7470 733a 2f2f 7079 7061 2e67 6974 6875  tps://pypa.githu
+00000560: 622e 696f 2f70 6970 782f 293a 0a0a 2020  b.io/pipx/):..  
+00000570: 2020 7069 7078 2069 6e73 7461 6c6c 2069    pipx install i
+00000580: 6e76 6f6b 650a 0a46 6f72 2061 206c 6973  nvoke..For a lis
+00000590: 7420 6f66 2061 7661 696c 6162 6c65 2073  t of available s
+000005a0: 6372 6970 7473 2072 756e 3a0a 0a20 2020  cripts run:..   
+000005b0: 2069 6e76 6f6b 6520 2d2d 6c69 7374 0a0a   invoke --list..
+000005c0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+000005d0: 7469 6f6e 2061 626f 7574 2061 2073 6372  tion about a scr
+000005e0: 6970 7420 7275 6e3a 0a0a 2020 2020 696e  ipt run:..    in
+000005f0: 766f 6b65 203c 7363 7269 7074 3e20 2d2d  voke <script> --
+00000600: 6865 6c70 0a0a 2323 2043 6f76 6572 6167  help..## Coverag
+00000610: 6520 7265 706f 7274 0a2a 205b 436f 6465  e report.* [Code
+00000620: 636f 765d 2868 7474 7073 3a2f 2f61 7070  cov](https://app
+00000630: 2e63 6f64 6563 6f76 2e69 6f2f 6768 2f61  .codecov.io/gh/a
+00000640: 6e64 6769 6e65 6572 2f67 6974 6875 622d  ndgineer/github-
+00000650: 6375 7374 6f6d 2d61 6374 696f 6e73 2f74  custom-actions/t
+00000660: 7265 652f 6d61 696e 2f73 7263 2532 4667  ree/main/src%2Fg
+00000670: 6974 6875 625f 6375 7374 6f6d 5f61 6374  ithub_custom_act
+00000680: 696f 6e73 290a 2a20 5b43 6f76 6572 616c  ions).* [Coveral
+00000690: 6c73 5d28 6874 7470 733a 2f2f 636f 7665  ls](https://cove
+000006a0: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
+000006b0: 616e 6467 696e 6565 722f 6769 7468 7562  andgineer/github
+000006c0: 2d63 7573 746f 6d2d 6163 7469 6f6e 7329  -custom-actions)
+000006d0: 0a0a 3e20 4372 6561 7465 6420 7769 7468  ..> Created with
+000006e0: 2063 6f6f 6b69 6563 7574 7465 7220 7573   cookiecutter us
+000006f0: 696e 6720 5b74 656d 706c 6174 655d 2868  ing [template](h
+00000700: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000710: 6d2f 616e 6467 696e 6565 722f 636f 6f6b  m/andgineer/cook
+00000720: 6965 6375 7474 6572 2d70 7974 686f 6e2d  iecutter-python-
+00000730: 7061 636b 6167 6529                      package)
```

### Comparing `github_custom_actions-0.0.2/pyproject.toml` & `github_custom_actions-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "github-custom-actions"
 dynamic = [ "version",]
 description = "Python package for creating custom GitHub Actions."
 keywords = [ "one", "two", ]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 dependencies = []
 [[project.authors]]
 name = "Andrey Sorokin"
 email = "andrey@sorokin.engineer"
 
 [project.license]
 file = "LICENSE.txt"
```

### Comparing `github_custom_actions-0.0.2/PKG-INFO` & `github_custom_actions-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 6769 7468  : 2.3.Name: gith
 00000020: 7562 2d63 7573 746f 6d2d 6163 7469 6f6e  ub-custom-action
-00000030: 730a 5665 7273 696f 6e3a 2030 2e30 2e32  s.Version: 0.0.2
+00000030: 730a 5665 7273 696f 6e3a 2031 2e30 2e31  s.Version: 1.0.1
 00000040: 0a53 756d 6d61 7279 3a20 5079 7468 6f6e  .Summary: Python
 00000050: 2070 6163 6b61 6765 2066 6f72 2063 7265   package for cre
 00000060: 6174 696e 6720 6375 7374 6f6d 2047 6974  ating custom Git
 00000070: 4875 6220 4163 7469 6f6e 732e 0a50 726f  Hub Actions..Pro
 00000080: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
 00000090: 6765 2c20 6874 7470 733a 2f2f 616e 6467  ge, https://andg
 000000a0: 696e 6565 722e 6769 7468 7562 2e69 6f2f  ineer.github.io/
@@ -106,15 +106,15 @@
 00000690: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
 000006a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 000006b0: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
 000006c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
 000006d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 000006e0: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
 000006f0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-00000700: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
+00000700: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
 00000710: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 00000720: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
 00000730: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
 00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
 00000750: 636f 6d2f 616e 6467 696e 6565 722f 6769  com/andgineer/gi
 00000760: 7468 7562 2d63 7573 746f 6d2d 6163 7469  thub-custom-acti
 00000770: 6f6e 732f 776f 726b 666c 6f77 732f 4349  ons/workflows/CI
@@ -138,55 +138,94 @@
 00000890: 6d2d 6163 7469 6f6e 732f 626c 6f62 2f70  m-actions/blob/p
 000008a0: 7974 686f 6e2d 636f 7665 7261 6765 2d63  ython-coverage-c
 000008b0: 6f6d 6d65 6e74 2d61 6374 696f 6e2d 6461  omment-action-da
 000008c0: 7461 2f68 746d 6c63 6f76 2f69 6e64 6578  ta/htmlcov/index
 000008d0: 2e68 746d 6c29 0a23 2067 6974 6875 622d  .html).# github-
 000008e0: 6375 7374 6f6d 2d61 6374 696f 6e73 0a0a  custom-actions..
 000008f0: 5079 7468 6f6e 2070 6163 6b61 6765 2066  Python package f
-00000900: 6f72 2063 7265 6174 696e 6720 6375 7374  or creating cust
-00000910: 6f6d 2047 6974 4875 6220 4163 7469 6f6e  om GitHub Action
-00000920: 732e 200a 0a23 2044 6f63 756d 656e 7461  s. ..# Documenta
-00000930: 7469 6f6e 0a0a 5b47 6974 6875 6220 4375  tion..[Github Cu
-00000940: 7374 6f6d 2041 6374 696f 6e73 5d28 6874  stom Actions](ht
-00000950: 7470 733a 2f2f 616e 6467 696e 6565 722e  tps://andgineer.
-00000960: 6769 7468 7562 2e69 6f2f 6769 7468 7562  github.io/github
-00000970: 2d63 7573 746f 6d2d 6163 7469 6f6e 732f  -custom-actions/
-00000980: 290a 0a23 2044 6576 656c 6f70 6572 730a  )..# Developers.
-00000990: 0a44 6f20 6e6f 7420 666f 7267 6574 2074  .Do not forget t
-000009a0: 6f20 7275 6e20 602e 202e 2f61 6374 6976  o run `. ./activ
-000009b0: 6174 652e 7368 602e 0a0a 2320 5363 7269  ate.sh`...# Scri
-000009c0: 7074 730a 496e 7374 616c 6c20 5b69 6e76  pts.Install [inv
-000009d0: 6f6b 655d 2868 7474 7073 3a2f 2f64 6f63  oke](https://doc
-000009e0: 732e 7079 696e 766f 6b65 2e6f 7267 2f65  s.pyinvoke.org/e
-000009f0: 6e2f 7374 6162 6c65 2f29 2070 7265 6665  n/stable/) prefe
-00000a00: 7261 626c 7920 7769 7468 205b 7069 7078  rably with [pipx
-00000a10: 5d28 6874 7470 733a 2f2f 7079 7061 2e67  ](https://pypa.g
-00000a20: 6974 6875 622e 696f 2f70 6970 782f 293a  ithub.io/pipx/):
-00000a30: 0a0a 2020 2020 7069 7078 2069 6e73 7461  ..    pipx insta
-00000a40: 6c6c 2069 6e76 6f6b 650a 0a46 6f72 2061  ll invoke..For a
-00000a50: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
-00000a60: 6c65 2073 6372 6970 7473 2072 756e 3a0a  le scripts run:.
-00000a70: 0a20 2020 2069 6e76 6f6b 6520 2d2d 6c69  .    invoke --li
-00000a80: 7374 0a0a 466f 7220 6d6f 7265 2069 6e66  st..For more inf
-00000a90: 6f72 6d61 7469 6f6e 2061 626f 7574 2061  ormation about a
-00000aa0: 2073 6372 6970 7420 7275 6e3a 0a0a 2020   script run:..  
-00000ab0: 2020 696e 766f 6b65 203c 7363 7269 7074    invoke <script
-00000ac0: 3e20 2d2d 6865 6c70 0a0a 2323 2043 6f76  > --help..## Cov
-00000ad0: 6572 6167 6520 7265 706f 7274 0a2a 205b  erage report.* [
-00000ae0: 436f 6465 636f 765d 2868 7474 7073 3a2f  Codecov](https:/
-00000af0: 2f61 7070 2e63 6f64 6563 6f76 2e69 6f2f  /app.codecov.io/
-00000b00: 6768 2f61 6e64 6769 6e65 6572 2f67 6974  gh/andgineer/git
-00000b10: 6875 622d 6375 7374 6f6d 2d61 6374 696f  hub-custom-actio
-00000b20: 6e73 2f74 7265 652f 6d61 696e 2f73 7263  ns/tree/main/src
-00000b30: 2532 4667 6974 6875 625f 6375 7374 6f6d  %2Fgithub_custom
-00000b40: 5f61 6374 696f 6e73 290a 2a20 5b43 6f76  _actions).* [Cov
-00000b50: 6572 616c 6c73 5d28 6874 7470 733a 2f2f  eralls](https://
-00000b60: 636f 7665 7261 6c6c 732e 696f 2f67 6974  coveralls.io/git
-00000b70: 6875 622f 616e 6467 696e 6565 722f 6769  hub/andgineer/gi
-00000b80: 7468 7562 2d63 7573 746f 6d2d 6163 7469  thub-custom-acti
-00000b90: 6f6e 7329 0a0a 3e20 4372 6561 7465 6420  ons)..> Created 
-00000ba0: 7769 7468 2063 6f6f 6b69 6563 7574 7465  with cookiecutte
-00000bb0: 7220 7573 696e 6720 5b74 656d 706c 6174  r using [templat
-00000bc0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000bd0: 622e 636f 6d2f 616e 6467 696e 6565 722f  b.com/andgineer/
-00000be0: 636f 6f6b 6965 6375 7474 6572 2d70 7974  cookiecutter-pyt
-00000bf0: 686f 6e2d 7061 636b 6167 6529            hon-package)
+00000900: 6f72 2063 7265 6174 696e 6720 5b63 7573  or creating [cus
+00000910: 746f 6d20 4769 7448 7562 2041 6374 696f  tom GitHub Actio
+00000920: 6e73 5d28 6874 7470 733a 2f2f 646f 6373  ns](https://docs
+00000930: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
+00000940: 6374 696f 6e73 2f63 7265 6174 696e 672d  ctions/creating-
+00000950: 6163 7469 6f6e 732f 6162 6f75 742d 6375  actions/about-cu
+00000960: 7374 6f6d 2d61 6374 696f 6e73 292e 200a  stom-actions). .
+00000970: 0a23 2323 2320 4578 616d 706c 6520 6f66  .#### Example of
+00000980: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+00000990: 6e0a 6672 6f6d 2067 6974 6875 625f 6375  n.from github_cu
+000009a0: 7374 6f6d 5f61 6374 696f 6e73 2069 6d70  stom_actions imp
+000009b0: 6f72 7420 4163 7469 6f6e 4261 7365 2c20  ort ActionBase, 
+000009c0: 4163 7469 6f6e 496e 7075 7473 0a0a 636c  ActionInputs..cl
+000009d0: 6173 7320 4d79 496e 7075 7473 2841 6374  ass MyInputs(Act
+000009e0: 696f 6e49 6e70 7574 7329 3a0a 2020 2020  ionInputs):.    
+000009f0: 6d79 5f69 6e70 7574 3a20 7374 720a 2020  my_input: str.  
+00000a00: 2020 2222 224d 7920 696e 7075 7420 6465    """My input de
+00000a10: 7363 7269 7074 696f 6e22 2222 0a20 2020  scription""".   
+00000a20: 200a 2020 2020 6d79 5f70 6174 683a 2050   .    my_path: P
+00000a30: 6174 680a 2020 2020 2222 224d 7920 7061  ath.    """My pa
+00000a40: 7468 2064 6573 6372 6970 7469 6f6e 2222  th description""
+00000a50: 220a 0a63 6c61 7373 204d 7941 6374 696f  "..class MyActio
+00000a60: 6e28 4163 7469 6f6e 4261 7365 293a 0a20  n(ActionBase):. 
+00000a70: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000a80: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00000a90: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00000aa0: 696e 7075 7473 3d4d 7949 6e70 7574 7328  inputs=MyInputs(
+00000ab0: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
+00000ac0: 6c66 2e69 6e70 7574 732e 6d79 5f70 6174  lf.inputs.my_pat
+00000ad0: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+00000ae0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00000af0: 7565 4572 726f 7228 226d 795f 7061 7468  ueError("my_path
+00000b00: 2069 7320 7265 7175 6972 6564 2229 0a0a   is required")..
+00000b10: 2020 2020 6465 6620 6d61 696e 2873 656c      def main(sel
+00000b20: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00000b30: 2e69 6e70 7574 732e 6d79 5f70 6174 682e  .inputs.my_path.
+00000b40: 6d6b 6469 7228 6578 6973 745f 6f6b 3d54  mkdir(exist_ok=T
+00000b50: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
+00000b60: 662e 6f75 7470 7574 735b 2252 554e 4e45  f.outputs["RUNNE
+00000b70: 525f 4f53 225d 203d 2073 656c 662e 7661  R_OS"] = self.va
+00000b80: 7273 2e72 756e 6e65 725f 6f73 0a60 6060  rs.runner_os.```
+00000b90: 0a23 2044 6f63 756d 656e 7461 7469 6f6e  .# Documentation
+00000ba0: 0a0a 5b47 6974 6875 6220 4375 7374 6f6d  ..[Github Custom
+00000bb0: 2041 6374 696f 6e73 5d28 6874 7470 733a   Actions](https:
+00000bc0: 2f2f 616e 6467 696e 6565 722e 6769 7468  //andgineer.gith
+00000bd0: 7562 2e69 6f2f 6769 7468 7562 2d63 7573  ub.io/github-cus
+00000be0: 746f 6d2d 6163 7469 6f6e 732f 290a 0a23  tom-actions/)..#
+00000bf0: 2044 6576 656c 6f70 6572 730a 0a44 6f20   Developers..Do 
+00000c00: 6e6f 7420 666f 7267 6574 2074 6f20 7275  not forget to ru
+00000c10: 6e20 602e 202e 2f61 6374 6976 6174 652e  n `. ./activate.
+00000c20: 7368 602e 0a0a 2320 5363 7269 7074 730a  sh`...# Scripts.
+00000c30: 496e 7374 616c 6c20 5b69 6e76 6f6b 655d  Install [invoke]
+00000c40: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+00000c50: 696e 766f 6b65 2e6f 7267 2f65 6e2f 7374  invoke.org/en/st
+00000c60: 6162 6c65 2f29 2070 7265 6665 7261 626c  able/) preferabl
+00000c70: 7920 7769 7468 205b 7069 7078 5d28 6874  y with [pipx](ht
+00000c80: 7470 733a 2f2f 7079 7061 2e67 6974 6875  tps://pypa.githu
+00000c90: 622e 696f 2f70 6970 782f 293a 0a0a 2020  b.io/pipx/):..  
+00000ca0: 2020 7069 7078 2069 6e73 7461 6c6c 2069    pipx install i
+00000cb0: 6e76 6f6b 650a 0a46 6f72 2061 206c 6973  nvoke..For a lis
+00000cc0: 7420 6f66 2061 7661 696c 6162 6c65 2073  t of available s
+00000cd0: 6372 6970 7473 2072 756e 3a0a 0a20 2020  cripts run:..   
+00000ce0: 2069 6e76 6f6b 6520 2d2d 6c69 7374 0a0a   invoke --list..
+00000cf0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+00000d00: 7469 6f6e 2061 626f 7574 2061 2073 6372  tion about a scr
+00000d10: 6970 7420 7275 6e3a 0a0a 2020 2020 696e  ipt run:..    in
+00000d20: 766f 6b65 203c 7363 7269 7074 3e20 2d2d  voke <script> --
+00000d30: 6865 6c70 0a0a 2323 2043 6f76 6572 6167  help..## Coverag
+00000d40: 6520 7265 706f 7274 0a2a 205b 436f 6465  e report.* [Code
+00000d50: 636f 765d 2868 7474 7073 3a2f 2f61 7070  cov](https://app
+00000d60: 2e63 6f64 6563 6f76 2e69 6f2f 6768 2f61  .codecov.io/gh/a
+00000d70: 6e64 6769 6e65 6572 2f67 6974 6875 622d  ndgineer/github-
+00000d80: 6375 7374 6f6d 2d61 6374 696f 6e73 2f74  custom-actions/t
+00000d90: 7265 652f 6d61 696e 2f73 7263 2532 4667  ree/main/src%2Fg
+00000da0: 6974 6875 625f 6375 7374 6f6d 5f61 6374  ithub_custom_act
+00000db0: 696f 6e73 290a 2a20 5b43 6f76 6572 616c  ions).* [Coveral
+00000dc0: 6c73 5d28 6874 7470 733a 2f2f 636f 7665  ls](https://cove
+00000dd0: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
+00000de0: 616e 6467 696e 6565 722f 6769 7468 7562  andgineer/github
+00000df0: 2d63 7573 746f 6d2d 6163 7469 6f6e 7329  -custom-actions)
+00000e00: 0a0a 3e20 4372 6561 7465 6420 7769 7468  ..> Created with
+00000e10: 2063 6f6f 6b69 6563 7574 7465 7220 7573   cookiecutter us
+00000e20: 696e 6720 5b74 656d 706c 6174 655d 2868  ing [template](h
+00000e30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000e40: 6d2f 616e 6467 696e 6565 722f 636f 6f6b  m/andgineer/cook
+00000e50: 6965 6375 7474 6572 2d70 7974 686f 6e2d  iecutter-python-
+00000e60: 7061 636b 6167 6529                      package)
```

