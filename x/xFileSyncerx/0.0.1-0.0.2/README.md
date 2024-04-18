# Comparing `tmp/xFileSyncerx-0.0.1.tar.gz` & `tmp/xFileSyncerx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xFileSyncerx-0.0.1.tar", last modified: Fri Mar 22 13:41:11 2024, max compression
+gzip compressed data, was "xFileSyncerx-0.0.2.tar", last modified: Thu Apr 18 14:11:23 2024, max compression
```

## Comparing `xFileSyncerx-0.0.1.tar` & `xFileSyncerx-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 13:41:11.914663 xFileSyncerx-0.0.1/
--rw-rw-rw-   0        0        0      185 2024-03-22 13:41:11.914663 xFileSyncerx-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-22 13:41:11.914663 xFileSyncerx-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-03-22 13:40:36.000000 xFileSyncerx-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 13:41:11.899037 xFileSyncerx-0.0.1/xFileSyncerx/
--rw-rw-rw-   0        0        0       36 2024-03-22 13:38:01.000000 xFileSyncerx-0.0.1/xFileSyncerx/__init__.py
--rw-rw-rw-   0        0        0      229 2024-03-21 20:41:09.000000 xFileSyncerx-0.0.1/xFileSyncerx/xfilesyncerx.py
-drwxrwxrwx   0        0        0        0 2024-03-22 13:41:11.899037 xFileSyncerx-0.0.1/xFileSyncerx.egg-info/
--rw-rw-rw-   0        0        0      185 2024-03-22 13:41:11.000000 xFileSyncerx-0.0.1/xFileSyncerx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-03-22 13:41:11.000000 xFileSyncerx-0.0.1/xFileSyncerx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 13:41:11.000000 xFileSyncerx-0.0.1/xFileSyncerx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-22 13:41:11.000000 xFileSyncerx-0.0.1/xFileSyncerx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 14:11:23.931007 xFileSyncerx-0.0.2/
+-rw-rw-rw-   0        0        0      185 2024-04-18 14:11:23.931007 xFileSyncerx-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:11:23.931007 xFileSyncerx-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-04-18 13:36:01.000000 xFileSyncerx-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:11:23.908757 xFileSyncerx-0.0.2/xFileSyncerx/
+-rw-rw-rw-   0        0        0       36 2024-03-22 13:38:01.000000 xFileSyncerx-0.0.2/xFileSyncerx/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-04-18 13:34:12.000000 xFileSyncerx-0.0.2/xFileSyncerx/xfilesyncerx.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:11:23.931007 xFileSyncerx-0.0.2/xFileSyncerx.egg-info/
+-rw-rw-rw-   0        0        0      185 2024-04-18 14:11:23.000000 xFileSyncerx-0.0.2/xFileSyncerx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-04-18 14:11:23.000000 xFileSyncerx-0.0.2/xFileSyncerx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:11:23.000000 xFileSyncerx-0.0.2/xFileSyncerx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 14:11:23.000000 xFileSyncerx-0.0.2/xFileSyncerx.egg-info/top_level.txt
```

