# Comparing `tmp/myarg-1.0.2.tar.gz` & `tmp/myarg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myarg-1.0.2.tar", last modified: Thu Apr 18 03:27:40 2024, max compression
+gzip compressed data, was "myarg-1.0.3.tar", last modified: Thu Apr 18 06:53:24 2024, max compression
```

## Comparing `myarg-1.0.2.tar` & `myarg-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:27:40.782010 myarg-1.0.2/
--rw-rw-rw-   0        0        0     1138 2024-04-18 03:27:40.782010 myarg-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:27:40.781511 myarg-1.0.2/myarg.egg-info/
--rw-rw-rw-   0        0        0     1138 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 03:27:40.782010 myarg-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     8690 2024-04-18 03:27:36.000000 myarg-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:53:24.254182 myarg-1.0.3/
+-rw-rw-rw-   0        0        0      503 2024-04-18 06:53:24.254182 myarg-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 06:53:24.251182 myarg-1.0.3/myarg/
+-rw-rw-rw-   0        0        0       70 2024-04-18 06:47:07.000000 myarg-1.0.3/myarg/__init__.py
+-rw-rw-rw-   0        0        0     2200 2024-04-18 06:47:07.000000 myarg-1.0.3/myarg/configuration_util.py
+-rw-rw-rw-   0        0        0      458 2024-04-18 06:50:54.000000 myarg-1.0.3/myarg/set_content_root.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:53:24.253182 myarg-1.0.3/myarg.egg-info/
+-rw-rw-rw-   0        0        0      503 2024-04-18 06:53:24.000000 myarg-1.0.3/myarg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 06:53:24.000000 myarg-1.0.3/myarg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:53:24.000000 myarg-1.0.3/myarg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-18 06:53:24.000000 myarg-1.0.3/myarg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 06:53:24.000000 myarg-1.0.3/myarg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:53:24.254182 myarg-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2024-04-18 06:53:18.000000 myarg-1.0.3/setup.py
```

