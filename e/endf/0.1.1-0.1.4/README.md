# Comparing `tmp/endf-0.1.1.tar.gz` & `tmp/endf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endf-0.1.1.tar", last modified: Tue May 30 21:51:51 2023, max compression
+gzip compressed data, was "endf-0.1.4.tar", last modified: Thu Apr 18 15:53:54 2024, max compression
```

## Comparing `endf-0.1.1.tar` & `endf-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.088273 endf-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-30 21:51:42.000000 endf-0.1.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 21:51:42.000000 endf-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 21:51:42.000000 endf-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 21:51:42.000000 endf-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-30 21:51:51.088273 endf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-30 21:51:42.000000 endf-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 21:51:42.000000 endf-0.1.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 21:51:42.000000 endf-0.1.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/_templates/myclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/doc/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.084273 endf-0.1.1/doc/source/user/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/user/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-30 21:51:42.000000 endf-0.1.1/doc/source/user/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-30 21:51:42.000000 endf-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:51:51.088273 endf-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-30 21:51:42.000000 endf-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.080273 endf-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.088273 endf-0.1.1/src/endf/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/_records.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/ace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/incident_neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf12.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf14.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf15.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf2.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf23.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf26.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf27.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf28.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf34.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf40.py
--rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf7.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/mf9.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-30 21:51:42.000000 endf-0.1.1/src/endf/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:51:51.088273 endf-0.1.1/src/endf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-30 21:51:51.000000 endf-0.1.1/src/endf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-30 21:51:51.000000 endf-0.1.1/src/endf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:51:51.000000 endf-0.1.1/src/endf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 21:51:51.000000 endf-0.1.1/src/endf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 21:51:51.000000 endf-0.1.1/src/endf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.181880 endf-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.169880 endf-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-18 15:53:50.000000 endf-0.1.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-18 15:53:50.000000 endf-0.1.4/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 15:53:50.000000 endf-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 15:53:50.000000 endf-0.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 15:53:50.000000 endf-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-18 15:53:50.000000 endf-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-18 15:53:54.181880 endf-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 15:53:50.000000 endf-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 15:53:50.000000 endf-0.1.4/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-18 15:53:50.000000 endf-0.1.4/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/_templates/myclass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/doc/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/doc/source/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/user/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-18 15:53:50.000000 endf-0.1.4/doc/source/user/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-18 15:53:50.000000 endf-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:53:54.181880 endf-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 15:53:50.000000 endf-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.173880 endf-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.181880 endf-0.1.4/src/endf/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/_records.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/ace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/incident_neutron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf23.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf28.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf33.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf34.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf40.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/mf9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-18 15:53:50.000000 endf-0.1.4/src/endf/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.181880 endf-0.1.4/src/endf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-18 15:53:54.000000 endf-0.1.4/src/endf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 15:53:54.000000 endf-0.1.4/src/endf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:53:54.000000 endf-0.1.4/src/endf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 15:53:54.000000 endf-0.1.4/src/endf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 15:53:54.000000 endf-0.1.4/src/endf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:53:54.181880 endf-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   163248 2024-04-18 15:53:50.000000 endf-0.1.4/tests/n-095_Am_244.endf
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-18 15:53:50.000000 endf-0.1.4/tests/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-18 15:53:50.000000 endf-0.1.4/tests/test_records.py
```

### Comparing `endf-0.1.1/.github/workflows/publish_pypi.yml` & `endf-0.1.4/.github/workflows/publish_pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -7,58 +7,62 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-11]
+        # macos-13 is an intel runner, macos-14 is apple silicon
+        os: [ubuntu-latest, windows-latest, macos-13, macos-14]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # needed for setuptools_scm
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.17
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          path: wheelhouse/*.whl
+          name: cibw-wheels-${{ matrix.os }}
+          path: ./wheelhouse/*.whl
 
   make_sdist:
     name: Make SDist
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # needed for setuptools_scm
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: Install build
         run: python -m pip install build
 
       - name: Build SDist
         run: python -m build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: cibw-sdist
           path: dist/*.tar.gz
 
   upload_all:
     needs: [build_wheels, make_sdist]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: artifact
+          pattern: cibw-*
           path: dist
+          merge-multiple: true
 
       - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `endf-0.1.1/LICENSE` & `endf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/PKG-INFO` & `endf-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endf
-Version: 0.1.1
+Version: 0.1.4
 Summary: Python interface to ENDF-6 files
 Author-email: Paul Romano <paul.k.romano@gmail.com>
 License: Copyright (c) 2023 Paul Romano
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -29,28 +29,36 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: uncertainties
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: pydata_sphinx_theme; extra == "docs"
+Requires-Dist: sphinx_design; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 
 # ENDF Python Interface
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/endf?label=PyPI)](https://pypi.org/project/endf)
 
 `endf` is a Python package for reading and interpreting
 [ENDF-6](https://doi.org/10.2172/1425114) and
 [ACE](https://github.com/NuclearData/ACEFormat) format nuclear data files.
 Compared to other packages that provide functionality for working with ENDF and
 ACE files, this package has numerous advantages:
```

### Comparing `endf-0.1.1/README.md` & `endf-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ENDF Python Interface
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/endf?label=PyPI)](https://pypi.org/project/endf)
 
 `endf` is a Python package for reading and interpreting
 [ENDF-6](https://doi.org/10.2172/1425114) and
 [ACE](https://github.com/NuclearData/ACEFormat) format nuclear data files.
 Compared to other packages that provide functionality for working with ENDF and
 ACE files, this package has numerous advantages:
```

### Comparing `endf-0.1.1/doc/Makefile` & `endf-0.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/make.bat` & `endf-0.1.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/source/conf.py` & `endf-0.1.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/source/index.rst` & `endf-0.1.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/source/reference/index.rst` & `endf-0.1.4/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/source/user/getting_started.rst` & `endf-0.1.4/doc/source/user/getting_started.rst`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/doc/source/user/usage.rst` & `endf-0.1.4/doc/source/user/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,28 @@
     {'ZA': 92235,
     'AWR': 233.0248,
     'QM': -5298000.0,
     'QI': -5298000.0,
     'LR': 0,
     'sigma': <Tabulated1D: 39 points, 1 regions>}
 
+Note that indexing the :class:`~endf.Material` object directly is equivalent to
+indexing the :attr:`~endf.Material.section_data` attribute:
+
+.. code-block:: pycon
+
+    >>> mat[3, 16]
+    {'ZA': 92235,
+    'AWR': 233.0248,
+    'QM': -5298000.0,
+    'QI': -5298000.0,
+    'LR': 0,
+    'sigma': <Tabulated1D: 39 points, 1 regions>}
+
+
 Tabulated1D Objects
 ~~~~~~~~~~~~~~~~~~~
 
 As the above example shows, whenever a TAB1 record is encountered in an ENDF
 file, it is represented as a :class:`~endf.Tabulated1D` object. The raw `x` and
 `y` values can be accessed through the :attr:`~endf.Tabulated1D.x` and
 :attr:`~endf.Tabulated1D.y` attributes. For example, if you wanted to make a
```

### Comparing `endf-0.1.1/pyproject.toml` & `endf-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "uncertainties",
 ]
```

### Comparing `endf-0.1.1/src/endf/_records.cpp` & `endf-0.1.4/src/endf/_records.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 #include <cstdlib>
+#include <cstring> // for strlen
 
 #include <pybind11/pybind11.h>
 
 //! Convert string representation of a floating point number into a double
 //
 //! This function handles converting floating point numbers from an ENDF 11
 //! character field into a double, covering all the corner cases. Floating point
 //! numbers are allowed to contain whitespace (which is ignored). Also, in
 //! exponential notation, it allows the 'e' to be omitted. A field containing
 //! only whitespace is to be interpreted as a zero.
 //
 //! \param buffer character input from an ENDF file
-//! \param n Length of character input
 //! \return Floating point number
 
 double cfloat_endf(const char* buffer)
 {
-  char arr[12]; // 11 characters plus a null terminator
+  char arr[13]; // 11 characters plus e and a null terminator
   int j = 0; // current position in arr
   int found_significand = 0;
   int found_exponent = 0;
 
   // limit n to 11 characters
   int n = std::strlen(buffer);
+  if (n > 11) n = 11;
 
-  int i;
-  for (i = 0; i < n; ++i) {
+  for (int i = 0; i < n; ++i) {
     char c = buffer[i];
 
     // Skip whitespace characters
     if (c == ' ') continue;
-
     if (found_significand) {
       if (!found_exponent) {
         if (c == '+' || c == '-') {
           // In the case that we encounter +/- and we haven't yet encountered
           // e/E, we manually add it
           arr[j++] = 'e';
           found_exponent = 1;
```

### Comparing `endf-0.1.1/src/endf/ace.py` & `endf-0.1.4/src/endf/ace.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/data.py` & `endf-0.1.4/src/endf/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,14 @@
 # Regex for GNDS nuclide names (used in zam function)
 _GNDS_NAME_RE = re.compile(r'([A-Zn][a-z]*)(\d+)((?:_[em]\d+)?)')
 
 
 def gnds_name(Z: int, A: int, m: int = 0) -> str:
     """Return nuclide name using GNDS convention
 
-    .. versionchanged:: 0.14.0
-        Function name changed from ``gnd_name`` to ``gnds_name``
-
     Parameters
     ----------
     Z
         Atomic number
     A
         Mass number
     m
```

### Comparing `endf-0.1.1/src/endf/function.py` & `endf-0.1.4/src/endf/function.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/incident_neutron.py` & `endf-0.1.4/src/endf/incident_neutron.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/material.py` & `endf-0.1.4/src/endf/material.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 All the classes and functions in this module are based on the ENDF-102 report
 titled "ENDF-6 Formats Manual: Data Formats and Procedures for the Evaluated
 Nuclear Data Files". The version from January 2018 can be found at
 https://doi.org/10.2172/1425114.
 
 """
 import io
-from typing import List, Tuple, Any, Union, TextIO
+from typing import List, Tuple, Any, Union, TextIO, Optional
 from warnings import warn
 
 import endf
-from .data import gnds_name
 from .fileutils import PathLike
 from .mf1 import parse_mf1_mt451, parse_mf1_mt452, parse_mf1_mt455, \
     parse_mf1_mt458, parse_mf1_mt460
 from .mf2 import parse_mf2
 from .mf3 import parse_mf3
 from .mf4 import parse_mf4
 from .mf5 import parse_mf5
 from .mf6 import parse_mf6
-from .mf7 import parse_mf7_mt2, parse_mf7_mt4
+from .mf7 import parse_mf7_mt2, parse_mf7_mt4, parse_mf7_mt451
 from .mf8 import parse_mf8, parse_mf8_mt454, parse_mf8_mt457
 from .mf9 import parse_mf9_mf10
 from .mf12 import parse_mf12
 from .mf13 import parse_mf13
 from .mf14 import parse_mf14
 from .mf15 import parse_mf15
 from .mf23 import parse_mf23
@@ -87,14 +86,16 @@
     """ENDF material with multiple files/sections
 
     Parameters
     ----------
     filename_or_obj
         Path to ENDF file to read or an open file positioned at the start of an
         ENDF material
+    encoding
+        Encoding of the ENDF-6 formatted file
 
     Attributes
     ----------
     MAT
         ENDF material number
     sections
         List of (MF, MT) sections
@@ -107,17 +108,17 @@
     """
     # TODO: Remove need to list properties here
     MAT: int
     sections: List[Tuple[int, int]]
     section_text: dict
     section_data: dict
 
-    def __init__(self, filename_or_obj: Union[PathLike, TextIO]):
+    def __init__(self, filename_or_obj: Union[PathLike, TextIO], encoding: Optional[str] = None):
         if isinstance(filename_or_obj, PathLike.__args__):
-            fh = open(str(filename_or_obj), 'r')
+            fh = open(str(filename_or_obj), 'r', encoding=encoding)
             need_to_close = True
         else:
             fh = filename_or_obj
             need_to_close = False
         self.section_text = {}
 
         # Skip TPID record. Evaluators sometimes put in TPID records that are
@@ -187,14 +188,16 @@
                 self.section_data[MF, MT] = parse_mf5(file_obj)
             elif MF == 6:
                 self.section_data[MF, MT] = parse_mf6(file_obj)
             elif MF == 7 and MT == 2:
                 self.section_data[MF, MT] = parse_mf7_mt2(file_obj)
             elif MF == 7 and MT == 4:
                 self.section_data[MF, MT] = parse_mf7_mt4(file_obj)
+            elif MF == 7 and MT == 451:
+                self.section_data[MF, MT] = parse_mf7_mt451(file_obj)
             elif MF == 8 and MT in (454, 459):
                 self.section_data[MF, MT] = parse_mf8_mt454(file_obj)
             elif MF == 8 and MT == 457:
                 self.section_data[MF, MT] = parse_mf8_mt457(file_obj)
             elif MF == 8:
                 self.section_data[MF, MT] = parse_mf8(file_obj)
             elif MF in (9, 10):
@@ -236,21 +239,14 @@
     def __repr__(self) -> str:
         metadata = self.section_data[1, 451]
         name = metadata['ZSYMAM'].replace(' ', '')
         return '<{} for {} {}>'.format(_SUBLIBRARY[metadata['NSUB']], name,
                                        _LIBRARY[metadata['NLIB']])
 
     @property
-    def gnds_name(self) -> str:
-        metadata = self[1, 451]
-        Z, A = divmod(metadata['ZA'], 1000)
-        m = metadata['LISO']
-        return gnds_name(Z, A, m)
-
-    @property
     def sections(self) -> List[Tuple[int, int]]:
         return list(self.section_text.keys())
 
     def interpret(self) -> Any:
         """Get high-level interface class for the ENDF material
 
         Returns
@@ -262,29 +258,31 @@
         NSUB = self.section_data[1, 451]['NSUB']
         if NSUB == 10:
             return endf.IncidentNeutron.from_endf(self)
         else:
             raise NotImplementedError(f"No class implemented for {NSUB=}")
 
 
-def get_materials(filename: PathLike) -> List[Material]:
+def get_materials(filename: PathLike, encoding: Optional[str] = None) -> List[Material]:
     """Return a list of all materials within an ENDF file.
 
     Parameters
     ----------
     filename
         Path to ENDF-6 formatted file
+    encoding
+        Encoding of the ENDF-6 formatted file
 
     Returns
     -------
     A list of ENDF materials
 
     """
     materials = []
-    with open(str(filename), 'r') as fh:
+    with open(str(filename), 'r', encoding=encoding) as fh:
         while True:
             pos = fh.tell()
             line = fh.readline()
             if line[66:70] == '  -1':
                 break
             fh.seek(pos)
             materials.append(Material(fh))
```

### Comparing `endf-0.1.1/src/endf/mf1.py` & `endf-0.1.4/src/endf/mf1.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf12.py` & `endf-0.1.4/src/endf/mf12.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf13.py` & `endf-0.1.4/src/endf/mf13.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf14.py` & `endf-0.1.4/src/endf/mf14.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf15.py` & `endf-0.1.4/src/endf/mf15.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf2.py` & `endf-0.1.4/src/endf/mf2.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf23.py` & `endf-0.1.4/src/endf/mf23.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf26.py` & `endf-0.1.4/src/endf/mf26.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf27.py` & `endf-0.1.4/src/endf/mf27.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf28.py` & `endf-0.1.4/src/endf/mf28.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf3.py` & `endf-0.1.4/src/endf/mf3.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf33.py` & `endf-0.1.4/src/endf/mf33.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf34.py` & `endf-0.1.4/src/endf/mf34.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf4.py` & `endf-0.1.4/src/endf/mf4.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf40.py` & `endf-0.1.4/src/endf/mf40.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf5.py` & `endf-0.1.4/src/endf/mf5.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf6.py` & `endf-0.1.4/src/endf/mf6.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf7.py` & `endf-0.1.4/src/endf/mf7.py`

 * *Files 11% similar despite different names*

```diff
@@ -108,7 +108,43 @@
     data['Teff'] = [Teff]
     for i in range(NS):
         if data['B'][6*(i + 1)] == 0.0:
             _, Teff = get_tab1_record(file_obj)
             data['Teff'].append(Teff)
 
     return data
+
+
+def parse_mf7_mt451(file_obj: TextIO) -> dict:
+    """Parse thermal scattering generalized information file from MF=7, MT=451
+
+    Parameters
+    ----------
+    file_obj
+        File-like object to read from
+
+    Returns
+    -------
+    dict
+        Thermal scattering data
+
+    """
+    # Read basic data from first record
+    ZA, AWR, NA, *_ = get_head_record(file_obj)
+    data = {'ZA': ZA, 'AWR': AWR, 'NA': NA}
+
+    # Read all other parameters from list record
+    data['elements'] = []
+    for _ in range(NA):
+        params, values = get_list_record(file_obj)
+        element = {
+            'NAS': params[2],
+            'NI': params[5],
+            'ZAI': values[::6],
+            'LISI': values[1::6],
+            'AFI': values[2::6],
+            'AWRI': values[3::6],
+            'SFI': values[4::6],
+        }
+        data['elements'].append(element)
+
+    return data
```

### Comparing `endf-0.1.1/src/endf/mf8.py` & `endf-0.1.4/src/endf/mf8.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/mf9.py` & `endf-0.1.4/src/endf/mf9.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/product.py` & `endf-0.1.4/src/endf/product.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/reaction.py` & `endf-0.1.4/src/endf/reaction.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf/records.py` & `endf-0.1.4/src/endf/records.py`

 * *Files identical despite different names*

### Comparing `endf-0.1.1/src/endf.egg-info/PKG-INFO` & `endf-0.1.4/src/endf.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endf
-Version: 0.1.1
+Version: 0.1.4
 Summary: Python interface to ENDF-6 files
 Author-email: Paul Romano <paul.k.romano@gmail.com>
 License: Copyright (c) 2023 Paul Romano
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -29,28 +29,36 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: uncertainties
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: pydata_sphinx_theme; extra == "docs"
+Requires-Dist: sphinx_design; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 
 # ENDF Python Interface
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/endf?label=PyPI)](https://pypi.org/project/endf)
 
 `endf` is a Python package for reading and interpreting
 [ENDF-6](https://doi.org/10.2172/1425114) and
 [ACE](https://github.com/NuclearData/ACEFormat) format nuclear data files.
 Compared to other packages that provide functionality for working with ENDF and
 ACE files, this package has numerous advantages:
```

### Comparing `endf-0.1.1/src/endf.egg-info/SOURCES.txt` & `endf-0.1.4/src/endf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 .readthedocs.yml
+CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 setup.py
 .github/workflows/publish_pypi.yml
+.github/workflows/run_tests.yml
 doc/Makefile
 doc/make.bat
 doc/source/conf.py
 doc/source/index.rst
 doc/source/_templates/myclass.rst
 doc/source/reference/index.rst
 doc/source/user/getting_started.rst
@@ -45,8 +47,11 @@
 src/endf/product.py
 src/endf/reaction.py
 src/endf/records.py
 src/endf.egg-info/PKG-INFO
 src/endf.egg-info/SOURCES.txt
 src/endf.egg-info/dependency_links.txt
 src/endf.egg-info/requires.txt
-src/endf.egg-info/top_level.txt
+src/endf.egg-info/top_level.txt
+tests/n-095_Am_244.endf
+tests/test_material.py
+tests/test_records.py
```

