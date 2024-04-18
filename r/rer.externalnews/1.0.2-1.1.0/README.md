# Comparing `tmp/rer.externalnews-1.0.2.tar.gz` & `tmp/rer.externalnews-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rer.externalnews-1.0.2.tar", last modified: Thu Sep  2 12:35:16 2021, max compression
+gzip compressed data, was "rer.externalnews-1.1.0.tar", last modified: Thu Apr 18 08:28:38 2024, max compression
```

## Comparing `rer.externalnews-1.0.2.tar` & `rer.externalnews-1.1.0.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/
--rw-r--r--   0 daniele    (501) staff       (20)      573 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/CHANGES.rst
--rw-r--r--   0 daniele    (501) staff       (20)       78 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 daniele    (501) staff       (20)      667 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/LICENSE.rst
--rw-r--r--   0 daniele    (501) staff       (20)      105 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/MANIFEST.in
--rw-r--r--   0 daniele    (501) staff       (20)     3974 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/PKG-INFO
--rw-r--r--   0 daniele    (501) staff       (20)     1613 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/README.rst
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/
--rw-r--r--   0 daniele    (501) staff       (20)    66786 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/ExternalNews_dettaglio_backend.JPG
--rw-r--r--   0 daniele    (501) staff       (20)    38783 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/ExternalNews_vista_archivio_news.JPG
--rw-r--r--   0 daniele    (501) staff       (20)    99689 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/ExternalNews_vista_news_con_foto.JPG
--rw-r--r--   0 daniele    (501) staff       (20)    26933 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/ExternalNews_vista_news_esterne.JPG
--rw-r--r--   0 daniele    (501) staff       (20)       79 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/index.rst
--rw-r--r--   0 daniele    (501) staff       (20)    32560 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/docs/rer-logo.png
--rw-r--r--   0 daniele    (501) staff       (20)       50 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/requirements.txt
--rw-r--r--   0 daniele    (501) staff       (20)      270 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/setup.cfg
--rw-r--r--   0 daniele    (501) staff       (20)     1851 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/setup.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/
--rw-r--r--   0 daniele    (501) staff       (20)       80 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/__init__.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/
--rw-r--r--   0 daniele    (501) staff       (20)      133 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/__init__.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      549 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     3149 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/externalnews_view.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      143 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/configure.zcml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/serializers/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/serializers/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      159 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/serializers/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     1098 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/serializers/externalnews.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/templates/
--rw-r--r--   0 daniele    (501) staff       (20)     1491 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/browser/templates/externalnews.pt
--rw-r--r--   0 daniele    (501) staff       (20)     1093 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     1048 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/interfaces.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/it/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/it/LC_MESSAGES/
--rw-r--r--   0 daniele    (501) staff       (20)     2461 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.po
--rw-r--r--   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.pot
--rw-r--r--   0 daniele    (501) staff       (20)     2090 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/rer.externalnews.pot
--rwxr-xr-x   0 daniele    (501) staff       (20)      485 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/locales/update.sh
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/
--rw-r--r--   0 daniele    (501) staff       (20)      174 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/browserlayer.xml
--rw-r--r--   0 daniele    (501) staff       (20)      196 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/diff_tool.xml
--rw-r--r--   0 daniele    (501) staff       (20)      188 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/metadata.xml
--rw-r--r--   0 daniele    (501) staff       (20)       46 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/registry.xml
--rw-r--r--   0 daniele    (501) staff       (20)      251 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/repositorytool.xml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/types/
--rw-r--r--   0 daniele    (501) staff       (20)     3063 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/types/ExternalNews.xml
--rw-r--r--   0 daniele    (501) staff       (20)      165 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/types.xml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/uninstall/
--rw-r--r--   0 daniele    (501) staff       (20)      126 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 daniele    (501) staff       (20)      616 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/setuphandlers.py
--rw-r--r--   0 daniele    (501) staff       (20)     1456 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/testing.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/__init__.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/robot/
--rw-r--r--   0 daniele    (501) staff       (20)     1995 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/robot/test_example.robot
--rw-r--r--   0 daniele    (501) staff       (20)     2730 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/robot/test_externalnews.robot
--rw-r--r--   0 daniele    (501) staff       (20)     1496 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/test_externalnews.py
--rw-r--r--   0 daniele    (501) staff       (20)      877 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/test_robot.py
--rw-r--r--   0 daniele    (501) staff       (20)     2189 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/tests/test_setup.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/upgrades/
--rw-r--r--   0 daniele    (501) staff       (20)       24 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/upgrades/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      458 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/upgrades/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)      487 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer/externalnews/upgrades/upgrades.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/
--rw-r--r--   0 daniele    (501) staff       (20)     3974 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/PKG-INFO
--rw-r--r--   0 daniele    (501) staff       (20)     2391 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/SOURCES.txt
--rw-r--r--   0 daniele    (501) staff       (20)        1 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/dependency_links.txt
--rw-r--r--   0 daniele    (501) staff       (20)       53 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/entry_points.txt
--rw-r--r--   0 daniele    (501) staff       (20)        4 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/namespace_packages.txt
--rw-r--r--   0 daniele    (501) staff       (20)        1 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/not-zip-safe
--rw-r--r--   0 daniele    (501) staff       (20)      172 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/requires.txt
--rw-r--r--   0 daniele    (501) staff       (20)        4 2021-09-02 12:35:16.000000 rer.externalnews-1.0.2/src/rer.externalnews.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.851682 rer.externalnews-1.1.0/
+-rw-r--r--   0 cekk       (501) staff       (20)      646 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       78 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      667 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     3028 2024-04-18 08:28:38.851742 rer.externalnews-1.1.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1613 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.845983 rer.externalnews-1.1.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)    66786 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/ExternalNews_dettaglio_backend.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)    38783 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/ExternalNews_vista_archivio_news.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)    99689 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/ExternalNews_vista_news_con_foto.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)    26933 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/ExternalNews_vista_news_esterne.JPG
+-rw-r--r--   0 cekk       (501) staff       (20)       79 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      270 2024-04-18 08:28:38.851965 rer.externalnews-1.1.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1851 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.843191 rer.externalnews-1.1.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.846105 rer.externalnews-1.1.0/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.847686 rer.externalnews-1.1.0/src/rer/externalnews/
+-rw-r--r--   0 cekk       (501) staff       (20)      133 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.848040 rer.externalnews-1.1.0/src/rer/externalnews/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      554 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3149 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/externalnews_view.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.848283 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      143 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.848610 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/serializers/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/serializers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/serializers/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1098 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/serializers/externalnews.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.848764 rer.externalnews-1.1.0/src/rer/externalnews/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     1491 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/browser/templates/externalnews.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1054 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1048 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.849030 rer.externalnews-1.1.0/src/rer/externalnews/locales/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.843716 rer.externalnews-1.1.0/src/rer/externalnews/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.849414 rer.externalnews-1.1.0/src/rer/externalnews/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1553 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     2461 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.po
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     2090 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/locales/rer.externalnews.pot
+-rwxr-xr-x   0 cekk       (501) staff       (20)      485 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/locales/update.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.843967 rer.externalnews-1.1.0/src/rer/externalnews/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.850284 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      174 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      152 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      196 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/diff_tool.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      188 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       46 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      251 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/repositorytool.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.850417 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)     3047 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/types/ExternalNews.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      165 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/types.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.850546 rer.externalnews-1.1.0/src/rer/externalnews/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      126 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      616 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1456 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.851033 rer.externalnews-1.1.0/src/rer/externalnews/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.851259 rer.externalnews-1.1.0/src/rer/externalnews/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     1995 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)     2730 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/robot/test_externalnews.robot
+-rw-r--r--   0 cekk       (501) staff       (20)     1496 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/test_externalnews.py
+-rw-r--r--   0 cekk       (501) staff       (20)      877 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2189 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.851580 rer.externalnews-1.1.0/src/rer/externalnews/upgrades/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/upgrades/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/upgrades/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      487 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer/externalnews/upgrades/upgrades.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:28:38.847059 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     3028 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2517 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       40 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      172 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-04-18 08:28:38.000000 rer.externalnews-1.1.0/src/rer.externalnews.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rer.externalnews-1.0.2/CHANGES.rst` & `rer.externalnews-1.1.0/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.1.0 (2024-04-18)
+------------------
+
+- Volto compatibility.
+  [cekk]
+
+
 1.0.2 (2021-09-02)
 ------------------
 
 - Added serializer and remoteUrl field. Updated translations.
   [daniele]
 
 1.0.1 (2021-09-01)
```

### Comparing `rer.externalnews-1.0.2/LICENSE.rst` & `rer.externalnews-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/README.rst` & `rer.externalnews-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/docs/ExternalNews_dettaglio_backend.JPG` & `rer.externalnews-1.1.0/docs/ExternalNews_dettaglio_backend.JPG`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/docs/ExternalNews_vista_archivio_news.JPG` & `rer.externalnews-1.1.0/docs/ExternalNews_vista_archivio_news.JPG`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/docs/ExternalNews_vista_news_con_foto.JPG` & `rer.externalnews-1.1.0/docs/ExternalNews_vista_news_con_foto.JPG`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/docs/ExternalNews_vista_news_esterne.JPG` & `rer.externalnews-1.1.0/docs/ExternalNews_vista_news_esterne.JPG`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/docs/rer-logo.png` & `rer.externalnews-1.1.0/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/setup.py` & `rer.externalnews-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='rer.externalnews',
-    version='1.0.2',
+    version='1.1.0',
     description="A Plone add-on for Regione Emilia Romagna",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 5.0",
```

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/browser/configure.zcml` & `rer.externalnews-1.1.0/src/rer/externalnews/browser/configure.zcml`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     i18n_domain="rer.externalnews">
 
   <include package=".restapi" />
 
 
   <!-- External News view -->
   <browser:page
-      name="externalnews_redirect_view"
-      for="rer.externalnews.interfaces.IExternalNews"
-      class=".externalnews_view.ExternalNewsRedirectView"
-      layer="rer.externalnews.interfaces.IRerExternalnewsLayer"
-      permission="zope2.View"
+    for="rer.externalnews.interfaces.IExternalNews"
+    name="link_redirect_view"
+    class="plone.app.contenttypes.browser.link_redirect_view.LinkRedirectView"
+    permission="zope2.View"
+    layer="rer.externalnews.interfaces.IRerExternalnewsLayer"
       />
 
 </configure>
```

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/browser/externalnews_view.py` & `rer.externalnews-1.1.0/src/rer/externalnews/browser/externalnews_view.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/browser/restapi/serializers/externalnews.py` & `rer.externalnews-1.1.0/src/rer/externalnews/browser/restapi/serializers/externalnews.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/browser/templates/externalnews.pt` & `rer.externalnews-1.1.0/src/rer/externalnews/browser/templates/externalnews.pt`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/configure.zcml` & `rer.externalnews-1.1.0/src/rer/externalnews/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,14 @@
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     i18n_domain="rer.externalnews">
 
   <i18n:registerTranslations directory="locales" />
 
-  <includeDependencies package="." />
-
   <include package=".browser" />
   <include package=".upgrades" />
 
   <genericsetup:registerProfile
       name="default"
       title="RER: External News"
       directory="profiles/default"
```

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/interfaces.py` & `rer.externalnews-1.1.0/src/rer/externalnews/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.po` & `rer.externalnews-1.1.0/src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.po`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/locales/rer.externalnews.pot` & `rer.externalnews-1.1.0/src/rer/externalnews/locales/rer.externalnews.pot`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/types/ExternalNews.xml` & `rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/types/ExternalNews.xml`

 * *Files 1% similar despite different names*

#### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/profiles/default/types/ExternalNews.xml` & `rer.externalnews-1.1.0/src/rer/externalnews/profiles/default/types/ExternalNews.xml`

```diff
@@ -30,18 +30,18 @@
     <element value="plone.app.relationfield.behavior.IRelatedItems"/>
     <element value="plone.app.versioningbehavior.behaviors.IVersionable"/>
     <element value="plone.app.lockingbehavior.behaviors.ILocking"/>
   </property>
   <!-- View information -->
   <property name="add_view_expr">string:${folder_url}/++add++ExternalNews</property>
   <property name="immediate_view">view</property>
-  <property name="default_view">externalnews_redirect_view</property>
+  <property name="default_view">link_redirect_view</property>
   <property name="default_view_fallback">False</property>
   <property name="view_methods">
-    <element value="externalnews_redirect_view"/>
+    <element value="link_redirect_view"/>
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
```

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/setuphandlers.py` & `rer.externalnews-1.1.0/src/rer/externalnews/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/testing.py` & `rer.externalnews-1.1.0/src/rer/externalnews/testing.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/tests/robot/test_example.robot` & `rer.externalnews-1.1.0/src/rer/externalnews/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/tests/robot/test_externalnews.robot` & `rer.externalnews-1.1.0/src/rer/externalnews/tests/robot/test_externalnews.robot`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/tests/test_externalnews.py` & `rer.externalnews-1.1.0/src/rer/externalnews/tests/test_externalnews.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/tests/test_robot.py` & `rer.externalnews-1.1.0/src/rer/externalnews/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer/externalnews/tests/test_setup.py` & `rer.externalnews-1.1.0/src/rer/externalnews/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.externalnews-1.0.2/src/rer.externalnews.egg-info/SOURCES.txt` & `rer.externalnews-1.1.0/src/rer.externalnews.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 CHANGES.rst
 CONTRIBUTORS.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 docs/ExternalNews_dettaglio_backend.JPG
@@ -33,17 +34,19 @@
 src/rer/externalnews/browser/restapi/configure.zcml
 src/rer/externalnews/browser/restapi/serializers/__init__.py
 src/rer/externalnews/browser/restapi/serializers/configure.zcml
 src/rer/externalnews/browser/restapi/serializers/externalnews.py
 src/rer/externalnews/browser/templates/externalnews.pt
 src/rer/externalnews/locales/rer.externalnews.pot
 src/rer/externalnews/locales/update.sh
+src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.mo
 src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.po
 src/rer/externalnews/locales/it/LC_MESSAGES/rer.externalnews.pot
 src/rer/externalnews/profiles/default/browserlayer.xml
+src/rer/externalnews/profiles/default/catalog.xml
 src/rer/externalnews/profiles/default/diff_tool.xml
 src/rer/externalnews/profiles/default/metadata.xml
 src/rer/externalnews/profiles/default/registry.xml
 src/rer/externalnews/profiles/default/repositorytool.xml
 src/rer/externalnews/profiles/default/types.xml
 src/rer/externalnews/profiles/default/types/ExternalNews.xml
 src/rer/externalnews/profiles/uninstall/browserlayer.xml
```

