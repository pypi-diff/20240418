# Comparing `tmp/semvergit-0.3.0.tar.gz` & `tmp/semvergit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semvergit-0.3.0.tar", last modified: Tue Apr  9 17:48:52 2024, max compression
+gzip compressed data, was "semvergit-0.4.0.tar", last modified: Thu Apr 18 15:06:53 2024, max compression
```

## Comparing `semvergit-0.3.0.tar` & `semvergit-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.974448 semvergit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 17:48:30.000000 semvergit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 17:48:52.974448 semvergit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-09 17:48:30.000000 semvergit-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-09 17:48:30.000000 semvergit-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.966448 semvergit-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 17:48:30.000000 semvergit-0.3.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 17:48:30.000000 semvergit-0.3.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:48:52.974448 semvergit-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.966448 semvergit-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/src/semvergit/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/src/semvergit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.374284 semvergit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 15:06:36.000000 semvergit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 15:06:53.374284 semvergit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-18 15:06:36.000000 semvergit-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-18 15:06:36.000000 semvergit-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.366284 semvergit-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-18 15:06:36.000000 semvergit-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 15:06:36.000000 semvergit-0.4.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:06:53.374284 semvergit-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.366284 semvergit-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/src/semvergit/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/src/semvergit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_log_utils.py
```

### Comparing `semvergit-0.3.0/LICENSE` & `semvergit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/PKG-INFO` & `semvergit-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: gitpython>=3.0.0
 Requires-Dist: semver>=3.0.0
 Requires-Dist: loguru>=0.7.0
 Requires-Dist: click>=8.0.0
 Provides-Extra: dev
 Requires-Dist: astroid==3.1.0; extra == "dev"
 Requires-Dist: bandit==1.7.8; extra == "dev"
-Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: black==24.4.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: dill==0.3.8; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: filelock==3.13.3; extra == "dev"
 Requires-Dist: identify==2.5.35; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
@@ -78,52 +78,64 @@
 The supported bump types are:
 
 - `major`
 - `minor`
 - `patch`
 - `prerelease`
 
-## Workflow
-
-- Use the latest git tag to determine the current version number.
-- Bump the version number
-- Create a new git tag
-- Push the tag to the remote
+## Internal Workflow
+___What's actully happening when you run this tool___
+1. Use the latest git tag to determine the current version number.
+2. Bump the version number
+3. Create a new git tag
+4. Push the tag to the remote
+
+## Why?
+I created this tool to help me manage my project's version numbers.
+I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
+
+## Features
+❇️ Bump the version number and update the git tag in one command
+❇️ Dry run mode
+❇️ Verbose mode
+❇️ Custom commit message
+❇️ Auto commit message
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
 
 Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
-Then you can use it in your project like this:
-``semvergit -t patch -v -am``
+Then you can use it in your project as simply as:
+``semvergit -t patch -v``
 (to bump the patch version)
 This will:
 
-1. create a tag
+1. create the relvant tag (in this case a patch bump 0.0.x -> 0.0.x+1)
 2. push it to the remote
-3. commit all changes
 
-Please cehckout ``semvergit --help`` for more info.
+Please checkout ``semvergit --help`` for more info.
 
 ```shell
 Usage: semvergit [OPTIONS] COMMAND [ARGS]...
 
   CLI for semvergit.
 
 Options:
-  --version             Show the version and exit.
-  -d, --dry_run         Dry run
-  -v, --verbose         Verbose  [0<=x<=2]
-  -t, --bump_type TEXT  Bump Type ['major', 'minor', 'patch', 'prerelease']
-  -m, --message TEXT    Commit message
-  -am, --auto_message   Auto commit message
-  --help                Show this message and exit.
+  --version                Show the version and exit.
+  -d, --dry_run            Dry run
+  -v, --verbose            Verbose level  [0<=x<=2]
+  -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
+  -m, --message TEXT       Commit message
+  -am, --auto_message      Auto commit message
+  -f, --version_file FILE  Version file
+  --help                   Show this message and exit.
 ```
 
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `semvergit-0.3.0/README.md` & `semvergit-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -13,52 +13,64 @@
 The supported bump types are:
 
 - `major`
 - `minor`
 - `patch`
 - `prerelease`
 
-## Workflow
-
-- Use the latest git tag to determine the current version number.
-- Bump the version number
-- Create a new git tag
-- Push the tag to the remote
+## Internal Workflow
+___What's actully happening when you run this tool___
+1. Use the latest git tag to determine the current version number.
+2. Bump the version number
+3. Create a new git tag
+4. Push the tag to the remote
+
+## Why?
+I created this tool to help me manage my project's version numbers.
+I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
+
+## Features
+❇️ Bump the version number and update the git tag in one command
+❇️ Dry run mode
+❇️ Verbose mode
+❇️ Custom commit message
+❇️ Auto commit message
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
 
 Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
-Then you can use it in your project like this:
-``semvergit -t patch -v -am``
+Then you can use it in your project as simply as:
+``semvergit -t patch -v``
 (to bump the patch version)
 This will:
 
-1. create a tag
+1. create the relvant tag (in this case a patch bump 0.0.x -> 0.0.x+1)
 2. push it to the remote
-3. commit all changes
 
-Please cehckout ``semvergit --help`` for more info.
+Please checkout ``semvergit --help`` for more info.
 
 ```shell
 Usage: semvergit [OPTIONS] COMMAND [ARGS]...
 
   CLI for semvergit.
 
 Options:
-  --version             Show the version and exit.
-  -d, --dry_run         Dry run
-  -v, --verbose         Verbose  [0<=x<=2]
-  -t, --bump_type TEXT  Bump Type ['major', 'minor', 'patch', 'prerelease']
-  -m, --message TEXT    Commit message
-  -am, --auto_message   Auto commit message
-  --help                Show this message and exit.
+  --version                Show the version and exit.
+  -d, --dry_run            Dry run
+  -v, --verbose            Verbose level  [0<=x<=2]
+  -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
+  -m, --message TEXT       Commit message
+  -am, --auto_message      Auto commit message
+  -f, --version_file FILE  Version file
+  --help                   Show this message and exit.
 ```
 
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `semvergit-0.3.0/pyproject.toml` & `semvergit-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/requirements/requirements-dev.txt` & `semvergit-0.4.0/requirements/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --annotation-style=line --output-file=requirements/requirements-dev.txt --strip-extras requirements/requirements-dev.in
 #
 astroid==3.1.0            # via pylint
 bandit==1.7.8             # via -r requirements/requirements-dev.in
-black==24.3.0             # via -r requirements/requirements-dev.in
+black==24.4.0             # via -r requirements/requirements-dev.in
 cfgv==3.4.0               # via pre-commit
 click==8.1.7              # via -c requirements/requirements.txt, black
 dill==0.3.8               # via pylint
 distlib==0.3.8            # via virtualenv
 filelock==3.13.3          # via virtualenv
 identify==2.5.35          # via pre-commit
 isort==5.13.2             # via -r requirements/requirements-dev.in, pylint
```

### Comparing `semvergit-0.3.0/requirements/requirements-test.txt` & `semvergit-0.4.0/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/src/semvergit/app.py` & `semvergit-0.4.0/src/semvergit/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum
 from importlib import metadata
 from typing import List, Optional
 
 from loguru import logger
 from semver import VersionInfo
 
+from semvergit.file_utils import update_verion_file
 from semvergit.git_utils import (
     get_active_branch,
     get_repo,
     get_tags_with_prefix,
     new_commit,
     pull_remote,
     push_remote,
@@ -68,23 +69,34 @@
     @staticmethod
     def remove_prefix(text: str, prefix: str) -> str:
         """Remove prefix."""
         if text.startswith(prefix):
             return text[len(prefix) :]
         return text
 
-    def update(self, bump_type: str, dry_run: bool, commit_message: Optional[str], auto_message: bool) -> str:
+    # pylint: disable=too-many-arguments
+    def update(
+        self, bump_type: str, dry_run: bool, commit_message: Optional[str], auto_message: bool, version_file: str
+    ) -> str:
         """Update."""
         new_version = self.latest_version.next_version(part=bump_type, prerelease_token=self.prerelease_token)
         logger.info(f"💡 Update from {self.latest_version} with {bump_type} to {new_version}")
         new_tag_str = f"{self.version_prefix}{new_version}"
 
         if dry_run:
             logger.warning("⚠️ Dry run (no tag set or pushed)")
 
+        if version_file:
+            logger.info(f"📝 Writing version to {version_file}...")
+            update_verion_file(version_file, new_version, dry_run)
+
+            if not commit_message:
+                # Upading the version file requires a commit message
+                auto_message = True
+
         if auto_message:
             commit_message = f"New version: {str(new_version)}"
         if auto_message or commit_message:
             logger.info("✍️ Committing...")
             new_commit(repo=self.current_repo, message=commit_message, dry_run=dry_run)
         else:
             logger.debug("No commit message")
```

### Comparing `semvergit-0.3.0/src/semvergit/cli.py` & `semvergit-0.4.0/src/semvergit/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,44 @@
     """Validate bump type."""
     try:
         return BumpType(value)
     except ValueError as exp:
         raise click.BadParameter(f"Please use {BumpType.print_options()}") from exp
 
 
+# pylint: disable=too-many-arguments
 @click.group(invoke_without_command=True, no_args_is_help=True)
 @click.version_option()
 @click.option("--dry_run", "-d", is_flag=True, help="Dry run", default=False)
 @click.option("--verbose", "-v", count=True, help="Verbose level", default=0, type=click.IntRange(0, 2))
 @click.option(
     "--bump_type",
     "-t",
     envvar="BUMP_TYPE",
     type=click.UNPROCESSED,
     help=f"Bump Type {BumpType.print_options()}",
     callback=validate_bump_type,
 )
 @click.option("message", "--message", "-m", envvar="COMMIT_MESSAGE", help="Commit message", default=None)
 @click.option("auto_message", "--auto_message", "-am", is_flag=True, help="Auto commit message", default=False)
-def cli(bump_type: str, verbose: int, dry_run: bool, message: Optional[str], auto_message: bool) -> None:
+@click.option(
+    "--version_file",
+    "-f",
+    envvar="VERSION_FILE",
+    help="Version file",
+    default=None,
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, resolve_path=True, readable=True, writable=True),
+)
+def cli(
+    bump_type: str, verbose: int, dry_run: bool, message: Optional[str], auto_message: bool, version_file: str
+) -> None:
     """CLI for semvergit."""
     set_logger(log_level=LogLevel(verbose))
     svg = SemverGit()
-    svg.update(bump_type=bump_type, dry_run=dry_run, commit_message=message, auto_message=auto_message)
+    svg.update(
+        bump_type=bump_type,
+        dry_run=dry_run,
+        commit_message=message,
+        auto_message=auto_message,
+        version_file=version_file,
+    )
     sys.exit(0)
```

### Comparing `semvergit-0.3.0/src/semvergit/git_utils.py` & `semvergit-0.4.0/src/semvergit/git_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/src/semvergit/log_utils.py` & `semvergit-0.4.0/src/semvergit/log_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/src/semvergit.egg-info/PKG-INFO` & `semvergit-0.4.0/src/semvergit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: gitpython>=3.0.0
 Requires-Dist: semver>=3.0.0
 Requires-Dist: loguru>=0.7.0
 Requires-Dist: click>=8.0.0
 Provides-Extra: dev
 Requires-Dist: astroid==3.1.0; extra == "dev"
 Requires-Dist: bandit==1.7.8; extra == "dev"
-Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: black==24.4.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: dill==0.3.8; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: filelock==3.13.3; extra == "dev"
 Requires-Dist: identify==2.5.35; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
@@ -78,52 +78,64 @@
 The supported bump types are:
 
 - `major`
 - `minor`
 - `patch`
 - `prerelease`
 
-## Workflow
-
-- Use the latest git tag to determine the current version number.
-- Bump the version number
-- Create a new git tag
-- Push the tag to the remote
+## Internal Workflow
+___What's actully happening when you run this tool___
+1. Use the latest git tag to determine the current version number.
+2. Bump the version number
+3. Create a new git tag
+4. Push the tag to the remote
+
+## Why?
+I created this tool to help me manage my project's version numbers.
+I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
+
+## Features
+❇️ Bump the version number and update the git tag in one command
+❇️ Dry run mode
+❇️ Verbose mode
+❇️ Custom commit message
+❇️ Auto commit message
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
 
 Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
-Then you can use it in your project like this:
-``semvergit -t patch -v -am``
+Then you can use it in your project as simply as:
+``semvergit -t patch -v``
 (to bump the patch version)
 This will:
 
-1. create a tag
+1. create the relvant tag (in this case a patch bump 0.0.x -> 0.0.x+1)
 2. push it to the remote
-3. commit all changes
 
-Please cehckout ``semvergit --help`` for more info.
+Please checkout ``semvergit --help`` for more info.
 
 ```shell
 Usage: semvergit [OPTIONS] COMMAND [ARGS]...
 
   CLI for semvergit.
 
 Options:
-  --version             Show the version and exit.
-  -d, --dry_run         Dry run
-  -v, --verbose         Verbose  [0<=x<=2]
-  -t, --bump_type TEXT  Bump Type ['major', 'minor', 'patch', 'prerelease']
-  -m, --message TEXT    Commit message
-  -am, --auto_message   Auto commit message
-  --help                Show this message and exit.
+  --version                Show the version and exit.
+  -d, --dry_run            Dry run
+  -v, --verbose            Verbose level  [0<=x<=2]
+  -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
+  -m, --message TEXT       Commit message
+  -am, --auto_message      Auto commit message
+  -f, --version_file FILE  Version file
+  --help                   Show this message and exit.
 ```
 
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `semvergit-0.3.0/src/semvergit.egg-info/SOURCES.txt` & `semvergit-0.4.0/src/semvergit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 pyproject.toml
 requirements/requirements-dev.txt
 requirements/requirements-test.txt
 src/semvergit/__init__.py
 src/semvergit/__main__.py
 src/semvergit/app.py
 src/semvergit/cli.py
+src/semvergit/file_utils.py
 src/semvergit/git_utils.py
 src/semvergit/log_utils.py
 src/semvergit.egg-info/PKG-INFO
 src/semvergit.egg-info/SOURCES.txt
 src/semvergit.egg-info/dependency_links.txt
 src/semvergit.egg-info/entry_points.txt
 src/semvergit.egg-info/requires.txt
 src/semvergit.egg-info/top_level.txt
 tests/test_app.py
 tests/test_cli.py
+tests/test_file_utils.py
 tests/test_git_utils.py
 tests/test_integration.py
 tests/test_log_utils.py
```

### Comparing `semvergit-0.3.0/src/semvergit.egg-info/requires.txt` & `semvergit-0.4.0/src/semvergit.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 semver>=3.0.0
 loguru>=0.7.0
 click>=8.0.0
 
 [dev]
 astroid==3.1.0
 bandit==1.7.8
-black==24.3.0
+black==24.4.0
 cfgv==3.4.0
 click==8.1.7
 dill==0.3.8
 distlib==0.3.8
 filelock==3.13.3
 identify==2.5.35
 isort==5.13.2
```

### Comparing `semvergit-0.3.0/tests/test_app.py` & `semvergit-0.4.0/tests/test_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test app."""
 
-from typing import List, Optional
+from typing import Callable, List, Optional
 
 from pytest import CaptureFixture, LogCaptureFixture, mark
 from semver import VersionInfo
 
 from semvergit.app import BumpType, SemverGit
 
 
@@ -79,30 +79,40 @@
     "commit_message, auto_message",
     [
         ("testmessage", False),
         (None, True),
         (None, False),
     ],
 )
-# type: ignore[no-untyped-def]
+@mark.parametrize(
+    "version_file",
+    [
+        "test_version_file",
+        None,
+    ],
+)
 def test_app_no_versions_update(  # pylint: disable=too-many-arguments
     bump_type: str,
     expected_version: VersionInfo,
     dry_run: bool,
     commit_message: Optional[str],
     auto_message: bool,
-    mock_get_tags_empty,  # pylint: disable=unused-argument
+    version_file: str,
+    mock_get_tags_empty: Callable,  # pylint: disable=unused-argument
+    mock_update_verion_file: Callable,  # pylint: disable=unused-argument
 ) -> None:
     """Test app with no versions."""
     svg = SemverGit()
     assert svg is not None
     assert svg.branch.name == "test_branch"
     assert svg.versions == []
     assert svg.latest_version == VersionInfo(0, 0, 0)
-    new_version = svg.update(bump_type, dry_run=dry_run, commit_message=commit_message, auto_message=auto_message)
+    new_version = svg.update(
+        bump_type, dry_run=dry_run, commit_message=commit_message, auto_message=auto_message, version_file=version_file
+    )
     expected_tag_str = f"{svg.version_prefix}{str(expected_version)}"
     assert new_version == expected_tag_str
 
 
 def check_substring(substring_match: str, strings_list: List[str]) -> bool:
     """Check if list contains substring."""
     for item in strings_list:
@@ -131,31 +141,46 @@
     "commit_message, auto_message",
     [
         ("testmessage", False),
         (None, True),
         (None, False),
     ],
 )
+@mark.parametrize(
+    "version_file",
+    [
+        "test_version_file",
+        None,
+    ],
+)
 def test_app_update(  # pylint: disable=too-many-arguments
     caplog: LogCaptureFixture,
+    mock_update_verion_file: Callable,  # pylint: disable=unused-argument
     bump_type: str,
     expected_version: VersionInfo,
     dry_run: bool,
     commit_message: Optional[str],
     auto_message: bool,
+    version_file: str,
     capsys: CaptureFixture,
 ) -> None:
     """Test app."""
     svg = SemverGit()
-    new_version = svg.update(bump_type, dry_run=dry_run, commit_message=commit_message, auto_message=auto_message)
+    new_version = svg.update(
+        bump_type, dry_run=dry_run, commit_message=commit_message, auto_message=auto_message, version_file=version_file
+    )
 
     expected_tag_str = f"{svg.version_prefix}{str(expected_version)}"
     assert f"Created mock-set-tag-{expected_tag_str}" in caplog.messages
     if commit_message or auto_message:
         assert check_substring("Committing...", caplog.messages)
     if dry_run:
         assert check_substring("Dry run (no tag set or pushed)", caplog.messages)
+    if version_file:
+        assert check_substring(f"Writing version to {version_file}...", caplog.messages)
+        if not commit_message:
+            assert check_substring("Committing...", caplog.messages)
     assert check_substring("Pushing...", caplog.messages)
     assert capsys.readouterr().out == expected_tag_str
     assert new_version == expected_tag_str
     print(f"{caplog.messages=}")
     assert check_substring(f"New version tag: {expected_tag_str}", caplog.messages)
```

### Comparing `semvergit-0.3.0/tests/test_cli.py` & `semvergit-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/tests/test_git_utils.py` & `semvergit-0.4.0/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.3.0/tests/test_integration.py` & `semvergit-0.4.0/tests/test_integration.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,20 +41,50 @@
 def update_version(repodirname: str, version_type: str, target_version: str) -> None:
     """Run the semvergit command to update the version."""
     result, logs = run_command(f"semvergit -v -t {version_type}", repodirname, "Created a new version")
     print(logs, end="")
     assert result == target_version
 
 
+def update_version_file(repodirname: str, version_type: str, target_version: str, version_file: str) -> None:
+    """Run the semvergit command to update the version on file."""
+    result, logs = run_command(
+        f"semvergit -v -t {version_type} -f {version_file}", repodirname, "Created a new version (in file)"
+    )
+    print(logs, end="")
+    assert result == target_version
+
+
+def update_version_file_custom(
+    repodirname: str, version_type: str, target_version: str, version_file: str, custom_message: str
+) -> None:
+    """Run the semvergit command to update the version on file with custom message."""
+    result, logs = run_command(
+        f'semvergit -v -t {version_type} -f {version_file} -m "{custom_message}"',
+        repodirname,
+        "Created a new version (in file)",
+    )
+    print(logs, end="")
+    assert result == target_version
+
+
 def set_credentials(repodirname: str) -> None:
     """Set the git credentials for the repository."""
     run_command("git config user.email 'test@test'", repodirname, "Set user email")
     run_command("git config user.name 'Test User'", repodirname, "Set user name")
 
 
+def check_file_content(filename: str, repodirname: str, expected: str) -> None:
+    """Check the content of a file."""
+    with open(repodirname + "/" + filename, "r", encoding="utf-8") as f:
+        file_content = f.read()
+        print(f"File content:\n{file_content}")
+        assert expected in file_content
+
+
 class TestIntegration:
     """Integration tests for the semvergit package."""
 
     # pylint: disable=attribute-defined-outside-init
     def setup_method(self) -> None:
         """Create a git repository and clone it."""
         self.tmpdirname = tempfile.mkdtemp()
@@ -130,7 +160,22 @@
         add_file_to_repo("test4.txt", self.clonedirname, "Even more content")
         check_git_log(self.clonedirname, "Added test4.txt")
         update_version(self.clonedirname, "minor", "v1.1.0")
         add_file_to_repo("test5.txt", self.clonedirname, "Some more content")
         check_git_log(self.clonedirname, "Added test5.txt")
         update_version(self.clonedirname, "patch", "v1.1.1")
         check_git_log(self.clonedirname, "v1.1.1")
+
+    def test_integration_version_file(self) -> None:
+        """Test the integration of the semvergit package with a version file."""
+        add_file_to_repo("test.txt", self.clonedirname, "Hello, World!")
+        add_file_to_repo("version.txt", self.clonedirname, "0.0.0")
+        check_file_content("version.txt", self.clonedirname, "0.0.0")
+        check_git_log(self.clonedirname, "Added test.txt")
+        check_git_log(self.clonedirname, "Added version.txt")
+        update_version_file(self.clonedirname, "patch", "v0.0.1", "version.txt")
+        check_file_content("version.txt", self.clonedirname, "0.0.1")
+        add_file_to_repo("test2.txt", self.clonedirname, "New content")
+        check_git_log(self.clonedirname, "Added test2.txt")
+        update_version_file_custom(self.clonedirname, "minor", "v0.1.0", "version.txt", "Updated version to 0.1.0")
+        check_file_content("version.txt", self.clonedirname, "0.1.0")
+        check_git_log(self.clonedirname, "0.1.0")
```

