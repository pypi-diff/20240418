# Comparing `tmp/culminator-0.1.tar.gz` & `tmp/culminator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culminator-0.1.tar", last modified: Thu Apr 18 04:14:48 2024, max compression
+gzip compressed data, was "culminator-0.3.tar", last modified: Thu Apr 18 05:16:16 2024, max compression
```

## Comparing `culminator-0.1.tar` & `culminator-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:14:48.148036 culminator-0.1/
--rw-rw-rw-   0        0        0      100 2024-04-18 04:14:48.145021 culminator-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 04:14:48.094745 culminator-0.1/culminator/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:53:45.000000 culminator-0.1/culminator/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-18 03:54:08.000000 culminator-0.1/culminator/classification.py
--rw-rw-rw-   0        0        0        0 2024-04-18 03:54:18.000000 culminator-0.1/culminator/clustering.py
--rw-rw-rw-   0        0        0        0 2024-04-18 03:54:12.000000 culminator-0.1/culminator/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:14:48.125859 culminator-0.1/culminator.egg-info/
--rw-rw-rw-   0        0        0      100 2024-04-18 04:14:47.000000 culminator-0.1/culminator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-04-18 04:14:47.000000 culminator-0.1/culminator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:14:47.000000 culminator-0.1/culminator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 04:14:47.000000 culminator-0.1/culminator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 04:14:47.000000 culminator-0.1/culminator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 04:14:48.148036 culminator-0.1/setup.cfg
--rw-rw-rw-   0        0        0      200 2024-04-18 04:13:09.000000 culminator-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.941354 culminator-0.3/
+-rw-rw-rw-   0        0        0      151 2024-04-18 05:16:16.939350 culminator-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-04-18 05:07:17.000000 culminator-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.929798 culminator-0.3/culminator/
+-rw-rw-rw-   0        0        0      197 2024-04-18 04:27:17.000000 culminator-0.3/culminator/__init__.py
+-rw-rw-rw-   0        0        0     4196 2024-04-18 04:25:35.000000 culminator-0.3/culminator/classification.py
+-rw-rw-rw-   0        0        0     4700 2024-04-18 04:25:45.000000 culminator-0.3/culminator/clustering.py
+-rw-rw-rw-   0        0        0     7417 2024-04-18 04:25:57.000000 culminator-0.3/culminator/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.937351 culminator-0.3/culminator.egg-info/
+-rw-rw-rw-   0        0        0      151 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:16:16.941354 culminator-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-18 05:07:57.000000 culminator-0.3/setup.py
```

