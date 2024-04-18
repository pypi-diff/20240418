# Comparing `tmp/jaraco.functools-4.0.0.tar.gz` & `tmp/jaraco_functools-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.functools-4.0.0.tar", last modified: Sat Nov  4 18:25:42 2023, max compression
+gzip compressed data, was "jaraco_functools-4.0.1.tar", last modified: Thu Apr 18 18:12:46 2024, max compression
```

## Comparing `jaraco.functools-4.0.0.tar` & `jaraco_functools-4.0.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.981990 jaraco.functools-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.977990 jaraco.functools-4.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.977990 jaraco.functools-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-11-04 18:25:42.981990 jaraco.functools-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.977990 jaraco.functools-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.973990 jaraco.functools-4.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.977990 jaraco.functools-4.0.0/jaraco/functools/
--rw-r--r--   0 runner    (1001) docker     (127)    16642 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/jaraco/functools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/jaraco/functools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/jaraco/functools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 18:25:42.977990 jaraco.functools-4.0.0/jaraco.functools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-11-04 18:25:42.000000 jaraco.functools-4.0.0/jaraco.functools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-04 18:25:42.000000 jaraco.functools-4.0.0/jaraco.functools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-04 18:25:42.000000 jaraco.functools-4.0.0/jaraco.functools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-04 18:25:42.000000 jaraco.functools-4.0.0/jaraco.functools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-04 18:25:42.000000 jaraco.functools-4.0.0/jaraco.functools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-04 18:25:42.981990 jaraco.functools-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-11-04 18:25:02.000000 jaraco.functools-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.521673 jaraco_functools-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.517673 jaraco_functools-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.517673 jaraco_functools-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-18 18:12:46.521673 jaraco_functools-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.517673 jaraco_functools-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.513673 jaraco_functools-4.0.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.521673 jaraco_functools-4.0.1/jaraco/functools/
+-rw-r--r--   0 runner    (1001) docker     (127)    16642 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/jaraco/functools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/jaraco/functools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/jaraco/functools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.521673 jaraco_functools-4.0.1/jaraco.functools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-18 18:12:46.000000 jaraco_functools-4.0.1/jaraco.functools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-18 18:12:46.000000 jaraco_functools-4.0.1/jaraco.functools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:12:46.000000 jaraco_functools-4.0.1/jaraco.functools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 18:12:46.000000 jaraco_functools-4.0.1/jaraco.functools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 18:12:46.000000 jaraco_functools-4.0.1/jaraco.functools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:12:46.521673 jaraco_functools-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 18:12:31.000000 jaraco_functools-4.0.1/tox.ini
```

### Comparing `jaraco.functools-4.0.0/.github/workflows/main.yml` & `jaraco_functools-4.0.1/.github/workflows/main.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
@@ -18,83 +27,73 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox
 
-  diffcov:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Evaluate coverage
-        run: tox
-        env:
-          TOXENV: diffcov
-
-  docs:
-    runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
-    steps:
-      - uses: actions/checkout@v3
-      - name: Setup Python
-        uses: actions/setup-python@v4
-      - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -105,20 +104,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.functools-4.0.0/LICENSE` & `jaraco_functools-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.functools-4.0.0/NEWS.rst` & `jaraco_functools-4.0.1/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v4.0.1
+======
+
+No significant changes.
+
+
 v4.0.0
 ======
 
 Features
 --------
 
 - Added ``splat`` function.
```

### Comparing `jaraco.functools-4.0.0/PKG-INFO` & `jaraco_functools-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 4.0.0
+Version: 4.0.1
 Summary: Functools like those found in stdlib
-Home-page: https://github.com/jaraco/jaraco.functools
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.functools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: jaraco.classes; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
@@ -32,30 +31,26 @@
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.functools.svg
    :target: https://pypi.org/project/jaraco.functools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
-.. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.functools/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.functools
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=readme
 
 Additional functools in the spirit of stdlib's functools.
```

### Comparing `jaraco.functools-4.0.0/README.rst` & `jaraco_functools-4.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.functools.svg
    :target: https://pypi.org/project/jaraco.functools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
-.. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.functools/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.functools
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=readme
 
 Additional functools in the spirit of stdlib's functools.
```

### Comparing `jaraco.functools-4.0.0/conftest.py` & `jaraco_functools-4.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-4.0.0/docs/conf.py` & `jaraco_functools-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-4.0.0/jaraco/functools/__init__.py` & `jaraco_functools-4.0.1/jaraco/functools/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-4.0.0/jaraco/functools/__init__.pyi` & `jaraco_functools-4.0.1/jaraco/functools/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,14 @@
 ) -> Callable[[Callable[_P, _R]], Callable[_P, _T]]: ...
 def result_invoke(
     action: Callable[[_R], Any]
 ) -> Callable[[Callable[_P, _R]], Callable[_P, _R]]: ...
 def invoke(
     f: Callable[_P, _R], /, *args: _P.args, **kwargs: _P.kwargs
 ) -> Callable[_P, _R]: ...
-def call_aside(
-    f: Callable[_P, _R], *args: _P.args, **kwargs: _P.kwargs
-) -> Callable[_P, _R]: ...
 
 class Throttler(Generic[_R]):
     last_called: float
     func: Callable[..., _R]
     max_rate: float
     def __init__(
         self, func: Callable[..., _R] | Throttler[_R], max_rate: float = ...
```

### Comparing `jaraco.functools-4.0.0/jaraco.functools.egg-info/PKG-INFO` & `jaraco_functools-4.0.1/jaraco.functools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 4.0.0
+Version: 4.0.1
 Summary: Functools like those found in stdlib
-Home-page: https://github.com/jaraco/jaraco.functools
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.functools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: jaraco.classes; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
@@ -32,30 +31,26 @@
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.functools.svg
    :target: https://pypi.org/project/jaraco.functools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
-.. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.functools/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.functools
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=readme
 
 Additional functools in the spirit of stdlib's functools.
```

### Comparing `jaraco.functools-4.0.0/jaraco.functools.egg-info/SOURCES.txt` & `jaraco_functools-4.0.1/jaraco.functools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 NEWS.rst
 README.rst
 SECURITY.md
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
+ruff.toml
 test_functools.py
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
```

### Comparing `jaraco.functools-4.0.0/test_functools.py` & `jaraco_functools-4.0.1/test_functools.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-4.0.0/tox.ini` & `jaraco_functools-4.0.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 	testing
 passenv =
 	GITHUB_ACTIONS
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
 description = build the documentation
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
-	python -m sphinxlint
+	python -m sphinxlint \
+		# workaround for sphinx-contrib/sphinx-lint#83
+		--jobs 1
 
 [testenv:finalize]
 description = assemble changelog and tag a release
 skip_install = True
 deps =
 	towncrier
 	jaraco.develop >= 7.23
```

