# Comparing `tmp/pre_commit_update-0.2.3.tar.gz` & `tmp/pre_commit_update-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.2.3.tar", max compression
+gzip compressed data, was "pre_commit_update-0.3.0.tar", max compression
```

## Comparing `pre_commit_update-0.2.3.tar` & `pre_commit_update-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-03-14 22:21:56.722257 pre_commit_update-0.2.3/LICENSE
--rw-r--r--   0        0        0     6121 2024-04-08 20:24:09.734523 pre_commit_update-0.2.3/README.md
--rw-r--r--   0        0        0     1660 2024-04-11 11:58:32.472296 pre_commit_update-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:52:38.000000 pre_commit_update-0.2.3/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0    11039 2024-04-11 11:58:09.552302 pre_commit_update-0.2.3/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.2.3/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     7665 1970-01-01 00:00:00.000000 pre_commit_update-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6689 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/README.md
+-rw-r--r--   0        0        0     1660 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 15:53:44.498016 pre_commit_update-0.3.0/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0      229 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/env.py
+-rw-r--r--   0        0        0     3116 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/message.py
+-rw-r--r--   0        0        0     4526 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/repo.py
+-rw-r--r--   0        0        0      800 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/yaml.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.3.0/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     2151 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/repo.py
+-rw-r--r--   0        0        0      759 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/utils.py
+-rw-r--r--   0        0        0     8233 1970-01-01 00:00:00.000000 pre_commit_update-0.3.0/PKG-INFO
```

### Comparing `pre_commit_update-0.2.3/LICENSE` & `pre_commit_update-0.3.0/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2024 Vojko Pribudić
+Copyright (c) 2022 Vojko Pribudić
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pre_commit_update-0.2.3/README.md` & `pre_commit_update-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 <div align="center"><h1>pre-commit-update</h1>
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update)
 ![PePy - Downloads](https://pepy.tech/badge/pre-commit-update)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-update?branch=main&label=pipeline)
 ![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
+![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-commit-update?style=flat&color=%23FFD700)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-update)
 ![Python - Formatter](https://img.shields.io/badge/code%20style-black-black)
 ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-update)
+![Codacy grade](https://img.shields.io/codacy/grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
 </div>
 <div align="center">
 <a href="https://ko-fi.com/H2H8WN45E" target="_blank"><img alt="kofi" src="https://i.imgur.com/wdSRlJB.png" width="141" height="36"></a>
 
 <strong>pre-commit-update</strong> is a simple CLI tool to check and update pre-commit hooks.
 </div>
 
@@ -66,16 +71,16 @@
 ```console
 Usage: pre-commit-update [OPTIONS]
 
 Options:
   -d, --dry-run / -nd, --no-dry-run             Dry run only checks for the new versions without updating  [default: nd]
   -a, --all-versions / -na, --no-all-versions   Include the alpha/beta versions when updating  [default: na]
   -v, --verbose / -nv, --no-verbose             Display the complete output  [default: nv]
-  -e, --exclude TEXT                            Exclude specific repo(s) by the `repo` url trim
-  -k, --keep TEXT                               Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
+  -e, --exclude REPO_URL_TRIM                   Exclude specific repo(s) by the `repo` url trim
+  -k, --keep REPO_URL_TRIM                      Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
   -h, --help                                    Show this message and exit.
 ```
 
 If you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:
 ```console
 $ pre-commit-update -d
 ```
@@ -111,15 +116,15 @@
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
 - repo: https://gitlab.com/vojko.pribudic/pre-commit-update
-  rev: v0.1.7  # Insert the latest tag here
+  rev: v0.3.0  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
 ### 3) pyproject.toml usage example
```

#### html2text {}

```diff
@@ -1,15 +1,22 @@
                         ************ pprree--ccoommmmiitt--uuppddaattee ************
   ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update) ![PePy -
-Downloads](https://pepy.tech/badge/pre-commit-update) ![GitLab Issues](https://
-img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![Python
- - Formatter](https://img.shields.io/badge/code%20style-black-black) ![PyPI -
-  License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333) !
-  [PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-
-                                    update)
+Downloads](https://pepy.tech/badge/pre-commit-update) ![Gitlab Pipeline Status]
+  (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-
+  update?branch=main&label=pipeline) ![GitLab Issues](https://img.shields.io/
+ gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![GitLab Last Commit]
+(https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
+   ![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-
+commit-update?style=flat&color=%23FFD700) ![Libraries.io dependency status for
+  latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-
+update) ![Python - Formatter](https://img.shields.io/badge/code%20style-black-
+      black) ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-
+ update?color=%23333333) ![PyPI - Python Version](https://img.shields.io/pypi/
+ pyversions/pre-commit-update) ![Codacy grade](https://img.shields.io/codacy/
+              grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
 example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
@@ -31,40 +38,40 @@
 update` is available on PyPI: ```console $ python -m pip install pre-commit-
 update ``` Python >= 3.8 is supported. **NOTE:** Please make sure that `git` is
 installed. ## 4. Usage `pre-commit-update` CLI can be used as below: ```console
 Usage: pre-commit-update [OPTIONS] Options: -d, --dry-run / -nd, --no-dry-run
 Dry run only checks for the new versions without updating [default: nd] -a, --
 all-versions / -na, --no-all-versions Include the alpha/beta versions when
 updating [default: na] -v, --verbose / -nv, --no-verbose Display the complete
-output [default: nv] -e, --exclude TEXT Exclude specific repo(s) by the `repo`
-url trim -k, --keep TEXT Keep the version of specific repo(s) by the `repo` url
-trim (still checks for the new versions) -h, --help Show this message and exit.
-``` If you want to just check for updates (without updating `pre-commit-
-config.yaml`), for example, you would use: ```console $ pre-commit-update -
-d ``` or ```console $ pre-commit-update --dry-run ``` **NOTE:** If you are to
-use the `exclude` or `keep` options, please pass the repo url trim as a
-parameter. Keep in mind that if you have multiple hooks (id's) configured for a
-single repo and you `exclude` that repo, **NONE** of the hooks will be updated,
-whole repo will be excluded. Example of repo url trim: https://github.com/ambv/
-black -> `black` (you will only pass `black` as a parameter to `exclude` or
-`keep`) ### 1) Pipeline usage example #### a) GitLab job: ```yaml pre-commit-
-hooks-update: stage: update script: # install git if not present in the image -
-pip install pre-commit-update - pre-commit-update --dry-run except: - main
-when: manual allow_failure: true ``` **NOTE:** This is just an example, feel
-free to do your own configuration ### 2) pre-commit hook usage example You can
-also use `pre-commit-update` as a hook in your `pre-commit` hooks: ```yaml -
-repo: https://gitlab.com/vojko.pribudic/pre-commit-update rev: v0.1.7 # Insert
-the latest tag here hooks: - id: pre-commit-update args: [--dry-run, --exclude,
-black, --keep, isort] ``` ### 3) pyproject.toml usage example You can configure
-`pre-commit-update` in your `pyproject.toml` as below (feel free to do your own
-configuration): ```toml [tool.pre-commit-update] dry_run = true all_versions =
-false verbose = true exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some
-of the options are missing (for example `exclude` option), `pre-commit-update`
-will use default value for that option (default for `exclude` option would be
-an empty list). ***IMPORTANT*** If you invoke `pre-commit-update` with any
-arguments (e.g. `pre-commit-update -d`), `pyproject.toml` configuration will be
-**overridden**. This means that all the arguments passed while calling `pre-
-commit-update` will have priority over configuration defined inside
-`pyproject.toml`. If you want to override boolean flags, you can do so by
-passing the negative flag value. For example, given the configuration above, to
-override `verbose` flag from `pyproject.toml`, you would invoke `pre-commit-
-update` with either `--no-verbose` or `-nv`.
+output [default: nv] -e, --exclude REPO_URL_TRIM Exclude specific repo(s) by
+the `repo` url trim -k, --keep REPO_URL_TRIM Keep the version of specific repo
+(s) by the `repo` url trim (still checks for the new versions) -h, --help Show
+this message and exit. ``` If you want to just check for updates (without
+updating `pre-commit-config.yaml`), for example, you would use: ```console $
+pre-commit-update -d ``` or ```console $ pre-commit-update --dry-run ```
+**NOTE:** If you are to use the `exclude` or `keep` options, please pass the
+repo url trim as a parameter. Keep in mind that if you have multiple hooks
+(id's) configured for a single repo and you `exclude` that repo, **NONE** of
+the hooks will be updated, whole repo will be excluded. Example of repo url
+trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
+parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
+job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
+not present in the image - pip install pre-commit-update - pre-commit-update --
+dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
+just an example, feel free to do your own configuration ### 2) pre-commit hook
+usage example You can also use `pre-commit-update` as a hook in your `pre-
+commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic/pre-commit-
+update rev: v0.3.0 # Insert the latest tag here hooks: - id: pre-commit-update
+args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3) pyproject.toml
+usage example You can configure `pre-commit-update` in your `pyproject.toml` as
+below (feel free to do your own configuration): ```toml [tool.pre-commit-
+update] dry_run = true all_versions = false verbose = true exclude = ["isort"]
+keep = ["black"] ``` **NOTE:** If some of the options are missing (for example
+`exclude` option), `pre-commit-update` will use default value for that option
+(default for `exclude` option would be an empty list). ***IMPORTANT*** If you
+invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
+`pyproject.toml` configuration will be **overridden**. This means that all the
+arguments passed while calling `pre-commit-update` will have priority over
+configuration defined inside `pyproject.toml`. If you want to override boolean
+flags, you can do so by passing the negative flag value. For example, given the
+configuration above, to override `verbose` flag from `pyproject.toml`, you
+would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
```

### Comparing `pre_commit_update-0.2.3/pyproject.toml` & `pre_commit_update-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.2.3"
+version = "0.3.0"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
 repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `pre_commit_update-0.2.3/PKG-INFO` & `pre_commit_update-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.2.3
+Version: 0.3.0
 Summary: Simple CLI tool to check and update pre-commit hooks.
 Home-page: https://gitlab.com/vojko.pribudic/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -34,18 +34,23 @@
 Project-URL: Tracker, https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues
 Description-Content-Type: text/markdown
 
 <div align="center"><h1>pre-commit-update</h1>
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update)
 ![PePy - Downloads](https://pepy.tech/badge/pre-commit-update)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-update?branch=main&label=pipeline)
 ![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
+![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-commit-update?style=flat&color=%23FFD700)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-update)
 ![Python - Formatter](https://img.shields.io/badge/code%20style-black-black)
 ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-update)
+![Codacy grade](https://img.shields.io/codacy/grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
 </div>
 <div align="center">
 <a href="https://ko-fi.com/H2H8WN45E" target="_blank"><img alt="kofi" src="https://i.imgur.com/wdSRlJB.png" width="141" height="36"></a>
 
 <strong>pre-commit-update</strong> is a simple CLI tool to check and update pre-commit hooks.
 </div>
 
@@ -102,16 +107,16 @@
 ```console
 Usage: pre-commit-update [OPTIONS]
 
 Options:
   -d, --dry-run / -nd, --no-dry-run             Dry run only checks for the new versions without updating  [default: nd]
   -a, --all-versions / -na, --no-all-versions   Include the alpha/beta versions when updating  [default: na]
   -v, --verbose / -nv, --no-verbose             Display the complete output  [default: nv]
-  -e, --exclude TEXT                            Exclude specific repo(s) by the `repo` url trim
-  -k, --keep TEXT                               Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
+  -e, --exclude REPO_URL_TRIM                   Exclude specific repo(s) by the `repo` url trim
+  -k, --keep REPO_URL_TRIM                      Keep the version of specific repo(s) by the `repo` url trim (still checks for the new versions)
   -h, --help                                    Show this message and exit.
 ```
 
 If you want to just check for updates (without updating `pre-commit-config.yaml`), for example, you would use:
 ```console
 $ pre-commit-update -d
 ```
@@ -147,15 +152,15 @@
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
 - repo: https://gitlab.com/vojko.pribudic/pre-commit-update
-  rev: v0.1.7  # Insert the latest tag here
+  rev: v0.3.0  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
 ### 3) pyproject.toml usage example
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pre-commit-update Version: 0.2.3 Summary: Simple
+Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.0 Summary: Simple
 CLI tool to check and update pre-commit hooks. Home-page: https://gitlab.com/
 vojko.pribudic/pre-commit-update License: MIT Author: Vojko PribudiÄ Author-
 email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ Maintainer-email:
 dmanthing@gmail.com Requires-Python: >=3.8 Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
@@ -17,20 +17,27 @@
 (>=0.9) Requires-Dist: ruamel.yaml (>=0.18) Project-URL: Changelog, https://
 gitlab.com/vojko.pribudic/pre-commit-update/-/releases Project-URL: Repository,
 https://gitlab.com/vojko.pribudic/pre-commit-update Project-URL: Tracker,
 https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues Description-
 Content-Type: text/markdown
                         ************ pprree--ccoommmmiitt--uuppddaattee ************
   ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update) ![PePy -
-Downloads](https://pepy.tech/badge/pre-commit-update) ![GitLab Issues](https://
-img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![Python
- - Formatter](https://img.shields.io/badge/code%20style-black-black) ![PyPI -
-  License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333) !
-  [PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-
-                                    update)
+Downloads](https://pepy.tech/badge/pre-commit-update) ![Gitlab Pipeline Status]
+  (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-
+  update?branch=main&label=pipeline) ![GitLab Issues](https://img.shields.io/
+ gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![GitLab Last Commit]
+(https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
+   ![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-
+commit-update?style=flat&color=%23FFD700) ![Libraries.io dependency status for
+  latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-
+update) ![Python - Formatter](https://img.shields.io/badge/code%20style-black-
+      black) ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-
+ update?color=%23333333) ![PyPI - Python Version](https://img.shields.io/pypi/
+ pyversions/pre-commit-update) ![Codacy grade](https://img.shields.io/codacy/
+              grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
 example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
@@ -52,40 +59,40 @@
 update` is available on PyPI: ```console $ python -m pip install pre-commit-
 update ``` Python >= 3.8 is supported. **NOTE:** Please make sure that `git` is
 installed. ## 4. Usage `pre-commit-update` CLI can be used as below: ```console
 Usage: pre-commit-update [OPTIONS] Options: -d, --dry-run / -nd, --no-dry-run
 Dry run only checks for the new versions without updating [default: nd] -a, --
 all-versions / -na, --no-all-versions Include the alpha/beta versions when
 updating [default: na] -v, --verbose / -nv, --no-verbose Display the complete
-output [default: nv] -e, --exclude TEXT Exclude specific repo(s) by the `repo`
-url trim -k, --keep TEXT Keep the version of specific repo(s) by the `repo` url
-trim (still checks for the new versions) -h, --help Show this message and exit.
-``` If you want to just check for updates (without updating `pre-commit-
-config.yaml`), for example, you would use: ```console $ pre-commit-update -
-d ``` or ```console $ pre-commit-update --dry-run ``` **NOTE:** If you are to
-use the `exclude` or `keep` options, please pass the repo url trim as a
-parameter. Keep in mind that if you have multiple hooks (id's) configured for a
-single repo and you `exclude` that repo, **NONE** of the hooks will be updated,
-whole repo will be excluded. Example of repo url trim: https://github.com/ambv/
-black -> `black` (you will only pass `black` as a parameter to `exclude` or
-`keep`) ### 1) Pipeline usage example #### a) GitLab job: ```yaml pre-commit-
-hooks-update: stage: update script: # install git if not present in the image -
-pip install pre-commit-update - pre-commit-update --dry-run except: - main
-when: manual allow_failure: true ``` **NOTE:** This is just an example, feel
-free to do your own configuration ### 2) pre-commit hook usage example You can
-also use `pre-commit-update` as a hook in your `pre-commit` hooks: ```yaml -
-repo: https://gitlab.com/vojko.pribudic/pre-commit-update rev: v0.1.7 # Insert
-the latest tag here hooks: - id: pre-commit-update args: [--dry-run, --exclude,
-black, --keep, isort] ``` ### 3) pyproject.toml usage example You can configure
-`pre-commit-update` in your `pyproject.toml` as below (feel free to do your own
-configuration): ```toml [tool.pre-commit-update] dry_run = true all_versions =
-false verbose = true exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some
-of the options are missing (for example `exclude` option), `pre-commit-update`
-will use default value for that option (default for `exclude` option would be
-an empty list). ***IMPORTANT*** If you invoke `pre-commit-update` with any
-arguments (e.g. `pre-commit-update -d`), `pyproject.toml` configuration will be
-**overridden**. This means that all the arguments passed while calling `pre-
-commit-update` will have priority over configuration defined inside
-`pyproject.toml`. If you want to override boolean flags, you can do so by
-passing the negative flag value. For example, given the configuration above, to
-override `verbose` flag from `pyproject.toml`, you would invoke `pre-commit-
-update` with either `--no-verbose` or `-nv`.
+output [default: nv] -e, --exclude REPO_URL_TRIM Exclude specific repo(s) by
+the `repo` url trim -k, --keep REPO_URL_TRIM Keep the version of specific repo
+(s) by the `repo` url trim (still checks for the new versions) -h, --help Show
+this message and exit. ``` If you want to just check for updates (without
+updating `pre-commit-config.yaml`), for example, you would use: ```console $
+pre-commit-update -d ``` or ```console $ pre-commit-update --dry-run ```
+**NOTE:** If you are to use the `exclude` or `keep` options, please pass the
+repo url trim as a parameter. Keep in mind that if you have multiple hooks
+(id's) configured for a single repo and you `exclude` that repo, **NONE** of
+the hooks will be updated, whole repo will be excluded. Example of repo url
+trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
+parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
+job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
+not present in the image - pip install pre-commit-update - pre-commit-update --
+dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
+just an example, feel free to do your own configuration ### 2) pre-commit hook
+usage example You can also use `pre-commit-update` as a hook in your `pre-
+commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic/pre-commit-
+update rev: v0.3.0 # Insert the latest tag here hooks: - id: pre-commit-update
+args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3) pyproject.toml
+usage example You can configure `pre-commit-update` in your `pyproject.toml` as
+below (feel free to do your own configuration): ```toml [tool.pre-commit-
+update] dry_run = true all_versions = false verbose = true exclude = ["isort"]
+keep = ["black"] ``` **NOTE:** If some of the options are missing (for example
+`exclude` option), `pre-commit-update` will use default value for that option
+(default for `exclude` option would be an empty list). ***IMPORTANT*** If you
+invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
+`pyproject.toml` configuration will be **overridden**. This means that all the
+arguments passed while calling `pre-commit-update` will have priority over
+configuration defined inside `pyproject.toml`. If you want to override boolean
+flags, you can do so by passing the negative flag value. For example, given the
+configuration above, to override `verbose` flag from `pyproject.toml`, you
+would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
```

