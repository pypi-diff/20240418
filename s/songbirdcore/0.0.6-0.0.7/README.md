# Comparing `tmp/songbirdcore-0.0.6.tar.gz` & `tmp/songbirdcore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcore-0.0.6.tar", last modified: Wed Apr 17 16:09:48 2024, max compression
+gzip compressed data, was "songbirdcore-0.0.7.tar", last modified: Wed Apr 17 19:35:17 2024, max compression
```

## Comparing `songbirdcore-0.0.6.tar` & `songbirdcore-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.177462 songbirdcore-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/style.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/songbirdcore/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/common.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/gdrive.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/itunes.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/docs/songbirdcore/models/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/models/itunes_api.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/models/modes.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/web.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/docs/songbirdcore/youtube.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/songbirdcore/
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/itunes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.181462 songbirdcore-0.0.6/songbirdcore/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/models/itunes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/models/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/songbirdcore/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/songbirdcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 16:09:48.000000 songbirdcore-0.0.6/songbirdcore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.177462 songbirdcore-0.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:48.185462 songbirdcore-0.0.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_itunes.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 16:09:34.000000 songbirdcore-0.0.6/tests/unit/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.527976 songbirdcore-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/style.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/gdrive.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/itunes.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/models/itunes_api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/models/modes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/youtube.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/itunes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/models/itunes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/models/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/songbirdcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.527976 songbirdcore-0.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_itunes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_youtube.py
```

### Comparing `songbirdcore-0.0.6/.github/workflows/pages.yaml` & `songbirdcore-0.0.7/.github/workflows/pages.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 name: pages
 
 on:
   pull_request:
     branches: [main]
-  release:
-    types: [published]
+  push:
+    tags:
+      - '*'
 
 jobs:
   lint:
     runs-on: ubuntu-latest
+    if: github.event_name == 'pull_request'
     steps:
       - uses: actions/checkout@v4
       - name: install requirements
         run: |
           sudo apt update
           sudo apt install nodejs npm
           sudo npm install -g markdownlint-cli
@@ -20,14 +22,15 @@
         run: |
           shopt -s globstar
           shopt -s extglob
           make docs-lint
 
   test:
     runs-on: ubuntu-latest
+    if: github.event_name == 'pull_request'
     steps:
       - uses: actions/checkout@v4
       - name: set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - name: install dependencies
@@ -35,15 +38,15 @@
           python -m pip install --upgrade pip
           pip install -e .[dev]
       - name: test the site builds
         run: make docs-build
 
   deploy:
     runs-on: ubuntu-latest
-    if: ${{ github.event_name == 'release' }}
+    if: startsWith(github.ref, 'refs/tags/')
     needs: [lint, test]
     steps:
       - uses: actions/checkout@v4
       - name: set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: 3.11
```

### Comparing `songbirdcore-0.0.6/.github/workflows/pypi-publish.yaml` & `songbirdcore-0.0.7/.github/workflows/pypi-publish.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
-    
+    if: github.ref != 'refs/heads/gh-pages'  
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "3.x"
     - name: Install pypa/build
```

### Comparing `songbirdcore-0.0.6/.github/workflows/tests.yaml` & `songbirdcore-0.0.7/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/LICENSE` & `songbirdcore-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/Makefile` & `songbirdcore-0.0.7/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 # variables as a list, required for pytest targets
 # in this makefile
 
 .PHONY: setup
 setup: env
 	@echo sets up the development environment
-	npm install -g markdownlint-cli
 	python3 -m venv venv
 	@echo activate venv with 'source venv/bin/activate'
 
 .PHONY: requirements
 requirements: env
 	pip install -r $(APP_NAME)/$(REQUIREMENTS_FILE)
 # only install dependencies locally if in dev env
```

### Comparing `songbirdcore-0.0.6/PKG-INFO` & `songbirdcore-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.6
+Version: 0.0.7
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -43,15 +43,15 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.4
+Requires-Dist: requests-htmlc==0.0.6
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
```

### Comparing `songbirdcore-0.0.6/README.md` & `songbirdcore-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/mkdocs.yml` & `songbirdcore-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/pyproject.toml` & `songbirdcore-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "songbirdcore"
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.0.6"
+version = "0.0.7"
 description = "core low level api for songbird"
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["songbirdcore/requirements.txt"]}
```

### Comparing `songbirdcore-0.0.6/songbirdcore/common.py` & `songbirdcore-0.0.7/songbirdcore/common.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore/gdrive.py` & `songbirdcore-0.0.7/songbirdcore/gdrive.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore/itunes.py` & `songbirdcore-0.0.7/songbirdcore/itunes.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore/models/itunes_api.py` & `songbirdcore-0.0.7/songbirdcore/models/itunes_api.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore/requirements.txt` & `songbirdcore-0.0.7/songbirdcore/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 pydantic-settings==2.2.1
 pydantic_core==2.18.1
 pyee==11.1.0
 pyparsing==3.1.2
 pyquery==2.0.0
 python-dotenv==1.0.1
 requests==2.31.0
-requests-htmlc==0.0.4
+requests-htmlc==0.0.6
 requests-oauthlib==2.0.0
 rsa==4.9
 soupsieve==2.5
 toml==0.10.2
 typing_extensions==4.11.0
 uritemplate==4.1.1
 urllib3==2.2.1
```

### Comparing `songbirdcore-0.0.6/songbirdcore/web.py` & `songbirdcore-0.0.7/songbirdcore/web.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore/youtube.py` & `songbirdcore-0.0.7/songbirdcore/youtube.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore.egg-info/PKG-INFO` & `songbirdcore-0.0.7/songbirdcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.6
+Version: 0.0.7
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -43,15 +43,15 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.4
+Requires-Dist: requests-htmlc==0.0.6
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
```

### Comparing `songbirdcore-0.0.6/songbirdcore.egg-info/SOURCES.txt` & `songbirdcore-0.0.7/songbirdcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.6/songbirdcore.egg-info/requires.txt` & `songbirdcore-0.0.7/songbirdcore.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 pydantic-settings==2.2.1
 pydantic_core==2.18.1
 pyee==11.1.0
 pyparsing==3.1.2
 pyquery==2.0.0
 python-dotenv==1.0.1
 requests==2.31.0
-requests-htmlc==0.0.4
+requests-htmlc==0.0.6
 requests-oauthlib==2.0.0
 rsa==4.9
 soupsieve==2.5
 toml==0.10.2
 typing_extensions==4.11.0
 uritemplate==4.1.1
 urllib3==2.2.1
```

### Comparing `songbirdcore-0.0.6/tests/unit/test_youtube.py` & `songbirdcore-0.0.7/tests/unit/test_youtube.py`

 * *Files identical despite different names*

