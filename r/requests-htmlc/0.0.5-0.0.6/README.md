# Comparing `tmp/requests_htmlc-0.0.5.tar.gz` & `tmp/requests_htmlc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_htmlc-0.0.5.tar", last modified: Wed Apr 17 18:56:47 2024, max compression
+gzip compressed data, was "requests_htmlc-0.0.6.tar", last modified: Wed Apr 17 19:21:26 2024, max compression
```

## Comparing `requests_htmlc-0.0.5.tar` & `requests_htmlc-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.929188 requests_htmlc-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/docs/requests-htmlc/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/docs/requests-htmlc/requests_html.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/ext/
--rw-r--r--   0 runner    (1001) docker     (127)  2899712 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/ext/requests-html-logo.ai
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)    32509 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requests_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.937188 requests_htmlc-0.0.5/requests_htmlc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.937188 requests_htmlc-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    48883 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/python.html
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/test_internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/test_requests_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.369072 requests_htmlc-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.357071 requests_htmlc-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.361072 requests_htmlc-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 19:21:26.369072 requests_htmlc-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.361072 requests_htmlc-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.361072 requests_htmlc-0.0.6/docs/requests-htmlc/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/docs/requests-htmlc/requests_html.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.361072 requests_htmlc-0.0.6/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)  2899712 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/ext/requests-html-logo.ai
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    32509 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/requests_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.365072 requests_htmlc-0.0.6/requests_htmlc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 19:21:26.000000 requests_htmlc-0.0.6/requests_htmlc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 19:21:26.000000 requests_htmlc-0.0.6/requests_htmlc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:21:26.000000 requests_htmlc-0.0.6/requests_htmlc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 19:21:26.000000 requests_htmlc-0.0.6/requests_htmlc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 19:21:26.000000 requests_htmlc-0.0.6/requests_htmlc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:21:26.369072 requests_htmlc-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:26.365072 requests_htmlc-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    48883 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/tests/python.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/tests/test_internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-17 19:21:22.000000 requests_htmlc-0.0.6/tests/test_requests_html.py
```

### Comparing `requests_htmlc-0.0.5/.github/workflows/pages.yaml` & `requests_htmlc-0.0.6/.github/workflows/pages.yaml`

 * *Files 10% similar despite different names*

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
@@ -35,16 +38,15 @@
           python -m pip install --upgrade pip
           pip install -e .[dev]
       - name: test the site builds
         run: make docs-build
 
   deploy:
     runs-on: ubuntu-latest
-    if: ${{ github.event_name == 'release' }}
-    needs: [lint, test]
+    if: startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: actions/checkout@v4
       - name: set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - name: install dependencies
```

### Comparing `requests_htmlc-0.0.5/.github/workflows/pypi-publish.yaml` & `requests_htmlc-0.0.6/.github/workflows/pypi-publish.yaml`

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

### Comparing `requests_htmlc-0.0.5/.github/workflows/tests.yaml` & `requests_htmlc-0.0.6/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/.gitignore` & `requests_htmlc-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/LICENSE` & `requests_htmlc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/Makefile` & `requests_htmlc-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/PKG-INFO` & `requests_htmlc-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-htmlc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fork of requests-html, powered by playwright
 Author: Christian Boin
 License: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `requests_htmlc-0.0.5/README.md` & `requests_htmlc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/ext/requests-html-logo.ai` & `requests_htmlc-0.0.6/ext/requests-html-logo.ai`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/mkdocs.yml` & `requests_htmlc-0.0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/pyproject.toml` & `requests_htmlc-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "requests-htmlc"
 license={text="MIT License"}
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.0.5"
+version = "0.0.6"
 description = "Fork of requests-html, powered by playwright"
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [tool.setuptools]
 py-modules = ["requests_html"]
```

### Comparing `requests_htmlc-0.0.5/requests_html.py` & `requests_htmlc-0.0.6/requests_html.py`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/requests_htmlc.egg-info/PKG-INFO` & `requests_htmlc-0.0.6/requests_htmlc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-htmlc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fork of requests-html, powered by playwright
 Author: Christian Boin
 License: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `requests_htmlc-0.0.5/requests_htmlc.egg-info/SOURCES.txt` & `requests_htmlc-0.0.6/requests_htmlc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/tests/python.html` & `requests_htmlc-0.0.6/tests/python.html`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/tests/test_internet.py` & `requests_htmlc-0.0.6/tests/test_internet.py`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.5/tests/test_requests_html.py` & `requests_htmlc-0.0.6/tests/test_requests_html.py`

 * *Files identical despite different names*

