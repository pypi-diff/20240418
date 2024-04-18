# Comparing `tmp/googleadsquerytool-0.1.1.tar.gz` & `tmp/GoogleAdsQueryTool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleadsquerytool-0.1.1.tar", last modified: Thu Apr 18 11:44:08 2024, max compression
+gzip compressed data, was "GoogleAdsQueryTool-0.1.3.tar", last modified: Thu Apr 18 12:44:54 2024, max compression
```

## Comparing `googleadsquerytool-0.1.1.tar` & `GoogleAdsQueryTool-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 11:44:08.476596 googleadsquerytool-0.1.1/
--rw-r--r--   0 caspercrause   (501) staff       (20)      432 2024-04-18 11:44:08.476381 googleadsquerytool-0.1.1/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 googleadsquerytool-0.1.1/README.md
--rw-r--r--   0 caspercrause   (501) staff       (20)      618 2024-04-18 11:43:11.000000 googleadsquerytool-0.1.1/pyproject.toml
--rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 11:44:08.476648 googleadsquerytool-0.1.1/setup.cfg
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 11:44:08.475477 googleadsquerytool-0.1.1/src/
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 11:44:08.476166 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.egg-info/
--rw-r--r--   0 caspercrause   (501) staff       (20)      432 2024-04-18 11:44:08.000000 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.egg-info/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      250 2024-04-18 11:44:08.000000 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.egg-info/SOURCES.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 11:44:08.000000 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.egg-info/dependency_links.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       28 2024-04-18 11:44:08.000000 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.egg-info/top_level.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)     3951 2024-04-18 11:09:01.000000 googleadsquerytool-0.1.1/src/GoogleAdsQueryTool.py
--rw-r--r--   0 caspercrause   (501) staff       (20)        0 2024-04-18 11:08:22.000000 googleadsquerytool-0.1.1/src/__init__.py
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 12:44:54.476101 GoogleAdsQueryTool-0.1.3/
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 12:44:54.475667 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      272 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/SOURCES.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/dependency_links.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       76 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/entry_points.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       30 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/requires.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/top_level.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 12:44:54.475896 GoogleAdsQueryTool-0.1.3/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 GoogleAdsQueryTool-0.1.3/README.md
+-rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 12:44:54.476148 GoogleAdsQueryTool-0.1.3/setup.cfg
+-rw-r--r--   0 caspercrause   (501) staff       (20)      642 2024-04-18 12:43:44.000000 GoogleAdsQueryTool-0.1.3/setup.py
```

