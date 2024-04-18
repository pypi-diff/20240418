# Comparing `tmp/wmflib-1.2.4.tar.gz` & `tmp/wmflib-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wmflib-1.2.4.tar", last modified: Tue Nov 28 13:18:15 2023, max compression
+gzip compressed data, was "wmflib-1.2.5.tar", last modified: Thu Apr 18 14:50:26 2024, max compression
```

## Comparing `wmflib-1.2.4.tar` & `wmflib-1.2.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:15.043144 wmflib-1.2.4/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.4/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.4/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.4/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.4/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)    14038 2023-11-28 12:08:05.000000 wmflib-1.2.4/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.4/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.4/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-11-28 13:18:15.043669 wmflib-1.2.4/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.4/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.426023 wmflib-1.2.4/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.455081 wmflib-1.2.4/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.484288 wmflib-1.2.4/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/_static/themes_override.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.653921 wmflib-1.2.4/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.4/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.4/doc/source/api/wmflib.actions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.4/doc/source/api/wmflib.config.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.4/doc/source/api/wmflib.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.4/doc/source/api/wmflib.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/api/wmflib.dns.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/api/wmflib.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.4/doc/source/api/wmflib.fileio.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.4/doc/source/api/wmflib.idm.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.4/doc/source/api/wmflib.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.4/doc/source/api/wmflib.irc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.4/doc/source/api/wmflib.phabricator.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.4/doc/source/api/wmflib.prometheus.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.4/doc/source/api/wmflib.requests.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.4/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.4/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.4/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.4/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2023-11-28 13:18:15.058617 wmflib-1.2.4/setup.cfg
--rw-r--r--   0 riccardo   (501) staff       (20)     2491 2023-07-31 13:28:37.000000 wmflib-1.2.4/setup.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1524 2023-11-28 12:08:05.000000 wmflib-1.2.4/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.838662 wmflib-1.2.4/wmflib/
--rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5894 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1796 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      576 2023-11-28 12:08:05.000000 wmflib-1.2.4/wmflib/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12445 2023-11-28 12:08:05.000000 wmflib-1.2.4/wmflib/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8282 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.4/wmflib/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2524 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4482 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-09-15 13:05:47.000000 wmflib-1.2.4/wmflib/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2879 2023-07-31 13:39:56.000000 wmflib-1.2.4/wmflib/irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.4/wmflib/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)     7357 2023-11-28 12:08:05.000000 wmflib-1.2.4/wmflib/requests.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.873517 wmflib-1.2.4/wmflib/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.388449 wmflib-1.2.4/wmflib/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.880450 wmflib-1.2.4/wmflib/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/config/config.ini
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/config/empty.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/config/invalid.ini
--rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/config/invalid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/config/valid.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.969986 wmflib-1.2.4/wmflib/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/phabricator/invalid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/fixtures/phabricator/valid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:15.040070 wmflib-1.2.4/wmflib/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.4/wmflib/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/unit/conftest.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.4/wmflib/tests/unit/test_actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.4/wmflib/tests/unit/test_config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/unit/test_constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8332 2023-07-31 13:28:37.000000 wmflib-1.2.4/wmflib/tests/unit/test_dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.4/wmflib/tests/unit/test_fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.4/wmflib/tests/unit/test_idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.4/wmflib/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3340 2023-07-31 13:39:56.000000 wmflib-1.2.4/wmflib/tests/unit/test_irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.4/wmflib/tests/unit/test_phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.4/wmflib/tests/unit/test_prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.4/wmflib/tests/unit/test_requests.py
--rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.4/wmflib/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-11-28 13:18:14.869051 wmflib-1.2.4/wmflib.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     2083 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        7 2023-11-28 13:18:14.000000 wmflib-1.2.4/wmflib.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.705683 wmflib-1.2.5/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.5/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.5/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.5/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.5/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)    14258 2024-04-18 14:12:38.000000 wmflib-1.2.5/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.5/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.5/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2024-04-18 14:50:26.705897 wmflib-1.2.5/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.5/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.541833 wmflib-1.2.5/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.554380 wmflib-1.2.5/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.555686 wmflib-1.2.5/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/_static/themes_override.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.590320 wmflib-1.2.5/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.5/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.5/doc/source/api/wmflib.actions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.5/doc/source/api/wmflib.config.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.5/doc/source/api/wmflib.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.5/doc/source/api/wmflib.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/api/wmflib.dns.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/api/wmflib.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.5/doc/source/api/wmflib.fileio.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.5/doc/source/api/wmflib.idm.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.5/doc/source/api/wmflib.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.5/doc/source/api/wmflib.irc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.5/doc/source/api/wmflib.phabricator.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.5/doc/source/api/wmflib.prometheus.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.5/doc/source/api/wmflib.requests.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.5/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.5/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.5/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.5/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2024-04-18 14:50:26.706980 wmflib-1.2.5/setup.cfg
+-rw-r--r--   0 riccardo   (501) staff       (20)     2491 2023-07-31 13:28:37.000000 wmflib-1.2.5/setup.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1524 2023-11-28 12:08:05.000000 wmflib-1.2.5/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.629632 wmflib-1.2.5/wmflib/
+-rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5894 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1796 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      603 2024-04-18 14:12:38.000000 wmflib-1.2.5/wmflib/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12445 2023-11-28 12:08:05.000000 wmflib-1.2.5/wmflib/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8282 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.5/wmflib/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2524 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4482 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-09-15 13:05:47.000000 wmflib-1.2.5/wmflib/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2879 2023-07-31 13:39:56.000000 wmflib-1.2.5/wmflib/irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.5/wmflib/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)     7357 2023-11-28 12:08:05.000000 wmflib-1.2.5/wmflib/requests.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.639127 wmflib-1.2.5/wmflib/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.505934 wmflib-1.2.5/wmflib/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.646722 wmflib-1.2.5/wmflib/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/config/config.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/config/empty.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/config/invalid.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/config/invalid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/config/valid.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.652551 wmflib-1.2.5/wmflib/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/phabricator/invalid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/fixtures/phabricator/valid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.704935 wmflib-1.2.5/wmflib/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.5/wmflib/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/unit/conftest.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.5/wmflib/tests/unit/test_actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.5/wmflib/tests/unit/test_config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/unit/test_constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8332 2023-07-31 13:28:37.000000 wmflib-1.2.5/wmflib/tests/unit/test_dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.5/wmflib/tests/unit/test_fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.5/wmflib/tests/unit/test_idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.5/wmflib/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3340 2023-07-31 13:39:56.000000 wmflib-1.2.5/wmflib/tests/unit/test_irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.5/wmflib/tests/unit/test_phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.5/wmflib/tests/unit/test_prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.5/wmflib/tests/unit/test_requests.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.5/wmflib/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-18 14:50:26.634396 wmflib-1.2.5/wmflib.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     2083 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        7 2024-04-18 14:50:26.000000 wmflib-1.2.5/wmflib.egg-info/top_level.txt
```

### Comparing `wmflib-1.2.4/CHANGELOG.rst` & `wmflib-1.2.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 wmflib Changelog
 ----------------
 
+`v1.2.5`_ (2024-04-18)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+constants: add the new magru datacenter.
+
 `v1.2.4`_ (2023-11-28)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Bug fixes
 """""""""
 
 * constants: update ``ns2.wikimedia.org`` IP address as it was recently changed.
@@ -382,7 +390,8 @@
 .. _`v1.1.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.1
 .. _`v1.1.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.2
 .. _`v1.2.0`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.0
 .. _`v1.2.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.1
 .. _`v1.2.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.2
 .. _`v1.2.3`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.3
 .. _`v1.2.4`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.4
+.. _`v1.2.5`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.5
```

### Comparing `wmflib-1.2.4/LICENSE` & `wmflib-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/PKG-INFO` & `wmflib-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.4
+Version: 1.2.5
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.4/README.rst` & `wmflib-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/doc/Makefile` & `wmflib-1.2.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/doc/source/conf.py` & `wmflib-1.2.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/doc/source/installation.rst` & `wmflib-1.2.5/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/prospector.yaml` & `wmflib-1.2.5/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/setup.cfg` & `wmflib-1.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/setup.py` & `wmflib-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/tox.ini` & `wmflib-1.2.5/tox.ini`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/actions.py` & `wmflib-1.2.5/wmflib/actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/config.py` & `wmflib-1.2.5/wmflib/config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/constants.py` & `wmflib-1.2.5/wmflib/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants module."""
 
 
-ALL_DATACENTERS = ('eqiad', 'codfw', 'esams', 'ulsfo', 'eqsin', 'drmrs')
+ALL_DATACENTERS = ('eqiad', 'codfw', 'esams', 'ulsfo', 'eqsin', 'drmrs', 'magru')
 """tuple: all WMF datacenters."""
 
 
 CORE_DATACENTERS = ("eqiad", "codfw")
 """tuple: WMF core datacenters."""
 
 
@@ -16,9 +16,10 @@
 DATACENTER_NUMBERING_PREFIX = {
     'eqiad': '1',
     'codfw': '2',
     'esams': '3',
     'ulsfo': '4',
     'eqsin': '5',
     'drmrs': '6',
+    'magru': '7',
 }
 """dict: mapping of hostname prefix for numbered servers for each WMF datacenter."""
```

### Comparing `wmflib-1.2.4/wmflib/decorators.py` & `wmflib-1.2.5/wmflib/decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/dns.py` & `wmflib-1.2.5/wmflib/dns.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/exceptions.py` & `wmflib-1.2.5/wmflib/exceptions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/fileio.py` & `wmflib-1.2.5/wmflib/fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/idm.py` & `wmflib-1.2.5/wmflib/idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/interactive.py` & `wmflib-1.2.5/wmflib/interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/irc.py` & `wmflib-1.2.5/wmflib/irc.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/phabricator.py` & `wmflib-1.2.5/wmflib/phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/prometheus.py` & `wmflib-1.2.5/wmflib/prometheus.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/requests.py` & `wmflib-1.2.5/wmflib/requests.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/__init__.py` & `wmflib-1.2.5/wmflib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/sphinx_checker.py` & `wmflib-1.2.5/wmflib/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_actions.py` & `wmflib-1.2.5/wmflib/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_config.py` & `wmflib-1.2.5/wmflib/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_decorators.py` & `wmflib-1.2.5/wmflib/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_dns.py` & `wmflib-1.2.5/wmflib/tests/unit/test_dns.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_fileio.py` & `wmflib-1.2.5/wmflib/tests/unit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_idm.py` & `wmflib-1.2.5/wmflib/tests/unit/test_idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_interactive.py` & `wmflib-1.2.5/wmflib/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_irc.py` & `wmflib-1.2.5/wmflib/tests/unit/test_irc.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_phabricator.py` & `wmflib-1.2.5/wmflib/tests/unit/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_prometheus.py` & `wmflib-1.2.5/wmflib/tests/unit/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib/tests/unit/test_requests.py` & `wmflib-1.2.5/wmflib/tests/unit/test_requests.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.4/wmflib.egg-info/PKG-INFO` & `wmflib-1.2.5/wmflib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.4
+Version: 1.2.5
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.4/wmflib.egg-info/SOURCES.txt` & `wmflib-1.2.5/wmflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

