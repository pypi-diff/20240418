# Comparing `tmp/ptmcmcsampler-2.1.1.tar.gz` & `tmp/ptmcmcsampler-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmcmcsampler-2.1.1.tar", last modified: Fri Nov  4 14:38:32 2022, max compression
+gzip compressed data, was "ptmcmcsampler-2.1.2.tar", last modified: Thu Apr 18 13:54:08 2024, max compression
```

## Comparing `ptmcmcsampler-2.1.1.tar` & `ptmcmcsampler-2.1.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.262883 ptmcmcsampler-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.246882 ptmcmcsampler-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.250882 ptmcmcsampler-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/.github/workflows/ci_test.yml
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-11-04 14:38:32.262883 ptmcmcsampler-2.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.254882 ptmcmcsampler-2.1.1/PTMCMCSampler/
--rwxr-xr-x   0 runner    (1001) docker     (121)    34034 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/PTMCMCSampler/PTMCMCSampler.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/PTMCMCSampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/PTMCMCSampler/nompi4py.py
--rw-r--r--   0 runner    (1001) docker     (121)    30428 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/PTMCMCSampler/nutsjump.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/PTMCMCSampler/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.254882 ptmcmcsampler-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7187 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/docs/PTMCMCSampler.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10464 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6715 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.258883 ptmcmcsampler-2.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    58621 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/examples/curved_likelihood.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   254702 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/examples/gaussian_likelihood.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  2217364 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/examples/simple.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/examples/simple.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      407 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/make_gh-pages.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.258883 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 14:38:31.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 14:38:32.000000 ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 14:38:32.262883 ptmcmcsampler-2.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1234 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 14:38:32.258883 ptmcmcsampler-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6886 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-11-04 14:37:00.000000 ptmcmcsampler-2.1.1/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.749829 ptmcmcsampler-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.749829 ptmcmcsampler-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/.github/workflows/ci_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.753829 ptmcmcsampler-2.1.2/PTMCMCSampler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37304 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/PTMCMCSampler/PTMCMCSampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/PTMCMCSampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/PTMCMCSampler/nompi4py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30428 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/PTMCMCSampler/nutsjump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/PTMCMCSampler/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.753829 ptmcmcsampler-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/docs/PTMCMCSampler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    58621 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/examples/curved_likelihood.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   254707 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/examples/gaussian_likelihood.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2217336 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/examples/simple.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/examples/simple.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      407 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/make_gh-pages.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:54:08.000000 ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1317 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:54:08.757829 ptmcmcsampler-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 13:53:05.000000 ptmcmcsampler-2.1.2/tests/test_simple.py
```

### Comparing `ptmcmcsampler-2.1.1/.github/workflows/ci_test.yml` & `ptmcmcsampler-2.1.2/.github/workflows/ci_test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9, '3.10', '3.11']
 
     steps:
     - name: Checkout repository
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `ptmcmcsampler-2.1.1/LICENSE` & `ptmcmcsampler-2.1.2/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 The MIT License (MIT)
 
-Copyright (c) 2015 Justin Ellis
+*** Copyright Notice ***
+PTMCMCSampler Copyright (c) 2015 to 2022, Justin Ellis.
+All rights reserved.
+
+PTMCMCSampler Copyright (c) 2022, Mark Forrer on behalf of
+National Technology & Engineering Solutions of Sandia, LLC.
+All rights reserved.
+
+NOTICE.  This Software was partially developed under funding from the U.S. Department
+of Energy.
+********
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ptmcmcsampler-2.1.1/Makefile` & `ptmcmcsampler-2.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/PKG-INFO` & `ptmcmcsampler-2.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 Metadata-Version: 2.1
 Name: ptmcmcsampler
-Version: 2.1.1
+Version: 2.1.2
 Summary: Parallel tempering MCMC sampler written in Python
-Home-page: https://github.com/jellis18/PTMCMCSampler
-Author: Justin A. Ellis
-Author-email: justin.ellis18@gmail.com
+Home-page: https://github.com/nanograv/PTMCMCSampler
+Author: Justin A. Ellis, Rutger van Haasteren
+Author-email: rutger@vhaasteren.com
+Maintainer: Aaron D. Johnson, Paul T. Baker, Ken D. Olum
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: mpi
 License-File: LICENSE
+Requires-Dist: numpy>=1.16.3
+Requires-Dist: scipy>=1.2.0
+Provides-Extra: mpi
+Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 
 # PTMCMCSampler
 
-[![GitHub release (latest by date)](https://img.shields.io/github/v/release/jellis18/PTMCMCSampler)](https://github.com/jellis18/PTMCMCSampler/releases/latest)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/nanograv/PTMCMCSampler)](https://github.com/nanograv/PTMCMCSampler/releases/latest)
 [![PyPI](https://img.shields.io/pypi/v/ptmcmcsampler)](https://pypi.org/project/ptmcmcsampler/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ptmcmcsampler.svg)](https://anaconda.org/conda-forge/ptmcmcsampler)
-[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jellis18/PTMCMCSampler/CI%20targets?label=CI%20Tests)](https://github.com/jellis18/PTMCMCSampler/actions/workflows/ci_test.yml)
+[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/nanograv/PTMCMCSampler/CI%20targets?label=CI%20Tests)](https://github.com/nanograv/PTMCMCSampler/actions/workflows/ci_test.yml)
 
 [![DOI](https://zenodo.org/badge/32821232.svg)](https://zenodo.org/badge/latestdoi/32821232)
-[![Python Versions](https://img.shields.io/badge/python-3.7%2C%203.8%2C%203.9%2C%203.10-blue.svg)]()
-[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/jellis18/PTMCMCSampler/blob/master/LICENSE)
+[![Python Versions](https://img.shields.io/badge/python-3.8%2C%203.9%2C%203.10%2C%203.11-blue.svg)]()
+[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/nanograv/PTMCMCSampler/blob/master/LICENSE)
+
+**NOTE: This project was moved under the [NANOGrav][https://github.com/nanograv] github organization in November 2023**
 
 MPI enabled Parallel Tempering MCMC code written in Python.
 
-See the [examples](https://github.com/jellis18/PTMCMCSampler/tree/master/examples) for some simple use cases.
+See the [examples](https://github.com/nanograv/PTMCMCSampler/tree/master/examples) for some simple use cases.
 
 For MPI support you will need A functional MPI 1.x/2.x/3.x implementation like:
 
 - [MPICH](http://www.mpich.org/)
 
   ```bash
   # mac
@@ -97,14 +103,61 @@
 
 for MPI support use
 
 ```bash
 conda install -c conda-forge ptmcmcsampler mpi4py
 ```
 
+#### Via Docker
+
+**Production**:
+
+For production use, the latest release of PTMCMCSampler is installed directly from PyPi.
+```
+# Build the image, tagging it as `ptmcmc:latest`.  
+# 
+# This example includes both optional MPI support and the optional `acor` library 
+# (you can omit either / both).
+docker build --pull --build-arg "MPI=1" --build-arg "ACOR=1" -t ptmcmc --no-cache .
+
+# Run the image, mounting the `data/` subdirectory on your computer 
+# to `/code/data/` inside the Docker container. Note that MPI won't work 
+# if we run as the root user (the default).
+docker run -it --rm --user mcmc_user -v $(pwd)/data:/code/data ptmcmc
+
+# When finished with the container, exit back to the host OS
+CTRL^D
+```
+
+
+**Development**: 
+
+For PTMCMCSampler development, dependencies are installed from `requirements.txt` and 
+`requirements_dev.txt`. 
+No PTMCMCSampler code is omitted from the built image, whose purpose is for testing new code. 
+You can also add `--build-arg "ACOR=1"` to the build command to include the optional `acor` 
+dependency (MPI is always included via `requirements.txt`).
+
+```bash
+# Build the image
+docker build --pull -t ptmcmc --build-arg "TARGET_ENV=dev" --no-cache .
+
+# Run the image, mounting the working directory on the host OS to /code/ inside the container.
+# MPI won't work if we run as the root user (the default).
+docker run -it --rm --user mcmc_user -v $(pwd)/:/code ptmcmc
+
+# Exit back to host OS
+CTRL-D
+```
+
+
+
+
+
+
 ## Attribution
 
 If you make use of this code, please cite:
 
 ```
 @misc{justin_ellis_2017_1037579,
   author       = {Justin Ellis and
```

### Comparing `ptmcmcsampler-2.1.1/PTMCMCSampler/PTMCMCSampler.py` & `ptmcmcsampler-2.1.2/PTMCMCSampler/PTMCMCSampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 except ImportError:
     print("Optional mpi4py package is not installed.  MPI support is not available.")
     from . import nompi4py as MPI
 
 try:
     import acor
 except ImportError:
-    print(
-        "Optional acor package is not installed. Acor is optionally used to calculate the "
-        "effective chain length for output in the chain file."
-    )
+    # Don't complain if not available.  If you set neff, you'll get an error.  Otherwise
+    # it doesn't matter.
+    #    print(
+    #        "Optional acor package is not installed. Acor is optionally used to calculate the "
+    #        "effective chain length for output in the chain file."
+    #    )
     pass
 
 
 def shift_array(arr, num, fill_value=0.0):
     result = np.empty_like(arr)
     if num > 0:
         result[:num] = fill_value
@@ -85,15 +87,14 @@
         logp_grad=None,
         comm=MPI.COMM_WORLD,
         outDir="./chains",
         verbose=True,
         resume=False,
         seed=None,
     ):
-
         # MPI initialization
         self.comm = comm
         self.MPIrank = self.comm.Get_rank()
         self.nchain = self.comm.Get_size()
 
         if self.MPIrank == 0:
             ss = np.random.SeedSequence(seed)
@@ -170,15 +171,15 @@
         MALAweight=0,
         burn=50000,
         HMCstepsize=0.1,
         HMCsteps=300,
         maxIter=None,
         thin=10,
         i0=0,
-        neff=100000,
+        neff=None,
         writeHotChains=False,
         hotChain=False,
     ):
         """
         Initialize MCMC quantities
 
         @param maxIter: maximum number of iterations
@@ -200,19 +201,20 @@
         self.Tskip = Tskip
         self.thin = thin
         self.isave = isave
         self.Niter = Niter
         self.neff = neff
         self.tstart = 0
 
-        N = int(maxIter / thin)
+        N = int(maxIter / thin) + 1  # first sample + those we generate
 
         self._lnprob = np.zeros(N)
         self._lnlike = np.zeros(N)
         self._chain = np.zeros((N, self.ndim))
+        self.ind_next_write = 0  # Next index in these arrays to write out
         self.naccepted = 0
         self.swapProposed = 0
         self.nswap_accepted = 0
 
         # set up covariance matrix and DE buffers
         if self.MPIrank == 0:
             self._AMbuffer = np.zeros((self.covUpdate, self.ndim))
@@ -287,21 +289,35 @@
 
         self.resumeLength = 0
         if self.resume and os.path.isfile(self.fname):
             if self.verbose:
                 print("Resuming run from chain file {0}".format(self.fname))
             try:
                 self.resumechain = np.loadtxt(self.fname)
-                self.resumeLength = self.resumechain.shape[0]
-            except ValueError:
-                print("WARNING: Cant read in file. Removing last line.")
-                os.system("sed -ie '$d' {0}".format(self.fname))
-                self.resumechain = np.loadtxt(self.fname)
-                self.resumeLength = self.resumechain.shape[0]
+                self.resumeLength = self.resumechain.shape[0]  # Number of samples read from old chain
+            except ValueError as error:
+                print("Reading old chain files failed with error", error)
+                raise Exception("Couldn't read old chain to resume")
             self._chainfile = open(self.fname, "a")
+            if (
+                self.isave != self.thin
+                and self.resumeLength % (self.isave / self.thin) != 1  # This special case is always OK
+            ):  # Initial sample plus blocks of isave/thin
+                raise Exception(
+                    (
+                        "Old chain has {0} rows, which is not the initial sample plus a multiple of isave/thin = {1}"
+                    ).format(self.resumeLength, self.isave // self.thin)
+                )
+            print(
+                "Resuming with",
+                self.resumeLength,
+                "samples from file representing",
+                (self.resumeLength - 1) * self.thin + 1,
+                "original samples",
+            )
         else:
             self._chainfile = open(self.fname, "w")
         self._chainfile.close()
 
     def updateChains(self, p0, lnlike0, lnprob0, iter):
         """
         Update chains after jump proposals
@@ -315,26 +331,48 @@
         if iter % self.thin == 0:
             ind = int(iter / self.thin)
             self._chain[ind, :] = p0
             self._lnlike[ind] = lnlike0
             self._lnprob[ind] = lnprob0
 
         # write to file
-        if iter % self.isave == 0 and iter > 1 and iter > self.resumeLength:
+        if iter % self.isave == 0:
+            self.writeOutput(iter)
+
+    def writeOutput(self, iter):
+        """
+        Write chains and covariance matrix.  Called every isave on samples or at end.
+        """
+        if iter // self.thin >= self.ind_next_write:
             if self.writeHotChains or self.MPIrank == 0:
                 self._writeToFile(iter)
 
             # write output covariance matrix
-            np.save(self.outDir + "/cov.npy", self.cov)
-            if self.MPIrank == 0 and self.verbose and iter > 1:
-                sys.stdout.write("\r")
-                sys.stdout.write(
-                    "Finished %2.2f percent in %f s Acceptance rate = %g"
-                    % (iter / self.Niter * 100, time.time() - self.tstart, self.naccepted / iter)
-                )
+            if iter > 0:
+                np.save(self.outDir + "/cov.npy", self.cov)
+
+            if self.MPIrank == 0 and self.verbose:
+                if iter > 0:
+                    sys.stdout.write("\r")
+                percent = iter / self.Niter * 100  # Percent of total work finished
+                acceptance = self.naccepted / iter if iter > 0 else 0
+                elapsed = time.time() - self.tstart
+                if self.resume:
+                    # Percentage of new work done
+                    percentnew = (
+                        (iter - self.resumeLength * self.thin) / (self.Niter - self.resumeLength * self.thin) * 100
+                    )
+                    sys.stdout.write(
+                        "Finished %2.2f percent (%2.2f percent of new work) in %f s Acceptance rate = %g"
+                        % (percent, percentnew, elapsed, acceptance)
+                    )
+                else:
+                    sys.stdout.write(
+                        "Finished %2.2f percent in %f s Acceptance rate = %g" % (percent, elapsed, acceptance)
+                    )
                 sys.stdout.flush()
 
     def sample(
         self,
         p0,
         Niter,
         ladder=None,
@@ -351,52 +389,61 @@
         HMCweight=20,
         burn=10000,
         HMCstepsize=0.1,
         HMCsteps=300,
         maxIter=None,
         thin=10,
         i0=0,
-        neff=100000,
+        neff=None,
         writeHotChains=False,
         hotChain=False,
     ):
         """
         Function to carry out PTMCMC sampling.
 
         @param p0: Initial parameter vector
         @param self.Niter: Number of iterations to use for T = 1 chain
         @param ladder: User defined temperature ladder
         @param Tmin: Minimum temperature in ladder (default=1)
         @param Tmax: Maximum temperature in ladder (default=None)
         @param Tskip: Number of steps between proposed temperature swaps (default=100)
-        @param isave: Number of iterations before writing to file (default=1000)
+        @param isave: Write to file every isave samples (default=1000)
         @param covUpdate: Number of iterations between AM covariance updates (default=1000)
         @param SCAMweight: Weight of SCAM jumps in overall jump cycle (default=20)
         @param AMweight: Weight of AM jumps in overall jump cycle (default=20)
         @param DEweight: Weight of DE jumps in overall jump cycle (default=20)
         @param NUTSweight: Weight of the NUTS jumps in jump cycle (default=20)
         @param MALAweight: Weight of the MALA jumps in jump cycle (default=20)
         @param HMCweight: Weight of the HMC jumps in jump cycle (default=20)
         @param HMCstepsize: Step-size of the HMC jumps (default=0.1)
         @param HMCsteps: Maximum number of steps in an HMC trajectory (default=300)
         @param burn: Burn in time (DE jumps added after this iteration) (default=10000)
         @param maxIter: Maximum number of iterations for high temperature chains
                         (default=2*self.Niter)
-        @param self.thin: Save every self.thin MCMC samples
+        @param self.thin: MCMC Samples are recorded every self.thin samples
         @param i0: Iteration to start MCMC (if i0 !=0, do not re-initialize)
         @param neff: Number of effective samples to collect before terminating
 
         """
 
         # get maximum number of iteration
         if maxIter is None and self.MPIrank > 0:
             maxIter = Niter
         elif maxIter is None and self.MPIrank == 0:
             maxIter = Niter
 
+        if isave % thin != 0:
+            raise ValueError("isave = %d is not a multiple of thin =  %d" % (isave, thin))
+
+        if Niter % thin != 0:
+            print(
+                "Niter = %d is not a multiple of thin = %d.  The last %d samples will be lost"
+                % (Niter, thin, Niter % thin)
+            )
+
         # set up arrays to store lnprob, lnlike and chain
         # if picking up from previous run, don't re-initialize
         if i0 == 0:
             self.initialize(
                 Niter,
                 ladder=ladder,
                 Tmin=Tmin,
@@ -422,69 +469,67 @@
             )
 
         # compute lnprob for initial point in chain
 
         # if resuming, just start with first point in chain
         if self.resume and self.resumeLength > 0:
             p0, lnlike0, lnprob0 = self.resumechain[0, :-4], self.resumechain[0, -3], self.resumechain[0, -4]
+            self.ind_next_write = self.resumeLength
         else:
             # compute prior
             lp = self.logp(p0)
 
             if lp == float(-np.inf):
-
                 lnprob0 = -np.inf
                 lnlike0 = -np.inf
 
             else:
-
                 lnlike0 = self.logl(p0)
                 lnprob0 = 1 / self.temp * lnlike0 + lp
 
         # record first values
+        self.tstart = time.time()
         self.updateChains(p0, lnlike0, lnprob0, i0)
 
         self.comm.barrier()
 
         # start iterations
         iter = i0
-        self.tstart = time.time()
+
         runComplete = False
-        Neff = 0
         while runComplete is False:
             iter += 1
             self.comm.barrier()  # make sure all processes are at the same iteration
             # call PTMCMCOneStep
             p0, lnlike0, lnprob0 = self.PTMCMCOneStep(p0, lnlike0, lnprob0, iter)
 
-            # compute effective number of samples
-            if iter % 1000 == 0 and iter > 2 * self.burn and self.MPIrank == 0:
-                try:
-                    Neff = iter / max(
-                        1,
-                        np.nanmax([acor.acor(self._chain[self.burn : (iter - 1), ii])[0] for ii in range(self.ndim)]),
-                    )
-                    # print('\n {0} effective samples'.format(Neff))
-                except NameError:
-                    Neff = 0
-                    pass
-
-            # stop if reached maximum number of iterations
-            if self.MPIrank == 0 and iter >= self.Niter - 1:
-                if self.verbose:
-                    print("\nRun Complete")
-                runComplete = True
-
-            # stop if reached effective number of samples
-            if self.MPIrank == 0 and int(Neff) > self.neff:
-                if self.verbose:
-                    print("\nRun Complete with {0} effective samples".format(int(Neff)))
-                runComplete = True
-
-            runComplete = self.comm.bcast(runComplete, root=0)
+            # rank 0 decides whether to stop
+            if self.MPIrank == 0:
+                if iter >= self.Niter:  # stop if reached maximum number of iterations
+                    message = "\nRun Complete"
+                    runComplete = True
+                elif self.neff:  # Stop if effective number of samples reached if requested
+                    if iter % 1000 == 0 and iter > 2 * self.burn and self.MPIrank == 0:
+                        Neff = iter / max(
+                            1,
+                            np.nanmax(
+                                [acor.acor(self._chain[self.burn : (iter - 1), ii])[0] for ii in range(self.ndim)]
+                            ),
+                        )
+                        # print('\n {0} effective samples'.format(Neff))
+                        if int(Neff) >= self.neff:
+                            message = "\nRun Complete with {0} effective samples".format(int(Neff))
+                            runComplete = True
+
+            runComplete = self.comm.bcast(runComplete, root=0)  # rank 0 tells others whether to stop
+
+            if runComplete:
+                self.writeOutput(iter)  # Possibly write partial block
+                if self.MPIrank == 0 and self.verbose:
+                    print(message)
 
     def PTMCMCOneStep(self, p0, lnlike0, lnprob0, iter):
         """
         Function to carry out PTMCMC sampling.
 
         @param p0: Initial parameter vector
         @param lnlike0: Initial log-likelihood value
@@ -537,40 +582,42 @@
             self.addProposalToCycle(self.DEJump, self.DEweight)
 
             # randomize cycle
             self.randomizeProposalCycle()
 
         # jump proposal ###
 
-        # if resuming, just use previous chain points
-        if self.resume and self.resumeLength > 0 and iter < self.resumeLength:
-            p0, lnlike0, lnprob0 = self.resumechain[iter, :-4], self.resumechain[iter, -3], self.resumechain[iter, -4]
+        # if resuming, just use previous chain points.  Use each one thin times to compensate for
+        # thinning when they were written out
+        if self.resume and self.resumeLength > 0 and iter < self.resumeLength * self.thin:
+            p0, lnlike0, lnprob0 = (
+                self.resumechain[iter // self.thin, :-4],
+                self.resumechain[iter // self.thin, -3],
+                self.resumechain[iter // self.thin, -4],
+            )
 
             # update acceptance counter
-            self.naccepted = iter * self.resumechain[iter, -2]
+            self.naccepted = iter * self.resumechain[iter // self.thin, -2]
         else:
             y, qxy, jump_name = self._jump(p0, iter)
             self.jumpDict[jump_name][0] += 1
 
             # compute prior and likelihood
             lp = self.logp(y)
 
             if lp == -np.inf:
-
                 newlnprob = -np.inf
 
             else:
-
                 newlnlike = self.logl(y)
                 newlnprob = 1 / self.temp * newlnlike + lp
 
             # hastings step
             diff = newlnprob - lnprob0 + qxy
             if diff > np.log(self.stream.random()):
-
                 # accept jump
                 p0, lnlike0, lnprob0 = y, newlnlike, newlnprob
 
                 # update acceptance counter
                 self.naccepted += 1
                 self.jumpDict[jump_name][1] += 1
         # temperature swap
@@ -581,33 +628,42 @@
 
         return p0, lnlike0, lnprob0
 
     def PTswap(self, p0, lnlike0, lnprob0, iter):
         """
         Do parallel tempering swap.
 
+        (Repurposed from Neil Cornish/Bence Becsy's code)
+
+        Swap acceptance rates are computed per chain by storing
+        the number of swaps proposed and accepted. Since swaps
+        are proposed for every chain, swapProposed is always
+        incremented and nswap_accepted will be incremented only
+        for chains that have the swap accepted. The swap acceptance
+        is calculated elsewhere.
+
         @param p0: current parameter vector
         @param lnlike0: current log-likelihood
         @param lnprob0: current log posterior value
         @param iter: current iteration number
 
         @return swapReturn: 0 = no swap proposed,
         1 = swap proposed and rejected,
         2 = swap proposed and accepted
 
         @return p0: new parameter vector
         @return lnlike0: new log-likelihood
         @return lnprob0: new log posterior value
 
-        Repurposed from Neil Cornish/Bence Becsy's code:
         """
         Ts = self.ladder
 
         log_Ls = self.comm.gather(lnlike0, root=0)  # list of likelihoods from each chain
         p0s = self.comm.gather(p0, root=0)  # list of parameter arrays from each chain
+        swap_accepted = np.zeros(self.nchain)
 
         if self.MPIrank == 0:
             # set up map to help keep track of swaps
             swap_map = list(range(self.nchain))
 
             # loop through and propose a swap at each chain (starting from hottest chain and going down in T)
             # and keep track of results in swap_map
@@ -616,27 +672,26 @@
                 log_acc_ratio += -log_Ls[swap_map[swap_chain + 1]] / Ts[swap_chain + 1]
                 log_acc_ratio += log_Ls[swap_map[swap_chain + 1]] / Ts[swap_chain]
                 log_acc_ratio += log_Ls[swap_map[swap_chain]] / Ts[swap_chain + 1]
 
                 acc_ratio = np.exp(log_acc_ratio)
                 if self.stream.uniform() <= acc_ratio:
                     swap_map[swap_chain], swap_map[swap_chain + 1] = swap_map[swap_chain + 1], swap_map[swap_chain]
-                    self.nswap_accepted += 1
-                    self.swapProposed += 1
-                else:
-                    self.swapProposed += 1
+                    swap_accepted[swap_chain] += 1
 
             # loop through the chains and record the new samples and log_Ls
             for j in range(self.nchain):
                 p0s[j] = p0s[swap_map[j]]
                 log_Ls[j] = log_Ls[swap_map[j]]
 
         # broadcast the new samples and log_Ls to all chains
         p0 = self.comm.scatter(p0s, root=0)
         lnlike0 = self.comm.scatter(log_Ls, root=0)
+        self.nswap_accepted += self.comm.scatter(swap_accepted, root=0)
+        self.swapProposed += 1
 
         # calculate new posterior values
         lnprob0 = 1 / self.temp * lnlike0 + self.logp(p0)
 
         return p0, lnlike0, lnprob0
 
     def temperatureLadder(self, Tmin, Tmax=None, tstep=None):
@@ -660,40 +715,43 @@
         else:
             ladder = np.array([1])
 
         return ladder
 
     def _writeToFile(self, iter):
         """
-        Function to write chain file. File has 3+ndim columns,
-        the first is log-posterior (unweighted), log-likelihood,
-        and acceptance probability, followed by parameter values.
+        Function to write chain file. File has ndim+4 columns,
+        appended to the parameter values are log-posterior (unnormalized),
+        log-likelihood, acceptance rate, and PT acceptance rate.
+        Rates are as of time of writing.
 
         @param iter: Iteration of sampler
 
         """
 
         self._chainfile = open(self.fname, "a+")
-        for jj in range((iter - self.isave), iter, self.thin):
-            ind = int(jj / self.thin)
+        # index 0 is the initial element.  So after 10*thin iterations we need to write elements 1..10
+        write_end = iter // self.thin + 1  # First element not to write.
+        for ind in range(self.ind_next_write, write_end):
             pt_acc = 1
             if self.MPIrank < self.nchain - 1 and self.swapProposed != 0:
                 pt_acc = self.nswap_accepted / self.swapProposed
 
             self._chainfile.write("\t".join(["%22.22f" % (self._chain[ind, kk]) for kk in range(self.ndim)]))
             self._chainfile.write(
-                "\t%f\t%f\t%f\t%f\n" % (self._lnprob[ind], self._lnlike[ind], self.naccepted / iter, pt_acc)
+                "\t%f\t%f\t%f\t%f\n"
+                % (self._lnprob[ind], self._lnlike[ind], self.naccepted / iter if iter > 0 else 0, pt_acc)
             )
         self._chainfile.close()
+        self.ind_next_write = write_end  # Ready for next write
 
         # write jump statistics files ####
 
         # only for T=1 chain
         if self.MPIrank == 0:
-
             # first write file contaning jump names and jump rates
             fout = open(self.outDir + "/jumps.txt", "w")
             njumps = len(self.propCycle)
             ujumps = np.array(list(set(self.propCycle)))
             for jump in ujumps:
                 fout.write("%s %4.2g\n" % (jump.__name__, np.sum(np.array(self.propCycle) == jump) / njumps))
 
@@ -722,15 +780,14 @@
             self.M2 = np.zeros((ndim, ndim))
             self.mu = np.zeros(ndim)
 
         for ii in range(mem):
             diff = np.zeros(ndim)
             it += 1
             for jj in range(ndim):
-
                 diff[jj] = self._AMbuffer[ii, jj] - self.mu[jj]
                 self.mu[jj] += diff[jj] / it
 
             self.M2 += np.outer(diff, (self._AMbuffer[ii, :] - self.mu))
 
         self.cov[:, :] = self.M2 / (it - 1)
 
@@ -913,15 +970,14 @@
         if prob > 0.5:
             scale = 1.0
 
         else:
             scale = self.stream.random() * 2.4 / np.sqrt(2 * ndim) * np.sqrt(1 / beta)
 
         for ii in range(ndim):
-
             # jump size
             sigma = self._DEbuffer[mm, self.groups[jumpind][ii]] - self._DEbuffer[nn, self.groups[jumpind][ii]]
 
             # jump
             q[self.groups[jumpind][ii]] += scale * sigma
 
         return q, qxy
```

### Comparing `ptmcmcsampler-2.1.1/PTMCMCSampler/nompi4py.py` & `ptmcmcsampler-2.1.2/PTMCMCSampler/nompi4py.py`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/PTMCMCSampler/nutsjump.py` & `ptmcmcsampler-2.1.2/PTMCMCSampler/nutsjump.py`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/docs/Makefile` & `ptmcmcsampler-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/docs/PTMCMCSampler.rst` & `ptmcmcsampler-2.1.2/docs/PTMCMCSampler.rst`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/docs/conf.py` & `ptmcmcsampler-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/docs/make.bat` & `ptmcmcsampler-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/examples/curved_likelihood.ipynb` & `ptmcmcsampler-2.1.2/examples/curved_likelihood.ipynb`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/examples/gaussian_likelihood.ipynb` & `ptmcmcsampler-2.1.2/examples/gaussian_likelihood.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999549549549549%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(32, '        return self.lnpost_grad(x)[0]\\n')], delete: "*

 * *            '[32]}}}'}*

```diff
@@ -70,15 +70,15 @@
                 "    \n",
                 "    def lnpost_grad(self, x):\n",
                 "        ll, ll_grad = self.lnlikefn_grad(x)\n",
                 "        lp, lp_grad = self.lnpriorfn_grad(x)\n",
                 "        return ll+lp, ll_grad+lp_grad\n",
                 "    \n",
                 "    def lnpost(self, x):\n",
-                "        return lnpost_grad(x)[0]\n",
+                "        return self.lnpost_grad(x)[0]\n",
                 "    \n",
                 "    def hessian(self, x):\n",
                 "        return -np.eye(len(x))"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `ptmcmcsampler-2.1.1/examples/simple.ipynb` & `ptmcmcsampler-2.1.2/examples/simple.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'cells'": "{0: {'source': {delete: [3]}}}"}*

```diff
@@ -19,15 +19,14 @@
                     ]
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pylab as plt\n",
                 "import corner\n",
-                "import numpy as np\n",
                 "import glob\n",
                 "from PTMCMCSampler import PTMCMCSampler\n",
                 "\n",
                 "%matplotlib inline"
             ]
         },
         {
```

### Comparing `ptmcmcsampler-2.1.1/examples/simple.py` & `ptmcmcsampler-2.1.2/examples/simple.py`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/PKG-INFO` & `ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 Metadata-Version: 2.1
 Name: ptmcmcsampler
-Version: 2.1.1
+Version: 2.1.2
 Summary: Parallel tempering MCMC sampler written in Python
-Home-page: https://github.com/jellis18/PTMCMCSampler
-Author: Justin A. Ellis
-Author-email: justin.ellis18@gmail.com
+Home-page: https://github.com/nanograv/PTMCMCSampler
+Author: Justin A. Ellis, Rutger van Haasteren
+Author-email: rutger@vhaasteren.com
+Maintainer: Aaron D. Johnson, Paul T. Baker, Ken D. Olum
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: mpi
 License-File: LICENSE
+Requires-Dist: numpy>=1.16.3
+Requires-Dist: scipy>=1.2.0
+Provides-Extra: mpi
+Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 
 # PTMCMCSampler
 
-[![GitHub release (latest by date)](https://img.shields.io/github/v/release/jellis18/PTMCMCSampler)](https://github.com/jellis18/PTMCMCSampler/releases/latest)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/nanograv/PTMCMCSampler)](https://github.com/nanograv/PTMCMCSampler/releases/latest)
 [![PyPI](https://img.shields.io/pypi/v/ptmcmcsampler)](https://pypi.org/project/ptmcmcsampler/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ptmcmcsampler.svg)](https://anaconda.org/conda-forge/ptmcmcsampler)
-[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jellis18/PTMCMCSampler/CI%20targets?label=CI%20Tests)](https://github.com/jellis18/PTMCMCSampler/actions/workflows/ci_test.yml)
+[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/nanograv/PTMCMCSampler/CI%20targets?label=CI%20Tests)](https://github.com/nanograv/PTMCMCSampler/actions/workflows/ci_test.yml)
 
 [![DOI](https://zenodo.org/badge/32821232.svg)](https://zenodo.org/badge/latestdoi/32821232)
-[![Python Versions](https://img.shields.io/badge/python-3.7%2C%203.8%2C%203.9%2C%203.10-blue.svg)]()
-[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/jellis18/PTMCMCSampler/blob/master/LICENSE)
+[![Python Versions](https://img.shields.io/badge/python-3.8%2C%203.9%2C%203.10%2C%203.11-blue.svg)]()
+[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/nanograv/PTMCMCSampler/blob/master/LICENSE)
+
+**NOTE: This project was moved under the [NANOGrav][https://github.com/nanograv] github organization in November 2023**
 
 MPI enabled Parallel Tempering MCMC code written in Python.
 
-See the [examples](https://github.com/jellis18/PTMCMCSampler/tree/master/examples) for some simple use cases.
+See the [examples](https://github.com/nanograv/PTMCMCSampler/tree/master/examples) for some simple use cases.
 
 For MPI support you will need A functional MPI 1.x/2.x/3.x implementation like:
 
 - [MPICH](http://www.mpich.org/)
 
   ```bash
   # mac
@@ -97,14 +103,61 @@
 
 for MPI support use
 
 ```bash
 conda install -c conda-forge ptmcmcsampler mpi4py
 ```
 
+#### Via Docker
+
+**Production**:
+
+For production use, the latest release of PTMCMCSampler is installed directly from PyPi.
+```
+# Build the image, tagging it as `ptmcmc:latest`.  
+# 
+# This example includes both optional MPI support and the optional `acor` library 
+# (you can omit either / both).
+docker build --pull --build-arg "MPI=1" --build-arg "ACOR=1" -t ptmcmc --no-cache .
+
+# Run the image, mounting the `data/` subdirectory on your computer 
+# to `/code/data/` inside the Docker container. Note that MPI won't work 
+# if we run as the root user (the default).
+docker run -it --rm --user mcmc_user -v $(pwd)/data:/code/data ptmcmc
+
+# When finished with the container, exit back to the host OS
+CTRL^D
+```
+
+
+**Development**: 
+
+For PTMCMCSampler development, dependencies are installed from `requirements.txt` and 
+`requirements_dev.txt`. 
+No PTMCMCSampler code is omitted from the built image, whose purpose is for testing new code. 
+You can also add `--build-arg "ACOR=1"` to the build command to include the optional `acor` 
+dependency (MPI is always included via `requirements.txt`).
+
+```bash
+# Build the image
+docker build --pull -t ptmcmc --build-arg "TARGET_ENV=dev" --no-cache .
+
+# Run the image, mounting the working directory on the host OS to /code/ inside the container.
+# MPI won't work if we run as the root user (the default).
+docker run -it --rm --user mcmc_user -v $(pwd)/:/code ptmcmc
+
+# Exit back to host OS
+CTRL-D
+```
+
+
+
+
+
+
 ## Attribution
 
 If you make use of this code, please cite:
 
 ```
 @misc{justin_ellis_2017_1037579,
   author       = {Justin Ellis and
```

### Comparing `ptmcmcsampler-2.1.1/ptmcmcsampler.egg-info/SOURCES.txt` & `ptmcmcsampler-2.1.2/ptmcmcsampler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
+Dockerfile
 HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 make_gh-pages.sh
 pyproject.toml
```

### Comparing `ptmcmcsampler-2.1.1/pyproject.toml` & `ptmcmcsampler-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 indent = '    '
 dedup_headings = true
 line_length = 120
 multi_line_output = 3
 
 [tool.black]
 line-length = 120
-target_version = ['py37', 'py38', 'py39', 'py310']
+target_version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
@@ -33,8 +33,8 @@
 
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=6.2",
     "wheel",
 ]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `ptmcmcsampler-2.1.1/setup.py` & `ptmcmcsampler-2.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from setuptools import setup
 
 setup(
     name="ptmcmcsampler",
-    author="Justin A. Ellis",
-    author_email="justin.ellis18@gmail.com",
+    author="Justin A. Ellis, Rutger van Haasteren",
+    author_email="rutger@vhaasteren.com",
+    maintainer="Aaron D. Johnson, Paul T. Baker, Ken D. Olum",
     packages=["PTMCMCSampler"],
     package_dir={"PTMCMCSampler": "PTMCMCSampler"},
-    url="https://github.com/jellis18/PTMCMCSampler",
+    url="https://github.com/nanograv/PTMCMCSampler",
     license="MIT",
     zip_safe=False,
     description="Parallel tempering MCMC sampler written in Python",
     long_description=open("README.md").read() + "\n\n" + "---------\n\n" + open("HISTORY.md").read(),
     long_description_content_type="text/markdown",
     package_data={"": ["README.md", "HISTORY.md"]},
     install_requires=["numpy>=1.16.3", "scipy>=1.2.0"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require={"mpi": ["mpi4py>=3.0.3"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ptmcmcsampler-2.1.1/tests/test_nuts.py` & `ptmcmcsampler-2.1.2/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `ptmcmcsampler-2.1.1/tests/test_simple.py` & `ptmcmcsampler-2.1.2/tests/test_simple.py`

 * *Files identical despite different names*

