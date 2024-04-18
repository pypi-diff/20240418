# Comparing `tmp/makenew_pypackage-5.0.1.tar.gz` & `tmp/makenew_pypackage-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makenew_pypackage-5.0.1.tar", max compression
+gzip compressed data, was "makenew_pypackage-5.1.0.tar", max compression
```

## Comparing `makenew_pypackage-5.0.1.tar` & `makenew_pypackage-5.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/LICENSE.txt
--rw-r--r--   0        0        0     6865 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/README.rst
--rw-r--r--   0        0        0       46 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/__init__.py
--rw-r--r--   0        0        0       56 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/todo.py
--rw-r--r--   0        0        0      156 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/todo_test.py
--rw-r--r--   0        0        0      615 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 makenew_pypackage-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     7662 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/README.rst
+-rw-r--r--   0        0        0       46 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/todo.py
+-rw-r--r--   0        0        0      156 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/todo_test.py
+-rw-r--r--   0        0        0      615 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 makenew_pypackage-5.1.0/PKG-INFO
```

### Comparing `makenew_pypackage-5.0.1/LICENSE.txt` & `makenew_pypackage-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `makenew_pypackage-5.0.1/README.rst` & `makenew_pypackage-5.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,27 +24,31 @@
 
 - Publishing to PyPI_.
 - Secure dependency management with Poetry_.
 - Linting with Pylint_.
 - Uncompromising code formatting with Black_.
 - pytest_ helps you write better programs.
 - Code coverage reporting with Codecov_.
-- Continuous testing and deployment with `GitHub Actions`__.
+- Fully automated version management and package publishing with semantic-release__.
+- Continuous checks and tests with `GitHub Actions`__.
 - `Keep a CHANGELOG`_.
 - Consistent coding with EditorConfig_.
 - Badges from Shields.io_.
+- Start coding instantly with `GitHub Codespaces`_.
 
 .. _Black: https://black.readthedocs.io/en/stable/
 .. _Codecov: https://codecov.io/
 .. _EditorConfig: https://editorconfig.org/
-.. __: https://github.com/features/actions
+.. _GitHub Codespaces: https://github.com/features/codespaces
 .. _Keep a CHANGELOG: https://keepachangelog.com/
 .. _PyPI: https://pypi.python.org/pypi
 .. _Pylint: https://www.pylint.org/
 .. _Shields.io: https://shields.io/
+.. __: https://semantic-release.gitbook.io/semantic-release/
+.. __: https://github.com/features/actions
 .. _pytest: https://docs.pytest.org/
 
 Bootstrapping a New Project
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 1. Create an empty (**non-initialized**) repository on GitHub.
 2. Clone the main branch of this repository with
@@ -207,22 +211,40 @@
 ::
 
     $ make watch
 
 Publishing
 ~~~~~~~~~~
 
-Use the `poetry version`_ command to release a new version.
-Then run `make version` to commit and push a new git tag
-which will trigger a GitHub action.
+New versions are created with `poetry version`_.
+
+Automatic
+^^^^^^^^^
+
+New versions are released automatically with semantic-release_
+as long as commits follow the `Angular Commit Message Conventions`_.
+
+.. _Angular Commit Message Conventions: https://semantic-release.gitbook.io/semantic-release/#commit-message-format
+.. _semantic-release: https://semantic-release.gitbook.io/
+
+Manual
+^^^^^^
+
+Publish a new version by triggering a `version workflow_dispatch on GitHub Actions`_.
+The `version` input will be passed as the first argument to `poetry version`_.
+
+This may be done on the web or using the `GitHub CLI`_ with
+
+::
 
-Publishing may be triggered using a `workflow_dispatch on GitHub Actions`_.
+    $ gh workflow run version.yml --raw-field version=<version>
 
 .. _Poetry version: https://python-poetry.org/docs/cli/#version
-.. _workflow_dispatch on GitHub Actions: https://github.com/makenew/pypackage/actions?query=workflow%3Aversion
+.. _GitHub CLI: https://cli.github.com/
+.. _version workflow_dispatch on GitHub Actions: https://github.com/seamapi/javascript-http/actions?query=workflow%3Aversion
 
 GitHub Actions
 --------------
 
 *GitHub Actions should already be configured: this section is for reference only.*
 
 The following repository secrets must be set on GitHub Actions.
@@ -230,15 +252,15 @@
 - ``PYPI_API_TOKEN``: API token for publishing on PyPI.
 
 These must be set manually.
 
 Secrets for Optional GitHub Actions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The version and format GitHub actions
+The version, format, generate, and semantic-release GitHub actions
 require a user with write access to the repository
 including access to read and write packages.
 Set these additional secrets to enable the action:
 
 - ``GH_TOKEN``: A personal access token for the user.
 - ``GIT_USER_NAME``: The name to set for Git commits.
 - ``GIT_USER_EMAIL``: The email to set for Git commits.
```

### Comparing `makenew_pypackage-5.0.1/pyproject.toml` & `makenew_pypackage-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makenew-pypackage"
-version = "5.0.1"
+version = "5.1.0"
 description = "Package skeleton for a Python module."
 authors = ["Evan Sosenko <razorx@evansosenko.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/makenew/pypackage"
 repository = "https://github.com/makenew/pypackage"
```

### Comparing `makenew_pypackage-5.0.1/PKG-INFO` & `makenew_pypackage-5.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makenew-pypackage
-Version: 5.0.1
+Version: 5.1.0
 Summary: Package skeleton for a Python module.
 Home-page: https://github.com/makenew/pypackage
 License: MIT
 Author: Evan Sosenko
 Author-email: razorx@evansosenko.com
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -40,27 +40,31 @@
 
 - Publishing to PyPI_.
 - Secure dependency management with Poetry_.
 - Linting with Pylint_.
 - Uncompromising code formatting with Black_.
 - pytest_ helps you write better programs.
 - Code coverage reporting with Codecov_.
-- Continuous testing and deployment with `GitHub Actions`__.
+- Fully automated version management and package publishing with semantic-release__.
+- Continuous checks and tests with `GitHub Actions`__.
 - `Keep a CHANGELOG`_.
 - Consistent coding with EditorConfig_.
 - Badges from Shields.io_.
+- Start coding instantly with `GitHub Codespaces`_.
 
 .. _Black: https://black.readthedocs.io/en/stable/
 .. _Codecov: https://codecov.io/
 .. _EditorConfig: https://editorconfig.org/
-.. __: https://github.com/features/actions
+.. _GitHub Codespaces: https://github.com/features/codespaces
 .. _Keep a CHANGELOG: https://keepachangelog.com/
 .. _PyPI: https://pypi.python.org/pypi
 .. _Pylint: https://www.pylint.org/
 .. _Shields.io: https://shields.io/
+.. __: https://semantic-release.gitbook.io/semantic-release/
+.. __: https://github.com/features/actions
 .. _pytest: https://docs.pytest.org/
 
 Bootstrapping a New Project
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 1. Create an empty (**non-initialized**) repository on GitHub.
 2. Clone the main branch of this repository with
@@ -223,22 +227,40 @@
 ::
 
     $ make watch
 
 Publishing
 ~~~~~~~~~~
 
-Use the `poetry version`_ command to release a new version.
-Then run `make version` to commit and push a new git tag
-which will trigger a GitHub action.
+New versions are created with `poetry version`_.
+
+Automatic
+^^^^^^^^^
+
+New versions are released automatically with semantic-release_
+as long as commits follow the `Angular Commit Message Conventions`_.
+
+.. _Angular Commit Message Conventions: https://semantic-release.gitbook.io/semantic-release/#commit-message-format
+.. _semantic-release: https://semantic-release.gitbook.io/
+
+Manual
+^^^^^^
+
+Publish a new version by triggering a `version workflow_dispatch on GitHub Actions`_.
+The `version` input will be passed as the first argument to `poetry version`_.
+
+This may be done on the web or using the `GitHub CLI`_ with
+
+::
 
-Publishing may be triggered using a `workflow_dispatch on GitHub Actions`_.
+    $ gh workflow run version.yml --raw-field version=<version>
 
 .. _Poetry version: https://python-poetry.org/docs/cli/#version
-.. _workflow_dispatch on GitHub Actions: https://github.com/makenew/pypackage/actions?query=workflow%3Aversion
+.. _GitHub CLI: https://cli.github.com/
+.. _version workflow_dispatch on GitHub Actions: https://github.com/seamapi/javascript-http/actions?query=workflow%3Aversion
 
 GitHub Actions
 --------------
 
 *GitHub Actions should already be configured: this section is for reference only.*
 
 The following repository secrets must be set on GitHub Actions.
@@ -246,15 +268,15 @@
 - ``PYPI_API_TOKEN``: API token for publishing on PyPI.
 
 These must be set manually.
 
 Secrets for Optional GitHub Actions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The version and format GitHub actions
+The version, format, generate, and semantic-release GitHub actions
 require a user with write access to the repository
 including access to read and write packages.
 Set these additional secrets to enable the action:
 
 - ``GH_TOKEN``: A personal access token for the user.
 - ``GIT_USER_NAME``: The name to set for Git commits.
 - ``GIT_USER_EMAIL``: The email to set for Git commits.
```

