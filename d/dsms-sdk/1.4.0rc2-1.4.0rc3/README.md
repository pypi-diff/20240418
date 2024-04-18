# Comparing `tmp/dsms_sdk-1.4.0rc2.tar.gz` & `tmp/dsms_sdk-1.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.4.0rc2.tar", last modified: Wed Apr 17 00:13:43 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc3.tar", last modified: Thu Apr 18 08:01:01 2024, max compression
```

## Comparing `dsms_sdk-1.4.0rc2.tar` & `dsms_sdk-1.4.0rc3.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.959988 dsms_sdk-1.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 00:13:43.959988 dsms_sdk-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.947988 dsms_sdk-1.4.0rc2/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.947988 dsms_sdk-1.4.0rc2/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.951988 dsms_sdk-1.4.0rc2/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.951988 dsms_sdk-1.4.0rc2/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.951988 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/custom_datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/custom_datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/custom_datatype/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/properties/user_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.959988 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 00:13:43.000000 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 00:13:43.000000 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:13:43.000000 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-17 00:13:43.000000 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 00:13:43.000000 dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-17 00:13:43.959988 dsms_sdk-1.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:43.955988 dsms_sdk-1.4.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-17 00:13:37.000000 dsms_sdk-1.4.0rc2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.456714 dsms_sdk-1.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-18 08:01:01.456714 dsms_sdk-1.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.444713 dsms_sdk-1.4.0rc3/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.444713 dsms_sdk-1.4.0rc3/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.448713 dsms_sdk-1.4.0rc3/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.448713 dsms_sdk-1.4.0rc3/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.448713 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.448713 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/properties/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-18 08:01:01.000000 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-18 08:01:01.000000 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:01:01.000000 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 08:01:01.000000 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 08:01:01.000000 dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-18 08:01:01.456714 dsms_sdk-1.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:01:01.452714 dsms_sdk-1.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 08:00:57.000000 dsms_sdk-1.4.0rc3/tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc2/LICENSE` & `dsms_sdk-1.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/PKG-INFO` & `dsms_sdk-1.4.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc2/README.md` & `dsms_sdk-1.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc3/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc3/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/core/configuration.py` & `dsms_sdk-1.4.0rc3/dsms/core/configuration.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/core/context.py` & `dsms_sdk-1.4.0rc3/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc3/dsms/core/dsms.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from enum import Enum
     from typing import Optional
 
     from dsms.apps import App
     from dsms.core.context import Buffers
     from dsms.knowledge.kitem import KItem
     from dsms.knowledge.ktype import KType
+    from dsms.knowledge.search import SearchResult
 
 
 class DSMS:
     """
     General class for connecting and interfacing with DSMS.
 
     This class provides methods to connect to and interact with a DSMS (Data
@@ -124,15 +125,15 @@
     def search(
         self,
         query: "Optional[str]" = None,
         ktypes: "Optional[List[KType]]" = [],
         annotations: "Optional[List[str]]" = [],
         limit: int = 10,
         allow_fuzzy: "Optional[bool]" = True,
-    ) -> "List[KItem]":
+    ) -> "List[SearchResult]":
         """Search for KItems in the remote backend."""
         return _search(query, ktypes, annotations, limit, allow_fuzzy)
 
     @property
     def sparql_interface(cls) -> SparqlInterface:
         """Sparql interface of the DSMS instance."""
         return cls._sparql_interface
```

### Comparing `dsms_sdk-1.4.0rc2/dsms/core/utils.py` & `dsms_sdk-1.4.0rc3/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/ktype.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/affiliations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/annotations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,25 @@
         description="Whether the app should be triggered when a file is uploaded",
     )
     triggerUponUploadFileExtensions: Optional[List[str]] = Field(
         None,
         description="File extensions for which the upload shall be triggered.",
     )
 
+    def __str__(self) -> str:
+        """Pretty print the KProperty"""
+        values = ", ".join(
+            [f"{key}: {value}" for key, value in self.__dict__.items()]
+        )
+        return f"{{{values}}}"
+
+    def __repr__(self) -> str:
+        """Pretty print the Apps"""
+        return str(self)
+
 
 class App(KPropertyItem):
     """App of a KItem."""
 
     kitem_app_id: Optional[int] = Field(
         None, description="ID of the KItem App"
     )
```

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/attachments.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/authors.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         from_attributes=True,
     )
 
     _kitem = PrivateAttr(default=None)
 
     def __str__(self) -> str:
         """Pretty print the KProperty"""
-        values = ", ".join(
+        values = ",\n\t\t\t".join(
             [
-                f"{key}={value}"
+                f"{key}: {value}"
                 for key, value in self.__dict__.items()
                 if key not in self.exclude
             ]
         )
-        return f"{self.__class__.__name__}({values})"
+        return f"{{\n\t\t\t{values}\n\t\t}}"
 
     def __repr__(self) -> str:
         """Pretty print the KProperty"""
         return str(self)
 
     def __setattr__(self, index: int, item: "Any") -> None:
         """Add KItem to updated buffer."""
```

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/contacts.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/custom_datatype/numerical.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/custom_datatype/numerical.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/external_links.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/external_links.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/hdf5.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/linked_kitems.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/properties/user_groups.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/properties/user_groups.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/queries/base.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/queries/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/base.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/conversion.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/conversion.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/sparql.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/sparql.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/semantics/units/utils.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/semantics/units/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc3/dsms/knowledge/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 from dsms.core.utils import _name_to_camel, _perform_request  # isort:skip
 
 from dsms.knowledge.properties.custom_datatype import (  # isort:skip
     NumericalDataType,
 )
 
+from dsms.knowledge.search import SearchResult  # isort:skip
+
 if TYPE_CHECKING:
     from dsms.core.context import Buffers
     from dsms.knowledge import KItem, KType
 
 
 def _is_number(value):
     try:
@@ -42,72 +44,73 @@
     value: Optional[Dict[str, Any]]
 ) -> BaseModel:
     """Convert the dict with the model schema into a pydantic model."""
     from dsms import KItem
 
     fields = {}
     if isinstance(value, dict):
-        title = _name_to_camel(value.get("title"))
-        for item in value.get("objects"):
+        for item in value.get("sections"):
             for form_input in item.get("inputs"):
                 label = form_input.get("label")
                 dtype = form_input.get("widget")
                 default = form_input.get("defaultValue")
                 slug = _slugify(label)
-                if dtype in ("text", "file"):
+                if dtype in ("Text", "File", "Textarea", "Vocabulary term"):
                     dtype = str
-                elif dtype in ("number", "slider"):
+                elif dtype in ("Number", "Slider"):
                     dtype = NumericalDataType
-                elif dtype == "checkbox":
+                elif dtype == "Checkbox":
                     dtype = bool
-                elif dtype in ("select", "radio"):
+                elif dtype in ("Select", "Radio"):
                     dtype = Enum(
                         _name_to_camel(label) + "Choices",
                         {
                             _name_to_camel(choice["value"]): choice["value"]
                             for choice in form_input.get("choices")
                         },
                     )
-                elif dtype == "knowledge-select":
+                elif dtype == "Knowledge item":
                     warnings.warn(
-                        "knowledge-select not fully supported for KTypes yet."
+                        "knowledge item not fully supported for KTypes yet."
                     )
                     dtype = str
+
                 fields[slug] = (dtype, default or None)
-    else:
-        title = "CustomPropertiesModel"
     fields["kitem"] = (
         Optional[KItem],
         Field(None, exclude=True),
     )
 
     config = ConfigDict(
         extra="allow", arbitrary_types_allowed=True, exclude={"kitem"}
     )
     validators = {
         "validate_model": model_validator(mode="before")(_validate_model)
     }
     model = create_model(
-        title, __config__=config, __validators__=validators, **fields
+        "CustomPropertiesModel",
+        __config__=config,
+        __validators__=validators,
+        **fields,
     )
     setattr(model, "__str__", _print_properties)
     setattr(model, "__repr__", _print_properties)
     setattr(model, "__setattr__", __setattr_property__)
     return model
 
 
 def _print_properties(self: Any) -> str:
     fields = ", \n".join(
         [
-            f"\t\t{key}={value}"
+            f"\t\t{key}: {value}"
             for key, value in self.model_dump().items()
             if key not in self.model_config["exclude"]
         ]
     )
-    return f"{{\n{fields}\n\t\t}}"
+    return f"{{\n{fields}\n\t}}"
 
 
 def __setattr_property__(self, key, value) -> None:
     if _is_number(value):
         # convert to convertable numeric object
         value = _create_numerical_dtype(key, value, self.kitem)
         # mark as updated
@@ -257,15 +260,15 @@
             "kitem_apps",
             "created_at",
             "external_links",
             "hdf5",
         },
         exclude_none=True,
     )
-    custom_properties = kitem.custom_properties.model_dump_json()
+    custom_properties = kitem.custom_properties.model_dump()
     payload = json.loads(dumped)
     payload.update(
         custom_properties={"content": custom_properties}, **differences
     )
     payload.update(
         external_links={
             link.label: str(link.url) for link in kitem.external_links
@@ -420,15 +423,15 @@
 
 def _search(
     query: Optional[str] = None,
     ktypes: "Optional[List[KType]]" = [],
     annotations: "Optional[List[str]]" = [],
     limit: "Optional[int]" = 10,
     allow_fuzzy: "Optional[bool]" = True,
-) -> "List[KItem]":
+) -> "List[SearchResult]":
     """Search for KItems in the remote backend"""
     from dsms import KItem  # isort:skip
 
     payload = {
         "search_term": query or "",
         "ktypes": [ktype.value for ktype in ktypes],
         "kitem_annotations": annotations,
@@ -446,15 +449,18 @@
         )
     try:
         dumped = response.json()
     except Exception as excep:
         raise RuntimeError(
             f"""Something went wrong while searching for KItems: {response.text}"""
         ) from excep
-    return [KItem(**item) for item in dumped]
+    return [
+        SearchResult(hit=KItem(**item.get("hit")), fuzzy=item.get("fuzzy"))
+        for item in dumped
+    ]
 
 
 def _slugify(input_string: str, replacement: str = ""):
     """Turn any arbitrary string into a slug."""
     slug = re.sub(
         r"[^\w\s\-_]", replacement, input_string
     )  # Remove all non-word characters (everything except numbers and letters)
```

### Comparing `dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc2/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc3/dsms_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 dsms/core/configuration.py
 dsms/core/context.py
 dsms/core/dsms.py
 dsms/core/utils.py
 dsms/knowledge/__init__.py
 dsms/knowledge/kitem.py
 dsms/knowledge/ktype.py
+dsms/knowledge/search.py
 dsms/knowledge/utils.py
 dsms/knowledge/properties/__init__.py
 dsms/knowledge/properties/affiliations.py
 dsms/knowledge/properties/annotations.py
 dsms/knowledge/properties/apps.py
 dsms/knowledge/properties/attachments.py
 dsms/knowledge/properties/authors.py
```

### Comparing `dsms_sdk-1.4.0rc2/setup.cfg` & `dsms_sdk-1.4.0rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.4.0rc2
+version = v1.4.0rc3
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `dsms_sdk-1.4.0rc2/tests/conftest.py` & `dsms_sdk-1.4.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/tests/test_kitem.py` & `dsms_sdk-1.4.0rc3/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc2/tests/test_utils.py` & `dsms_sdk-1.4.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

