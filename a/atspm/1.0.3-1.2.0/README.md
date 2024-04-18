# Comparing `tmp/atspm-1.0.3.tar.gz` & `tmp/atspm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atspm-1.0.3.tar", last modified: Thu Apr 11 18:45:01 2024, max compression
+gzip compressed data, was "atspm-1.2.0.tar", last modified: Thu Apr 18 18:49:37 2024, max compression
```

## Comparing `atspm-1.0.3.tar` & `atspm-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 18:45:01.180761 atspm-1.0.3/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       77 2024-04-11 18:44:34.000000 atspm-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2452 2024-04-11 18:45:01.179761 atspm-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1979 2024-04-11 00:14:17.000000 atspm-1.0.3/README.md
--rw-rw-rw-   0        0        0      564 2024-04-11 18:44:37.000000 atspm-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 18:45:01.180761 atspm-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 18:45:01.156761 atspm-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 18:45:01.165761 atspm-1.0.3/src/atspm/
--rw-rw-rw-   0        0        0    16337 2024-04-11 16:55:36.000000 atspm-1.0.3/src/atspm/Aggregations.py
--rw-rw-rw-   0        0        0       78 2024-04-11 16:51:21.000000 atspm-1.0.3/src/atspm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:45:01.177758 atspm-1.0.3/src/atspm/data/
--rw-rw-rw-   0        0        0    13072 2024-04-11 00:14:17.000000 atspm-1.0.3/src/atspm/data/sample_detector-config.parquet
--rw-rw-rw-   0        0        0  1335371 2024-04-11 00:14:17.000000 atspm-1.0.3/src/atspm/data/sample_hi-res_data.parquet
--rw-rw-rw-   0        0        0    13989 2024-04-11 00:14:17.000000 atspm-1.0.3/src/atspm/queries.sql
--rw-rw-rw-   0        0        0      505 2024-04-11 18:44:17.000000 atspm-1.0.3/src/atspm/sample_data.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:45:01.178761 atspm-1.0.3/src/atspm.egg-info/
--rw-rw-rw-   0        0        0     2452 2024-04-11 18:45:01.000000 atspm-1.0.3/src/atspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-04-11 18:45:01.000000 atspm-1.0.3/src/atspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 18:45:01.000000 atspm-1.0.3/src/atspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-11 18:45:01.000000 atspm-1.0.3/src/atspm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.290141 atspm-1.2.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3441 2024-04-18 18:49:37.290141 atspm-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-04-18 18:32:57.000000 atspm-1.2.0/README.md
+-rw-rw-rw-   0        0        0      568 2024-04-18 18:06:31.000000 atspm-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:49:37.290141 atspm-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.243796 atspm-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.258886 atspm-1.2.0/src/atspm/
+-rw-rw-rw-   0        0        0       92 2024-04-18 18:05:56.000000 atspm-1.2.0/src/atspm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.274579 atspm-1.2.0/src/atspm/data/
+-rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.2.0/src/atspm/data/sample_config.parquet
+-rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.2.0/src/atspm/data/sample_raw_data.parquet
+-rw-rw-rw-   0        0        0      999 2024-04-16 16:12:10.000000 atspm-1.2.0/src/atspm/data_aggregator.py
+-rw-rw-rw-   0        0        0     1792 2024-04-18 17:11:03.000000 atspm-1.2.0/src/atspm/data_loader.py
+-rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.2.0/src/atspm/data_saver.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.274579 atspm-1.2.0/src/atspm/queries/
+-rw-rw-rw-   0        0        0      406 2024-04-16 01:24:53.000000 atspm-1.2.0/src/atspm/queries/actuations.sql
+-rw-rw-rw-   0        0        0     3867 2024-04-18 16:10:41.000000 atspm-1.2.0/src/atspm/queries/arrival_on_green.sql
+-rw-rw-rw-   0        0        0      532 2024-04-16 01:24:58.000000 atspm-1.2.0/src/atspm/queries/communications.sql
+-rw-rw-rw-   0        0        0      409 2024-04-15 21:20:28.000000 atspm-1.2.0/src/atspm/queries/coordination.sql
+-rw-rw-rw-   0        0        0     2602 2024-04-17 00:12:30.000000 atspm-1.2.0/src/atspm/queries/detector_faults.sql
+-rw-rw-rw-   0        0        0      668 2024-04-18 01:09:44.000000 atspm-1.2.0/src/atspm/queries/ped.sql
+-rw-rw-rw-   0        0        0    10285 2024-04-16 21:28:57.000000 atspm-1.2.0/src/atspm/queries/split_failures.sql
+-rw-rw-rw-   0        0        0      376 2024-04-18 13:37:09.000000 atspm-1.2.0/src/atspm/queries/splits.sql
+-rw-rw-rw-   0        0        0      571 2024-04-16 01:25:11.000000 atspm-1.2.0/src/atspm/queries/terminations.sql
+-rw-rw-rw-   0        0        0     1017 2024-04-18 15:20:29.000000 atspm-1.2.0/src/atspm/queries/unique_ped.sql
+-rw-rw-rw-   0        0        0     4776 2024-04-18 16:01:23.000000 atspm-1.2.0/src/atspm/queries/yellow_red.sql
+-rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.2.0/src/atspm/sample_data.py
+-rw-rw-rw-   0        0        0     2261 2024-04-18 17:44:46.000000 atspm-1.2.0/src/atspm/signal_data_processor.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.290141 atspm-1.2.0/src/atspm.egg-info/
+-rw-rw-rw-   0        0        0     3441 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/top_level.txt
```

### Comparing `atspm-1.0.3/LICENSE` & `atspm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atspm-1.0.3/pyproject.toml` & `atspm-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "atspm"
-version = "1.0.3"
+version = "1.2.0"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tools.setuptools]
 include_package_data = true
-package_data = {"atspm" = ["*.sql", "data/*"]}
+package_data = {"atspm" = ["queries/*", "data/*"]}
```

