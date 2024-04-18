# Comparing `tmp/alfpack-0.1.tar.gz` & `tmp/alfpack-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfpack-0.1.tar", last modified: Thu Apr 18 10:47:16 2024, max compression
+gzip compressed data, was "alfpack-0.2.tar", last modified: Thu Apr 18 10:48:12 2024, max compression
```

## Comparing `alfpack-0.1.tar` & `alfpack-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 10:47:16.208112 alfpack-0.1/
--rw-rw-rw-   0        0        0       52 2024-04-18 10:47:16.208112 alfpack-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 10:47:16.201030 alfpack-0.1/alfpack/
--rw-rw-rw-   0        0        0       59 2024-04-18 10:40:52.000000 alfpack-0.1/alfpack/__init__.py
--rw-rw-rw-   0        0        0     5508 2024-04-18 10:00:56.000000 alfpack-0.1/alfpack/coloraex.py
--rw-rw-rw-   0        0        0     3530 2024-04-18 10:47:01.000000 alfpack-0.1/alfpack/desc.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:47:16.207309 alfpack-0.1/alfpack.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-18 10:47:16.000000 alfpack-0.1/alfpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-18 10:47:16.000000 alfpack-0.1/alfpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 10:47:16.000000 alfpack-0.1/alfpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 10:47:16.000000 alfpack-0.1/alfpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 10:47:16.208112 alfpack-0.1/setup.cfg
--rw-rw-rw-   0        0        0      142 2024-04-18 10:46:21.000000 alfpack-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:48:12.020454 alfpack-0.2/
+-rw-rw-rw-   0        0        0       52 2024-04-18 10:48:12.020454 alfpack-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 10:48:12.009448 alfpack-0.2/alfpack/
+-rw-rw-rw-   0        0        0       59 2024-04-18 10:40:52.000000 alfpack-0.2/alfpack/__init__.py
+-rw-rw-rw-   0        0        0     5508 2024-04-18 10:00:56.000000 alfpack-0.2/alfpack/coloraex.py
+-rw-rw-rw-   0        0        0     3530 2024-04-18 10:47:01.000000 alfpack-0.2/alfpack/desc.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:48:12.019446 alfpack-0.2/alfpack.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-18 10:48:11.000000 alfpack-0.2/alfpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-18 10:48:11.000000 alfpack-0.2/alfpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:48:11.000000 alfpack-0.2/alfpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 10:48:11.000000 alfpack-0.2/alfpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:48:12.020454 alfpack-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      142 2024-04-18 10:48:06.000000 alfpack-0.2/setup.py
```

### Comparing `alfpack-0.1/alfpack/coloraex.py` & `alfpack-0.2/alfpack/coloraex.py`

 * *Files identical despite different names*

### Comparing `alfpack-0.1/alfpack/desc.py` & `alfpack-0.2/alfpack/desc.py`

 * *Files identical despite different names*

