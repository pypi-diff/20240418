# Comparing `tmp/calitp-littlepay-2024.3.3.tar.gz` & `tmp/calitp_littlepay-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp-littlepay-2024.3.3.tar", last modified: Fri Mar 22 18:07:42 2024, max compression
+gzip compressed data, was "calitp_littlepay-2024.4.1.tar", last modified: Thu Apr 18 18:57:11 2024, max compression
```

## Comparing `calitp-littlepay-2024.3.3.tar` & `calitp_littlepay-2024.4.1.tar`

### file list

```diff
@@ -1,73 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.456020 calitp-littlepay-2024.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/.config/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.config/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.devcontainer/postAttach.sh
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-03-22 18:07:42.456020 calitp-littlepay-2024.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/bin/coverage.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/bin/web.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.456020 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 18:07:42.000000 calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/data/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.448020 calitp-littlepay-2024.3.3/littlepay/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.452020 calitp-littlepay-2024.3.3/littlepay/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/card_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/funding_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/api/products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.452020 calitp-littlepay-2024.3.3/littlepay/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/commands/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/commands/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/littlepay/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:07:42.456020 calitp-littlepay-2024.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.452020 calitp-littlepay-2024.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.452020 calitp-littlepay-2024.3.3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/test_card_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/test_funding_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/api/test_products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:42.456020 calitp-littlepay-2024.3.3/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/commands/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/commands/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/commands/test_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/commands/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/test_littlepay.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-03-22 18:07:34.000000 calitp-littlepay-2024.3.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21254 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21254 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 18:57:11.000000 calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.424705 calitp_littlepay-2024.4.1/littlepay/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.424705 calitp_littlepay-2024.4.1/littlepay/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/card_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/funding_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/api/products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.424705 calitp_littlepay-2024.4.1/littlepay/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/commands/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/commands/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/littlepay/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.424705 calitp_littlepay-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/test_card_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/test_funding_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/api/test_products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:11.428705 calitp_littlepay-2024.4.1/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/commands/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/commands/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/commands/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/commands/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/test_littlepay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-18 18:57:04.000000 calitp_littlepay-2024.4.1/tests/test_main.py
```

### Comparing `calitp-littlepay-2024.3.3/LICENSE` & `calitp_littlepay-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/PKG-INFO` & `calitp_littlepay-2024.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-littlepay
-Version: 2024.3.3
+Version: 2024.4.1
 Summary: Cal-ITP API implementations and admin tasks for Littlepay.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -337,20 +337,22 @@
 littlepay switch participant <participant_id>
 ```
 
 ## Work with groups
 
 ```console
 $ littlepay groups -h
-usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,link,products,remove,unlink} ...
+usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,funding_sources,link,migrate,products,remove,unlink} ...
 
 positional arguments:
-  {create,link,products,remove,unlink}
+  {create,funding_sources,link,migrate,products,remove,unlink}
     create              Create a new concession group
+    funding_sources     List funding sources for one or more concession groups
     link                Link one or more concession groups to a product
+    migrate             Migrate a group from the old Customer Group format to the current format
     products            List products for one or more concession groups
     remove              Remove an existing concession group
     unlink              Unlink a product from one or more concession groups
 
 options:
   -h, --help            show this help message and exit
   -f GROUP_TERMS, --filter GROUP_TERMS
```

### Comparing `calitp-littlepay-2024.3.3/README.md` & `calitp_littlepay-2024.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -110,20 +110,22 @@
 littlepay switch participant <participant_id>
 ```
 
 ## Work with groups
 
 ```console
 $ littlepay groups -h
-usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,link,products,remove,unlink} ...
+usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,funding_sources,link,migrate,products,remove,unlink} ...
 
 positional arguments:
-  {create,link,products,remove,unlink}
+  {create,funding_sources,link,migrate,products,remove,unlink}
     create              Create a new concession group
+    funding_sources     List funding sources for one or more concession groups
     link                Link one or more concession groups to a product
+    migrate             Migrate a group from the old Customer Group format to the current format
     products            List products for one or more concession groups
     remove              Remove an existing concession group
     unlink              Unlink a product from one or more concession groups
 
 options:
   -h, --help            show this help message and exit
   -f GROUP_TERMS, --filter GROUP_TERMS
```

### Comparing `calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/PKG-INFO` & `calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-littlepay
-Version: 2024.3.3
+Version: 2024.4.1
 Summary: Cal-ITP API implementations and admin tasks for Littlepay.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -337,20 +337,22 @@
 littlepay switch participant <participant_id>
 ```
 
 ## Work with groups
 
 ```console
 $ littlepay groups -h
-usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,link,products,remove,unlink} ...
+usage: littlepay groups [-h] [-f GROUP_TERMS] [--csv] {create,funding_sources,link,migrate,products,remove,unlink} ...
 
 positional arguments:
-  {create,link,products,remove,unlink}
+  {create,funding_sources,link,migrate,products,remove,unlink}
     create              Create a new concession group
+    funding_sources     List funding sources for one or more concession groups
     link                Link one or more concession groups to a product
+    migrate             Migrate a group from the old Customer Group format to the current format
     products            List products for one or more concession groups
     remove              Remove an existing concession group
     unlink              Unlink a product from one or more concession groups
 
 options:
   -h, --help            show this help message and exit
   -f GROUP_TERMS, --filter GROUP_TERMS
```

### Comparing `calitp-littlepay-2024.3.3/calitp_littlepay.egg-info/SOURCES.txt` & `calitp_littlepay-2024.4.1/calitp_littlepay.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,17 @@
-.flake8
-.gitignore
-.pre-commit-config.yaml
 LICENSE
+MANIFEST.in
 README.md
-compose.yaml
 pyproject.toml
-.config/README.md
-.devcontainer/Dockerfile
-.devcontainer/devcontainer.json
-.devcontainer/postAttach.sh
-.github/CODEOWNERS
-.github/dependabot.yml
-.github/workflows/pytest.yml
-.github/workflows/release.yml
-.github/workflows/scrape.yml
-.vscode/settings.json
-bin/coverage.sh
-bin/web.sh
 calitp_littlepay.egg-info/PKG-INFO
 calitp_littlepay.egg-info/SOURCES.txt
 calitp_littlepay.egg-info/dependency_links.txt
 calitp_littlepay.egg-info/entry_points.txt
 calitp_littlepay.egg-info/requires.txt
 calitp_littlepay.egg-info/top_level.txt
-data/README.md
 littlepay/__init__.py
 littlepay/config.py
 littlepay/main.py
 littlepay/api/__init__.py
 littlepay/api/card_tokenization.py
 littlepay/api/client.py
 littlepay/api/funding_sources.py
```

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/__init__.py` & `calitp_littlepay-2024.4.1/littlepay/api/__init__.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/card_tokenization.py` & `calitp_littlepay-2024.4.1/littlepay/api/card_tokenization.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/client.py` & `calitp_littlepay-2024.4.1/littlepay/api/client.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/funding_sources.py` & `calitp_littlepay-2024.4.1/littlepay/api/funding_sources.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/groups.py` & `calitp_littlepay-2024.4.1/littlepay/api/groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,73 +24,72 @@
         instance = GroupResponse("", "", "")
         return ",".join(vars(instance).keys())
 
 
 @dataclass
 class GroupFundingSourceResponse:
     id: str
-    participant_id: str
-    concession_expiry: datetime | None = None
-    concession_created_at: datetime | None = None
-    concession_updated_at: datetime | None = None
+    created_date: datetime | None = None
+    updated_date: datetime | None = None
+    expiry_date: datetime | None = None
 
     def __post_init__(self):
         """Parses any date parameters into Python datetime objects.
 
         Includes a workaround for Python 3.10 where datetime.fromisoformat() can only parse the format output
         by datetime.isoformat(), i.e. without a trailing 'Z' offset character and with UTC offset expressed
         as +/-HH:mm
 
         https://docs.python.org/3.11/library/datetime.html#datetime.datetime.fromisoformat
         """
-        if self.concession_expiry:
-            self.concession_expiry = datetime.fromisoformat(self.concession_expiry.replace("Z", "+00:00", 1))
+        if self.created_date:
+            self.created_date = datetime.fromisoformat(self.created_date.replace("Z", "+00:00", 1))
         else:
-            self.concession_expiry = None
-        if self.concession_created_at:
-            self.concession_created_at = datetime.fromisoformat(self.concession_created_at.replace("Z", "+00:00", 1))
+            self.created_date = None
+        if self.updated_date:
+            self.updated_date = datetime.fromisoformat(self.updated_date.replace("Z", "+00:00", 1))
         else:
-            self.concession_created_at = None
-        if self.concession_updated_at:
-            self.concession_updated_at = datetime.fromisoformat(self.concession_updated_at.replace("Z", "+00:00", 1))
+            self.updated_date = None
+        if self.expiry_date:
+            self.expiry_date = datetime.fromisoformat(self.expiry_date.replace("Z", "+00:00", 1))
         else:
-            self.concession_updated_at = None
+            self.expiry_date = None
 
 
 class GroupsMixin(ClientProtocol):
     """Mixin implements APIs for concession groups."""
 
     CONCESSION_GROUPS = "concession_groups"
 
-    def _format_concession_expiry(self, concession_expiry: datetime):
-        """Formats a concession expiry datetime into a string suitable for using in an API request body."""
-        if not isinstance(concession_expiry, datetime):
-            raise TypeError("concession_expiry must be a Python datetime instance")
-        # determine if concession_expiry is an "aware" or "naive" datetime instance
+    def _format_expiry(self, expiry: datetime):
+        """Formats an expiry datetime into a string suitable for using in an API request body."""
+        if not isinstance(expiry, datetime):
+            raise TypeError("expiry must be a Python datetime instance")
+        # determine if expiry is an "aware" or "naive" datetime instance
         # https://docs.python.org/3/library/datetime.html#determining-if-an-object-is-aware-or-naive
-        if concession_expiry.tzinfo is not None and concession_expiry.tzinfo.utcoffset(concession_expiry) is not None:
-            # concession_expiry is an "aware" datetime instance, meaning it has associated time zone information
+        if expiry.tzinfo is not None and expiry.tzinfo.utcoffset(expiry) is not None:
+            # expiry is an "aware" datetime instance, meaning it has associated time zone information
             # ensure this datetime instance is expressed in UTC
-            concession_expiry = concession_expiry.astimezone(timezone.utc)
+            expiry = expiry.astimezone(timezone.utc)
         else:
-            # concession_expiry is a "naive" datetime instance, meaning it has no associated time zone information
+            # expiry is a "naive" datetime instance, meaning it has no associated time zone information
             # assume this datetime instance was provided in UTC
-            concession_expiry = concession_expiry.replace(tzinfo=timezone.utc)
-        # now concession_expiry is an "aware" datetime instance in UTC, format and add to the payload
+            expiry = expiry.replace(tzinfo=timezone.utc)
+        # now expiry is an "aware" datetime instance in UTC, format and add to the payload
         # datetime.isoformat() adds the UTC offset like +00:00
         # so keep everything but the last 6 characters and add the Z offset character
-        return f"{concession_expiry.isoformat(timespec='seconds')[:-6]}Z"
+        return f"{expiry.isoformat(timespec='seconds')[:-6]}Z"
 
     def concession_groups_endpoint(self, group_id: str = None, *parts: str) -> str:
         """Endpoint for concession groups. Optionally provide a group_id for a group-specific endpoint."""
         return self._make_endpoint(self.CONCESSION_GROUPS, group_id, *parts)
 
-    def concession_group_funding_source_endpoint(self, group_id: str) -> str:
+    def concession_group_funding_source_endpoint(self, group_id: str, funding_source_id: str = None) -> str:
         """Endpoint for a concession group's funding sources."""
-        return self.concession_groups_endpoint(group_id, FundingSourcesMixin.FUNDING_SOURCES)
+        return self.concession_groups_endpoint(group_id, FundingSourcesMixin.FUNDING_SOURCES, funding_source_id)
 
     def create_concession_group(self, group_label: str) -> dict:
         """Create a new concession group."""
         endpoint = self.concession_groups_endpoint()
         data = {"label": group_label}
         return self._post(endpoint, data, dict)
 
@@ -101,35 +100,38 @@
             yield GroupResponse(**item)
 
     def remove_concession_group(self, group_id) -> bool:
         """Remove an existing concession group."""
         endpoint = self.concession_groups_endpoint(group_id)
         return self._delete(endpoint)
 
+    def migrate_concession_group(self, group_id) -> dict:
+        """Migrates a group from the old Customer Group format to current format."""
+        endpoint = self.concession_groups_endpoint(group_id, "migrate")
+        return self._post(endpoint, None, dict)
+
     def get_concession_group_linked_funding_sources(self, group_id) -> Generator[GroupFundingSourceResponse, None, None]:
         """Yield GroupFundingSourceResponse objects representing linked funding sources from the concession_groups endpoint."""
         endpoint = self.concession_group_funding_source_endpoint(group_id)
         for item in self._get_list(endpoint):
             yield GroupFundingSourceResponse(**item)
 
-    def link_concession_group_funding_source(
-        self, group_id: str, funding_source_id: str, concession_expiry: datetime = None
-    ) -> dict:
+    def link_concession_group_funding_source(self, group_id: str, funding_source_id: str, expiry: datetime = None) -> dict:
         """Link a funding source to a concession group."""
         endpoint = self.concession_group_funding_source_endpoint(group_id)
         data = {"id": funding_source_id}
 
-        if concession_expiry is not None:
-            data["concession_expiry"] = self._format_concession_expiry(concession_expiry)
+        if expiry is not None:
+            data["expiry"] = self._format_expiry(expiry)
 
         return self._post(endpoint, data, dict)
 
     def update_concession_group_funding_source_expiry(
-        self, group_id: str, funding_source_id: str, concession_expiry: datetime
+        self, group_id: str, funding_source_id: str, expiry: datetime
     ) -> GroupFundingSourceResponse:
         """Update the expiry of a funding source already linked to a concession group."""
-        endpoint = self.concession_group_funding_source_endpoint(group_id)
-        data = {"id": funding_source_id, "concession_expiry": self._format_concession_expiry(concession_expiry)}
+        endpoint = self.concession_group_funding_source_endpoint(group_id, funding_source_id)
+        data = {"expiry": self._format_expiry(expiry)}
 
         response = self._put(endpoint, data, ListResponse)
 
         return GroupFundingSourceResponse(**response.list[0])
```

### Comparing `calitp-littlepay-2024.3.3/littlepay/api/products.py` & `calitp_littlepay-2024.4.1/littlepay/api/products.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/commands/configure.py` & `calitp_littlepay-2024.4.1/littlepay/commands/configure.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/commands/groups.py` & `calitp_littlepay-2024.4.1/littlepay/commands/groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,22 +33,26 @@
     if hasattr(args, "group_terms") and args.group_terms is not None:
         terms = [t.lower() for t in args.group_terms if t]
         groups = filter(
             lambda g: any([term in g.id.lower() or term in g.label.lower() for term in terms]),
             groups,
         )
 
+    groups = list(groups)
+
     if command == "link":
         for group in groups:
             return_code += link_product(client, group.id, args.product_id)
     elif command == "unlink":
         for group in groups:
             return_code += unlink_product(client, group.id, args.product_id)
+    elif command == "migrate":
+        for group in groups:
+            return_code += migrate_group(client, group.id, getattr(args, "force", False))
 
-    groups = list(groups)
     if csv_output and command != "products":
         print(GroupResponse.csv_header())
     elif csv_output and command == "products":
         # print a custom CSV header for group<>product associations
         print("group_id,product_id,participant_id")
     else:
         print_active_message(config, f"👥 Matching groups ({len(groups)})")
@@ -61,14 +65,16 @@
             if not csv_output:
                 print(f"  🛒 Linked products ({len(products)})")
             for product in products:
                 if csv_output:
                     print(f"{group.id},{product.id},{group.participant_id}")
                 else:
                     print(" ", product)
+        elif command == "funding_sources":
+            return_code += funding_sources(client, group.id)
         elif csv_output:
             print(group.csv())
 
     return RESULT_SUCCESS if return_code == RESULT_SUCCESS else RESULT_FAILURE
 
 
 def create_group(client: Client, group_label: str) -> int:
@@ -137,7 +143,50 @@
         client.unlink_concession_group_product(group_id, product_id)
         print("✅ Unlinked")
     except HTTPError as err:
         print(f"❌ Error: {err}")
         return_code = RESULT_FAILURE
 
     return return_code
+
+
+def migrate_group(client: Client, group_id: str, force: bool = False) -> int:
+    config = Config()
+    print_active_message(config, "Migrating group", f"[{group_id}]")
+    return_code = RESULT_SUCCESS
+
+    if force is True:
+        confirm = "yes"
+    else:
+        try:
+            confirm = input("❔ Are you sure? (yes/no): ")
+        except EOFError:
+            confirm = "no"
+
+    if confirm.lower().startswith("y"):
+        print("Migrating group...")
+        try:
+            client.migrate_concession_group(group_id)
+            print("✅ Migrated")
+        except HTTPError as err:
+            print(f"❌ Error: {err}")
+            return_code = RESULT_FAILURE
+    else:
+        print("Canceled...")
+
+    return return_code
+
+
+def funding_sources(client: Client, group_id: str) -> int:
+    return_code = RESULT_SUCCESS
+
+    try:
+        funding_sources = client.get_concession_group_linked_funding_sources(group_id)
+        funding_sources = list(funding_sources)
+        print(f"  💵 Linked funding sources ({len(funding_sources)})")
+        for funding_source in funding_sources:
+            print(" ", funding_source)
+    except HTTPError as err:
+        print(f"❌ Error: {err}")
+        return_code = RESULT_FAILURE
+
+    return return_code
```

### Comparing `calitp-littlepay-2024.3.3/littlepay/commands/products.py` & `calitp_littlepay-2024.4.1/littlepay/commands/products.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/config.py` & `calitp_littlepay-2024.4.1/littlepay/config.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/littlepay/main.py` & `calitp_littlepay-2024.4.1/littlepay/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,26 @@
     )
 
     groups_commands = groups_parser.add_subparsers(dest="group_command", required=False)
 
     groups_create = _subcmd(groups_commands, "create", help="Create a new concession group")
     groups_create.add_argument("group_label", help="A unique label associated with the concession group", metavar="LABEL")
 
+    _subcmd(groups_commands, "funding_sources", help="List funding sources for one or more concession groups")
+
     groups_link = _subcmd(groups_commands, "link", help="Link one or more concession groups to a product")
     groups_link.add_argument("product_id", help="The ID of the product to link to")
 
+    groups_migrate = _subcmd(
+        groups_commands, "migrate", help="Migrate a group from the old Customer Group format to the current format"
+    )
+    groups_migrate.add_argument(
+        "--force", action="store_true", default=False, help="Don't ask for confirmation before migration"
+    )
+
     groups_products = _subcmd(groups_commands, "products", help="List products for one or more concession groups")
     groups_products.add_argument(
         "--csv", action="store_true", default=False, help="Output results in simple CSV format", dest="csv"
     )
 
     groups_remove = _subcmd(groups_commands, "remove", help="Remove an existing concession group")
     groups_remove.add_argument("--force", action="store_true", default=False, help="Don't ask for confirmation before removal")
```

### Comparing `calitp-littlepay-2024.3.3/pyproject.toml` & `calitp_littlepay-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/api/test_card_tokenization.py` & `calitp_littlepay-2024.4.1/tests/api/test_card_tokenization.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/api/test_client.py` & `calitp_littlepay-2024.4.1/tests/api/test_client.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/api/test_funding_sources.py` & `calitp_littlepay-2024.4.1/tests/api/test_funding_sources.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/api/test_groups.py` & `calitp_littlepay-2024.4.1/tests/api/test_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,25 @@
 
 
 @pytest.fixture
 def ListResponse_GroupFundingSources(expected_expiry_str):
     items = [
         dict(
             id="0",
-            participant_id="zero_0",
-            concession_expiry=expected_expiry_str,
-            concession_created_at=expected_expiry_str,
-            concession_updated_at=expected_expiry_str,
+            expiry_date=expected_expiry_str,
+            created_date=expected_expiry_str,
+            updated_date=expected_expiry_str,
         ),
         dict(
             id="1",
-            participant_id="one_1",
-            concession_expiry=expected_expiry_str,
-            concession_created_at=expected_expiry_str,
-            concession_updated_at=expected_expiry_str,
+            expiry_date=expected_expiry_str,
+            created_date=expected_expiry_str,
+            updated_date=expected_expiry_str,
         ),
-        dict(id="2", participant_id="two_2", concession_expiry="", concession_created_at=""),
+        dict(id="2", expiry_date="", created_date=""),
     ]
     return ListResponse(list=items, total_count=3)
 
 
 @pytest.fixture
 def mock_ClientProtocol_get_list_Groups(mocker):
     items = [
@@ -54,14 +52,20 @@
     return mocker.patch(
         "littlepay.api.ClientProtocol._get_list",
         side_effect=lambda *args, **kwargs: (g for g in ListResponse_GroupFundingSources.list),
     )
 
 
 @pytest.fixture
+def mock_ClientProtocol_post_migrate_concession_group(mocker):
+    response = {"status_code": 204}
+    return mocker.patch("littlepay.api.ClientProtocol._post", side_effect=lambda *args, **kwargs: response)
+
+
+@pytest.fixture
 def mock_ClientProtocol_post_create_concession_group(mocker):
     response = dict(id="0", participant_id="zero_0")
     return mocker.patch("littlepay.api.ClientProtocol._post", side_effect=lambda *args, **kwargs: response)
 
 
 @pytest.fixture
 def mock_ClientProtocol_post_link_concession_group_funding_source(mocker):
@@ -85,46 +89,41 @@
 
 
 def test_GroupResponse_csv_header():
     assert GroupResponse.csv_header() == "id,label,participant_id"
 
 
 def test_GroupFundingSourceResponse_no_dates():
-    response = GroupFundingSourceResponse("id", "participant_id")
+    response = GroupFundingSourceResponse("id")
 
     assert response.id == "id"
-    assert response.participant_id == "participant_id"
-    assert response.concession_expiry is None
-    assert response.concession_created_at is None
-    assert response.concession_updated_at is None
+    assert response.expiry_date is None
+    assert response.created_date is None
+    assert response.updated_date is None
 
 
 def test_GroupFundingSourceResponse_empty_dates():
-    response = GroupFundingSourceResponse("id", "participant_id", "", "", "")
+    response = GroupFundingSourceResponse("id", "", "", "")
 
     assert response.id == "id"
-    assert response.participant_id == "participant_id"
-    assert response.concession_expiry is None
-    assert response.concession_created_at is None
-    assert response.concession_updated_at is None
+    assert response.expiry_date is None
+    assert response.created_date is None
+    assert response.updated_date is None
 
 
 def test_GroupFundingSourceResponse_with_dates(expected_expiry, expected_expiry_str):
-    response = GroupFundingSourceResponse(
-        "id", "participant_id", expected_expiry_str, expected_expiry_str, expected_expiry_str
-    )
+    response = GroupFundingSourceResponse("id", expected_expiry_str, expected_expiry_str, expected_expiry_str)
 
     assert response.id == "id"
-    assert response.participant_id == "participant_id"
-    assert response.concession_expiry == expected_expiry
-    assert response.concession_expiry.tzinfo == timezone.utc
-    assert response.concession_created_at == expected_expiry
-    assert response.concession_created_at.tzinfo == timezone.utc
-    assert response.concession_updated_at == expected_expiry
-    assert response.concession_updated_at.tzinfo == timezone.utc
+    assert response.expiry_date == expected_expiry
+    assert response.expiry_date.tzinfo == timezone.utc
+    assert response.created_date == expected_expiry
+    assert response.created_date.tzinfo == timezone.utc
+    assert response.updated_date == expected_expiry
+    assert response.updated_date.tzinfo == timezone.utc
 
 
 def test_GroupsMixin_concession_groups_endpoint(url):
     client = GroupsMixin()
 
     assert client.concession_groups_endpoint() == f"{url}/concession_groups"
 
@@ -143,14 +142,22 @@
 
 def test_GroupsMixin_concession_groups_funding_sources_endpoint(url):
     client = GroupsMixin()
 
     assert client.concession_group_funding_source_endpoint("1234") == f"{url}/concession_groups/1234/fundingsources"
 
 
+def test_GroupsMixin_concession_groups_funding_sources_funding_source_id(url):
+    client = GroupsMixin()
+
+    assert (
+        client.concession_group_funding_source_endpoint("1234", "4567") == f"{url}/concession_groups/1234/fundingsources/4567"
+    )
+
+
 def test_GroupsMixin_create_concession_group(mock_ClientProtocol_post_create_concession_group):
     client = GroupsMixin()
 
     result = client.create_concession_group("the-label")
 
     mock_ClientProtocol_post_create_concession_group.assert_called_once_with(
         client.concession_groups_endpoint(), {"label": "the-label"}, dict
@@ -187,14 +194,26 @@
 
     result = client.remove_concession_group("1234")
 
     mock_ClientProtocol_delete.assert_called_once_with(client.concession_groups_endpoint("1234"))
     assert result is True
 
 
+def test_GroupMixin_migrate_concession_group(mock_ClientProtocol_post_migrate_concession_group):
+    client = GroupsMixin()
+
+    result = client.migrate_concession_group("1234")
+
+    mock_ClientProtocol_post_migrate_concession_group.assert_called_once_with(
+        client.concession_groups_endpoint("1234", "migrate"), None, dict
+    )
+    assert isinstance(result, dict)
+    assert result["status_code"] == 204
+
+
 def test_GroupsMixin_get_concession_group_linked_funding_sources(
     ListResponse_GroupFundingSources, mock_ClientProtocol_get_list_FundingSources, expected_expiry, expected_expiry_str
 ):
     client = GroupsMixin()
 
     result = client.get_concession_group_linked_funding_sources("group-1234")
     assert isinstance(result, Generator)
@@ -208,101 +227,100 @@
     expected_list = ListResponse_GroupFundingSources.list
 
     assert len(result_list) == len(expected_list)
     assert all([isinstance(i, GroupFundingSourceResponse) for i in result_list])
 
     for i in range(len(result_list)):
         assert result_list[i].id == expected_list[i]["id"]
-        assert result_list[i].participant_id == expected_list[i]["participant_id"]
 
-        if expected_list[i].get("concession_expiry") == expected_expiry_str:
-            assert result_list[i].concession_expiry == expected_expiry
+        if expected_list[i].get("expiry_date") == expected_expiry_str:
+            assert result_list[i].expiry_date == expected_expiry
         else:
-            assert result_list[i].concession_expiry is None
+            assert result_list[i].expiry_date is None
 
-        if expected_list[i].get("concession_created_at") == expected_expiry_str:
-            assert result_list[i].concession_created_at == expected_expiry
+        if expected_list[i].get("created_date") == expected_expiry_str:
+            assert result_list[i].created_date == expected_expiry
         else:
-            assert result_list[i].concession_created_at is None
+            assert result_list[i].created_date is None
 
-        if expected_list[i].get("concession_updated_at") == expected_expiry_str:
-            assert result_list[i].concession_updated_at == expected_expiry
+        if expected_list[i].get("updated_date") == expected_expiry_str:
+            assert result_list[i].updated_date == expected_expiry
         else:
-            assert result_list[i].concession_updated_at is None
+            assert result_list[i].updated_date is None
 
 
 def test_GroupsMixin_link_concession_group_funding_source(mock_ClientProtocol_post_link_concession_group_funding_source):
     client = GroupsMixin()
     result = client.link_concession_group_funding_source("group-1234", "funding-source-1234")
 
     endpoint = client.concession_group_funding_source_endpoint("group-1234")
     mock_ClientProtocol_post_link_concession_group_funding_source.assert_called_once_with(
         endpoint, {"id": "funding-source-1234"}, dict
     )
     assert result == {"status_code": 201}
 
 
-def test_GroupsMixin_format_concession_expiry_not_datetime(expected_expiry_str):
+def test_GroupsMixin_format_expiry_not_datetime(expected_expiry_str):
     client = GroupsMixin()
-    with pytest.raises(TypeError, match="concession_expiry must be a Python datetime instance"):
-        client._format_concession_expiry(expected_expiry_str)
+    with pytest.raises(TypeError, match="expiry must be a Python datetime instance"):
+        client._format_expiry(expected_expiry_str)
 
 
-def test_GroupsMixin_format_concession_expiry_aware_utc(expected_expiry, expected_expiry_str):
+def test_GroupsMixin_format_expiry_aware_utc(expected_expiry, expected_expiry_str):
     client = GroupsMixin()
-    result = client._format_concession_expiry(expected_expiry)
+    result = client._format_expiry(expected_expiry)
 
     assert result == expected_expiry_str
 
 
-def test_GroupsMixin_format_concession_expiry_aware_not_utc():
+def test_GroupsMixin_format_expiry_aware_not_utc():
     # construct a datetime in UTC-7 and the expected string formatting
-    concession_expiry = datetime(2024, 3, 18, 1, 2, 3, tzinfo=timezone(timedelta(hours=-7)))
+    expiry = datetime(2024, 3, 18, 1, 2, 3, tzinfo=timezone(timedelta(hours=-7)))
     expected_body_expiry = "2024-03-18T08:02:03Z"
 
     client = GroupsMixin()
-    result = client._format_concession_expiry(concession_expiry)
+    result = client._format_expiry(expiry)
 
     assert result == expected_body_expiry
 
 
-def test_GroupsMixin_format_concession_expiry_naive():
+def test_GroupsMixin_format_expiry_naive():
     # construct a naive datetime and the expected string formatting
-    concession_expiry = datetime(2024, 3, 18, 1, 2, 3, tzinfo=None)
+    expiry = datetime(2024, 3, 18, 1, 2, 3, tzinfo=None)
     expected_body_expiry = "2024-03-18T01:02:03Z"
 
     client = GroupsMixin()
-    result = client._format_concession_expiry(concession_expiry)
+    result = client._format_expiry(expiry)
 
     assert result == expected_body_expiry
 
 
 def test_GroupsMixin_link_concession_group_funding_source_expiry(
     mock_ClientProtocol_post_link_concession_group_funding_source, mocker
 ):
     client = GroupsMixin()
-    mocker.patch.object(client, "_format_concession_expiry", return_value="formatted concession expiry")
+    mocker.patch.object(client, "_format_expiry", return_value="formatted expiry")
 
     result = client.link_concession_group_funding_source("group-1234", "funding-source-1234", datetime.now())
 
     endpoint = client.concession_group_funding_source_endpoint("group-1234")
     mock_ClientProtocol_post_link_concession_group_funding_source.assert_called_once_with(
-        endpoint, {"id": "funding-source-1234", "concession_expiry": "formatted concession expiry"}, dict
+        endpoint, {"id": "funding-source-1234", "expiry": "formatted expiry"}, dict
     )
     assert result == {"status_code": 201}
 
 
 def test_GroupsMixin_update_concession_group_funding_source_expiry(
     mock_ClientProtocol_put_update_concession_group_funding_source, ListResponse_GroupFundingSources, mocker
 ):
     client = GroupsMixin()
-    mocker.patch.object(client, "_format_concession_expiry", return_value="formatted concession expiry")
+    mocker.patch.object(client, "_format_expiry", return_value="formatted expiry")
 
     result = client.update_concession_group_funding_source_expiry("group-1234", "funding-source-1234", datetime.now())
 
-    endpoint = client.concession_group_funding_source_endpoint("group-1234")
+    endpoint = client.concession_group_funding_source_endpoint("group-1234", "funding-source-1234")
     mock_ClientProtocol_put_update_concession_group_funding_source.assert_called_once_with(
-        endpoint, {"id": "funding-source-1234", "concession_expiry": "formatted concession expiry"}, ListResponse
+        endpoint, {"expiry": "formatted expiry"}, ListResponse
     )
 
     expected = GroupFundingSourceResponse(**ListResponse_GroupFundingSources.list[0])
     assert result == expected
```

### Comparing `calitp-littlepay-2024.3.3/tests/api/test_products.py` & `calitp_littlepay-2024.4.1/tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/commands/test_configure.py` & `calitp_littlepay-2024.4.1/tests/commands/test_configure.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/commands/test_groups.py` & `calitp_littlepay-2024.4.1/tests/commands/test_groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from argparse import Namespace
 
 import pytest
 from requests import HTTPError
 
-from littlepay.api.groups import GroupResponse
+from littlepay.api.groups import GroupResponse, GroupFundingSourceResponse
 from littlepay.commands import RESULT_FAILURE, RESULT_SUCCESS
 from littlepay.commands.groups import groups
 
 from tests.commands.test_products import PRODUCT_RESPONSES
 
 GROUP_RESPONSES = [
     GroupResponse("id0", "zero", "participant123"),
     GroupResponse("id1", "one", "participant123"),
     GroupResponse("id2", "two", "participant123"),
 ]
 
+GROUP_FUND_RESPONSES = [
+    GroupFundingSourceResponse("group_funding_id0", "2024-04-01T00:05:23Z", "2024-04-02T00:05:23Z", "2024-04-03T00:05:23Z"),
+    GroupFundingSourceResponse("group_funding_id1", "2024-04-04T00:05:23Z", "2024-04-05T00:05:23Z", "2024-04-06T00:05:23Z"),
+    GroupFundingSourceResponse("group_funding_id2", "2024-04-07T00:05:23Z", "2024-04-08T00:05:23Z", "2024-04-09T00:05:23Z"),
+]
+
 
 @pytest.fixture(autouse=True)
 def mock_config(mocker):
     mocker.patch("littlepay.commands.groups.Config")
 
 
 @pytest.fixture
@@ -34,15 +40,16 @@
         return mocker.patch("littlepay.commands.groups.input", return_value=return_value)
 
     return _input
 
 
 @pytest.fixture(autouse=True)
 def mock_get_groups(mock_client):
-    mock_client.get_concession_groups.return_value = GROUP_RESPONSES
+    # return a generator comprehension to mimic how the real function returns a Generator
+    mock_client.get_concession_groups.return_value = (r for r in GROUP_RESPONSES)
 
 
 def test_groups_default(mock_client, capfd):
     res = groups()
     capture = capfd.readouterr()
 
     assert res == RESULT_SUCCESS
@@ -112,30 +119,54 @@
     capture = capfd.readouterr()
 
     mock_client.create_concession_group.assert_called_once_with("the-label")
 
     assert res == RESULT_SUCCESS
     assert "Creating group" in capture.out
     assert "Created" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__create_HTTPError(mock_client, capfd):
     mock_client.create_concession_group.side_effect = HTTPError
 
     args = Namespace(group_command="create", group_label="the-label")
     res = groups(args)
     capture = capfd.readouterr()
 
     mock_client.create_concession_group.assert_called_once_with("the-label")
 
     assert res == RESULT_FAILURE
     assert "Creating group" in capture.out
     assert "Error" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
+
+
+def test_groups_group_command__funding_sources(mock_client, capfd):
+    mock_client.get_concession_group_linked_funding_sources.return_value = (r for r in GROUP_FUND_RESPONSES)
+
+    args = Namespace(group_command="funding_sources")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    assert res == RESULT_SUCCESS
+    assert "Matching groups (3)" in capture.out
+    assert "  💵 Linked funding sources (3)" in capture.out
+
+
+def test_groups_group_command__funding_sources_HTTPError(mock_client, capfd):
+    mock_client.get_concession_group_linked_funding_sources.side_effect = HTTPError
+
+    args = Namespace(group_command="funding_sources")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    assert res == RESULT_FAILURE
+    assert "Matching groups (3)" in capture.out
+    assert "Error:" in capture.out
 
 
 def test_groups_group_command__link(mock_client, capfd):
     args = Namespace(group_command="link", product_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
@@ -209,90 +240,167 @@
     args = Namespace(group_command="remove", group_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_SUCCESS
     assert "Removing group" in capture.out
     assert "Removed" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__remove_confirm_error(capfd, mock_input):
     _input = mock_input(None)
     _input.side_effect = EOFError
 
     args = Namespace(group_command="remove", group_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_SUCCESS
     assert "Removing group" in capture.out
     assert "Canceled" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 @pytest.mark.parametrize("sample_input", ["n", "N", "no", "No", "NO"])
 def test_groups_group_command__remove_decline(capfd, mock_input, sample_input):
     mock_input(sample_input)
 
     args = Namespace(group_command="remove", group_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_SUCCESS
     assert "Removing group" in capture.out
     assert "Canceled" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__remove_force(capfd, mock_input):
     _input = mock_input("no")
 
     args = Namespace(group_command="remove", group_id="1234", force=True)
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_SUCCESS
     assert _input.called is False
     assert "Removing group" in capture.out
     assert "Removed" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__remove_HTTPError(capfd, mock_client, mock_input):
     mock_client.remove_concession_group.side_effect = HTTPError
     mock_input("y")
 
     args = Namespace(group_command="remove", group_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_FAILURE
     assert "Removing group" in capture.out
     assert "Error" in capture.out
-    assert "Matching groups" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__unlink(mock_client, capfd):
     args = Namespace(group_command="unlink", product_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     for group in GROUP_RESPONSES:
         mock_client.unlink_concession_group_product.assert_any_call(group.id, "1234")
 
     assert res == RESULT_SUCCESS
     assert "Unlinking group <-> product" in capture.out
     assert "Unlinked" in capture.out
+    assert "Matching groups (3)" in capture.out
 
 
 def test_groups_group_command__unlink_HTTPError(mock_client, capfd):
     mock_client.unlink_concession_group_product.side_effect = HTTPError
 
     args = Namespace(group_command="unlink", product_id="1234")
     res = groups(args)
     capture = capfd.readouterr()
 
     assert res == RESULT_FAILURE
     assert "Unlinking group <-> product" in capture.out
     assert "Error" in capture.out
     assert "Unlinked" not in capture.out
+
+
+@pytest.mark.parametrize("sample_input", ["y", "Y", "yes", "Yes", "YES"])
+def test_groups_group_command__migrate_confirm(mock_client, capfd, mock_input, sample_input):
+    mock_input(sample_input)
+
+    args = Namespace(group_command="migrate")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    for group in GROUP_RESPONSES:
+        mock_client.migrate_concession_group.assert_any_call(group.id)
+
+    assert res == RESULT_SUCCESS
+    assert "Migrating group" in capture.out
+    assert "Migrated" in capture.out
+    assert "Matching groups (3)" in capture.out
+
+
+def test_groups_group_command__migrate_confirm_error(capfd, mock_input):
+    _input = mock_input(None)
+    _input.side_effect = EOFError
+
+    args = Namespace(group_command="migrate")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    assert res == RESULT_SUCCESS
+    assert "Migrating group" in capture.out
+    assert "Canceled" in capture.out
+    assert "Matching groups (3)" in capture.out
+
+
+@pytest.mark.parametrize("sample_input", ["n", "N", "no", "No", "NO"])
+def test_groups_group_command__migrate_decline(capfd, mock_input, sample_input):
+    mock_input(sample_input)
+
+    args = Namespace(group_command="migrate")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    assert res == RESULT_SUCCESS
+    assert "Migrating group" in capture.out
+    assert "Canceled" in capture.out
+    assert "Matching groups (3)" in capture.out
+
+
+def test_groups_group_command__migrate_force(mock_client, capfd, mock_input):
+    _input = mock_input("no")
+
+    args = Namespace(group_command="migrate", force=True)
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    for group in GROUP_RESPONSES:
+        mock_client.migrate_concession_group.assert_any_call(group.id)
+
+    assert res == RESULT_SUCCESS
+    assert _input.called is False
+    assert "Migrating group" in capture.out
+    assert "Migrated" in capture.out
+    assert "Matching groups (3)" in capture.out
+
+
+def test_groups_group_command__migrate_HTTPError(mock_client, capfd, mock_input):
+    mock_client.migrate_concession_group.side_effect = HTTPError
+    mock_input("y")
+
+    args = Namespace(group_command="migrate", group_id="1234")
+    res = groups(args)
+    capture = capfd.readouterr()
+
+    assert res == RESULT_FAILURE
+    assert "Migrating group" in capture.out
+    assert "Error" in capture.out
+    assert "Matching groups (3)" in capture.out
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calitp-littlepay-2024.3.3/tests/commands/test_products.py` & `calitp_littlepay-2024.4.1/tests/commands/test_products.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/commands/test_switch.py` & `calitp_littlepay-2024.4.1/tests/commands/test_switch.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/conftest.py` & `calitp_littlepay-2024.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/test_config.py` & `calitp_littlepay-2024.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/test_littlepay.py` & `calitp_littlepay-2024.4.1/tests/test_littlepay.py`

 * *Files identical despite different names*

### Comparing `calitp-littlepay-2024.3.3/tests/test_main.py` & `calitp_littlepay-2024.4.1/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,24 +117,52 @@
     assert result == RESULT_SUCCESS
     mock_commands_groups.assert_called_once()
     call_args = mock_commands_groups.call_args.args[0]
     assert call_args.group_command == "create"
     assert call_args.group_label == "label"
 
 
+def test_main_groups_funding_sources(mock_commands_groups):
+    result = main(argv=["groups", "funding_sources"])
+
+    assert result == RESULT_SUCCESS
+    mock_commands_groups.assert_called_once()
+    call_args = mock_commands_groups.call_args.args[0]
+    assert call_args.group_command == "funding_sources"
+
+
 def test_main_groups_link(mock_commands_groups):
     result = main(argv=["groups", "link", "1234"])
 
     assert result == RESULT_SUCCESS
     mock_commands_groups.assert_called_once()
     call_args = mock_commands_groups.call_args.args[0]
     assert call_args.group_command == "link"
     assert call_args.product_id == "1234"
 
 
+def test_main_groups_migrate(mock_commands_groups):
+    result = main(argv=["groups", "migrate"])
+
+    assert result == RESULT_SUCCESS
+    mock_commands_groups.assert_called_once()
+    call_args = mock_commands_groups.call_args.args[0]
+    assert call_args.group_command == "migrate"
+
+
+def test_main_groups_migrate_force(mock_commands_groups):
+    result = main(argv=["groups", "migrate", "--force"])
+
+    assert result == RESULT_SUCCESS
+    mock_commands_groups.assert_called_once()
+    call_args = mock_commands_groups.call_args.args[0]
+    assert call_args.group_command == "migrate"
+    assert call_args.force is True
+
+
 def test_main_groups_products(mock_commands_groups):
     result = main(argv=["groups", "products"])
 
     assert result == RESULT_SUCCESS
     mock_commands_groups.assert_called_once()
     call_args = mock_commands_groups.call_args.args[0]
     assert call_args.group_command == "products"
```

