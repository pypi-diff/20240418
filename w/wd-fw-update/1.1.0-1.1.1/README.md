# Comparing `tmp/wd_fw_update-1.1.0.tar.gz` & `tmp/wd_fw_update-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wd_fw_update-1.1.0.tar", last modified: Mon Mar 11 12:51:24 2024, max compression
+gzip compressed data, was "wd_fw_update-1.1.1.tar", last modified: Thu Apr 18 14:05:22 2024, max compression
```

## Comparing `wd_fw_update-1.1.0.tar` & `wd_fw_update-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.667790 wd_fw_update-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.659790 wd_fw_update-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.663790 wd_fw_update-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-11 12:51:24.667790 wd_fw_update-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.663790 wd_fw_update-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.663790 wd_fw_update-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-11 12:51:24.667790 wd_fw_update-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.659790 wd_fw_update-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.663790 wd_fw_update-1.1.0/src/wd_fw_update/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/src/wd_fw_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-03-11 12:51:17.000000 wd_fw_update-1.1.0/src/wd_fw_update/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:51:24.667790 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 12:51:24.000000 wd_fw_update-1.1.0/src/wd_fw_update.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.326020 wd_fw_update-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   138313 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/gif.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.326020 wd_fw_update-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/src/wd_fw_update/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/src/wd_fw_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/src/wd_fw_update/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/top_level.txt
```

### Comparing `wd_fw_update-1.1.0/.coveragerc` & `wd_fw_update-1.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/.github/workflows/python-publish.yml` & `wd_fw_update-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/.gitignore` & `wd_fw_update-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/.pre-commit-config.yaml` & `wd_fw_update-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/.readthedocs.yml` & `wd_fw_update-1.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/CONTRIBUTING.md` & `wd_fw_update-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/LICENSE` & `wd_fw_update-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/PKG-INFO` & `wd_fw_update-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.1.0
+Version: 1.1.1
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
@@ -21,15 +21,14 @@
 Requires-Dist: tqdm<5,>=4
 Requires-Dist: requests<3,>=2.2
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 
 [![ReadTheDocs](https://readthedocs.org/projects/wd_fw_update/badge/?version=latest)](https://wd-fw-update.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/wd_fw_update.svg)](https://pypi.org/project/wd_fw_update/)
-[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/wd_fw_update.svg)](https://anaconda.org/conda-forge/wd_fw_update)
 [![Monthly Downloads](https://pepy.tech/badge/wd_fw_update/month)](https://pepy.tech/project/wd_fw_update)
 
 # wd_fw_update
 <img alt="Western Digital SSD Firmware Update Tool" src=https://github.com/not-a-feature/wd_fw_update/raw/main/logo.png height=90>
 
 This is a firmware update tool for Western Digital SSDs on Ubuntu / Linux Mint.
 
@@ -37,14 +36,15 @@
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
 See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
 
+<img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
 - sudo
 - nvme-cli
```

### Comparing `wd_fw_update-1.1.0/README.md` & `wd_fw_update-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [![ReadTheDocs](https://readthedocs.org/projects/wd_fw_update/badge/?version=latest)](https://wd-fw-update.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/wd_fw_update.svg)](https://pypi.org/project/wd_fw_update/)
-[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/wd_fw_update.svg)](https://anaconda.org/conda-forge/wd_fw_update)
 [![Monthly Downloads](https://pepy.tech/badge/wd_fw_update/month)](https://pepy.tech/project/wd_fw_update)
 
 # wd_fw_update
 <img alt="Western Digital SSD Firmware Update Tool" src=https://github.com/not-a-feature/wd_fw_update/raw/main/logo.png height=90>
 
 This is a firmware update tool for Western Digital SSDs on Ubuntu / Linux Mint.
 
@@ -12,14 +11,15 @@
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
 See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
 
+<img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
 - sudo
 - nvme-cli
```

### Comparing `wd_fw_update-1.1.0/docs/Makefile` & `wd_fw_update-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/docs/conf.py` & `wd_fw_update-1.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,23 +167,20 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -297,8 +294,8 @@
     "sklearn": ("https://scikit-learn.org/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
-print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `wd_fw_update-1.1.0/docs/index.md` & `wd_fw_update-1.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/logo.png` & `wd_fw_update-1.1.1/logo.png`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/setup.cfg` & `wd_fw_update-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/setup.py` & `wd_fw_update-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/src/wd_fw_update/__init__.py` & `wd_fw_update-1.1.1/src/wd_fw_update/__init__.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.0/src/wd_fw_update/main.py` & `wd_fw_update-1.1.1/src/wd_fw_update/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import logging
 import subprocess
 import sys
 import xml.etree.ElementTree as ET
 from shutil import which
 from tempfile import NamedTemporaryFile
+from typing import Dict, List, Tuple
 
 import inquirer
 import requests
 from tqdm.auto import tqdm
 
 from wd_fw_update import __name__ as package_name
 from wd_fw_update import __version__
@@ -55,41 +56,41 @@
         help="set loglevel to DEBUG",
         action="store_const",
         const=logging.DEBUG,
     )
     return parser.parse_args(args)
 
 
-def setup_logging(loglevel):
+def setup_logging(loglevel) -> None:
     """Setup basic logging
 
     Args:
       loglevel (int): minimum loglevel for emitting messages
     """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
         level=loglevel,
         stream=sys.stdout,
         format=logformat,
         datefmt="[%Y-%m-%d %H:%M:%S]",
     )
 
 
-def check_missing_dependencies():
+def check_missing_dependencies() -> bool:
     """Check for missing dependencies
 
     Returns:
       bool: True if any dependency is missing, False otherwise
     """
     dependencies = ["sudo", "nvme"]  # List of commands to check
 
     return any(which(cmd) is None for cmd in dependencies)
 
 
-def ask_device():
+def ask_device() -> str:
     """Prompt the user to select an NVME drive for the update
 
     Returns:
       str: Selected NVME drive
     """
     _logger.debug("Getting device list.")
 
@@ -114,15 +115,15 @@
             carousel=True,
         ),
     ]
     device = inquirer.prompt(questions)["device"]
     return device
 
 
-def get_model_properties(device):
+def get_model_properties(device) -> Dict:
     """Retrieve model properties for the specified NVME device
 
     Args:
       device (str): NVME device identifier
 
     Returns:
       dict: Model properties
@@ -140,15 +141,15 @@
     for line in result.stdout.split("\n")[1:]:
         if ":" in line:
             k, v = line.split(":", 1)
             model_properties[k.strip()] = v.strip()
     return model_properties
 
 
-def get_fw_url(model):
+def get_fw_url(model) -> List[str]:
     """Fetch firmware URL for the specified model from the device list
 
     Args:
       model (str): Model name
 
     Returns:
       list: List of firmware URLs
@@ -162,15 +163,15 @@
     for device in root.findall("lista_device"):
         if device.get("model") == model:
             return [u.text for u in device.findall("url")]
 
     raise RuntimeError("No Firmware found for this model. Please check your selection / model.")
 
 
-def ask_fw_version(relative_urls, model, current_fw_version):
+def ask_fw_version(device, relative_urls, model, current_fw_version) -> str:
     """Prompt the user to select a firmware version
 
     Args:
       relative_urls (list): List of firmware URLs
       model (str): Model name
       current_fw_version (str): Current firmware version
 
@@ -180,14 +181,18 @@
     if not relative_urls:
         raise RuntimeWarning("No Firmware Version to select.")
 
     fw_versions = [v for url in relative_urls if not (v := url.split("/")[3]) == current_fw_version]
     _logger.debug(f"Firmware versions: f{fw_versions}")
 
     if not fw_versions:
+        print("========== Summary ==========")
+        print(f"NVME location:     {device}")
+        print(f"Model:             {model}")
+        print(f"Firmware Version:  {current_fw_version}")
         print("No different / newer firmware version found.")
         print("You are probably already on the latest version.")
         exit(0)
 
     if len(fw_versions) == 1:
         _logger.debug("Only one firmware to select, skipping user-promt.")
 
@@ -203,15 +208,15 @@
             ),
         ]
         version = inquirer.prompt(questions)["version"]
 
     return version
 
 
-def ask_slot(device):
+def ask_slot(device) -> Tuple[int, int]:
     """Prompt the user to select a firmware slot
 
     Args:
       device (str): NVME device identifier
 
     Returns:
       int, int: Current active firmware slot, Selected firmware slot
@@ -236,16 +241,18 @@
                 next Controller Level Reset. If this field is 0h, then the
                 controller does not indicate the firmware slot that is
                 going to be activated at the next Controller Level Reset.
 
     - Bit 3     Reserved.
     - Bits 2:0  The firmware slot from which the actively running firmware revision was loaded.
     """
-    current_slot = int(result[1].split(":")[1], 0)  # From Hex to Base 10.
-    current_slot = int("0b" + bin(current_slot)[-2:], base=0)  # Take last two bits
+    current_slot = result[1].split(":")[1].strip()
+    current_slot = int(current_slot, 0)  # From Hex to Base 10
+    if not current_slot == 1:
+        current_slot = int("0b" + bin(current_slot)[-2:], base=0)  # Take last two bits
 
     print(f"Current Active Firmware Slot (afi): {current_slot}")
 
     slots = [s[3:] for s in sorted(result[2:10]) if s]
     _logger.debug(f"Firmware slots: {slots}")
 
     if len(slots) == 1:
@@ -263,15 +270,15 @@
         ),
     ]
     slot = inquirer.prompt(questions)["slot"]
     slot = int(slot.split(":", 1)[0])
     return current_slot, slot
 
 
-def ask_mode():
+def ask_mode() -> int:
     """Prompt the user to select the firmware update mode
 
     Returns:
       int: Selected update mode
     """
     o0 = "0 Downloaded image replaces the image indicated by the Firmware Slot field. This image is not activated."
     o1 = "1 Downloaded image replaces the image indicated by the Firmware Slot field. This image is activated at the next reset."
@@ -289,15 +296,15 @@
         ),
     ]
     mode = inquirer.prompt(questions)["mode"]
     mode = int(mode.split(" ", 1)[0])
     return mode
 
 
-def update_fw(version, current_fw_version, model, device, current_slot, slot, mode):
+def update_fw(version, current_fw_version, model, device, current_slot, slot, mode) -> bool:
     """Update firmware for the specified NVME device
 
     Args:
       version (str): Firmware version to be installed
       current_fw_version (str): Current firmware version
       model (str): Model name
       device (str): NVME device identifier
@@ -402,15 +409,15 @@
         _logger.debug(f"NVME Commit returncode: {result.returncode}")
 
     if result.returncode == 0:
         success = True
     else:
         success = False
 
-    return success, mode
+    return success
 
 
 def wd_fw_update():
     """Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
     The user will be prompted for version / model / slot selection.
     """
     _logger.info("Starting firmware update process.")
@@ -433,27 +440,28 @@
     model = model_properties["mn"]
     relative_urls = get_fw_url(model=model)
 
     # Step 3: Check firmware version and dependencies
     current_fw_version = model_properties["fr"]
 
     selected_version = ask_fw_version(
-        relative_urls,
+        device=device,
+        relative_urls=relative_urls,
         model=model,
         current_fw_version=current_fw_version,
     )
 
     # Step 4: Ask for the slot to install the firmware
     current_slot, slot = ask_slot(device)
 
     # Step 5: Ask for installation mode
     mode = ask_mode()
 
     # Step 6: Download and install the firmware file
-    result, mode = update_fw(
+    result = update_fw(
         version=selected_version,
         current_fw_version=current_fw_version,
         model=model,
         device=device,
         current_slot=current_slot,
         slot=slot,
         mode=mode,
```

### Comparing `wd_fw_update-1.1.0/src/wd_fw_update.egg-info/PKG-INFO` & `wd_fw_update-1.1.1/src/wd_fw_update.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.1.0
+Version: 1.1.1
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
@@ -21,15 +21,14 @@
 Requires-Dist: tqdm<5,>=4
 Requires-Dist: requests<3,>=2.2
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 
 [![ReadTheDocs](https://readthedocs.org/projects/wd_fw_update/badge/?version=latest)](https://wd-fw-update.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/wd_fw_update.svg)](https://pypi.org/project/wd_fw_update/)
-[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/wd_fw_update.svg)](https://anaconda.org/conda-forge/wd_fw_update)
 [![Monthly Downloads](https://pepy.tech/badge/wd_fw_update/month)](https://pepy.tech/project/wd_fw_update)
 
 # wd_fw_update
 <img alt="Western Digital SSD Firmware Update Tool" src=https://github.com/not-a-feature/wd_fw_update/raw/main/logo.png height=90>
 
 This is a firmware update tool for Western Digital SSDs on Ubuntu / Linux Mint.
 
@@ -37,14 +36,15 @@
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
 See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
 
+<img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
 - sudo
 - nvme-cli
```

### Comparing `wd_fw_update-1.1.0/src/wd_fw_update.egg-info/SOURCES.txt` & `wd_fw_update-1.1.1/src/wd_fw_update.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 README.md
+gif.gif
 logo.png
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci.yml
 .github/workflows/python-publish.yml
 docs/Makefile
```

