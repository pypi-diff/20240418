# Comparing `tmp/django_strict_fields-1.3.1.tar.gz` & `tmp/django_strict_fields-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_strict_fields-1.3.1.tar", max compression
+gzip compressed data, was "django_strict_fields-1.3.2.tar", max compression
```

## Comparing `django_strict_fields-1.3.1.tar` & `django_strict_fields-1.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1456 2024-04-06 16:49:42.202648 django_strict_fields-1.3.1/LICENSE
--rw-r--r--   0        0        0      829 2024-04-06 16:49:42.202648 django_strict_fields-1.3.1/README.md
--rw-r--r--   0        0        0     2251 2024-04-06 16:50:25.818954 django_strict_fields-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      442 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/__init__.py
--rw-r--r--   0        0        0     3032 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/apps.py
--rw-r--r--   0        0        0     2900 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/fields.py
--rw-r--r--   0        0        0      990 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/helpers.py
--rw-r--r--   0        0        0       87 2024-04-06 16:49:42.206648 django_strict_fields-1.3.1/strict_fields/version.py
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 django_strict_fields-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/LICENSE
+-rw-r--r--   0        0        0      829 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/README.md
+-rw-r--r--   0        0        0     2470 2024-04-18 12:17:57.705106 django_strict_fields-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      442 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/apps.py
+-rw-r--r--   0        0        0     2900 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/fields.py
+-rw-r--r--   0        0        0      990 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/helpers.py
+-rw-r--r--   0        0        0       87 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/version.py
+-rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 django_strict_fields-1.3.2/PKG-INFO
```

### Comparing `django_strict_fields-1.3.1/LICENSE` & `django_strict_fields-1.3.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `django_strict_fields-1.3.1/README.md` & `django_strict_fields-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.1/pyproject.toml` & `django_strict_fields-1.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,106 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py38']
-
 [tool.coverage.run]
 branch = true
 source = ["strict_fields"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "django-strict-fields"
 packages = [
   { include = "strict_fields" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.1"
+version = "1.3.2"
 description = "A collection of fields and utilities to help make model fields more strict."
 authors = ["Tomas Arni Jonasson"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
+  
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
+  
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Opus10/django-strict-fields"
 repository = "https://github.com/Opus10/django-strict-fields"
 documentation = "https://django-strict-fields.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
 django = ">=3"
 
 [tool.poetry.dev-dependencies]
-black = "23.9.1"
-dj-database-url = "2.1.0"
 git-tidy = "1.2.0"
-psycopg2-binary = "2.9.9"
 pytest = "7.4.2"
 pytest-cov = "4.1.0"
 pytest-dotenv = "0.5.2"
-pytest-django = "4.5.2"
 pytest-mock = "3.1.0"
-django-dynamic-fixture = "4.0.1"
 tox = "4.11.3"
-ruff = "0.0.292"
+ruff = "0.3.7"
+pyright = "1.1.358"
 mkdocs = "1.5.3"
-mkdocs-material = "9.4.4"
-mkdocstrings-python = "1.7.2"
+black = "24.4.0"
+mkdocs-material = "9.5.18"
+mkdocstrings-python = "1.9.2"
 footing = "*"
 setuptools = "*"
 poetry-core = "*"
+dj-database-url = "2.1.0"
+psycopg2-binary = "2.9.9"
+pytest-django = "4.5.2"
+django-dynamic-fixture = "4.0.1"
+
 
 [tool.pytest.ini_options]
 xfail_strict = true
-addopts = "--reuse-db"
 testpaths = "strict_fields/tests"
 norecursedirs = ".venv"
+addopts = "--reuse-db"
 DJANGO_SETTINGS_MODULE = "settings"
 
 [tool.ruff]
-select = ["E", "F", "B", "I", "G", "C4"]
+lint.select = ["E", "F", "B", "I", "G", "C4"]
 line-length = 99
 target-version = "py38"
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/migrations/**",
+    "**/tests/**",
+]
+pythonVersion = "3.8"
+typeCheckingMode = "standard"
```

### Comparing `django_strict_fields-1.3.1/strict_fields/apps.py` & `django_strict_fields-1.3.2/strict_fields/apps.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.1/strict_fields/fields.py` & `django_strict_fields-1.3.2/strict_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.1/strict_fields/helpers.py` & `django_strict_fields-1.3.2/strict_fields/helpers.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.1/PKG-INFO` & `django_strict_fields-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-strict-fields
-Version: 1.3.1
+Version: 1.3.2
 Summary: A collection of fields and utilities to help make model fields more strict.
 Home-page: https://github.com/Opus10/django-strict-fields
 License: BSD-3-Clause
 Author: Tomas Arni Jonasson
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -17,16 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: django (>=3)
 Project-URL: Documentation, https://django-strict-fields.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-strict-fields
 Description-Content-Type: text/markdown
 
 # django-strict-fields
```

