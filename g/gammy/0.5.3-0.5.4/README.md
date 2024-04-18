# Comparing `tmp/gammy-0.5.3.tar.gz` & `tmp/gammy-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammy-0.5.3.tar", last modified: Tue Jan  2 10:22:57 2024, max compression
+gzip compressed data, was "gammy-0.5.4.tar", last modified: Thu Apr 18 09:30:08 2024, max compression
```

## Comparing `gammy-0.5.3.tar` & `gammy-0.5.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.952249 gammy-0.5.3/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        0 2021-10-05 12:57:59.000000 gammy-0.5.3/.gitattributes
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       82 2023-12-25 20:53:18.000000 gammy-0.5.3/.gitignore
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4361 2023-12-26 07:11:06.000000 gammy-0.5.3/CHANGELOG.md
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1083 2021-10-05 12:57:59.000000 gammy-0.5.3/LICENSE.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       20 2021-10-05 12:57:59.000000 gammy-0.5.3/MANIFEST.in
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11766 2024-01-02 10:22:57.952249 gammy-0.5.3/PKG-INFO
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    10730 2024-01-02 10:20:21.000000 gammy-0.5.3/README.md
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.941249 gammy-0.5.3/doc/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      638 2021-10-05 12:57:59.000000 gammy-0.5.3/doc/Makefile
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.942249 gammy-0.5.3/doc/source/
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.942249 gammy-0.5.3/doc/source/_static/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        0 2021-10-05 12:57:59.000000 gammy-0.5.3/doc/source/_static/.gitkeep
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.937249 gammy-0.5.3/doc/source/_templates/
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.943249 gammy-0.5.3/doc/source/_templates/autosummary/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      147 2021-10-19 20:24:01.000000 gammy-0.5.3/doc/source/_templates/autosummary/base.rst
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      254 2021-10-05 12:57:59.000000 gammy-0.5.3/doc/source/_templates/autosummary/class.rst
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      513 2021-10-19 20:24:01.000000 gammy-0.5.3/doc/source/_templates/autosummary/module.rst
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       51 2021-10-19 20:24:01.000000 gammy-0.5.3/doc/source/api.rst
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3357 2021-11-19 16:52:11.000000 gammy-0.5.3/doc/source/conf.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1082 2021-10-30 04:11:06.000000 gammy-0.5.3/doc/source/index.rst
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      126 2021-10-05 12:57:59.000000 gammy-0.5.3/doc/source/installation.rst
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.946249 gammy-0.5.3/gammy/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      425 2023-12-26 07:11:06.000000 gammy-0.5.3/gammy/__init__.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       22 2024-01-02 10:22:37.000000 gammy-0.5.3/gammy/__version__.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3739 2021-10-30 04:11:06.000000 gammy-0.5.3/gammy/arraymapper.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      561 2021-10-05 12:57:59.000000 gammy-0.5.3/gammy/conftest.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    13795 2021-11-19 16:52:11.000000 gammy-0.5.3/gammy/formulae.py
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.948249 gammy-0.5.3/gammy/models/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      125 2021-10-05 12:57:59.000000 gammy-0.5.3/gammy/models/__init__.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11466 2021-10-30 04:11:06.000000 gammy-0.5.3/gammy/models/bayespy.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11117 2021-10-30 04:11:06.000000 gammy-0.5.3/gammy/models/numpy.py
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.948249 gammy-0.5.3/gammy/models/tests/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     8392 2021-10-05 12:57:59.000000 gammy-0.5.3/gammy/models/tests/test_models.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     7315 2021-11-19 16:52:11.000000 gammy-0.5.3/gammy/plot.py
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.949249 gammy-0.5.3/gammy/tests/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1207 2021-10-19 20:24:01.000000 gammy-0.5.3/gammy/tests/test_arraymapper.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4322 2021-10-30 04:11:06.000000 gammy-0.5.3/gammy/tests/test_formulae.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3513 2021-10-05 12:57:59.000000 gammy-0.5.3/gammy/tests/test_smoke.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     6863 2021-10-18 08:52:43.000000 gammy-0.5.3/gammy/tests/test_utils.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     9626 2021-10-30 04:11:06.000000 gammy-0.5.3/gammy/utils.py
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-01-02 10:22:57.950249 gammy-0.5.3/gammy.egg-info/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11766 2024-01-02 10:22:57.000000 gammy-0.5.3/gammy.egg-info/PKG-INFO
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      853 2024-01-02 10:22:57.000000 gammy-0.5.3/gammy.egg-info/SOURCES.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        1 2024-01-02 10:22:57.000000 gammy-0.5.3/gammy.egg-info/dependency_links.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       97 2024-01-02 10:22:57.000000 gammy-0.5.3/gammy.egg-info/requires.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        6 2024-01-02 10:22:57.000000 gammy-0.5.3/gammy.egg-info/top_level.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      151 2023-05-03 07:52:38.000000 gammy-0.5.3/pyproject.toml
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      919 2024-01-02 10:22:57.953249 gammy-0.5.3/setup.cfg
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      148 2023-05-03 07:52:38.000000 gammy-0.5.3/setup.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.099262 gammy-0.5.4/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        0 2021-10-05 12:57:59.000000 gammy-0.5.4/.gitattributes
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       82 2024-01-02 10:48:33.000000 gammy-0.5.4/.gitignore
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4403 2024-04-18 07:43:22.000000 gammy-0.5.4/CHANGELOG.md
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1083 2021-10-05 12:57:59.000000 gammy-0.5.4/LICENSE.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       20 2021-10-05 12:57:59.000000 gammy-0.5.4/MANIFEST.in
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11812 2024-04-18 09:30:08.099262 gammy-0.5.4/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    10730 2024-04-18 07:43:22.000000 gammy-0.5.4/README.md
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.094262 gammy-0.5.4/doc/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      638 2021-10-05 12:57:59.000000 gammy-0.5.4/doc/Makefile
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.094262 gammy-0.5.4/doc/source/
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.094262 gammy-0.5.4/doc/source/_static/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        0 2021-10-05 12:57:59.000000 gammy-0.5.4/doc/source/_static/.gitkeep
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.091262 gammy-0.5.4/doc/source/_templates/
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.095262 gammy-0.5.4/doc/source/_templates/autosummary/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      147 2021-10-19 20:24:01.000000 gammy-0.5.4/doc/source/_templates/autosummary/base.rst
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      254 2021-10-05 12:57:59.000000 gammy-0.5.4/doc/source/_templates/autosummary/class.rst
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      513 2021-10-19 20:24:01.000000 gammy-0.5.4/doc/source/_templates/autosummary/module.rst
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       51 2021-10-19 20:24:01.000000 gammy-0.5.4/doc/source/api.rst
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3357 2021-11-19 16:52:11.000000 gammy-0.5.4/doc/source/conf.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1082 2021-10-30 04:11:06.000000 gammy-0.5.4/doc/source/index.rst
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      126 2021-10-05 12:57:59.000000 gammy-0.5.4/doc/source/installation.rst
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.095262 gammy-0.5.4/gammy/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      425 2023-12-26 07:11:06.000000 gammy-0.5.4/gammy/__init__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       22 2024-04-18 09:30:00.000000 gammy-0.5.4/gammy/__version__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3739 2021-10-30 04:11:06.000000 gammy-0.5.4/gammy/arraymapper.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      561 2021-10-05 12:57:59.000000 gammy-0.5.4/gammy/conftest.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    13795 2021-11-19 16:52:11.000000 gammy-0.5.4/gammy/formulae.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.097262 gammy-0.5.4/gammy/models/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      125 2021-10-05 12:57:59.000000 gammy-0.5.4/gammy/models/__init__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11466 2021-10-30 04:11:06.000000 gammy-0.5.4/gammy/models/bayespy.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11117 2021-10-30 04:11:06.000000 gammy-0.5.4/gammy/models/numpy.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.097262 gammy-0.5.4/gammy/models/tests/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     8392 2021-10-05 12:57:59.000000 gammy-0.5.4/gammy/models/tests/test_models.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     7315 2021-11-19 16:52:11.000000 gammy-0.5.4/gammy/plot.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.097262 gammy-0.5.4/gammy/tests/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1207 2021-10-19 20:24:01.000000 gammy-0.5.4/gammy/tests/test_arraymapper.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4322 2021-10-30 04:11:06.000000 gammy-0.5.4/gammy/tests/test_formulae.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3812 2024-04-18 07:43:22.000000 gammy-0.5.4/gammy/tests/test_smoke.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     6863 2021-10-18 08:52:43.000000 gammy-0.5.4/gammy/tests/test_utils.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     9626 2021-10-30 04:11:06.000000 gammy-0.5.4/gammy/utils.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2024-04-18 09:30:08.097262 gammy-0.5.4/gammy.egg-info/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11812 2024-04-18 09:30:08.000000 gammy-0.5.4/gammy.egg-info/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      853 2024-04-18 09:30:08.000000 gammy-0.5.4/gammy.egg-info/SOURCES.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        1 2024-04-18 09:30:08.000000 gammy-0.5.4/gammy.egg-info/dependency_links.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      112 2024-04-18 09:30:08.000000 gammy-0.5.4/gammy.egg-info/requires.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        6 2024-04-18 09:30:08.000000 gammy-0.5.4/gammy.egg-info/top_level.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      151 2023-05-03 07:52:38.000000 gammy-0.5.4/pyproject.toml
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      935 2024-04-18 09:30:08.100262 gammy-0.5.4/setup.cfg
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      148 2023-05-03 07:52:38.000000 gammy-0.5.4/setup.py
```

### Comparing `gammy-0.5.3/CHANGELOG.md` & `gammy-0.5.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Change Log
 
 
+## 0.5.3
+- Bump `Pillow` to `>= 10.3.0`
+
+
 ## 0.5.2
 
 ### Add
 - `Makefile` with releasing script
 - `__version__.py` source file for version in code
```

### Comparing `gammy-0.5.3/LICENSE.txt` & `gammy-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/PKG-INFO` & `gammy-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: gammy
-Version: 0.5.3
+Version: 0.5.4
 Summary: Generalized additive models with a Bayesian twist
 Home-page: https://malmgrek.github.io/gammy
 Author: Stratos Staboulis <stratos@stratokraft.fi>
 Maintainer: Stratos Staboulis <stratos@stratokraft.fi>
 License: MIT
 Keywords: bayesian,statistics,modeling,gaussian processes,splines
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy>=1.10.0
-Requires-Dist: scipy>=0.13.0
 Requires-Dist: bayespy
 Requires-Dist: h5py
+Requires-Dist: numpy>=1.10.0
+Requires-Dist: scipy>=0.13.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: pillow>=10.3.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 
 # Gammy – Generalized additive models in Python with a Bayesian twist
 
 ![](https://raw.githubusercontent.com/malmgrek/gammy/develop/doc/resources/cover.png)
@@ -87,15 +88,15 @@
 ```python
 >>> import numpy as np
 
 >>> import gammy
 >>> from gammy.models.bayespy import GAM
 
 >>> gammy.__version__
-'0.5.3'
+'0.5.4'
 
 ```
 
 Let's simulate a dataset:
 
 ```python
 >>> np.random.seed(42)
```

### Comparing `gammy-0.5.3/README.md` & `gammy-0.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ```python
 >>> import numpy as np
 
 >>> import gammy
 >>> from gammy.models.bayespy import GAM
 
 >>> gammy.__version__
-'0.5.3'
+'0.5.4'
 
 ```
 
 Let's simulate a dataset:
 
 ```python
 >>> np.random.seed(42)
```

### Comparing `gammy-0.5.3/doc/Makefile` & `gammy-0.5.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/doc/source/_templates/autosummary/module.rst` & `gammy-0.5.4/doc/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/doc/source/conf.py` & `gammy-0.5.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/doc/source/index.rst` & `gammy-0.5.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/arraymapper.py` & `gammy-0.5.4/gammy/arraymapper.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/conftest.py` & `gammy-0.5.4/gammy/conftest.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/formulae.py` & `gammy-0.5.4/gammy/formulae.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/models/bayespy.py` & `gammy-0.5.4/gammy/models/bayespy.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/models/numpy.py` & `gammy-0.5.4/gammy/models/numpy.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/models/tests/test_models.py` & `gammy-0.5.4/gammy/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/plot.py` & `gammy-0.5.4/gammy/plot.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/tests/test_arraymapper.py` & `gammy-0.5.4/gammy/tests/test_arraymapper.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/tests/test_formulae.py` & `gammy-0.5.4/gammy/tests/test_formulae.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/tests/test_smoke.py` & `gammy-0.5.4/gammy/tests/test_smoke.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 """Sanity checks for semi-realistic modeling cases
 
 """
 
+from configparser import ConfigParser
+import os
+
 import numpy as np
 from numpy.testing import assert_almost_equal
 import pytest
 
 import gammy
 from gammy.arraymapper import x
 
 
+def test_version():
+    config = ConfigParser()
+    config.read(os.path.join(os.path.dirname(__file__), "..", "..", "setup.cfg"))
+    metadata = dict(config["metadata"])
+    assert metadata["version"] == gammy.__version__, "Update package version"
+
+
 def test_polynomial(fit_model):
     np.random.seed(42)
     input_data = 10 * np.random.rand(30)
     y = (
         5 * input_data +
         2.0 * input_data ** 2 +
         7 +
```

### Comparing `gammy-0.5.3/gammy/tests/test_utils.py` & `gammy-0.5.4/gammy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy/utils.py` & `gammy-0.5.4/gammy/utils.py`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/gammy.egg-info/PKG-INFO` & `gammy-0.5.4/gammy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: gammy
-Version: 0.5.3
+Version: 0.5.4
 Summary: Generalized additive models with a Bayesian twist
 Home-page: https://malmgrek.github.io/gammy
 Author: Stratos Staboulis <stratos@stratokraft.fi>
 Maintainer: Stratos Staboulis <stratos@stratokraft.fi>
 License: MIT
 Keywords: bayesian,statistics,modeling,gaussian processes,splines
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy>=1.10.0
-Requires-Dist: scipy>=0.13.0
 Requires-Dist: bayespy
 Requires-Dist: h5py
+Requires-Dist: numpy>=1.10.0
+Requires-Dist: scipy>=0.13.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: pillow>=10.3.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 
 # Gammy – Generalized additive models in Python with a Bayesian twist
 
 ![](https://raw.githubusercontent.com/malmgrek/gammy/develop/doc/resources/cover.png)
@@ -87,15 +88,15 @@
 ```python
 >>> import numpy as np
 
 >>> import gammy
 >>> from gammy.models.bayespy import GAM
 
 >>> gammy.__version__
-'0.5.3'
+'0.5.4'
 
 ```
 
 Let's simulate a dataset:
 
 ```python
 >>> np.random.seed(42)
```

### Comparing `gammy-0.5.3/gammy.egg-info/SOURCES.txt` & `gammy-0.5.4/gammy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gammy-0.5.3/setup.cfg` & `gammy-0.5.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.5.3
+version = 0.5.4
 name = gammy
 author = Stratos Staboulis <stratos@stratokraft.fi>
 maintainer = Stratos Staboulis <stratos@stratokraft.fi>
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 	Development Status :: 3 - Alpha
@@ -16,25 +16,26 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://malmgrek.github.io/gammy
 
 [options]
 packages = find:
 install_requires = 
-	numpy>=1.10.0
-	scipy>=0.13.0
 	bayespy
 	h5py
+	numpy>=1.10.0
+	scipy>=0.13.0
 python_requires > = 3.8
 
 [options.extras_require]
 test = 
 	pytest
 dev = 
 	matplotlib
+	pillow>=10.3.0
 doc = 
 	sphinx
 	numpydoc
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

