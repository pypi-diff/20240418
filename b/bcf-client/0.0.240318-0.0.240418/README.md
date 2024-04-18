# Comparing `tmp/bcf-client-0.0.240318.tar.gz` & `tmp/bcf_client-0.0.240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcf-client-0.0.240318.tar", last modified: Mon Mar 18 00:36:26 2024, max compression
+gzip compressed data, was "bcf_client-0.0.240418.tar", last modified: Thu Apr 18 00:35:45 2024, max compression
```

## Comparing `bcf-client-0.0.240318.tar` & `bcf_client-0.0.240418.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.133543 bcf-client-0.0.240318/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-18 00:36:26.133543 bcf-client-0.0.240318/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-18 00:36:23.000000 bcf-client-0.0.240318/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 00:36:26.133543 bcf-client-0.0.240318/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.121543 bcf-client-0.0.240318/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.125542 bcf-client-0.0.240318/src/bcf/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/bcfxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/inmemory_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.125542 bcf-client-0.0.240318/src/bcf/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/bcfxml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.125542 bcf-client-0.0.240318/src/bcf/v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/model/markup.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/model/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/model/visinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/visinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.125542 bcf-client-0.0.240318/src/bcf/v2/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/xsd/markup.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/xsd/project.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/xsd/version.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v2/xsd/visinfo.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.129542 bcf-client-0.0.240318/src/bcf/v3/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/bcfapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/bcfxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.129542 bcf-client-0.0.240318/src/bcf/v3/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/markup.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/model/visinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/visinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.129542 bcf-client-0.0.240318/src/bcf/v3/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/documents.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/extensions.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/markup.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/project.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/shared-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/version.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/v3/xsd/visinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-18 00:36:18.000000 bcf-client-0.0.240318/src/bcf/xml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:36:26.133543 bcf-client-0.0.240318/src/bcf_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-18 00:36:26.000000 bcf-client-0.0.240318/src/bcf_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-18 00:36:26.000000 bcf-client-0.0.240318/src/bcf_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 00:36:26.000000 bcf-client-0.0.240318/src/bcf_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-18 00:36:26.000000 bcf-client-0.0.240318/src/bcf_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-18 00:36:26.000000 bcf-client-0.0.240318/src/bcf_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-18 00:35:42.000000 bcf_client-0.0.240418/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.183573 bcf_client-0.0.240418/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/bcfxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/inmemory_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/bcfxml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.187573 bcf_client-0.0.240418/src/bcf/v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/model/visinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/visinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v2/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/markup.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/project.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/version.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v2/xsd/visinfo.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/bcfapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/bcfxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.191573 bcf_client-0.0.240418/src/bcf/v3/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/model/visinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/visinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/src/bcf/v3/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/documents.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/extensions.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/markup.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/project.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/shared-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/version.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/v3/xsd/visinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-18 00:35:38.000000 bcf_client-0.0.240418/src/bcf/xml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:45.195573 bcf_client-0.0.240418/src/bcf_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 00:35:45.000000 bcf_client-0.0.240418/src/bcf_client.egg-info/top_level.txt
```

### Comparing `bcf-client-0.0.240318/COPYING` & `bcf_client-0.0.240418/COPYING`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/COPYING.LESSER` & `bcf_client-0.0.240418/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/PKG-INFO` & `bcf_client-0.0.240418/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcf-client
-Version: 0.0.240318
+Version: 0.0.240418
 Summary: BCF-XML file handler.
 Project-URL: Source, https://github.com/IfcOpenShell/IfcOpenShell
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BCF,BIM
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcf-client-0.0.240318/pyproject.toml` & `bcf_client-0.0.240418/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 requires-python = ">=3.8"
 keywords = ["IFC", "BCF", "BIM"]
 dependencies = [
     "xsdata",
     "numpy",
     "ifcopenshell",
 ]
-version = "0.0.240318"
+version = "0.0.240418"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
```

### Comparing `bcf-client-0.0.240318/src/bcf/__init__.py` & `bcf_client-0.0.240418/src/bcf/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/bcfxml.py` & `bcf_client-0.0.240418/src/bcf/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/geometry.py` & `bcf_client-0.0.240418/src/bcf/geometry.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/inmemory_zipfile.py` & `bcf_client-0.0.240418/src/bcf/inmemory_zipfile.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/__init__.py` & `bcf_client-0.0.240418/src/bcf/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/bcfxml.py` & `bcf_client-0.0.240418/src/bcf/v2/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/model/__init__.py` & `bcf_client-0.0.240418/src/bcf/v2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/model/markup.py` & `bcf_client-0.0.240418/src/bcf/v2/model/markup.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/model/project.py` & `bcf_client-0.0.240418/src/bcf/v2/model/project.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/model/visinfo.py` & `bcf_client-0.0.240418/src/bcf/v2/model/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/topic.py` & `bcf_client-0.0.240418/src/bcf/v2/topic.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/visinfo.py` & `bcf_client-0.0.240418/src/bcf/v2/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/xsd/markup.xsd` & `bcf_client-0.0.240418/src/bcf/v2/xsd/markup.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/xsd/project.xsd` & `bcf_client-0.0.240418/src/bcf/v2/xsd/project.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v2/xsd/visinfo.xsd` & `bcf_client-0.0.240418/src/bcf/v2/xsd/visinfo.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/bcfapi.py` & `bcf_client-0.0.240418/src/bcf/v3/bcfapi.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/bcfxml.py` & `bcf_client-0.0.240418/src/bcf/v3/bcfxml.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/document.py` & `bcf_client-0.0.240418/src/bcf/v3/document.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/__init__.py` & `bcf_client-0.0.240418/src/bcf/v3/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/documents.py` & `bcf_client-0.0.240418/src/bcf/v3/model/documents.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/extensions.py` & `bcf_client-0.0.240418/src/bcf/v3/model/extensions.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/markup.py` & `bcf_client-0.0.240418/src/bcf/v3/model/markup.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/project.py` & `bcf_client-0.0.240418/src/bcf/v3/model/project.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/model/visinfo.py` & `bcf_client-0.0.240418/src/bcf/v3/model/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/topic.py` & `bcf_client-0.0.240418/src/bcf/v3/topic.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/visinfo.py` & `bcf_client-0.0.240418/src/bcf/v3/visinfo.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/documents.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/documents.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/extensions.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/extensions.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/markup.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/markup.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/project.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/project.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/shared-types.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/shared-types.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/v3/xsd/visinfo.xsd` & `bcf_client-0.0.240418/src/bcf/v3/xsd/visinfo.xsd`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf/xml_parser.py` & `bcf_client-0.0.240418/src/bcf/xml_parser.py`

 * *Files identical despite different names*

### Comparing `bcf-client-0.0.240318/src/bcf_client.egg-info/PKG-INFO` & `bcf_client-0.0.240418/src/bcf_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcf-client
-Version: 0.0.240318
+Version: 0.0.240418
 Summary: BCF-XML file handler.
 Project-URL: Source, https://github.com/IfcOpenShell/IfcOpenShell
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BCF,BIM
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcf-client-0.0.240318/src/bcf_client.egg-info/SOURCES.txt` & `bcf_client-0.0.240418/src/bcf_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

