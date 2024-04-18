# Comparing `tmp/scrummd-0.0.8.tar.gz` & `tmp/scrummd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrummd-0.0.8.tar", last modified: Tue Mar 26 11:09:15 2024, max compression
+gzip compressed data, was "scrummd-0.1.0.tar", last modified: Wed Apr 17 10:47:25 2024, max compression
```

## Comparing `scrummd-0.0.8.tar` & `scrummd-0.1.0.tar`

### file list

```diff
@@ -1,181 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/lint-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/pipy-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/test-pypi-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-26 11:09:01.000000 scrummd-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-26 11:09:01.000000 scrummd-0.0.8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-26 11:09:01.000000 scrummd-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-03-26 11:09:01.000000 scrummd-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-26 11:09:15.426374 scrummd-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-26 11:09:01.000000 scrummd-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/card.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/commands.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/sbench.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/sbl.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/scard.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/svalid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/semver.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/source/scrummd.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial1.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/reports/bug1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug4.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum.toml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-26 11:09:01.000000 scrummd-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-26 11:09:01.000000 scrummd-0.0.8/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.418374 scrummd-0.0.8/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli001.md
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli002.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli003.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli004.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli005.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli006.md
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli007.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli008.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli009.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli010.md
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli011.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli012.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli013.md
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli014.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli015.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli016.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli017.md
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli018.md
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli019.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli020.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli021.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli022.md
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli023.md
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli024.md
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli025.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli026.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli027.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli028.md
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli029.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/v0-1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.418374 scrummd-0.0.8/scrummd/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/card.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/sbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/sbl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/scard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/source_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/svalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/scrummd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:09:15.426374 scrummd-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/collection1/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c1.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c2.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/collection1/embedded/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/embedded/e1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/.ignorethis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/.ignorethis/collection/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/.ignorethis/collection/i2.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/.ignorethis/i1.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c4.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c5.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c6.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection4/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection4/c7.md
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/md1.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/md2.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/test/fail_cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/collection_rule_violation/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/collection_rule_violation/bad_status.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/invalid/no_summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/rule_violation/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/rule_violation/bad_status.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_in_anger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_sbl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_scard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_source_md.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_svalid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.922955 scrummd-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-17 10:47:10.000000 scrummd-0.1.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-17 10:47:10.000000 scrummd-0.1.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-17 10:47:10.000000 scrummd-0.1.0/.github/workflows/pipy-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 10:47:10.000000 scrummd-0.1.0/.github/workflows/test-pypi-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-17 10:47:10.000000 scrummd-0.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.922955 scrummd-0.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-17 10:47:10.000000 scrummd-0.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 10:47:10.000000 scrummd-0.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-04-17 10:47:10.000000 scrummd-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-17 10:47:25.946955 scrummd-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-17 10:47:10.000000 scrummd-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/card.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/sbench.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/sbl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/sboard.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/scard.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/commands/svalid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   507035 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/semver.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/source/scrummd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial1.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1/scrum/reports/bug1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.2/scrum/reports/bug3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.926955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.3/scrum/reports/bug3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum/reports/bug4.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.4/scrum.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.5/scrum.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.918955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 10:47:10.000000 scrummd-0.1.0/docs/tutorial_examples/tutorial1.6/scrum.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 10:47:10.000000 scrummd-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-17 10:47:10.000000 scrummd-0.1.0/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.930955 scrummd-0.1.0/scrum/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/bugs/cli019.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/bugs/cli026.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.934955 scrummd-0.1.0/scrum/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli002.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli003.md
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli004.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli005.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli006.md
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli007.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli008.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli009.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli010.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli011.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli012.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli013.md
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli014.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli015.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli016.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli017.md
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli018.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli020.md
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli022.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli023.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli024.md
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli025.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli027.md
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli028.md
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli029.md
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli032.md
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli033.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/stories/cli034.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.938955 scrummd-0.1.0/scrum/techdebt/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/techdebt/cli021.md
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/techdebt/cli030.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/techdebt/cli031.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/techdebt/td1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrum/v0-1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.938955 scrummd-0.1.0/scrummd/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.942955 scrummd-0.1.0/scrummd/sbl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbl/board_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbl/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbl/sbl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sbl/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/sboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/scard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/source_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/svalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 10:47:10.000000 scrummd-0.1.0/scrummd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/scrummd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 10:47:25.000000 scrummd-0.1.0/scrummd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:47:25.946955 scrummd-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.942955 scrummd-0.1.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/.scrum.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection1/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection1/c1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection1/c2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection1/c3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection1/embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection1/embedded/e1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection2/.ignorethis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection2/.ignorethis/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection2/.ignorethis/collection/i2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection2/.ignorethis/i1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection2/c4.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection2/c5.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection2/c6.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/data/collection4/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/collection4/c7.md
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/md1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/md2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/data/sort_collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.922955 scrummd-0.1.0/test/special_cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/special_cases/collection_rule_violation/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/special_cases/collection_rule_violation/bad_status.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/special_cases/header_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/special_cases/header_summary/md3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/special_cases/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/special_cases/invalid/no_summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:47:25.946955 scrummd-0.1.0/test/special_cases/rule_violation/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/special_cases/rule_violation/bad_status.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_in_anger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_sbl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_scard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_source_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 10:47:10.000000 scrummd-0.1.0/test/test_svalid.py
```

### Comparing `scrummd-0.0.8/.github/workflows/lint-and-test.yml` & `scrummd-0.1.0/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/.github/workflows/mypy.yml` & `scrummd-0.1.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/.github/workflows/pipy-publish.yml` & `scrummd-0.1.0/.github/workflows/pipy-publish.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/.github/workflows/test-pypi-deploy.yml` & `scrummd-0.1.0/.github/workflows/test-pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/.gitignore` & `scrummd-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/.vscode/launch.json` & `scrummd-0.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/LICENSE.md` & `scrummd-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/Makefile` & `scrummd-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/card.rst` & `scrummd-0.1.0/docs/card.rst`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,55 @@
 - It has a summary
 - It has user defined Status, Description, Depends, Cucumber and Implementation note fields.
 - It has a collection defined as the Depends - so, ``sbl cli017`` will return the card cli004.
 - It has two tags defined - so, ``sbl Required`` and ``sbl "Required for v1""`` will return this card
 - That Summary and Status are 'Property' style fields
 - The the remainder of the fields are 'Paragraph' style fields and spread over multiple lines, divided by headers.
 
+Alternative Heading Style
+=========================
+
+Headings can also be done in the 'underline' style with a line that starts with
+``----`` or ``====`` underneath the header. So - an alternative formatting to
+:ref:`cli017` above would be:
+
+
+``cli017-alternative.md``
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: markdown
+
+    ---
+    Status: Done
+    ---
+
+    `sbl` relative file path output only
+    ====================================
+
+    Tags
+    ----
+
+    - Feature
+    - Required for v1
+
+    Description
+    -----------
+
+    We want to be able to just list the paths of all the cards that `sbl` returns when `sbl -b` or `sbl --bare` is called. The idea is that you'll be able to call
+    (etc)
+
+
+This example also makes use of the :ref:`allow_header_summary` configuration
+(which defaults to off). The option permits setting the ``summary`` for the card
+by creating an empty block with the summary as a heading.
+
+The underlining and hash styles can be combined - for instance, to use a summary
+with underline headers, and fields starting with ``#`` symbols.
+
+
 Fields
 ======
 
 Special fields
 --------------
 
 The following fields have special meaning to ScrumMD.
```

### Comparing `scrummd-0.0.8/docs/concepts.rst` & `scrummd-0.1.0/docs/concepts.rst`

 * *Files 13% similar despite different names*

```diff
@@ -71,8 +71,34 @@
 collection that will include ``tool02`` and ``tool03``.
 
 A folder inside a folder becomes a **sub-collection** - so, if you had a
 ``backlog`` folder and inside that, a ``epics`` folder, then any cards inside
 the ``epics`` folder would be in both the ``backlog`` and ``backlog.epics``
 collections.
 
-A card may be in multiple collections.
+A card may be in multiple collections.
+
+Collection sorting
+^^^^^^^^^^^^^^^^^^
+
+``sbl`` provides ``sort-by`` as an argument to allow you to sort cards, but - if
+you define a collection with the cards referenced in a card, they'll maintain
+the same order. 
+
+Given Scrum treats the order of cards in the Backlog and Sprint as important,
+you might choose to have your cards in a ``stories`` or ``features`` folder,
+and then intentionally create a backlog - for instance:
+
+``backlog.md``
+
+.. code-block:: markdown
+
+    ---
+    Summary: Backlog
+    ---
+
+    # Items
+
+    - [[card1]]
+    - [[card5]]
+    - [[card12]]
+    - [[card2]]
```

### Comparing `scrummd-0.0.8/docs/conf.py` & `scrummd-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/configuration.rst` & `scrummd-0.1.0/docs/configuration.rst`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,38 @@
 
 Supported fields
 ================
 
 ``[tool.scrummd]``
 ##################
 
+.. _allow_header_summary:
+
+``allow_header_summary``
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+Type
+""""
+
+bool
+
+Description
+"""""""""""
+
+Permit summaries to be set by an empty summary. For instance:
+
+.. code-block:: markdown
+
+   This is a valid summary
+   =======================
+
+   # Description
+
+   Description goes here
+
 ``strict``
 ^^^^^^^^^^
 
 Type
 """"
 
 bool
@@ -47,122 +71,173 @@
 string
 
 Description
 """""""""""
 
 Path to the Scrum repository containing cards and collections.
 
-``columns``
-^^^^^^^^^^^
+
+
+
+``required``
+^^^^^^^^^^^^
 
 Type
 """"
 
-string
+array of str
 
 Description
 """""""""""
 
-Array of columns to show with ``sbl``.
+List of fields that must be present in all cards.
 
-``omit_headers``
-^^^^^^^^^^^^^^^^
+``[tools.scrummd.fields.<field name>]``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Type
 """"
 
-bool
+array of str
 
 Description
 """""""""""
 
-Whether to omit headers from ``sbl`` output.
+Limit *field name* to specific values. Each member is an array of str.
 
+``[tools.scrummd.collections.<collection name>]``
+#################################################
 
-``scard_reference_format``
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+Additional restrictions which apply only to a specific collection.
+
+``required``
 
 Type
 """"
 
-str
+array of str
 
 Description
 """""""""""
 
-Format of ``[[card]]`` fields when shown by ``scard``. Replaces ``$field`` with the field from the card.
+List of fields that must be present in all cards in the collection.
 
-``required``
+
+``[tools.scrummd.collections.<collection name>.fields.<field name>]``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Type
 """"
 
 array of str
 
 Description
 """""""""""
 
-List of fields that must be present in all cards.
+Limit *field name* to specific values for all cards in the collection. Each
+member is an array of str.
 
-``[tools.scrummd.fields.<field name>]``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+``[tools.scrummd.sbl]``
+#######################
+
+``columns``
+^^^^^^^^^^^
 
 Type
 """"
 
-array of str
+array of string
 
 Description
 """""""""""
 
-Limit *field name* to specific values. Each member is an array of str.
+Array of columns to show with ``sbl``.
 
-``[tools.scrummd.collections.<collection name>]``
-#################################################
+``omit_headers``
+^^^^^^^^^^^^^^^^
 
-Additional restrictions which apply only to a specific collection.
+Type
+""""
 
-``required``
+bool
+
+Description
+"""""""""""
+
+Whether to omit headers from ``sbl`` output.
+
+``default_group_by``
+^^^^^^^^^^^^^^^^^^^^
 
 Type
 """"
 
-array of str
+array of string
 
 Description
 """""""""""
 
-List of fields that must be present in all cards in the collection.
+Default fields to group by if there's no ``--group-by`` field. Defaults to none.
 
-``[tools.scrummd.collections.<collection name>.fields.<field name>]``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+``[tools.scrummd.sboard]``
+##########################
+
+``default_group_by``
+^^^^^^^^^^^^^^^^^^^^
 
 Type
 """"
 
-array of str
+array of string
 
 Description
 """""""""""
 
-Limit *field name* to specific values for all cards in the collection. Each
-member is an array of str.
+Default fields to group by if there's no ``--group-by`` field. 
+A ``--group-by`` argument or ``default_group_by`` configuration must be set
+for ``sboard`` to work.
+
+``[tools.scrummd.scard]``
+#########################
+
+``reference_format``
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Type
+""""
+
+str
+
+Description
+"""""""""""
+
+Format of ``[[card]]`` fields when shown by ``scard``. Replaces ``$field`` with the field from the card.
 
 Example configuration file
 ==========================
 
 .. code-block:: toml
 
     [tool.scrummd]
     strict = true
     scrum_path = "scrum"
+    allow_header_summary = false
+    required = ["status"]
+
+    [tool.scrummd.sbl]
     columns = ["index", "status", "summary"]
-    scard_reference_format = "$index [$status] ($assignee)"
     omit_headers = false
-    required = ["status"]
+    # default_group_by is unset but commented as example
+    # default_group_by = ["status"]
+
+    [tool.scrummd.sboard]
+    default_group_by = ["status"]
+    
+    [tool.scrummd.scard]
+    reference_format = "$index [$status] ($assignee)"
 
     [tool.scrummd.fields]
     status = ["Not Fully Defined", "Ready", "In Progress", "In Testing", "Done"]
 
     [tool.scrummd.collections.epic]
     required = ["cost centre", "members"]
```

### Comparing `scrummd-0.0.8/docs/index.rst` & `scrummd-0.1.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. ScrumMD documentation master file, created by
    sphinx-quickstart on Sat Mar  9 12:49:29 2024.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
+.. image:: images/logo.png
+   :width: 50%
+   :align: center
+   :alt: ScrumMD Logo
+
 ScrumMD |version|
 ===================================
 
 Welcome to the documentation for ScrumMD.
 
-**ScrumMD** has tools for self-organising teams to manage cards written in md.
-As the name suggests, it was originally designed for teams to use in the Scrum
-process, but it can also be used for:
+**ScrumMD** has tools for self-organising teams to manage cards written in
+markdown.  As the name suggests, it was originally designed for teams to use in
+the Scrum process, but it can also be used for:
 
 - Kanban style processes
 - Tracking bugs and issues
 - Tracking decisions or questions
 
 It still has room to grow, but the fundamental tools are there to use it.
 :ref:`getting-started` shows you how to use it, and offers suggestions about how
```

### Comparing `scrummd-0.0.8/docs/installation.rst` & `scrummd-0.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/make.bat` & `scrummd-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/semver.rst` & `scrummd-0.1.0/docs/semver.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/source/scrummd.rst` & `scrummd-0.1.0/docs/source/scrummd.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/docs/tutorial1.rst` & `scrummd-0.1.0/docs/tutorial1.rst`

 * *Files 14% similar despite different names*

```diff
@@ -192,23 +192,46 @@
     bug1, Bug with project
 
 But - we could group by the Severity by using ``--group-by severity`` and add
 the output of the reporter with a ``-c`` command as follows:
 
 .. code-block:: text
 
-    sbl reports --group-by severity --columns index,summary,reporter
+    $ sbl reports --group-by severity --columns index,summary,reporter
     index, summary, reporter
     [severity = high]
     bug3, Bad bug, example2@example.com
     bug1, Bug with project, example@example.com
     [severity = low]
     bug2, Bug with project 2, example@example.com
     [severity = None]
 
+Board output
+^^^^^^^^^^^^
+
+Sometimes, it's helpful to get a more visual representation of the groups in a
+collection. By using ``--output board`` with ``sbl`` or ``sboard``, we can do
+this.
+
+For instance - with the example of the bugs above:
+
+.. code-block:: text
+
+    $ sboard reports --group-by severity
+    |high               |medium             |low                |None               |
+    |-------------------|-------------------|-------------------|-------------------|
+    |bug3               |                   |bug2               |                   |
+    |Bad bug            |                   |Bug with project 2 |                   |
+    |                   |                   |                   |                   |
+    |bug1               |                   |                   |                   |
+    |Bug with project   |                   |                   |                   |
+    |                   |                   |                   |                   |
+
+This can be helpful for showing reports like this, or for viewing the scrum
+board when grouping by status.
 
 ``bare`` mode
 ^^^^^^^^^^^^^
 
 Using ``sbl -b`` can give a list of relative paths in the collection and nothing
 more:
 
@@ -358,15 +381,17 @@
 Next, we'll change the references in the config to suit our fields. Modify
 ``scrum.toml`` as follows:
 
 .. code-block:: toml
 
     [tool.scrummd]
     strict = true
-    scard_reference_format = "$index [$status]"
+
+    [tool.scrummd.scard]
+    reference_format = "$index [$status]"
 
     [tool.scrummd.fields]
     severity = ["High", "Medium", "Low"]
     status = ["Ready For Development", "In Progress", "Done"]
 
 We added a reference format, and expected values for the status.
 
@@ -402,14 +427,40 @@
     index, summary
     bug3, Bad bug
     bug1, Bug with project
 
 You can see that just high severity bugs are returned. Alternatively - you could
 go ``sbl --include severity=high,medium`` to show all medium and high bugs.
 
+Sorting
+^^^^^^^
+
+Sorting can be a helpful thing to do.  If instead of filtering our bugs, we
+wanted to sort them priority, we can use ``--sort-by`` statements.
+
+.. code-block:: text
+
+    $ sbl --sort-by severity --columns "index, summary, severity"
+    index, summary, severity
+    card1, My first Scrum card,
+    bug3, Bad bug, High
+    bug1, Bug with project, High
+    bug2, Bug with project 2, Low
+
+Multiple ``--sort-by`` statements can be combined, and you can use ``^`` to
+reverse the order.
+
+.. code-block:: text
+
+    $ sbl --sort-by ^severity --columns "index, summary, severity"
+    index, summary, severity
+    bug2, Bug with project 2, Low
+    bug3, Bad bug, High
+    bug1, Bug with project, High
+    card1, My first Scrum card,
 
 Tags
 ^^^^
 
 Cards can be added to additional collections by 'tagging' them. If you add a
 ``tags`` field, any listed values will be created as a collection. Modify
 the following cards as follows:
@@ -489,14 +540,15 @@
     index, summary
     card1, My first Scrum card
     bug1, Bug with project 
 
 You can create an ``items`` field if you wish to add cards to the collection
 without creating a sub-collection.
 
+
 Conclusion
 ^^^^^^^^^^
 
 You have seen how to set up a basic repository, do some basic configuration,
 add some cards, and seen some ways of interacting with them.
 
 There should be enough tools here for you to go off and start managing your
```

### Comparing `scrummd-0.0.8/readthedocs.yaml` & `scrummd-0.1.0/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli001.md` & `scrummd-0.1.0/scrum/stories/cli001.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli002.md` & `scrummd-0.1.0/scrum/stories/cli002.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli004.md` & `scrummd-0.1.0/scrum/stories/cli004.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli009.md` & `scrummd-0.1.0/scrum/stories/cli009.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli011.md` & `scrummd-0.1.0/scrum/stories/cli011.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli017.md` & `scrummd-0.1.0/scrum/stories/cli017.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli021.md` & `scrummd-0.1.0/scrum/techdebt/cli021.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli022.md` & `scrummd-0.1.0/scrum/stories/cli022.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 Summary: Sort `sbl`
-Status: Ready
+Status: Done
 ---
 
 # Description
 
 We need to be able to sort cards in `sbl`.
 
 The expectation is that the user should be able to:
```

### Comparing `scrummd-0.0.8/scrum/backlog/cli023.md` & `scrummd-0.1.0/scrum/stories/cli023.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrum/backlog/cli024.md` & `scrummd-0.1.0/scrum/stories/cli024.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrummd/card.py` & `scrummd-0.1.0/scrummd/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             values per config has another value present.
         RequiredFieldNotPresentError: A field required by the config is not
             present
 
     Returns:
         Card: The card for the md file
     """
-    fields: dict[str, Field] = extract_fields(input_card)
+    fields: dict[str, Field] = extract_fields(config, input_card)
     collections: list[str] = [collection]
     index = path.name.split(".")[0]
     udf: dict[str, Field] = {k: v for k, v in fields.items() if k not in NON_UDF_FIELDS}
 
     assert_valid_fields(config, fields)
 
     if "index" in fields:
```

### Comparing `scrummd-0.0.8/scrummd/collection.py` & `scrummd-0.1.0/scrummd/collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-from argparse import ArgumentError
 from collections import OrderedDict
 from copy import copy
 from dataclasses import dataclass
 from enum import Enum
 import itertools
 import os
 import pathlib
-from typing import Optional, Union
+from typing import Optional
 from scrummd.card import Card, from_str
 import logging
 from scrummd.config import ScrumConfig
 from scrummd.exceptions import ValidationError, DuplicateIndexError
+from scrummd.source_md import Field, FieldNumber, FieldStr, typed_field
 
 logger = logging.getLogger(__name__)
 
-Collection = dict[str, Card]
+
+Collection = OrderedDict[str | Field, Card]
+
+
+# Weird use of tuple here - but we need to be able to distinguish whether it's
+# a "Groups" or "Collection"
+@dataclass
+class Group:
+    groups: "Groups"
+    collection: Collection
+
+
+Groups = OrderedDict[Optional[str | Field], Group]
 
 
 @dataclass
 class Filter:
     """Filter for filtering through a collection"""
 
     class FilterMode(Enum):
@@ -45,20 +57,33 @@
             Collection: The filtered collection
         """
         if isinstance(self.values, list):
             values = [value.strip().lower() for value in self.values]
         else:
             values = [str(self.values).strip().lower()]
 
-        return {
-            card_index: card
-            for card_index, card in collection.items()
-            if not isinstance(card.get_field(self.field), list)
-            and str(card.get_field(self.field)).strip().lower() in values
-        }
+        return OrderedDict(
+            [
+                (card_index, card)
+                for card_index, card in collection.items()
+                if not isinstance(card.get_field(self.field), list)
+                and str(card.get_field(self.field)).strip().lower() in values
+            ]
+        )
+
+
+@dataclass
+class SortCriteria:
+    """Fields and order to sort by"""
+
+    key: str
+    """Field name to sort by"""
+
+    reversed: bool
+    """Reverse the order of the collection"""
 
 
 def get_collection(
     config: ScrumConfig, collection_name: Optional[str] = None
 ) -> Collection:
     """Get a collection of cards
 
@@ -69,15 +94,15 @@
     Raises:
         DuplicateIndexError: A card with an index is found twice
 
     Returns:
         dict[str, Card]: A dict with the index of the card, and a card object
     """
 
-    all_cards: dict[str, Card] = {}
+    all_cards = Collection()
 
     collection_path = pathlib.Path(config.scrum_path)
     for root, _, files in os.walk(collection_path, followlinks=True):
         # So - this'll turn "scrum/backlog/special" into "backlog.special"
         path_parts = pathlib.Path(root).relative_to(collection_path).parts
         collection_from_path = ".".join(path_parts)
         # Ignore any folder starting with .
@@ -93,26 +118,26 @@
                 with open(path, "r") as fo:
                     contents = fo.read()
                     card = from_str(config, contents, collection_from_path, path)
                     if card.index in all_cards:
                         raise DuplicateIndexError(card.index, path)
                     all_cards[card.index] = card
 
-            except ValidationError as ex:
+            except DuplicateIndexError as ex:
                 if config.strict:
-                    logging.error("ValidationError (%s) reading %s", ex, path)
                     raise
                 else:
-                    logging.warning("ValidationError (%s) reading %s", ex, path)
+                    logging.warning("%s ignored", path)
 
-            except DuplicateIndexError as ex:
+            except ValidationError as ex:
                 if config.strict:
+                    logging.error("ValidationError (%s) reading %s", ex, path)
                     raise
                 else:
-                    logging.warning("%s ignored", path)
+                    logging.warning("ValidationError (%s) reading %s", ex, path)
 
     collections: dict[str, Collection] = {}
 
     # Get all the cards in each collection per implicit collection from folder
     # and collections listed in the card
     for index, card in all_cards.items():
         for _collection in card.collections:
@@ -122,136 +147,201 @@
             # A, then A.B, then A.B.C
             for partial_name in itertools.accumulate(
                 _collection.split("."), lambda i, j: f"{i}.{j}"
             ):
                 if partial_name in collections:
                     collections[partial_name][index] = card
                 else:
-                    collections[partial_name] = {index: card}
+                    collections[partial_name] = Collection({index: card})
 
     # Get all the collections defined in a card in the fields. Again - needs to
     # add to parent collections too.
     # Holy horizontal ladder, Batman!
-    for index, card in all_cards.items():
+    for all_card_index, card in all_cards.items():
+        assert isinstance(all_card_index, str)
         for defined_name, defined_collection in card.defined_collections.items():
             for referenced_card_index in defined_collection:
                 if referenced_card_index not in all_cards:
                     # Card not found
                     continue
 
                 if defined_name in collections:
                     collections[defined_name][referenced_card_index] = all_cards[
                         referenced_card_index
                     ]
                 else:
-                    collections[defined_name] = {
-                        referenced_card_index: all_cards[referenced_card_index]
-                    }
-                if index in collections:
-                    collections[index][referenced_card_index] = all_cards[
+                    collections[defined_name] = Collection(
+                        {referenced_card_index: all_cards[referenced_card_index]}
+                    )
+                if all_card_index in collections:
+                    collections[all_card_index][referenced_card_index] = all_cards[
                         referenced_card_index
                     ]
                 else:
-                    collections[index] = {
-                        referenced_card_index: all_cards[referenced_card_index]
-                    }
+                    collections[all_card_index] = Collection(
+                        {referenced_card_index: all_cards[referenced_card_index]}
+                    )
 
     # Validate that all cards in a collection are valid per its rules in config
     for _collection_name, collection in collections.items():
         collection_config = config.collections.get(_collection_name)
         if not collection_config:
             continue
-        for index, card in collection.items():
+        for _, card in collection.items():
             try:
                 card.assert_valid_rules(collection_config)
             except ValidationError as ex:
                 if config.strict:
                     logging.error("ValidationError (%s) reading %s", ex, path)
                     raise
                 else:
                     logging.warn("ValidationError (%s) reading %s", ex, path)
 
     if not collection_name:
-        return all_cards
+        return Collection(all_cards)
 
-    return collections.get(collection_name) or {}
+    return collections.get(collection_name) or Collection({})
 
 
-Groups = dict[Optional[str], Union["Groups", list[Card]]]
+def _sort_key(field: Field | str | None) -> tuple[float, str]:
+    """
+    Sort by None, then Numerical order, then Strings
+
+    Args:
+        field (Field): Field to sort
+
+    Raises:
+        TypeError: There was a field that wasn't an expected type
+
+    Returns:
+        tuple[float, str]: A tuple suitable for sorting by
+    """
+    if field is None:
+        return (float("-inf"), "")
+    elif isinstance(field, FieldNumber):
+        return (field, "")
+    elif isinstance(field, FieldStr) or isinstance(field, str):
+        return (float("inf"), field)
+    else:
+        raise TypeError("%s is not an available type", type(field))
 
 
 def group_collection(
-    config: ScrumConfig, collection: Collection, groups: list[str]
+    config: ScrumConfig,
+    collection: Collection,
+    groups: list[str],
+    sort_criteria: list[SortCriteria] = [],
 ) -> Groups:
-    """Group collection into (potentially nested) groups by the field in the Card
+    """Group collection into (potentially nested) groups by the field in the Card, sorted if
+    required
 
     Args:
         config (ScrumConfig): Scrum config
         collection (Collection): Collection of cards to group
         groups (list[str]): All the groups that need to be made
+        sort_criteria (list[SortCriteria]): Criteria to sort the groups and cards by
 
     Returns:
         Groups: A dict with the group value, and either more groups or the field value
     """
 
+    # Why are we sorting here? It means we don't need to store the grouping fields to sort them
+    # later. This may change
+
     cur_group = groups[0].casefold()
     predefined = cur_group in [k.casefold() for k in config.fields.keys()]
-    card_groups: Groups = OrderedDict()
+    card_groups: Groups = Groups()
 
     if predefined:
         group = next(
             fields
             for key, fields in config.fields.items()
             if key.casefold() == cur_group
         )
-        for f in [f.casefold() for f in group]:
-            card_groups[f] = []
+        for predefined_field in [typed_field(f.casefold()) for f in group]:
+            card_groups[predefined_field] = Group(Groups(), Collection())
     else:
-        fields: set[str] = set()
+        fields: set[Optional[Field]] = set()
         for card in collection.values():
             card_field = card.get_field(cur_group)
             if isinstance(card_field, str):
-                fields.add(card_field.casefold())
-        ordered_fields = sorted(fields)
-        for f in ordered_fields:
-            card_groups[f] = []
-
-    card_groups[None] = []
+                fields.add(typed_field(card_field.casefold()))
+            else:
+                fields.add(card_field)
+        ordered_fields = sorted(fields, key=_sort_key)
+        for ordered_field in ordered_fields:
+            card_groups[ordered_field] = Group(Groups(), Collection())
+
+    card_groups[None] = Group(Groups(), Collection())
+
+    # This chunk here sorts the group headings themselves, if there is a sort
+    # for them
+    matching_sort = [
+        criteria for criteria in sort_criteria if criteria.key.casefold() == cur_group
+    ]
+    if matching_sort:
+        # sort by matching_sort[0]
+        sorted_card_groups_result = sorted(
+            card_groups.items(),
+            key=lambda k: _sort_key(k[0]),
+            reverse=matching_sort[0].reversed,
+        )
+        sorted_card_groups = OrderedDict(sorted_card_groups_result)
+    else:
+        sorted_card_groups = card_groups
 
-    # This could potentially be squished into the generating the fields so we don't have to pass through all of the cards multiple times
-    # But - this is clearer, and don't want to prematurely optimize
+    # The FieldStr/FieldNumber was supposed to make this more readable, but I
+    # really have more reflection here than I'd prefer
     for card in collection.values():
         card_field = card.get_field(cur_group)
         if card_field:
-            if not isinstance(card_field, str):
-                msg = f"{card.get_field('index')} can't group by {cur_group}: must be string."
+            if isinstance(card_field, FieldStr):
+                output_collection = sorted_card_groups[
+                    FieldStr(card_field.casefold())
+                ].collection
+            elif isinstance(card_field, FieldNumber):
+                output_collection = sorted_card_groups[card_field].collection
+            else:
+                msg = f"{card.get_field('index')} can't group by {cur_group}: must be string or number."
                 if config.strict:
                     raise ValidationError(msg)
                 else:
                     logger.warn(msg)
                     continue
-            else:
-                field = card_field.casefold()
         else:
-            field = None
+            output_collection = sorted_card_groups[None].collection
 
-        output_collection = card_groups[field]
-        assert isinstance(output_collection, list)
-        output_collection.append(card)
+        assert output_collection is not None
+        output_collection[card.index] = card
+
+    for group_key, group_value in sorted_card_groups.items():
+        sorted_output_collection = sort_collection(
+            group_value.collection, sort_criteria
+        )
+        sorted_card_groups[group_key].collection = sorted_output_collection
 
     if len(groups) == 1:
-        return card_groups
+        return sorted_card_groups
 
     # This is not particularly clear - if there's more groups to embed, recurse.
-    return {
-        key: group_collection(
-            config, {c.index: c for c in group if isinstance(c, Card)}, groups[1:]
+    embedded_groups = [
+        (
+            key,
+            Group(
+                group_collection(
+                    config,
+                    Collection({c.index: c for c in group.collection.values()}),
+                    groups[1:],
+                ),
+                Collection(),
+            ),
         )
         for key, group in card_groups.items()
-    }
+    ]
+    return Groups(embedded_groups)
 
 
 def filter_collection(collection: Collection, filters: list[Filter]) -> Collection:
     """Apply all filters to a collection
 
     Args:
         collection (Collection): Collection to apply filters to.
@@ -260,7 +350,47 @@
     Returns:
         Collection: Filtered collection of cards.
     """
     working_collection = copy(collection)
     for f in filters:
         working_collection = f.apply(working_collection)
     return working_collection
+
+
+def sort_collection(collection: Collection, criteria: list[SortCriteria]) -> Collection:
+    """Sort a collection of cards by the sort criteria
+
+    Args:
+        collection (Collection): Collection to sort
+        criteria (list[SortCriteria]): Criteria to sort by
+
+    Returns:
+        SortedCollection: Sorted collection of cards
+    """
+
+    # Yet more recursion. We can't just use `sorted` with multiple tuples joined
+    # together because some criteria might be reversed
+    # The 'O's with the loop are bigger than I'd prefer, but practically, I'm
+    # seeing ~0.04-0.05s with `sbench` sorting 10000 cards by 2 criteria - so
+    # not _really_ wanting to prematurely optimize it yet.
+
+    if len(criteria) == 0:
+        return OrderedDict(collection)
+
+    sorted_by_criteria = sorted(
+        collection.items(),
+        key=lambda k: _sort_key(k[1].get_field(criteria[0].key)),
+        reverse=criteria[0].reversed,
+    )
+    if len(criteria) > 1:
+        output_collection = Collection()
+        grouped = itertools.groupby(
+            sorted_by_criteria, key=lambda k: _sort_key(k[1].get_field(criteria[0].key))
+        )
+        for _, group in grouped:
+            subcollection = Collection(group)
+            sorted_subcollection = sort_collection(subcollection, criteria[1:])
+            for index, card in sorted_subcollection.items():
+                output_collection[FieldStr(index)] = card
+        return output_collection
+    else:
+        return OrderedDict(sorted_by_criteria)
```

### Comparing `scrummd-0.0.8/scrummd/config.py` & `scrummd-0.1.0/scrummd/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """The ScrumConfig class to configure processing scrum files."""
 
 from dataclasses import dataclass, field, fields
+from typing import Optional
 from scrummd import const
 
 
 @dataclass
 class CollectionConfig:
     """Configuration for any specific collection of cards"""
 
@@ -12,32 +13,69 @@
     """Fields with limited permitted values and defined order"""
 
     required: list[str] = field(default_factory=list)
     """Fields that are required to be in a card"""
 
 
 @dataclass
+class SblConfig:
+    """Configuration specific to sbl"""
+
+    columns: list[str] = field(default_factory=lambda: ["index", "summary"])
+    """List of columns to return in output"""
+    default_group_by: Optional[str] = None
+    """Default group-by for sbl"""
+    omit_headers: bool = False
+    """Omit headers from output"""
+
+
+@dataclass
+class SboardConfig:
+    """Configuration specific to sboard"""
+
+    columns: list[str] = field(default_factory=lambda: ["index", "summary"])
+    """List of columns to return in output"""
+    default_group_by: Optional[str] = None
+    """Default group-by for sboard"""
+
+
+@dataclass
+class ScardConfig:
+    """Configuration specific to scard"""
+
+    reference_format: str = "[$index]"
+    """Fields to show when a card is referenced in a field in `scard`"""
+
+
+@dataclass
 class ScrumConfig(CollectionConfig):
     """The configuration that applies to all cards and ScrumMD"""
 
     scrum_path: str = const.DEFAULT_SCRUM_FOLDER_NAME
     """Base path for the scrum folder"""
 
     strict: bool = False
     """Fail on any error with the scrum folder (such as duplicate index or invalid file)"""
 
-    columns: list[str] = field(default_factory=lambda: ["index", "summary"])
-    """List of columns to return in output"""
+    collections: dict[str, CollectionConfig] = field(default_factory=dict)
+    """Embedded collection config"""
 
-    omit_headers: bool = False
-    """Omit headers from output"""
+    scard: ScardConfig = field(default_factory=ScardConfig)
 
-    scard_reference_format: str = "[$index]"
-    """Fields to show when a card is referenced in a field in `scard`"""
+    sbl: SblConfig = field(default_factory=SblConfig)
 
-    collections: dict[str, CollectionConfig] = field(default_factory=dict)
+    sboard: SboardConfig = field(default_factory=SboardConfig)
+
+    allow_header_summary: bool = False
 
     def __post_init__(self):
-        """Fix up 'CollectionConfig' which is erroneously a dict after initialising"""
+        """Fix up embedded fields, which default to dicts"""
 
         for key, collection in self.collections.items():
             self.collections[key] = CollectionConfig(**collection)
+
+        if isinstance(self.sbl, dict):
+            self.sbl = SblConfig(**self.sbl)
+        if isinstance(self.scard, dict):
+            self.scard = ScardConfig(**self.scard)
+        if isinstance(self.sboard, dict):
+            self.sboard = SboardConfig(**self.sboard)
```

### Comparing `scrummd-0.0.8/scrummd/exceptions.py` & `scrummd-0.1.0/scrummd/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrummd/sbench.py` & `scrummd-0.1.0/scrummd/sbench.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,56 @@
 from statistics import mean
 import timeit
 import logging
 import tempfile
 import contextlib
 from collections.abc import Iterator
 import random
-from scrummd.collection import get_collection
+from scrummd.collection import SortCriteria, get_collection, sort_collection
 from scrummd.version import version_to_output
 from scrummd.config import ScrumConfig
 
 
-def rand_str(size: int):
+def rand_str(size: int, whitespace: bool = False):
     return "".join(
         [
-            random.choice("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ ")
+            random.choice(
+                f"abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ{' ' if whitespace else ''}"
+            )
             for _ in range(size)
         ]
     )
 
 
 @contextlib.contextmanager
-def scrum_repo(count: int, references: int, minsize: int) -> Iterator[ScrumConfig]:
+def scrum_repo(
+    count: int, references: int, minsize: int, sortcount: int
+) -> Iterator[ScrumConfig]:
     """Create a temporary folder full of cards
 
     Args:
         count (int): Amount of files to generate
         references (int): Amount of card references to add to each card
         minsize (int): Min size of each card in bytes
+        sortcount (int): Amount of sort criteria to apply
 
     Returns:
         ScrumConfig: The ScrumConfig to load files with
     """
     logging.info("Creating scrum repo")
     with tempfile.TemporaryDirectory() as tmpdir:
         for cardno in range(count):
             path = Path(tmpdir, f"c{cardno}.md")
             with open(path, "w") as card_f:
                 logging.debug("Writing %s", [path])
                 cur_references: list[str] = []
-                contents = f"---\n summary: {rand_str(50)}\n---"
+                contents = f"---\n summary: {rand_str(50)}"
+                for sortnum in range(sortcount):
+                    contents += f"\ns{sortnum}: {random.choice([random.randint(0,20), rand_str(2)]) }"
+                contents += "\n---"
                 block_count = 0
                 while len(contents) < minsize and len(cur_references) < references:
                     block_count += 1
                     block_type = random.choice(["str", "list"])
                     contents += f"\n\n#header{block_count} \n\n"
                     if block_type == "str":
                         while random.random() > 0.2:
@@ -62,15 +70,14 @@
                             contents += "\n- "
                             if random.random() < 0.5:
                                 contents += rand_str(50)
                             else:
                                 reference = f"c{random.choice(range(count))}"
                                 cur_references.append(reference)
                                 contents += f"[[{reference}]]"
-
                 card_f.write(contents)
 
         yield ScrumConfig(scrum_path=tmpdir)
     logging.info("Cleaned up")
 
 
 def create_parser() -> argparse.ArgumentParser:
@@ -86,14 +93,15 @@
     parser.add_argument(
         "--references", help="Amount of references to add in each card", default=10
     )
     parser.add_argument(
         "--size", help="Minimum size of each card in bytes", default=1000
     )
     parser.add_argument("--times", help="Times to test collection", default=5)
+    parser.add_argument("--sorts", help="Amount of sort criteria to sort by", default=2)
     # parser.add_argument(
     #    "--cache", help="Test twice each time to test caching time", action="store_true"
     # )
     parser.add_argument("-v", help="Level of verbosity", action="count", default=0)
     parser.add_argument(
         "--version",
         action="version",
@@ -107,19 +115,37 @@
 def entry():
     """Entry point for sbench"""
 
     args = create_parser().parse_args()
 
     logging.basicConfig(level=30 - args.v * 10)
 
-    with scrum_repo(int(args.count), int(args.references), int(args.size)) as config:
+    with scrum_repo(
+        int(args.count), int(args.references), int(args.size), int(args.sorts)
+    ) as config:
         times = []
         print(f"get_collection executions")
         for count in range(int(args.times)):
             ex_time = timeit.timeit(lambda: get_collection(config), number=1)
             times.append(ex_time)
             print(f"{count}: {ex_time} s")
         print(f" Avg: {mean(times)} s")
 
+        if args.sorts > 0:
+            sort_times = []
+            collection = get_collection(config)
+            print("\nsort_collection executions")
+            criteria = [
+                SortCriteria(f"s{sort_number}", False)
+                for sort_number in range(args.sorts)
+            ]
+            for count in range(int(args.times)):
+                ex_time = timeit.timeit(
+                    lambda: sort_collection(collection, criteria), number=1
+                )
+                sort_times.append(ex_time)
+                print(f"{count}: {ex_time} s")
+            print(f" Avg: {mean(sort_times)} s")
+
 
 if __name__ == "__main__":
     entry()
```

### Comparing `scrummd-0.0.8/scrummd/sbl.py` & `scrummd-0.1.0/scrummd/scard.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,164 +1,170 @@
-"""Display a collection of scrum cards"""
+"""Display any number of scrum cards"""
 
 import argparse
-
-from scrummd.collection import (
-    Filter,
-    Groups,
-    get_collection,
-    group_collection,
-    filter_collection,
-)
+import logging
+import re
+from typing import Optional
+from scrummd.card import Card
+from scrummd.collection import Collection, get_collection
 from scrummd.config import ScrumConfig
 from scrummd.config_loader import load_fs_config
-from scrummd.exceptions import ValidationError
-from scrummd.scard import format_field
+from scrummd.source_md import (
+    CardComponent,
+    Field,
+    FieldNumber,
+    FieldStr,
+    StringComponent,
+)
 from scrummd.version import version_to_output
 
-VALIDATION_ERROR = 1
+logger = logging.getLogger(__name__)
+
+_field_re = re.compile(r"\$(\w+)")
 
 
-def include_to_filter(source: str) -> Filter:
-    """Transform an --include argument into a Filter
+def format_field(value: Optional[Field]) -> str:
+    """Format a given field for output
 
     Args:
-        source (str): FILTER from --include
+        value (Optional[Field]): Field to output
+
+    Raises:
+        TypeError: Field is not a recognised formattable type
 
     Returns:
-        Filter: Filter object from the string
+        str: Field suitable to use in output
     """
-    try:
-        field, value_str = source.split("=")
-    except ValueError:
-        raise argparse.ArgumentTypeError(
-            "Filter not in valid format. Expected format is --include key=value1[, value2]"
-        )
-
-    values = [value.strip() for value in value_str.split(",")]
+    if value is None:
+        return ""
+    if isinstance(value, FieldStr):
+        return value
+    if isinstance(value, list):
+        return f"[{', '.join(value)}]"
+    if isinstance(value, FieldNumber):
+        return f"{value:g}"
+    else:
+        raise TypeError(f"Unsupported type {type(value)}")
 
-    return Filter(field.strip(), values, Filter.FilterMode.EQUALS)
 
+def format_card_summary(config: ScrumConfig, card: Card) -> str:
+    """Format the summary of a card per the config
 
-def create_parser() -> argparse.ArgumentParser:
-    """Create an argument parser for sbl
+    Args:
+        config (ScrumConfig): Active scrum configuration
+        card (Card): Card to format
 
     Returns:
-        argparse.ArgumentParser: ArgumentParser for sbl
+        str: Card formatted per configuration
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "collection",
-        nargs="?",
-        help="The collection to return. If none is given, all cards are returned.",
-    )
-    parser.add_argument(
-        "-c",
-        "--columns",
-        nargs="?",
-        help="A comma separated list of columns to return.",
-    )
-    parser.add_argument(
-        "-b",
-        "--bare",
-        action="store_true",
-        help="Return bare paths only suitable for scripting. Effectively shorthand for `sbl -H -c path`.",
-    )
-    parser.add_argument(
-        "-H",
-        "--omit-headers",
-        action="store_true",
-        help="Omit headers from output.",
-    )
+    format = config.scard.reference_format
 
-    parser.add_argument(
-        "-g",
-        "--group-by",
-        action="append",
-        metavar="FIELD",
-        help="Group by field in card. Can use multiple group-by arguments to have multiple levels of grouping.",
-    )
+    output = _field_re.sub(lambda m: format_field(card.get_field(m.group(1))), format)
+    return output
 
-    parser.add_argument(
-        "-i",
-        "--include",
-        action="append",
-        metavar="FILTER",
-        type=include_to_filter,
-        help="Only include collections that match this filter. The filter is in the format "
-        + "`key=value1[, value2, ...]`. Multiple values verify if the field is any of the values. "
-        + "Multiple --include statements must all be matched.",
-    )
 
-    parser.add_argument(
-        "--version",
-        action="version",
-        version=version_to_output(),
-    )
-    parser.description = __doc__
-    return parser
+def output_fieldstr(config: ScrumConfig, value: Field, collection: Collection) -> str:
+    """Generate the formatted output value for the field from the components
 
+    Args:
+        config (ScrumConfig): Active scrum configuration
+        value (FieldStr): Value to generate output for
+        collection (Collection): Full collection of cards for reference's sake
 
-def entry():
-    """Entry point for sbl"""
-    parser = create_parser()
-    args = parser.parse_args()
+    Returns:
+        str: Output ready field
+    """
+    output = ""
+    if not isinstance(value, FieldStr) and isinstance(value, str):
+        # Likely index
+        return value
+
+    if isinstance(value, FieldStr):
+        for component in value.components():
+            if isinstance(component, StringComponent):
+                output += component.value
+            elif isinstance(component, CardComponent):
+                card = collection.get(component.cardIndex)
+                if card:
+                    output += format_card_summary(config, card)
+                else:
+                    output += f"[[{component.cardIndex}]] (NOT FOUND)"
+                    logger.warning(
+                        f"Card index {component.cardIndex} not found when expanding"
+                    )
+                    # Should strict fail here?
+            else:
+                raise ValueError("Component of invalid type")
 
-    config = load_fs_config()
+    return output
 
-    try:
-        collection = get_collection(config, args.collection)
-    except ValidationError:
-        if config.strict:
-            return VALIDATION_ERROR
 
-    if args.columns:
-        columns = [column.strip() for column in args.columns.split(",")]
-    else:
-        columns = config.columns
+def output_cards(config: ScrumConfig, collection: Collection, card_indexes: list[str]):
+    """Output cards to stdout
 
-    omit_headers = args.omit_headers or config.omit_headers
+    Args:
+        config (ScrumConfig): Current configuration
+        collection (Collection): Complete collection of cards
+        card_index (list[str]): Indexes of cards to output
+    """
 
-    if args.bare:
-        columns = ["path"]
-        omit_headers = True
+    for card_index in card_indexes:
+        if card_index not in collection:
+            logger.error("Card %s not found", card_index)
+            continue
+        card = collection[card_index]
+        print("---")
+        print(f"{card_index}: {card.summary}")
+        print("---")
+        for k, v in card.udf.items():
+            if v is None:
+                continue
+
+            if isinstance(v, list):
+                for item in v:
+                    formatted_value = output_fieldstr(config, item, collection)
+                    print(f"- {formatted_value}")
+            elif isinstance(v, FieldStr):
+                formatted_value = output_fieldstr(config, v, collection)
+                if v.find("\n") > 0:
+                    print(f"# {k}")
+                    print(formatted_value)
+                    print()
+                else:
+                    print(f"{k}: {formatted_value}")
+            elif isinstance(v, FieldNumber):
+                formatted_value = f"{v:g}"
+                print(f"{k}: {formatted_value}")
+            else:
+                raise ValueError(f"Unsupported type {type(v)}")
 
-    if not omit_headers:
-        print(", ".join(columns))
 
-    if args.include:
-        collection = filter_collection(collection, args.include)
+def create_parser() -> argparse.ArgumentParser:
+    """Create an argument parser for scard
 
-    if not args.group_by:
-        for card in collection.values():
-            values = [format_field(card.get_field(col)) for col in columns]
-            print(", ".join(values))
+    Returns:
+        ArgumentParser: Argument parser to use
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument("card", nargs="*", help="Index of cards to return")
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=version_to_output(),
+    )
+    parser.description = __doc__
+    return parser
 
-    else:
-        grouped = group_collection(config, collection, args.group_by)
 
-        def output_group(
-            config: ScrumConfig, collection: Groups, group_fields: list[str], level=1
-        ):
-            for group_key, cards in collection.items():
-                if not omit_headers:
-                    print(
-                        f"[" * level
-                        + group_fields[0]
-                        + " = "
-                        + str(group_key)
-                        + "]" * level
-                    )
+def entry():
+    """Entry point for scard"""
+    args = create_parser().parse_args()
 
-                if isinstance(cards, dict):
-                    output_group(config, cards, group_fields[1:], level + 1)
+    config = load_fs_config()
 
-                else:
-                    for card in cards:
-                        values = [format_field(card.get_field(col)) for col in columns]
-                        print(", ".join(values))
+    collection = get_collection(config)
 
-        output_group(config, grouped, args.group_by)
+    output_cards(config, collection, args.card)
 
 
 if __name__ == "__main__":
-    entry()
+    pass
```

### Comparing `scrummd-0.0.8/scrummd/source_md.py` & `scrummd-0.1.0/scrummd/source_md.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import re
 
 from enum import Enum
 from typing import Optional, Any, Union
 
+from scrummd.config import ScrumConfig
 from scrummd.exceptions import InvalidFileError
 
 
 class FieldComponent:
     """A section of the field component"""
 
     pass
@@ -61,15 +62,17 @@
             cursor = match.end()
         if cursor != len(self):
             self._components.append(StringComponent(self[cursor:]))
 
         return self._components
 
 
-Field = Union[FieldStr, list[FieldStr]]
+FieldNumber = float
+
+Field = FieldStr | list[FieldStr] | FieldNumber
 """A field from the md file"""
 
 
 def get_block_name(md_line: str) -> str:
     """Get the name of the block from the header line"""
     results = re.match(r"\#+(.*)", md_line)
     if results is not None:
@@ -102,27 +105,52 @@
         return ""
 
 
 def extract_collection(field_value: Field) -> list[str]:
     """Extract all of the card ids from a field (str or list of strings)
 
     Args:
-        field_value (Union[str, list[str]]): Field from the md file
+        field_value (Field): Field from the md file
 
     Returns:
         list[Index]: A list of all card indexes
     """
-    field_list = field_value if isinstance(field_value, list) else [field_value]
+    field_list: list[Field] = []
+    if isinstance(field_value, list):
+        field_list.extend(field_value)
+    else:
+        field_list.append(field_value)
+
     results = []
     for value in field_list:
-        results.extend(_extract_re.findall(value))
+        results.extend(_extract_re.findall(str(value)))
     return results
 
 
-def extract_fields(md_file: str) -> dict[str, Field]:
+def typed_field(field: str) -> Field:
+    """Return a Field of an appropriate type from the string
+
+    Currently supports strings and numbers - not lists.
+
+    Args:
+        field (str): Field value to interpret
+
+    Returns:
+        Field: A correctly typed field
+    """
+
+    try:
+        # I don't really like doing this as a non-exceptional exception, but it
+        # is at least clear
+        return FieldNumber(field)
+    except ValueError:
+        return FieldStr(field)
+
+
+def extract_fields(config: ScrumConfig, md_file: str) -> dict[str, Field]:
     """Extract all fields from the md_file
 
     There are two types of fields:
     - 'Property' style fields
     - 'md header' style fields:
 
     There are two types of value:
@@ -166,39 +194,53 @@
                 block_status = BlockStatus.IN_PROPERTY_BLOCK
                 continue
             elif stripped_line[0] == "#":
                 block_name = get_block_name(stripped_line)
                 block_value = ""
                 block_status = BlockStatus.IN_HEADER_BLOCK
                 continue
+            elif len(stripped_line) >= 4 and (
+                stripped_line[0:4] == "====" or stripped_line[0:4] == "----"
+            ):
+                # Currently, ==== and ---- are conflated, but they may become
+                # first and second level headers respectively
+                block_value_lines = block_value.splitlines()
+                if len(block_value_lines) > 1:
+                    block_name = (block_value_lines[-1]).strip().casefold()
+                    block_value = ""
+                    block_status = BlockStatus.IN_HEADER_BLOCK
+                    continue
+            else:
+                block_value += line
+                continue
 
         if block_status == BlockStatus.IN_PROPERTY_LIST:
             if stripped_line[0] == "-" and stripped_line != "---":
                 value = split_list_item(stripped_line)
                 field_list = fields[list_field_key]
                 assert isinstance(field_list, list)
                 field_list.append(FieldStr(value))
                 continue
             else:
                 list_field_key = ""
-                block_status == BlockStatus.IN_PROPERTY_BLOCK
+                block_status = BlockStatus.IN_PROPERTY_BLOCK
 
         if block_status == BlockStatus.IN_PROPERTY_BLOCK:
             if stripped_line == "---":
                 block_status = BlockStatus.NO_BLOCK
                 continue
             if ":" not in stripped_line:
                 raise InvalidFileError("Invalid property line %s", stripped_line)
             key, value = split_property(stripped_line)
             if value == "":
                 block_status = BlockStatus.IN_PROPERTY_LIST
                 list_field_key = key
                 fields[list_field_key] = []
             else:
-                fields[key] = FieldStr(value)
+                fields[key] = typed_field(value)
             continue
 
         if block_status == BlockStatus.IN_HEADER_LIST:
             if stripped_line[0] == "-" and stripped_line != "---":
                 value = split_list_item(stripped_line)
                 field_list = fields[list_field_key]
                 assert isinstance(field_list, list)
@@ -215,21 +257,35 @@
             block_value += line + "\n"
             continue
 
         if block_status == BlockStatus.IN_HEADER_BLOCK:
             if stripped_line == "---":
                 block_status = BlockStatus.IN_PROPERTY_BLOCK
                 if block_name is not None:
-                    fields[block_name] = FieldStr(block_value)
+                    fields[block_name] = typed_field(block_value)
                 block_value = ""
                 continue
+            elif len(stripped_line) >= 4 and (
+                stripped_line[0:4] == "====" or stripped_line[0:4] == "----"
+            ):
+                # Currently, ==== and ---- are conflated, but they may become
+                # first and second level headers respectively
+                block_value_lines = block_value.splitlines()
+                if block_name is not None:
+                    if len(block_value_lines) > 1:
+                        fields[block_name] = typed_field(
+                            "\n".join(block_value_lines[0:-1]).strip()
+                        )
+                if len(block_value_lines) > 1:
+                    block_name = (block_value_lines[-1]).strip().casefold()
+                block_value = ""
             elif stripped_line[0] == "#":
                 block_status = BlockStatus.IN_HEADER_BLOCK
                 if block_name is not None:
-                    fields[block_name] = FieldStr(block_value.strip())
+                    fields[block_name] = typed_field(block_value.strip())
                 block_name = get_block_name(stripped_line)
                 block_value = ""
                 continue
             elif stripped_line[0] == "-" and block_value.strip() == "":
                 block_status = BlockStatus.IN_HEADER_LIST
                 if block_name is not None:
                     list_field_key = block_name
@@ -238,10 +294,28 @@
                 block_status = BlockStatus.IN_CODE_BLOCK
                 block_value += line + "\n"
             else:
                 block_value += line + "\n"
 
     if block_status == BlockStatus.IN_HEADER_BLOCK:
         if block_name is not None:
-            fields[block_name] = FieldStr(block_value)
+            fields[block_name] = FieldStr(block_value.strip())
+
+    if config.allow_header_summary and "summary" not in fields:
+        possible_headers: list[str] = [
+            key
+            for key, value in fields.items()
+            if value == None or (isinstance(value, FieldStr) and len(value) == 0)
+        ]
+        if len(possible_headers) == 1:
+            header_key = possible_headers[0]
+            # Need to get the actual casing of the summary -
+            # the summary has been CaseFold. By doing a second pass
+            # we can reduce the complexity of holding the data in
+            # the algorithm proper
+            for line in md_file.splitlines():
+                if line.casefold().strip() == header_key:
+                    fields["summary"] = FieldStr(line.strip())
+        else:
+            raise InvalidFileError("No clear summary field")
 
     return fields
```

### Comparing `scrummd-0.0.8/scrummd/svalid.py` & `scrummd-0.1.0/scrummd/svalid.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/scrummd.egg-info/SOURCES.txt` & `scrummd-0.1.0/scrummd.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 docs/make.bat
 docs/requirements.txt
 docs/semver.rst
 docs/tutorial1.rst
 docs/commands/commands.rst
 docs/commands/sbench.rst
 docs/commands/sbl.rst
+docs/commands/sboard.rst
 docs/commands/scard.rst
 docs/commands/svalid.rst
+docs/images/logo.png
 docs/source/modules.rst
 docs/source/scrummd.rst
 docs/tutorial_examples/tutorial1.2/scrum/backlog/card1.md
 docs/tutorial_examples/tutorial1.2/scrum/reports/bug1.md
 docs/tutorial_examples/tutorial1.2/scrum/reports/bug2.md
 docs/tutorial_examples/tutorial1.2/scrum/reports/bug3.md
 docs/tutorial_examples/tutorial1.3/scrum/backlog/card1.md
@@ -51,81 +53,95 @@
 docs/tutorial_examples/tutorial1.6/scrum/backlog/card1.md
 docs/tutorial_examples/tutorial1.6/scrum/reports/bug1.md
 docs/tutorial_examples/tutorial1.6/scrum/reports/bug2.md
 docs/tutorial_examples/tutorial1.6/scrum/reports/bug3.md
 docs/tutorial_examples/tutorial1/scrum/backlog/card1.md
 docs/tutorial_examples/tutorial1/scrum/reports/bug1.md
 scrum/v0-1.md
-scrum/backlog/cli001.md
-scrum/backlog/cli002.md
-scrum/backlog/cli003.md
-scrum/backlog/cli004.md
-scrum/backlog/cli005.md
-scrum/backlog/cli006.md
-scrum/backlog/cli007.md
-scrum/backlog/cli008.md
-scrum/backlog/cli009.md
-scrum/backlog/cli010.md
-scrum/backlog/cli011.md
-scrum/backlog/cli012.md
-scrum/backlog/cli013.md
-scrum/backlog/cli014.md
-scrum/backlog/cli015.md
-scrum/backlog/cli016.md
-scrum/backlog/cli017.md
-scrum/backlog/cli018.md
-scrum/backlog/cli019.md
-scrum/backlog/cli020.md
-scrum/backlog/cli021.md
-scrum/backlog/cli022.md
-scrum/backlog/cli023.md
-scrum/backlog/cli024.md
-scrum/backlog/cli025.md
-scrum/backlog/cli026.md
-scrum/backlog/cli027.md
-scrum/backlog/cli028.md
-scrum/backlog/cli029.md
+scrum/bugs/cli019.md
+scrum/bugs/cli026.md
+scrum/stories/cli001.md
+scrum/stories/cli002.md
+scrum/stories/cli003.md
+scrum/stories/cli004.md
+scrum/stories/cli005.md
+scrum/stories/cli006.md
+scrum/stories/cli007.md
+scrum/stories/cli008.md
+scrum/stories/cli009.md
+scrum/stories/cli010.md
+scrum/stories/cli011.md
+scrum/stories/cli012.md
+scrum/stories/cli013.md
+scrum/stories/cli014.md
+scrum/stories/cli015.md
+scrum/stories/cli016.md
+scrum/stories/cli017.md
+scrum/stories/cli018.md
+scrum/stories/cli020.md
+scrum/stories/cli022.md
+scrum/stories/cli023.md
+scrum/stories/cli024.md
+scrum/stories/cli025.md
+scrum/stories/cli027.md
+scrum/stories/cli028.md
+scrum/stories/cli029.md
+scrum/stories/cli032.md
+scrum/stories/cli033.md
+scrum/stories/cli034.md
+scrum/techdebt/cli021.md
+scrum/techdebt/cli030.md
+scrum/techdebt/cli031.md
+scrum/techdebt/td1.md
 scrummd/__init__.py
 scrummd/_version.py
 scrummd/card.py
 scrummd/collection.py
 scrummd/config.py
 scrummd/config_loader.py
 scrummd/const.py
 scrummd/exceptions.py
 scrummd/sbench.py
-scrummd/sbl.py
+scrummd/sboard.py
 scrummd/scard.py
 scrummd/source_md.py
 scrummd/svalid.py
 scrummd/version.py
 scrummd.egg-info/PKG-INFO
 scrummd.egg-info/SOURCES.txt
 scrummd.egg-info/dependency_links.txt
 scrummd.egg-info/entry_points.txt
 scrummd.egg-info/requires.txt
 scrummd.egg-info/top_level.txt
+scrummd/sbl/__init__.py
+scrummd/sbl/board_output.py
+scrummd/sbl/output.py
+scrummd/sbl/sbl.py
+scrummd/sbl/text_output.py
 test/fixtures.py
 test/test_card.py
 test/test_collection.py
 test/test_config_loader.py
 test/test_in_anger.py
 test/test_sbl.py
 test/test_scard.py
 test/test_source_md.py
 test/test_svalid.py
+test/data/.scrum.toml
 test/data/collection3.md
 test/data/md1.md
 test/data/md2.md
+test/data/sort_collection.md
 test/data/collection1/c1.md
 test/data/collection1/c2.md
 test/data/collection1/c3.md
 test/data/collection1/embedded/e1.md
 test/data/collection2/c4.md
 test/data/collection2/c5.md
 test/data/collection2/c6.md
 test/data/collection2/.ignorethis/i1.md
 test/data/collection2/.ignorethis/collection/i2.md
 test/data/collection4/c7.md
-test/fail_cases/collection_rule_violation/bad_status.md
-test/fail_cases/invalid/no_summary.md
-test/fail_cases/rule_violation/bad_status.md
+test/special_cases/collection_rule_violation/bad_status.md
+test/special_cases/header_summary/md3.md
+test/special_cases/invalid/no_summary.md
+test/special_cases/rule_violation/bad_status.md
```

### Comparing `scrummd-0.0.8/test/fixtures.py` & `scrummd-0.1.0/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.8/test/test_collection.py` & `scrummd-0.1.0/test/test_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import os
 import pytest
 from pathlib import Path
 
 from scrummd.config import ScrumConfig
 from scrummd.collection import (
     Filter,
+    SortCriteria,
     get_collection,
     group_collection,
     filter_collection,
+    sort_collection,
 )
 from fixtures import data_config
 from scrummd.exceptions import RuleViolationError
 
 
 # NOTE: These almost all retrieve the same set of data. We might want to think
 # about ways we can restructure this to see more useful fail cases if something
@@ -99,63 +101,84 @@
     assert test_collection["e1"].path == "test/data/collection1/embedded/e1.md"
 
 
 def test_group_collection_defined_fields(data_config):
     """Test that grouping when a field is defined by config returns correct groups"""
     test_collection = get_collection(data_config, "collection1")
     grouped = group_collection(data_config, test_collection, ["status"])
-    assert set((card.index for card in grouped["ready"])) == set(["c1", "c2", "e1"])
-    assert set((card.index for card in grouped["done"])) == set(["c3"])
+    assert set((card.index for card in grouped["ready"].collection.values())) == set(
+        ["c1", "c2", "e1"]
+    )
+    assert set((card.index for card in grouped["done"].collection.values())) == set(
+        ["c3"]
+    )
 
 
 def test_group_collection_undefined_fields(data_config):
     """Test that grouping when a field is defined by config returns correct groups"""
     test_collection = get_collection(data_config, "collection1")
     grouped = group_collection(data_config, test_collection, ["assignee"])
-    assert set((card.index for card in grouped["bob"])) == set(["c1", "c3"])
-    assert set((card.index for card in grouped["mary"])) == set(["c2"])
+    assert set((card.index for card in grouped["bob"].collection.values())) == set(
+        ["c1", "c3"]
+    )
+    assert set((card.index for card in grouped["mary"].collection.values())) == set(
+        ["c2"]
+    )
 
 
 def test_multiple_groupbys(data_config):
     """Test that grouping when there are two fields is correct"""
     test_collection = get_collection(data_config, "collection1")
     grouped = group_collection(data_config, test_collection, ["status", "assignee"])
-    assert set((card.index for card in grouped["ready"]["bob"])) == set(["c1"])
-    assert set((card.index for card in grouped["ready"]["mary"])) == set(["c2"])
-    assert set((card.index for card in grouped["done"]["bob"])) == set(["c3"])
+    assert set(
+        (card.index for card in grouped["ready"].groups["bob"].collection.values())
+    ) == set(["c1"])
+    assert set(
+        (card.index for card in grouped["ready"].groups["mary"].collection.values())
+    ) == set(["c2"])
+    assert set(
+        (card.index for card in grouped["done"].groups["bob"].collection.values())
+    ) == set(["c3"])
 
 
 def test_collection_with_rules(data_config):
     """Test that a card with valid collection-level rules is added"""
     collection4 = get_collection(data_config, "collection4").values()
     assert set((card.index for card in collection4)) == set(["c7"])
 
 
 def test_collection_with_invalid_collection_rules(data_config):
     """Test that a card violating collection rules raises an error"""
     config = copy(data_config)
-    config.scrum_path = "test/fail_cases/collection_rule_violation"
+    config.scrum_path = "test/special_cases/collection_rule_violation"
     with pytest.raises(RuleViolationError):
         get_collection(config, "collection4")
 
 
 def test_path_correctly_set(data_config):
     """Test that the path for a card is as expected"""
     test_collection = get_collection(data_config, "collection1")
     assert Path(test_collection["c1"].path) == Path("test/data/collection1/c1.md")
     assert Path(test_collection["e1"].path) == Path(
         "test/data/collection1/embedded/e1.md"
     )
 
 
+def test_get_collection_maintains_listed_order(data_config):
+    """Test that where a collection is formed from references in a file, that
+    the order of the cards is maintained when that collection is 'got'"""
+    test_collection = get_collection(data_config, "sort_collection")
+    assert list(test_collection.keys()) == ["c6", "c2", "c3", "c4", "c5", "c1"]
+
+
 @pytest.mark.parametrize(
     ["filters", "expected_card_ids"],
     [
         [[Filter("assignee", "Bob")], ["c1", "c3"]],
-        [[Filter("assignee", ["Bob", "Mary"])], ["c1", "c2", "c3"]],
+        [[Filter("assignee", ["Bob", "Mary"])], ["c1", "c2", "c3", "c5", "c6"]],
         [[Filter("assignee", "bob")], ["c1", "c3"]],
         [[Filter("assignee", "bob"), Filter("status", "ready")], ["c1"]],
         [[Filter("assignee", " bob"), Filter("status", "ready")], ["c1"]],
     ],
     ids=[
         "1 field",
         "1 field, 2 values",
@@ -165,7 +188,81 @@
     ],
 )
 def test_filtering(data_config, filters, expected_card_ids):
     """Test that filters are correctly applied"""
     test_collection = get_collection(data_config)
     result = filter_collection(test_collection, filters).keys()
     assert set(result) == set(expected_card_ids)
+
+
+@pytest.mark.parametrize(
+    ["field", "expected_card_order"],
+    [["Estimate", ["c6", "c4", "c5"]]],
+    ids=["Sort by number field"],
+)
+def test_sorting(data_config, field, expected_card_order):
+    pass
+
+
+def test_group_sorting(data_config):
+    """Test that groups are in the order specified by sort"""
+    test_collection = get_collection(data_config, "collection1")
+    grouped_collection = group_collection(
+        data_config, test_collection, ["assignee"], [SortCriteria("assignee", False)]
+    )
+    assert list(grouped_collection.keys()) == [None, "aleph", "bob", "mary"]
+
+
+def test_group_reverse_sorting(data_config):
+    """Test that groups are in the order specified by sort when sort is reversed"""
+    test_collection = get_collection(data_config, "collection1")
+    grouped_collection = group_collection(
+        data_config, test_collection, ["assignee"], [SortCriteria("assignee", True)]
+    )
+    assert list(grouped_collection.keys()) == ["mary", "bob", "aleph", None]
+
+
+def test_sorting_collection_with_numbers(data_config):
+    """Test that an ungrouped collection of cards is sorted by criteria including numbers in the values"""
+    # SBL output for the collection:
+    # index, assignee, estimate
+    # c3, Bob,
+    # c2, Mary, 2.5
+    # c1, Bob, 5
+    # e1, Aleph, Unknown
+    test_collection = get_collection(data_config, "collection1")
+    sorted_collection = sort_collection(
+        test_collection, [SortCriteria("estimate", False)]
+    )
+    assert list(sorted_collection.keys()) == ["c3", "c2", "c1", "e1"]
+
+
+def test_sorting_collection_multiple_criteria(data_config):
+    """Test that sorting with multiple sort criteria. without grouping, applies
+    them correctly"""
+    test_collection = get_collection(data_config, "sort_collection")
+    sorted_collection = sort_collection(
+        test_collection,
+        [SortCriteria("assignee", False), SortCriteria("estimate", True)],
+    )
+    # SBL output for the collection:
+    # index, assignee, estimate
+    # c1, Bob, 5
+    # c2, Mary, 2.5
+    # c3, Bob,
+    # c4, Aleph, Unknown
+    # c5, Mary, 1
+    # c6, Mary, Unknown
+    assert list(sorted_collection.keys()) == ["c4", "c1", "c3", "c6", "c2", "c5"]
+
+
+def test_sorting_inside_group(data_config):
+    """Test that the inner parts of groups are sorted correctly"""
+    test_collection = get_collection(data_config, "sort_collection")
+    grouped_sorted_collection = group_collection(
+        data_config, test_collection, ["Assignee"], [SortCriteria("estimate", False)]
+    )
+    assert list(grouped_sorted_collection["mary"].collection.keys()) == [
+        "c5",
+        "c2",
+        "c6",
+    ]
```

### Comparing `scrummd-0.0.8/test/test_config_loader.py` & `scrummd-0.1.0/test/test_config_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,7 +130,27 @@
     """Test that a setting in [tool.scrummd.collections.*.fields] is set"""
     config = load_fs_config()
     assert config.collections["epic"].fields["status"] == [
         "Not Defined",
         "Started",
         "Done",
     ]
+
+
+SBL_CONFIG = """
+[tool.scrummd.sbl]
+columns = ["index"]
+"""
+
+
+@pytest.fixture(scope="function")
+def sbl_config_f(temp_dir):
+    with open(Path(temp_dir, "scrum.toml"), "w") as fo:
+        fo.write(SBL_CONFIG)
+        fo.flush()
+        yield
+
+
+def test_sbl_config(temp_dir, sbl_config_f):
+    """Test that the SBL config field is set from the file"""
+    config = load_fs_config()
+    assert config.sbl.columns == ["index"]
```

### Comparing `scrummd-0.0.8/test/test_in_anger.py` & `scrummd-0.1.0/test/test_in_anger.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 def scrumcli_config() -> ScrumConfig:
     # TODO: Read the actual config
     return ScrumConfig(scrum_path="scrum")
 
 
 def test_get_backlog(scrumcli_config):
     """Gets the backlog from the scrummd project"""
-    backlog = get_collection(scrumcli_config, "backlog")
+    backlog = get_collection(scrumcli_config)
     assert len(backlog) > 0
 
 
 def test_scard(scrumcli_config):
     """Calls scard's output function for each card in the project"""
-    backlog = get_collection(scrumcli_config, "backlog")
+    backlog = get_collection(scrumcli_config)
     for index, _card in backlog.items():
         output_cards(scrumcli_config, backlog, index)
```

### Comparing `scrummd-0.0.8/test/test_sbl.py` & `scrummd-0.1.0/test/test_sbl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from scrummd.collection import Filter
-import scrummd.sbl
+import scrummd.sbl.sbl
 
 
 @pytest.mark.parametrize(
     ["argument_value", "expected_filter"],
     [
         [
             "a=b",
@@ -33,8 +33,8 @@
         [
             "a= b 2, c",
             Filter("a", ["b 2", "c"], mode=Filter.FilterMode.EQUALS),
         ],
     ],
 )
 def test_include_to_filter(argument_value, expected_filter):
-    assert scrummd.sbl.include_to_filter(argument_value) == expected_filter
+    assert scrummd.sbl.sbl.include_to_filter(argument_value) == expected_filter
```

### Comparing `scrummd-0.0.8/test/test_scard.py` & `scrummd-0.1.0/test/test_scard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from copy import copy
 from pathlib import Path
 from scrummd.card import Card, from_str
-from scrummd.scard import output_value, format_card
+from scrummd.scard import format_field, output_fieldstr, format_card_summary
+from scrummd.source_md import Field, FieldNumber, FieldStr
 from fixtures import data_config, test_collection
 import pytest
 
 
 @pytest.fixture(scope="function")
 def test_card(data_config) -> Card:
     test_card = """
@@ -17,43 +18,58 @@
 """
     card = from_str(data_config, test_card, "collection", Path("collection/card.md"))
     return card
 
 
 def test_output_value(data_config, test_card, test_collection):
     config = copy(data_config)
-    config.scard_reference_format = "[$index $assignee $status]"
+    config.scard.reference_format = "[$index $assignee $status]"
     assert (
-        output_value(config, test_card.get_field("key"), test_collection)
+        output_fieldstr(config, test_card.get_field("key"), test_collection)
         == "Field [c1 Bob Ready]"
     )
     assert (
-        output_value(config, test_card.get_field("key 2"), test_collection)
+        output_fieldstr(config, test_card.get_field("key 2"), test_collection)
         == "[c2 Mary ready][c3 Bob Done]"
     )
 
 
 @pytest.fixture()
 def sample_card(data_config):
     return Card(
-        index="i",
-        summary="1",
+        index=FieldStr("i"),
+        summary=FieldStr("1"),
         collections=[],
         defined_collections=[],
-        path="test/i.md",
-        udf={"assignee": "me"},
+        path=FieldStr("test/i.md"),
+        udf={"assignee": FieldStr("me"), "estimate": FieldNumber(5)},
         _config=data_config,
     )
 
 
 @pytest.mark.parametrize(
     ["input_format", "expected"],
     [
         ["$index", "i"],
         ["$index $assignee", "i me"],
         ["[$index] $assignee", "[i] me"],
     ],
 )
 def test_format_card(data_config, sample_card, input_format, expected):
     config = copy(data_config)
-    config.scard_reference_format = input_format
-    assert format_card(config, sample_card) == expected
+    config.scard.reference_format = input_format
+    assert format_card_summary(config, sample_card) == expected
+
+
+@pytest.mark.parametrize(
+    ["input_data", "expected"],
+    [
+        [FieldStr("abc"), "abc"],
+        [FieldNumber(123), "123"],
+        [FieldNumber(123.0), "123"],
+        [FieldNumber(123.1), "123.1"],
+        [["a", "b", "3"], "[a, b, 3]"],
+    ],
+)
+def test_format_field(input_data: Field | list[str], expected: str):
+    """Test that formatting a field produces the expected output"""
+    assert format_field(input_data) == expected
```

### Comparing `scrummd-0.0.8/test/test_svalid.py` & `scrummd-0.1.0/test/test_svalid.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     config = copy(data_config)
     config.scrum_path = "test/data/collection1"
     assert get_exit_code(config) == ExitCode.SUCCESSFUL
 
 
 def test_invalid(data_config):
     config = copy(data_config)
-    config.scrum_path = "test/fail_cases/invalid"
+    config.scrum_path = "test/special_cases/invalid"
     assert get_exit_code(config) == ExitCode.INVALID_FILE
 
 
 def test_rule_violation(data_config):
     config = copy(data_config)
-    config.scrum_path = "test/fail_cases/rule_violation"
+    config.scrum_path = "test/special_cases/rule_violation"
     assert get_exit_code(config) == ExitCode.RULE_VIOLATION
```

