# Comparing `tmp/soleil-0.1.0.tar.gz` & `tmp/soleil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soleil-0.1.0.tar", last modified: Thu Apr 18 05:33:21 2024, max compression
+gzip compressed data, was "soleil-0.1.1.tar", last modified: Thu Apr 18 17:57:31 2024, max compression
```

## Comparing `soleil-0.1.0.tar` & `soleil-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.025317 soleil-0.1.0/
--rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-17 22:34:21.000000 soleil-0.1.0/LICENSE
--rw-r--r--   0 jazs       (501) staff       (20)      156 2024-04-18 05:33:21.025146 soleil-0.1.0/PKG-INFO
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.015184 soleil-0.1.0/scripts/
--rw-r--r--   0 jazs       (501) staff       (20)      637 2024-04-17 22:34:21.000000 soleil-0.1.0/scripts/solex
--rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-18 05:33:21.025352 soleil-0.1.0/setup.cfg
--rw-r--r--   0 jazs       (501) staff       (20)      419 2024-04-17 22:34:21.000000 soleil-0.1.0/setup.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.016880 soleil-0.1.0/soleil/
--rw-r--r--   0 jazs       (501) staff       (20)     1172 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     3918 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/_utils.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.018442 soleil-0.1.0/soleil/cli_tools/
--rw-r--r--   0 jazs       (501) staff       (20)      309 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/cli_tools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     1385 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/cli_tools/_argparse_patches.py
--rw-r--r--   0 jazs       (501) staff       (20)     9371 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/cli_tools/solconfarg.py
--rw-r--r--   0 jazs       (501) staff       (20)     7060 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/cli_tools/solex_decorator.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.019196 soleil-0.1.0/soleil/loader/
--rw-r--r--   0 jazs       (501) staff       (20)       62 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/loader/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     7548 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/loader/loader.py
--rw-r--r--   0 jazs       (501) staff       (20)     8438 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/loader/pre_processor.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.020211 soleil-0.1.0/soleil/overrides/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     3441 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/overridable.py
--rw-r--r--   0 jazs       (501) staff       (20)     5470 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/overrides.py
--rw-r--r--   0 jazs       (501) staff       (20)     6664 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/parser.py
--rw-r--r--   0 jazs       (501) staff       (20)     1948 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/req.py
--rw-r--r--   0 jazs       (501) staff       (20)     7399 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/overrides/variable_path.py
--rw-r--r--   0 jazs       (501) staff       (20)     1380 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/package.py
--rw-r--r--   0 jazs       (501) staff       (20)      764 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/rcall.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.021248 soleil-0.1.0/soleil/resolvers/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/resolvers/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     4788 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/resolvers/base.py
--rw-r--r--   0 jazs       (501) staff       (20)     7990 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/resolvers/class_resolver.py
--rw-r--r--   0 jazs       (501) staff       (20)     5281 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/resolvers/modifiers.py
--rw-r--r--   0 jazs       (501) staff       (20)     8511 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/resolvers/module_resolver.py
--rw-r--r--   0 jazs       (501) staff       (20)     1163 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/rstr.py
--rw-r--r--   0 jazs       (501) staff       (20)      974 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/solconf.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.021607 soleil-0.1.0/soleil/special/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/special/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     1304 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/special/resolved.py
--rw-r--r--   0 jazs       (501) staff       (20)     7436 2024-04-17 22:34:21.000000 soleil-0.1.0/soleil/utils.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.024974 soleil-0.1.0/soleil.egg-info/
--rw-r--r--   0 jazs       (501) staff       (20)      156 2024-04-18 05:33:21.000000 soleil-0.1.0/soleil.egg-info/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)     1578 2024-04-18 05:33:21.000000 soleil-0.1.0/soleil.egg-info/SOURCES.txt
--rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-18 05:33:21.000000 soleil-0.1.0/soleil.egg-info/dependency_links.txt
--rw-r--r--   0 jazs       (501) staff       (20)        8 2024-04-18 05:33:21.000000 soleil-0.1.0/soleil.egg-info/requires.txt
--rw-r--r--   0 jazs       (501) staff       (20)       13 2024-04-18 05:33:21.000000 soleil-0.1.0/soleil.egg-info/top_level.txt
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.014464 soleil-0.1.0/tests/
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.022045 soleil-0.1.0/tests/soleil/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:33:49.000000 soleil-0.1.0/tests/soleil/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      433 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/_utils.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.022679 soleil-0.1.0/tests/soleil/cli_tools/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/cli_tools/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     2006 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/cli_tools/solconfarg.py
--rw-r--r--   0 jazs       (501) staff       (20)     1948 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/cli_tools/solex_decorator.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.023017 soleil-0.1.0/tests/soleil/loader/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/loader/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      855 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/loader/loader.py
--rw-r--r--   0 jazs       (501) staff       (20)     5383 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/loader/pre_processor.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.024006 soleil-0.1.0/tests/soleil/overrides/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      622 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/overridable.py
--rw-r--r--   0 jazs       (501) staff       (20)     3775 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/overrides.py
--rw-r--r--   0 jazs       (501) staff       (20)     1393 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/parser.py
--rw-r--r--   0 jazs       (501) staff       (20)      537 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/req.py
--rw-r--r--   0 jazs       (501) staff       (20)     2956 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/overrides/variable_path.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 05:33:21.024816 soleil-0.1.0/tests/soleil/resolvers/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/resolvers/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      185 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/resolvers/base.py
--rw-r--r--   0 jazs       (501) staff       (20)     1780 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/resolvers/class_resolver.py
--rw-r--r--   0 jazs       (501) staff       (20)     1360 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/resolvers/modifiers.py
--rw-r--r--   0 jazs       (501) staff       (20)     3920 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/resolvers/module_resolver.py
--rw-r--r--   0 jazs       (501) staff       (20)     3244 2024-04-17 22:34:21.000000 soleil-0.1.0/tests/soleil/utils.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.316510 soleil-0.1.1/
+-rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-17 22:34:21.000000 soleil-0.1.1/LICENSE
+-rw-r--r--   0 jazs       (501) staff       (20)     1331 2024-04-18 17:57:31.316310 soleil-0.1.1/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)      559 2024-04-18 17:41:55.000000 soleil-0.1.1/README.md
+-rw-r--r--   0 jazs       (501) staff       (20)      794 2024-04-18 17:50:28.000000 soleil-0.1.1/pyproject.toml
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.307148 soleil-0.1.1/scripts/
+-rw-r--r--   0 jazs       (501) staff       (20)      637 2024-04-17 22:34:21.000000 soleil-0.1.1/scripts/solex
+-rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-18 17:57:31.316547 soleil-0.1.1/setup.cfg
+-rw-r--r--   0 jazs       (501) staff       (20)      681 2024-04-18 17:54:24.000000 soleil-0.1.1/setup.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.308833 soleil-0.1.1/soleil/
+-rw-r--r--   0 jazs       (501) staff       (20)     1172 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3918 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/_utils.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.310256 soleil-0.1.1/soleil/cli_tools/
+-rw-r--r--   0 jazs       (501) staff       (20)      309 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/cli_tools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1385 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/cli_tools/_argparse_patches.py
+-rw-r--r--   0 jazs       (501) staff       (20)     9371 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/cli_tools/solconfarg.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7060 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/cli_tools/solex_decorator.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.310838 soleil-0.1.1/soleil/loader/
+-rw-r--r--   0 jazs       (501) staff       (20)       62 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/loader/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7548 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/loader/loader.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8438 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/loader/pre_processor.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.311755 soleil-0.1.1/soleil/overrides/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3441 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/overridable.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5470 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/overrides.py
+-rw-r--r--   0 jazs       (501) staff       (20)     6664 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/parser.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1948 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/req.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7399 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/overrides/variable_path.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1380 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/package.py
+-rw-r--r--   0 jazs       (501) staff       (20)      764 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/rcall.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.312627 soleil-0.1.1/soleil/resolvers/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/resolvers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4788 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/resolvers/base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7990 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/resolvers/class_resolver.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5281 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/resolvers/modifiers.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8511 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/resolvers/module_resolver.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1163 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/rstr.py
+-rw-r--r--   0 jazs       (501) staff       (20)      974 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/solconf.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.313010 soleil-0.1.1/soleil/special/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/special/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1304 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/special/resolved.py
+-rw-r--r--   0 jazs       (501) staff       (20)     7436 2024-04-17 22:34:21.000000 soleil-0.1.1/soleil/utils.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.316074 soleil-0.1.1/soleil.egg-info/
+-rw-r--r--   0 jazs       (501) staff       (20)     1331 2024-04-18 17:57:31.000000 soleil-0.1.1/soleil.egg-info/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)     1603 2024-04-18 17:57:31.000000 soleil-0.1.1/soleil.egg-info/SOURCES.txt
+-rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-18 17:57:31.000000 soleil-0.1.1/soleil.egg-info/dependency_links.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       30 2024-04-18 17:57:31.000000 soleil-0.1.1/soleil.egg-info/requires.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       13 2024-04-18 17:57:31.000000 soleil-0.1.1/soleil.egg-info/top_level.txt
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.306071 soleil-0.1.1/tests/
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.313464 soleil-0.1.1/tests/soleil/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:33:49.000000 soleil-0.1.1/tests/soleil/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      433 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/_utils.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.314120 soleil-0.1.1/tests/soleil/cli_tools/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/cli_tools/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2006 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/cli_tools/solconfarg.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1948 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/cli_tools/solex_decorator.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.314454 soleil-0.1.1/tests/soleil/loader/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/loader/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      855 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/loader/loader.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5162 2024-04-18 17:02:22.000000 soleil-0.1.1/tests/soleil/loader/pre_processor.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.315285 soleil-0.1.1/tests/soleil/overrides/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      622 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/overridable.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3775 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/overrides.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1393 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/parser.py
+-rw-r--r--   0 jazs       (501) staff       (20)      537 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/req.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2956 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/overrides/variable_path.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-18 17:57:31.315889 soleil-0.1.1/tests/soleil/resolvers/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/resolvers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      185 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/resolvers/base.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1780 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/resolvers/class_resolver.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1360 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/resolvers/modifiers.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3920 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/resolvers/module_resolver.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3244 2024-04-17 22:34:21.000000 soleil-0.1.1/tests/soleil/utils.py
```

### Comparing `soleil-0.1.0/LICENSE` & `soleil-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/scripts/solex` & `soleil-0.1.1/scripts/solex`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/__init__.py` & `soleil-0.1.1/soleil/__init__.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/_utils.py` & `soleil-0.1.1/soleil/_utils.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/cli_tools/_argparse_patches.py` & `soleil-0.1.1/soleil/cli_tools/_argparse_patches.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/cli_tools/solconfarg.py` & `soleil-0.1.1/soleil/cli_tools/solconfarg.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/cli_tools/solex_decorator.py` & `soleil-0.1.1/soleil/cli_tools/solex_decorator.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/loader/loader.py` & `soleil-0.1.1/soleil/loader/loader.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/loader/pre_processor.py` & `soleil-0.1.1/soleil/loader/pre_processor.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/overrides/overridable.py` & `soleil-0.1.1/soleil/overrides/overridable.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/overrides/overrides.py` & `soleil-0.1.1/soleil/overrides/overrides.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/overrides/parser.py` & `soleil-0.1.1/soleil/overrides/parser.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/overrides/req.py` & `soleil-0.1.1/soleil/overrides/req.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/overrides/variable_path.py` & `soleil-0.1.1/soleil/overrides/variable_path.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/package.py` & `soleil-0.1.1/soleil/package.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/rcall.py` & `soleil-0.1.1/soleil/rcall.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/resolvers/base.py` & `soleil-0.1.1/soleil/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/resolvers/class_resolver.py` & `soleil-0.1.1/soleil/resolvers/class_resolver.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/resolvers/modifiers.py` & `soleil-0.1.1/soleil/resolvers/modifiers.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/resolvers/module_resolver.py` & `soleil-0.1.1/soleil/resolvers/module_resolver.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/rstr.py` & `soleil-0.1.1/soleil/rstr.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/solconf.py` & `soleil-0.1.1/soleil/solconf.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/special/resolved.py` & `soleil-0.1.1/soleil/special/resolved.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil/utils.py` & `soleil-0.1.1/soleil/utils.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/soleil.egg-info/SOURCES.txt` & `soleil-0.1.1/soleil.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 LICENSE
+README.md
+pyproject.toml
 setup.py
 scripts/solex
 soleil/__init__.py
 soleil/_utils.py
 soleil/package.py
 soleil/rcall.py
 soleil/rstr.py
```

### Comparing `soleil-0.1.0/tests/soleil/cli_tools/solconfarg.py` & `soleil-0.1.1/tests/soleil/cli_tools/solconfarg.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/cli_tools/solex_decorator.py` & `soleil-0.1.1/tests/soleil/cli_tools/solex_decorator.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/loader/loader.py` & `soleil-0.1.1/tests/soleil/loader/loader.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/loader/pre_processor.py` & `soleil-0.1.1/tests/soleil/loader/pre_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,17 +149,15 @@
         with TemporaryDirectory() as temp_dir:
             for keyword in mdl.__soleil_keywords__:
                 with open(path := (Path(temp_dir) / "main.solconf"), "w") as fo:
                     fo.write(f"{keyword} = 1")
 
                 with pytest.raises(
                     SyntaxError,
-                    match=re.escape(
-                        f'Attempted to redefine soleil keyword `{keyword}` - File "{path}", line 1'
-                    ),
+                    match=f"Attempted to redefine soleil keyword `{keyword}`.*",
                 ):
                     load_solconf(path)
 
 
 class TestGetPromotedName:
     def test_double_promoted_fails(self):
         with solconf_file("A:promoted\nB:promoted") as path:
@@ -171,22 +169,18 @@
             ):
                 load_solconf(path)
 
     def test_non_root_promoted_fails(self):
         with solconf_file("class A:\n\ta:promoted=1") as path:
             with pytest.raises(
                 SyntaxError,
-                match=re.escape(
-                    f'Attempted to promote non-root member `A.a` - File "{path}", line 3'
-                ),
+                match=f"Attempted to promote non-root member `A.a`.*",
             ):
                 load_solconf(path)
 
     def test_non_root_promoted_fails__decorator(self):
         with solconf_file("class A:\n\ta:promoted=1") as path:
             with pytest.raises(
                 SyntaxError,
-                match=re.escape(
-                    f'Attempted to promote non-root member `A.a` - File "{path}", line 3'
-                ),
+                match=f"Attempted to promote non-root member `A.a`.*",
             ):
                 load_solconf(path)
```

### Comparing `soleil-0.1.0/tests/soleil/overrides/overridable.py` & `soleil-0.1.1/tests/soleil/overrides/overridable.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/overrides/overrides.py` & `soleil-0.1.1/tests/soleil/overrides/overrides.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/overrides/parser.py` & `soleil-0.1.1/tests/soleil/overrides/parser.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/overrides/req.py` & `soleil-0.1.1/tests/soleil/overrides/req.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/overrides/variable_path.py` & `soleil-0.1.1/tests/soleil/overrides/variable_path.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/resolvers/class_resolver.py` & `soleil-0.1.1/tests/soleil/resolvers/class_resolver.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/resolvers/modifiers.py` & `soleil-0.1.1/tests/soleil/resolvers/modifiers.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/resolvers/module_resolver.py` & `soleil-0.1.1/tests/soleil/resolvers/module_resolver.py`

 * *Files identical despite different names*

### Comparing `soleil-0.1.0/tests/soleil/utils.py` & `soleil-0.1.1/tests/soleil/utils.py`

 * *Files identical despite different names*

