# Comparing `tmp/generate-sequences-0.0.0.tar.gz` & `tmp/generate_sequences-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate-sequences-0.0.0.tar", last modified: Sat Mar 30 12:35:02 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.1.tar", last modified: Thu Apr 18 14:46:18 2024, max compression
```

## Comparing `generate-sequences-0.0.0.tar` & `generate_sequences-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:35:02.517669 generate-sequences-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-30 12:35:02.517669 generate-sequences-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:35:02.513669 generate-sequences-0.0.0/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:35:02.517669 generate-sequences-0.0.0/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-30 12:35:02.000000 generate-sequences-0.0.0/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-30 12:35:02.000000 generate-sequences-0.0.0/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:35:02.000000 generate-sequences-0.0.0/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-30 12:35:02.000000 generate-sequences-0.0.0/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 12:35:02.000000 generate-sequences-0.0.0/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-30 12:34:45.000000 generate-sequences-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:35:02.517669 generate-sequences-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.984746 generate_sequences-0.0.1/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.984746 generate_sequences-0.0.1/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/setup.cfg
```

### Comparing `generate-sequences-0.0.0/LICENSE` & `generate_sequences-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `generate-sequences-0.0.0/PKG-INFO` & `generate_sequences-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.0
+Version: 0.0.1
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -211,14 +211,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm==4.66.*
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: torch==2.2.*
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
@@ -230,9 +233,15 @@
 Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
 Requires-Dist: furo==2024.1.29; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
+Requires-Dist: pre-commit==3.5.0; extra == "dev"
+Requires-Dist: evaluate==0.4.*; extra == "dev"
+Requires-Dist: sacrebleu==2.4.*; extra == "dev"
+Requires-Dist: sacremoses==0.1.*; extra == "dev"
+Requires-Dist: sentencepiece==0.2.*; extra == "dev"
+Requires-Dist: transformers==4.39.*; extra == "dev"
 
 # generate-sequences
```

### Comparing `generate-sequences-0.0.0/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.1/generate_sequences.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.0
+Version: 0.0.1
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -211,14 +211,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm==4.66.*
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: torch==2.2.*
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
@@ -230,9 +233,15 @@
 Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
 Requires-Dist: furo==2024.1.29; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
+Requires-Dist: pre-commit==3.5.0; extra == "dev"
+Requires-Dist: evaluate==0.4.*; extra == "dev"
+Requires-Dist: sacrebleu==2.4.*; extra == "dev"
+Requires-Dist: sacremoses==0.1.*; extra == "dev"
+Requires-Dist: sentencepiece==0.2.*; extra == "dev"
+Requires-Dist: transformers==4.39.*; extra == "dev"
 
 # generate-sequences
```

### Comparing `generate-sequences-0.0.0/pyproject.toml` & `generate_sequences-0.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,75 +4,76 @@
 
 [project]
 # See https://setuptools.pypa.io/en/latest/userguide/quickstart.html for more project configuration options.
 name = "generate-sequences"
 dynamic = ["version"]
 readme = "README.md"
 classifiers = [
-    "Intended Audience :: Science/Research",
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-]
-authors = [
-    {name = "Maged S. Al-Shaibani", email = "mageedsaeed1@gmail.com"}
+  "Intended Audience :: Science/Research",
+  "Development Status :: 3 - Alpha",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python :: 3",
+  "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
+authors = [{ name = "Maged S. Al-Shaibani", email = "mageedsaeed1@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
   # Add your own dependencies here
+  "tqdm==4.66.*",
+  "numpy>=1.24.0",
+  "torch==2.2.*",
 ]
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/MagedSaeed/generate-sequences"
 Repository = "https://github.com/MagedSaeed/generate-sequences"
 Changelog = "https://github.com/MagedSaeed/generate-sequences/blob/main/CHANGELOG.md"
 # Documentation = "https://generate-sequences.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
-    "ruff",
-    "mypy>=1.0,<1.10",
-    "black>=23.0,<25.0",
-    "isort>=5.12,<5.14",
-    "pytest",
-    "pytest-sphinx",
-    "pytest-cov",
-    "twine>=1.11.0",
-    "build",
-    "setuptools",
-    "wheel",
-    "Sphinx>=4.3.0,<7.3.0",
-    "furo==2024.1.29",
-    "myst-parser>=1.0,<2.1",
-    "sphinx-copybutton==0.5.2",
-    "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==2.0.0",
-    "packaging"
+  "ruff",
+  "mypy>=1.0,<1.10",
+  "black>=23.0,<25.0",
+  "isort>=5.12,<5.14",
+  "pytest",
+  "pytest-sphinx",
+  "pytest-cov",
+  "twine>=1.11.0",
+  "build",
+  "setuptools",
+  "wheel",
+  "Sphinx>=4.3.0,<7.3.0",
+  "furo==2024.1.29",
+  "myst-parser>=1.0,<2.1",
+  "sphinx-copybutton==0.5.2",
+  "sphinx-autobuild==2021.3.14",
+  "sphinx-autodoc-typehints==2.0.0",
+  "packaging",
+  "pre-commit==3.5.0",
+  # added for testing
+  "evaluate==0.4.*",
+  "sacrebleu==2.4.*",
+  "sacremoses==0.1.*",
+  "sentencepiece==0.2.*",
+  "transformers==4.39.*",
 ]
 
 [tool.setuptools.packages.find]
-exclude = [
-    "*.tests",
-    "*.tests.*",
-    "tests.*",
-    "tests",
-    "docs*",
-    "scripts*"
-]
+exclude = ["*.tests", "*.tests.*", "tests.*", "tests", "docs*", "scripts*"]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 generate_sequences = ["py.typed"]
 
 [tool.setuptools.dynamic]
-version = {attr = "generate_sequences.version.VERSION"}
+version = { attr = "generate_sequences.version.VERSION" }
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 (
       __pycache__
@@ -108,13 +109,10 @@
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 strict_optional = false
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
-python_classes = [
-  "Test*",
-  "*Test"
-]
+python_classes = ["Test*", "*Test"]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
```

