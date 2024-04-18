# Comparing `tmp/quirtylog-0.2.0.tar.gz` & `tmp/quirtylog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quirtylog-0.2.0.tar", last modified: Wed Feb 28 13:58:59 2024, max compression
+gzip compressed data, was "quirtylog-0.3.0.tar", last modified: Thu Apr 18 13:22:53 2024, max compression
```

## Comparing `quirtylog-0.2.0.tar` & `quirtylog-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:58:59.236808 quirtylog-0.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)       12 2024-02-28 13:58:47.000000 quirtylog-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-28 13:58:47.000000 quirtylog-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-28 13:58:47.000000 quirtylog-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-28 13:58:47.000000 quirtylog-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-28 13:58:59.236808 quirtylog-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-28 13:58:47.000000 quirtylog-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-02-28 13:58:47.000000 quirtylog-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:58:59.232808 quirtylog-0.2.0/quirtylog/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/sqlite_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-28 13:58:47.000000 quirtylog-0.2.0/quirtylog/tqdm_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:58:59.232808 quirtylog-0.2.0/quirtylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-28 13:58:59.000000 quirtylog-0.2.0/quirtylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-28 13:58:59.000000 quirtylog-0.2.0/quirtylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 13:58:59.000000 quirtylog-0.2.0/quirtylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-28 13:58:59.000000 quirtylog-0.2.0/quirtylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-28 13:58:59.000000 quirtylog-0.2.0/quirtylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 13:58:59.236808 quirtylog-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:22:53.989059 quirtylog-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       12 2024-04-18 13:22:50.000000 quirtylog-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-18 13:22:50.000000 quirtylog-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 13:22:50.000000 quirtylog-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 13:22:50.000000 quirtylog-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 13:22:53.989059 quirtylog-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-18 13:22:50.000000 quirtylog-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 13:22:50.000000 quirtylog-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:22:53.985059 quirtylog-0.3.0/quirtylog/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/sqlite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-18 13:22:50.000000 quirtylog-0.3.0/quirtylog/tqdm_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:22:53.989059 quirtylog-0.3.0/quirtylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 13:22:53.000000 quirtylog-0.3.0/quirtylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 13:22:53.000000 quirtylog-0.3.0/quirtylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:22:53.000000 quirtylog-0.3.0/quirtylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 13:22:53.000000 quirtylog-0.3.0/quirtylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 13:22:53.000000 quirtylog-0.3.0/quirtylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:22:53.989059 quirtylog-0.3.0/setup.cfg
```

### Comparing `quirtylog-0.2.0/CONTRIBUTING.md` & `quirtylog-0.3.0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,11 +27,7 @@
 A common error on `macOS` is related to `UTC-8` format. See [this](https://stackoverflow.com/questions/60557160/python3-8-fails-with-fatal-python-error-config-get-locale-encoding) issue
 on StackOverflow. To update the tool use `pre-commit autoupdate`.
 
 
 ### Contributors
 
 Authors and contributors have been collected in [`AUTHORS.rst`](AUTHORS.rst) file.
-
-### Dockerization
-A minimal `docker` environment is contained in [`Dockerfile`](Dockerfile).
-The command is `docker build -t quirty .`
```

### Comparing `quirtylog-0.2.0/LICENSE` & `quirtylog-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/PKG-INFO` & `quirtylog-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quirtylog
-Version: 0.2.0
+Version: 0.3.0
 Author-email: agdiiura <andreadiiura@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 quirtylog
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,21 +30,21 @@
 Requires-Dist: coloredlogs>=10.0
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: requests>=2.18.4
 Requires-Dist: tqdm>=4.66.1
 Provides-Extra: build
-Requires-Dist: ruff>=0.2.0; extra == "build"
+Requires-Dist: ruff>=0.3.0; extra == "build"
 Requires-Dist: colorama>=0.4.6; extra == "build"
 Requires-Dist: coverage>=7.0; extra == "build"
 Requires-Dist: isort>=5.12.0; extra == "build"
 Requires-Dist: pre-commit>=3.3.0; extra == "build"
 Requires-Dist: setuptools-git-versioning>=1.13.4; extra == "build"
-Requires-Dist: xmlrunner>=1.7.7; extra == "build"
+Requires-Dist: unittest-xml-reporting>=3.2.0; extra == "build"
 Provides-Extra: docs
 Requires-Dist: GitPython>=3.1.3; extra == "docs"
 Requires-Dist: recommonmark>=0.5.0; extra == "docs"
 Requires-Dist: requests>=2.23.0; extra == "docs"
 Requires-Dist: Sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.20.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=2.0.0; extra == "docs"
@@ -55,17 +55,14 @@
 
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Quick & dirty logging in python.
 
 
-The file `requirements.txt` contains the packages needed for the installation.
-The code requires `python3.11+`.
-
 ### Installation
 To install the package the simplest procedure is:
 ```bash
 pip install quirtylog
 ```
 Now you can test the installation... In a python shell:
 
@@ -78,14 +75,17 @@
 #### Installation from source
 Once you have cloned the repository
 ```bash
 pip install .
 ```
 To use the develop mode just write `pip install -e .`.
 
+The file `pyproject.toml` contains the packages needed for the installation.
+The code requires `python3.11+`.
+
 
 ### Examples
 The package creates custom loggers object.
 
 ```python
 import quirtylog
 
@@ -106,15 +106,20 @@
 
 
 @quirtylog.measure_time(logger)
 def g(x):
     """A function that raise an exception"""
     return x / 0.
 ```
+It can also be used as a wrapper for
+external scripts
 
+```bash
+python -m quirtylog main.py
+```
 For further examples see the folder [`examples`](examples).
 
 ### Contributing
 If you want to contribute to this project, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ### Official soundtrack
 [Jhonny Cash - The Frozen Logger](https://www.youtube.com/watch?v=KUfzDIKGkQI)
```

### Comparing `quirtylog-0.2.0/README.md` & `quirtylog-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Quick & dirty logging in python.
 
 
-The file `requirements.txt` contains the packages needed for the installation.
-The code requires `python3.11+`.
-
 ### Installation
 To install the package the simplest procedure is:
 ```bash
 pip install quirtylog
 ```
 Now you can test the installation... In a python shell:
 
@@ -27,14 +24,17 @@
 #### Installation from source
 Once you have cloned the repository
 ```bash
 pip install .
 ```
 To use the develop mode just write `pip install -e .`.
 
+The file `pyproject.toml` contains the packages needed for the installation.
+The code requires `python3.11+`.
+
 
 ### Examples
 The package creates custom loggers object.
 
 ```python
 import quirtylog
 
@@ -55,15 +55,20 @@
 
 
 @quirtylog.measure_time(logger)
 def g(x):
     """A function that raise an exception"""
     return x / 0.
 ```
+It can also be used as a wrapper for
+external scripts
 
+```bash
+python -m quirtylog main.py
+```
 For further examples see the folder [`examples`](examples).
 
 ### Contributing
 If you want to contribute to this project, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ### Official soundtrack
 [Jhonny Cash - The Frozen Logger](https://www.youtube.com/watch?v=KUfzDIKGkQI)
```

### Comparing `quirtylog-0.2.0/pyproject.toml` & `quirtylog-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-git-versioning", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quirtylog"
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 authors = [
     {name = "agdiiura", email="andreadiiura@gmail.com"}
 ]
 license = {file = 'LICENSE'}
 dependencies = [
     "coloredlogs>=10.0",
@@ -23,34 +23,34 @@
     "PyYAML>=6.0.1",
     "requests>=2.18.4",
     "tqdm>=4.66.1"
 ]
 
 [project.optional-dependencies]
 build = [
-    "ruff>=0.2.0",
+    "ruff>=0.3.0",
     "colorama>=0.4.6",
     "coverage>=7.0",
     "isort>=5.12.0",
     "pre-commit>=3.3.0",
     "setuptools-git-versioning>=1.13.4",
-    "xmlrunner>=1.7.7"
+    "unittest-xml-reporting>=3.2.0"
 ]
 docs = [
     "GitPython>=3.1.3",
     "recommonmark>=0.5.0",
     "requests>=2.23.0",
     "Sphinx==7.2.6",
     "sphinx-autodoc-typehints>=1.20.0",
     "sphinx-rtd-theme>=2.0.0"
 ]
 
 [tool.ruff]
 src = ['quirtylog']
-line-length = 119
+line-length = 90
 
 [tool.ruff.lint]
 select = ['E', 'W', 'D']
 ignore = [
     #"W503",
     #"W504",
     "E402",
@@ -77,14 +77,17 @@
 
 [tool.ruff.lint.per-file-ignores]
 "*__init__.py" = ["F401", "F403"]
 "setup.py" = ["F401", "D100"]
 #"tests/*.py" = ["I900"]
 #"examples/*.py" = ["I900"]
 
+[tool.ruff.lint.pycodestyle]
+max-line-length = 119
+
 [tool.isort]
 combine_as_imports = true
 multi_line_output = 0
 length_sort = true
 lines_between_types = 1
 sections = ["FUTURE","STDLIB","THIRDPARTY","FIRSTPARTY","LOCALFOLDER"]
```

### Comparing `quirtylog-0.2.0/quirtylog/__init__.py` & `quirtylog-0.3.0/quirtylog/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def _read_version():
     """Read version from metadata or pyproject.toml"""
 
     try:
         return version("quirtylog")
 
-    except Exception:
+    except Exception:  # pragma: no cover
         # For development
         file = Path(__file__).absolute().parents[1] / "pyproject.toml"
 
         if file.exists():
             with open(file, "r") as f:
                 lines = f.read().splitlines()
                 for line in lines:
```

### Comparing `quirtylog-0.2.0/quirtylog/core.py` & `quirtylog-0.3.0/quirtylog/core.py`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/quirtylog/logging.yaml` & `quirtylog-0.3.0/quirtylog/logging.yaml`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/quirtylog/singleton.py` & `quirtylog-0.3.0/quirtylog/singleton.py`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/quirtylog/sqlite_logger.py` & `quirtylog-0.3.0/quirtylog/sqlite_logger.py`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/quirtylog/tqdm_logger.py` & `quirtylog-0.3.0/quirtylog/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `quirtylog-0.2.0/quirtylog.egg-info/PKG-INFO` & `quirtylog-0.3.0/quirtylog.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quirtylog
-Version: 0.2.0
+Version: 0.3.0
 Author-email: agdiiura <andreadiiura@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 quirtylog
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,21 +30,21 @@
 Requires-Dist: coloredlogs>=10.0
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: requests>=2.18.4
 Requires-Dist: tqdm>=4.66.1
 Provides-Extra: build
-Requires-Dist: ruff>=0.2.0; extra == "build"
+Requires-Dist: ruff>=0.3.0; extra == "build"
 Requires-Dist: colorama>=0.4.6; extra == "build"
 Requires-Dist: coverage>=7.0; extra == "build"
 Requires-Dist: isort>=5.12.0; extra == "build"
 Requires-Dist: pre-commit>=3.3.0; extra == "build"
 Requires-Dist: setuptools-git-versioning>=1.13.4; extra == "build"
-Requires-Dist: xmlrunner>=1.7.7; extra == "build"
+Requires-Dist: unittest-xml-reporting>=3.2.0; extra == "build"
 Provides-Extra: docs
 Requires-Dist: GitPython>=3.1.3; extra == "docs"
 Requires-Dist: recommonmark>=0.5.0; extra == "docs"
 Requires-Dist: requests>=2.23.0; extra == "docs"
 Requires-Dist: Sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.20.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=2.0.0; extra == "docs"
@@ -55,17 +55,14 @@
 
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Quick & dirty logging in python.
 
 
-The file `requirements.txt` contains the packages needed for the installation.
-The code requires `python3.11+`.
-
 ### Installation
 To install the package the simplest procedure is:
 ```bash
 pip install quirtylog
 ```
 Now you can test the installation... In a python shell:
 
@@ -78,14 +75,17 @@
 #### Installation from source
 Once you have cloned the repository
 ```bash
 pip install .
 ```
 To use the develop mode just write `pip install -e .`.
 
+The file `pyproject.toml` contains the packages needed for the installation.
+The code requires `python3.11+`.
+
 
 ### Examples
 The package creates custom loggers object.
 
 ```python
 import quirtylog
 
@@ -106,15 +106,20 @@
 
 
 @quirtylog.measure_time(logger)
 def g(x):
     """A function that raise an exception"""
     return x / 0.
 ```
+It can also be used as a wrapper for
+external scripts
 
+```bash
+python -m quirtylog main.py
+```
 For further examples see the folder [`examples`](examples).
 
 ### Contributing
 If you want to contribute to this project, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ### Official soundtrack
 [Jhonny Cash - The Frozen Logger](https://www.youtube.com/watch?v=KUfzDIKGkQI)
```

