# Comparing `tmp/panoptes-data-0.1.5.tar.gz` & `tmp/panoptes_data-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptes-data-0.1.5.tar", last modified: Sat Feb  3 09:16:44 2024, max compression
+gzip compressed data, was "panoptes_data-0.1.6.tar", last modified: Thu Apr 18 19:35:33 2024, max compression
```

## Comparing `panoptes-data-0.1.5.tar` & `panoptes_data-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.168313 panoptes-data-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.176313 panoptes-data-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.github/workflows/create-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.176313 panoptes-data-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.176313 panoptes-data-0.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.176313 panoptes-data-0.1.5/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   277957 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/notebooks/ObservationBasicStats.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    41975 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/notebooks/SearchObservations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.172313 panoptes-data-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.172313 panoptes-data-0.1.5/src/panoptes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/src/panoptes/data/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.172313 panoptes-data-0.1.5/src/panoptes/data/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/src/panoptes/data/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/src/panoptes/data/utils/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/src/panoptes_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 09:16:43.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-03 09:16:44.000000 panoptes-data-0.1.5/src/panoptes_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:16:44.180313 panoptes-data-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/tests/test_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-03 09:15:55.000000 panoptes-data-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.343132 panoptes_data-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.331132 panoptes_data-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.github/workflows/create-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-18 19:35:33.343132 panoptes_data-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   277957 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/notebooks/ObservationBasicStats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    41975 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/notebooks/SearchObservations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-18 19:35:33.343132 panoptes_data-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.335132 panoptes_data-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.335132 panoptes_data-0.1.6/src/panoptes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/src/panoptes/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.335132 panoptes_data-0.1.6/src/panoptes/data/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.339132 panoptes_data-0.1.6/src/panoptes/data/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/src/panoptes/data/utils/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.343132 panoptes_data-0.1.6/src/panoptes_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 19:35:33.000000 panoptes_data-0.1.6/src/panoptes_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:35:33.343132 panoptes_data-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/tests/test_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 19:34:43.000000 panoptes_data-0.1.6/tox.ini
```

### Comparing `panoptes-data-0.1.5/.coveragerc` & `panoptes_data-0.1.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/.github/workflows/create-release.yml` & `panoptes_data-0.1.6/.github/workflows/create-release.yml`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/.gitignore` & `panoptes_data-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/.pre-commit-config.yaml` & `panoptes_data-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/.readthedocs.yaml` & `panoptes_data-0.1.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/CHANGELOG.md` & `panoptes_data-0.1.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/CODE_OF_CONDUCT.md` & `panoptes_data-0.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/CONTRIBUTING.md` & `panoptes_data-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/LICENSE.txt` & `panoptes_data-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/PKG-INFO` & `panoptes_data-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes-data
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for working with PANOPTES data.
 Home-page: https://github.com/panoptes/panoptes-data
 Author: Wilfred Tyler Gee
 Author-email: wtylergee@gmail.com
 License: MIT
 Project-URL: Documentation, https://projectpanoptes.org/
 Project-URL: Source, https://github.com/panoptes/panoptes-data/
```

### Comparing `panoptes-data-0.1.5/README.md` & `panoptes_data-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/docs/Makefile` & `panoptes_data-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/docs/conf.py` & `panoptes_data-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/notebooks/ObservationBasicStats.ipynb` & `panoptes_data-0.1.6/notebooks/ObservationBasicStats.ipynb`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/notebooks/SearchObservations.ipynb` & `panoptes_data-0.1.6/notebooks/SearchObservations.ipynb`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/setup.cfg` & `panoptes_data-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/setup.py` & `panoptes_data-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes/data/__init__.py` & `panoptes_data-0.1.6/src/panoptes/data/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes/data/images.py` & `panoptes_data-0.1.6/src/panoptes/data/images.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes/data/observations.py` & `panoptes_data-0.1.6/src/panoptes/data/observations.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,18 +93,16 @@
         images_df = images_df.set_index(['time']).sort_index()
 
         if query > '':
             images_df = images_df.query(query)
 
         return images_df
 
-    def get_image_list(self):
+    def get_image_list(self, bucket='panoptes-images-incoming', file_ext='.fits.fz'):
         """Get the images for the observation."""
-        bucket = 'panoptes-images'
-        file_ext = '.fits.fz'
 
         # Build up the image list from the metadata.
         image_list = [self._settings.img_base_url.unicode_string()
                       + bucket + '/'
                       + str(s).replace("_", "/")
                       + file_ext for s in
                       self.image_metadata.uid.values]
```

### Comparing `panoptes-data-0.1.5/src/panoptes/data/search.py` & `panoptes_data-0.1.6/src/panoptes/data/search.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes/data/settings.py` & `panoptes_data-0.1.6/src/panoptes/data/settings.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes/data/utils/cli/main.py` & `panoptes_data-0.1.6/src/panoptes/data/utils/cli/main.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/src/panoptes_data.egg-info/PKG-INFO` & `panoptes_data-0.1.6/src/panoptes_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes-data
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for working with PANOPTES data.
 Home-page: https://github.com/panoptes/panoptes-data
 Author: Wilfred Tyler Gee
 Author-email: wtylergee@gmail.com
 License: MIT
 Project-URL: Documentation, https://projectpanoptes.org/
 Project-URL: Source, https://github.com/panoptes/panoptes-data/
```

### Comparing `panoptes-data-0.1.5/src/panoptes_data.egg-info/SOURCES.txt` & `panoptes_data-0.1.6/src/panoptes_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/tests/test_skeleton.py` & `panoptes_data-0.1.6/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `panoptes-data-0.1.5/tox.ini` & `panoptes_data-0.1.6/tox.ini`

 * *Files identical despite different names*

