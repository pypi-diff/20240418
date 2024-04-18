# Comparing `tmp/qm9loader-0.1.tar.gz` & `tmp/qm9loader-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm9loader-0.1.tar", last modified: Tue Apr 16 20:50:45 2024, max compression
+gzip compressed data, was "qm9loader-0.4.tar", last modified: Thu Apr 18 19:46:02 2024, max compression
```

## Comparing `qm9loader-0.1.tar` & `qm9loader-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 20:50:45.392547 qm9loader-0.1/
--rw-rw-rw-   0        0        0      182 2024-04-16 20:50:45.390284 qm9loader-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 20:50:45.363268 qm9loader-0.1/QM9Importer/
--rw-rw-rw-   0        0        0        0 2024-04-15 21:11:06.000000 qm9loader-0.1/QM9Importer/__init__.py
--rw-rw-rw-   0        0        0      183 2024-04-15 21:09:04.000000 qm9loader-0.1/QM9Importer/load_data.py
-drwxrwxrwx   0        0        0        0 2024-04-16 20:50:45.387262 qm9loader-0.1/qm9loader.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-16 20:50:45.000000 qm9loader-0.1/qm9loader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-04-16 20:50:45.000000 qm9loader-0.1/qm9loader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 20:50:45.000000 qm9loader-0.1/qm9loader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 20:50:45.000000 qm9loader-0.1/qm9loader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 20:50:45.392547 qm9loader-0.1/setup.cfg
--rw-rw-rw-   0        0        0      308 2024-04-16 20:48:36.000000 qm9loader-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:46:02.533887 qm9loader-0.4/
+-rw-rw-rw-   0        0        0      182 2024-04-18 19:46:02.531795 qm9loader-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 19:46:02.501720 qm9loader-0.4/qm9load/
+-rw-rw-rw-   0        0        0        0 2024-04-18 04:21:10.000000 qm9loader-0.4/qm9load/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-04-18 04:28:48.000000 qm9loader-0.4/qm9load/load_qm9.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:46:02.528594 qm9loader-0.4/qm9loader.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-18 19:46:02.000000 qm9loader-0.4/qm9loader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-18 19:46:02.000000 qm9loader-0.4/qm9loader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:46:02.000000 qm9loader-0.4/qm9loader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 19:46:02.000000 qm9loader-0.4/qm9loader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:46:02.533887 qm9loader-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      306 2024-04-18 04:37:47.000000 qm9loader-0.4/setup.py
```

