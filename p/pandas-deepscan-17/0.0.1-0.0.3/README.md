# Comparing `tmp/pandas-deepscan-17-0.0.1.tar.gz` & `tmp/pandas-deepscan-17-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-deepscan-17-0.0.1.tar", last modified: Wed Apr 10 10:26:47 2024, max compression
+gzip compressed data, was "pandas-deepscan-17-0.0.3.tar", last modified: Thu Apr 18 13:09:27 2024, max compression
```

## Comparing `pandas-deepscan-17-0.0.1.tar` & `pandas-deepscan-17-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-10 10:26:47.011959 pandas-deepscan-17-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)      166 2024-04-10 10:26:47.011675 pandas-deepscan-17-0.0.1/PKG-INFO
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-10 10:26:47.011257 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      166 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      176 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-10 10:26:47.012045 pandas-deepscan-17-0.0.1/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      205 2024-04-10 10:21:30.000000 pandas-deepscan-17-0.0.1/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-18 13:09:27.699910 pandas-deepscan-17-0.0.3/
+-rw-r--r--   0 user       (501) staff       (20)      166 2024-04-18 13:09:27.699576 pandas-deepscan-17-0.0.3/PKG-INFO
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-18 13:09:27.699031 pandas-deepscan-17-0.0.3/pandas_deepscan_17.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      166 2024-04-18 13:09:27.000000 pandas-deepscan-17-0.0.3/pandas_deepscan_17.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      176 2024-04-18 13:09:27.000000 pandas-deepscan-17-0.0.3/pandas_deepscan_17.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-18 13:09:27.000000 pandas-deepscan-17-0.0.3/pandas_deepscan_17.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-18 13:09:27.000000 pandas-deepscan-17-0.0.3/pandas_deepscan_17.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-18 13:09:27.700001 pandas-deepscan-17-0.0.3/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     2705 2024-04-18 13:09:21.000000 pandas-deepscan-17-0.0.3/setup.py
```

