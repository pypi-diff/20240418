# Comparing `tmp/reprompt-0.0.7.3.tar.gz` & `tmp/reprompt-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.3.tar` & `reprompt-0.0.7.4.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0      334 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.pypirc
--rw-r--r--   0        0        0      459 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-16 22:28:37.984977 reprompt-0.0.7.3/README.md
--rw-r--r--   0        0        0      634 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/README.md
--rw-r--r--   0        0        0     1241 2024-04-16 22:28:54.157175 reprompt-0.0.7.3/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      167 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/config.py
--rw-r--r--   0        0        0     3371 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-16 22:28:37.988977 reprompt-0.0.7.3/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17737 1970-01-01 00:00:00.000000 reprompt-0.0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-18 00:05:46.805623 reprompt-0.0.7.4/LICENSE
+-rw-r--r--   0        0        0     7855 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/README.md
+-rw-r--r--   0        0        0      634 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1241 2024-04-18 00:06:01.921841 reprompt-0.0.7.4/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      167 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/config.py
+-rw-r--r--   0        0        0     3371 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-18 00:05:46.809623 reprompt-0.0.7.4/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 reprompt-0.0.7.4/PKG-INFO
```

### Comparing `reprompt-0.0.7.3/.devcontainer/devcontainer.json` & `reprompt-0.0.7.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.4/.github/workflows/schedule-update-actions.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     - cron:  '0 0 * * 0'
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3.5.2
+      - uses: actions/checkout@v4.1.1
         with:
           # [Required] Access token with `workflow` scope.
           token: ${{ secrets.PAT }}
 
       - name: Run GitHub Actions Version Updater
-        uses: saadmk11/github-actions-version-updater@v0.7.4
+        uses: saadmk11/github-actions-version-updater@v0.8.1
         with:
           # [Required] Access token with `workflow` scope.
           token: ${{ secrets.PAT }}
           pull_request_title: "ci: Update GitHub Actions to Latest Version"
```

### Comparing `reprompt-0.0.7.3/.gitignore` & `reprompt-0.0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/.pre-commit-config.yaml` & `reprompt-0.0.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/.vscode/settings.json` & `reprompt-0.0.7.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/LICENSE` & `reprompt-0.0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/docs/Makefile` & `reprompt-0.0.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/docs/conf.py` & `reprompt-0.0.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/docs/make.bat` & `reprompt-0.0.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/docs/pylint.md` & `reprompt-0.0.7.4/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/pyproject.toml` & `reprompt-0.0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/src/reprompt/__init__.py` & `reprompt-0.0.7.4/src/reprompt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import config
 from .tracing import FunctionTrace, get_edits, write_traces
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.3"
+__version__ = "0.0.7.4"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces", "get_edits"]
 
 
 def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
     if debug:
         logger.setLevel(logging.DEBUG)
```

### Comparing `reprompt-0.0.7.3/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.4/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/src/reprompt/tracing.py` & `reprompt-0.0.7.4/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/tests/conftest.py` & `reprompt-0.0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.3/tests/test_openai_tracing.py` & `reprompt-0.0.7.4/tests/test_openai_tracing.py`

 * *Files identical despite different names*

