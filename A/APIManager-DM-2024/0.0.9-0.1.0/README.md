# Comparing `tmp/apimanager_dm_2024-0.0.9.tar.gz` & `tmp/apimanager_dm_2024-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimanager_dm_2024-0.0.9.tar", last modified: Wed Apr 17 23:22:26 2024, max compression
+gzip compressed data, was "apimanager_dm_2024-0.1.0.tar", last modified: Thu Apr 18 00:13:32 2024, max compression
```

## Comparing `apimanager_dm_2024-0.0.9.tar` & `apimanager_dm_2024-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:22:26.977024 apimanager_dm_2024-0.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-17 23:22:26.959023 apimanager_dm_2024-0.0.9/APIManager-DM-2024/
--rw-rw-rw-   0        0        0       36 2024-04-17 23:09:34.000000 apimanager_dm_2024-0.0.9/APIManager-DM-2024/__init__.py
--rw-rw-rw-   0        0        0     1362 2024-04-17 23:22:14.000000 apimanager_dm_2024-0.0.9/APIManager-DM-2024/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:22:26.975022 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/
--rw-rw-rw-   0        0        0       98 2024-04-17 23:22:26.000000 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-17 23:22:26.000000 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:22:26.000000 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 23:22:26.000000 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-17 23:22:26.000000 apimanager_dm_2024-0.0.9/APIManager_DM_2024.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       98 2024-04-17 23:22:26.976024 apimanager_dm_2024-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-04-17 23:00:45.000000 apimanager_dm_2024-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 23:22:26.977024 apimanager_dm_2024-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      200 2024-04-17 23:22:14.000000 apimanager_dm_2024-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:13:32.954139 apimanager_dm_2024-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-18 00:13:32.941142 apimanager_dm_2024-0.1.0/APIManager-DM-2024/
+-rw-rw-rw-   0        0        0       30 2024-04-17 23:51:27.000000 apimanager_dm_2024-0.1.0/APIManager-DM-2024/__init__.py
+-rw-rw-rw-   0        0        0     1130 2024-04-17 23:56:59.000000 apimanager_dm_2024-0.1.0/APIManager-DM-2024/main.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:13:32.952139 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-04-18 00:13:32.000000 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-18 00:13:32.000000 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 00:13:32.000000 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 00:13:32.000000 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-18 00:13:32.000000 apimanager_dm_2024-0.1.0/APIManager_DM_2024.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-04-18 00:13:32.953140 apimanager_dm_2024-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2024-04-18 00:12:05.000000 apimanager_dm_2024-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 00:13:32.954139 apimanager_dm_2024-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      354 2024-04-18 00:12:24.000000 apimanager_dm_2024-0.1.0/setup.py
```

