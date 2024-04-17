# Comparing `tmp/tukey-0.0.1.tar.gz` & `tmp/tukey-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tukey-0.0.1.tar", last modified: Wed Apr 17 16:05:27 2024, max compression
+gzip compressed data, was "tukey-0.0.2.tar", last modified: Wed Apr 17 22:09:28 2024, max compression
```

## Comparing `tukey-0.0.1.tar` & `tukey-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 16:05:27.165874 tukey-0.0.1/
--rw-rw-rw-   0        0        0      489 2024-04-17 16:05:27.165874 tukey-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 16:05:27.165874 tukey-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      706 2024-04-17 16:04:18.000000 tukey-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:05:27.091420 tukey-0.0.1/tukey/
--rw-rw-rw-   0        0        0       21 2024-04-16 22:34:42.000000 tukey-0.0.1/tukey/__init__.py
--rw-rw-rw-   0        0        0      281 2024-04-16 22:34:07.000000 tukey-0.0.1/tukey/tukey.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:05:27.165874 tukey-0.0.1/tukey.egg-info/
--rw-rw-rw-   0        0        0      489 2024-04-17 16:05:27.000000 tukey-0.0.1/tukey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2024-04-17 16:05:27.000000 tukey-0.0.1/tukey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 16:05:27.000000 tukey-0.0.1/tukey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 16:05:27.000000 tukey-0.0.1/tukey.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.390659 tukey-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2024-04-17 16:42:19.000000 tukey-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    44214 2024-04-17 22:09:28.388374 tukey-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-17 21:54:19.000000 tukey-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1379 2024-04-17 22:07:39.000000 tukey-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 22:09:28.390659 tukey-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.324175 tukey-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.343287 tukey-0.0.2/src/tukey/
+-rw-rw-rw-   0        0        0       25 2024-04-17 16:40:37.000000 tukey-0.0.2/src/tukey/__init__.py
+-rw-rw-rw-   0        0        0      302 2024-04-17 21:55:15.000000 tukey-0.0.2/src/tukey/tukey.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.380409 tukey-0.0.2/src/tukey.egg-info/
+-rw-rw-rw-   0        0        0    44214 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/top_level.txt
```

