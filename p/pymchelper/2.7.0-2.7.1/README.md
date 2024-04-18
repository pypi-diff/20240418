# Comparing `tmp/pymchelper-2.7.0.tar.gz` & `tmp/pymchelper-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymchelper-2.7.0.tar", last modified: Wed Mar 27 18:07:11 2024, max compression
+gzip compressed data, was "pymchelper-2.7.1.tar", last modified: Thu Apr 18 08:11:43 2024, max compression
```

## Comparing `pymchelper-2.7.0.tar` & `pymchelper-2.7.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.212558 pymchelper-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-27 18:06:40.000000 pymchelper-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-27 18:07:11.212558 pymchelper-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-27 18:06:40.000000 pymchelper-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.204558 pymchelper-2.7.0/pymchelper/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.204558 pymchelper-2.7.0/pymchelper/executor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/executor/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/executor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.204558 pymchelper-2.7.0/pymchelper/flair/
--rw-r--r--   0 runner    (1001) docker     (127)    30952 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)   219827 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/Input.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.204558 pymchelper-2.7.0/pymchelper/flair/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68308 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/bmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    21373 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/csg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/fortran.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/common/rexx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/flair/db/
--rw-r--r--   0 runner    (1001) docker     (127)   183075 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/db/card.db
--rw-r--r--   0 runner    (1001) docker     (127)   234077 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/db/card.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/flair/db/db2ini.r
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/fluka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/readers/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/binary_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bdo2016.py
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bdo2019.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bin2010.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/readers/topas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/shieldhit/detector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/estimator_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/fortran_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/detector/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/shieldhit/particle.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/simulator_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.208558 pymchelper-2.7.0/pymchelper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/utils/mcscripter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.212558 pymchelper-2.7.0/pymchelper/utils/radiotherapy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/utils/radiotherapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29026 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/utils/radiotherapy/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/utils/runmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.212558 pymchelper-2.7.0/pymchelper/writers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/fortranformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/mcpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/shieldhit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/trip98cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    36804 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/trip98ddd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-27 18:06:40.000000 pymchelper-2.7.0/pymchelper/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:07:11.204558 pymchelper-2.7.0/pymchelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 18:07:11.000000 pymchelper-2.7.0/pymchelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 18:07:11.212558 pymchelper-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-03-27 18:06:40.000000 pymchelper-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.443266 pymchelper-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-18 08:11:16.000000 pymchelper-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-18 08:11:43.443266 pymchelper-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 08:11:16.000000 pymchelper-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/executor/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/executor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper/flair/
+-rw-r--r--   0 runner    (1001) docker     (127)    30952 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219827 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/Input.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper/flair/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68308 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/bmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21373 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/csg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/common/rexx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper/flair/db/
+-rw-r--r--   0 runner    (1001) docker     (127)   183075 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/db/card.db
+-rw-r--r--   0 runner    (1001) docker     (127)   234077 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/db/card.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/flair/db/db2ini.r
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/fluka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/readers/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/binary_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bdo2016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bdo2019.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bin2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/readers/topas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/shieldhit/detector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/estimator_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/fortran_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/detector/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/shieldhit/particle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/simulator_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/utils/mcscripter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.439266 pymchelper-2.7.1/pymchelper/utils/radiotherapy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/utils/radiotherapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29026 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/utils/radiotherapy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/utils/runmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.443266 pymchelper-2.7.1/pymchelper/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/fortranformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/mcpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/shieldhit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/trip98cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36804 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/trip98ddd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-18 08:11:16.000000 pymchelper-2.7.1/pymchelper/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:11:43.435266 pymchelper-2.7.1/pymchelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 08:11:43.000000 pymchelper-2.7.1/pymchelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 08:11:43.443266 pymchelper-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-18 08:11:16.000000 pymchelper-2.7.1/setup.py
```

### Comparing `pymchelper-2.7.0/PKG-INFO` & `pymchelper-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.7.0/README.md` & `pymchelper-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/__init__.py` & `pymchelper-2.7.1/pymchelper/__init__.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/averaging.py` & `pymchelper-2.7.1/pymchelper/averaging.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/axis.py` & `pymchelper-2.7.1/pymchelper/axis.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/estimator.py` & `pymchelper-2.7.1/pymchelper/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/executor/options.py` & `pymchelper-2.7.1/pymchelper/executor/options.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/executor/runner.py` & `pymchelper-2.7.1/pymchelper/executor/runner.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/Data.py` & `pymchelper-2.7.1/pymchelper/flair/Data.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/Input.py` & `pymchelper-2.7.1/pymchelper/flair/Input.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/common/bmath.py` & `pymchelper-2.7.1/pymchelper/flair/common/bmath.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/common/csg.py` & `pymchelper-2.7.1/pymchelper/flair/common/csg.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/common/fortran.py` & `pymchelper-2.7.1/pymchelper/flair/common/fortran.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/common/log.py` & `pymchelper-2.7.1/pymchelper/flair/common/log.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/common/rexx.py` & `pymchelper-2.7.1/pymchelper/flair/common/rexx.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/db/card.db` & `pymchelper-2.7.1/pymchelper/flair/db/card.db`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/db/card.ini` & `pymchelper-2.7.1/pymchelper/flair/db/card.ini`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/flair/db/db2ini.r` & `pymchelper-2.7.1/pymchelper/flair/db/db2ini.r`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/input_output.py` & `pymchelper-2.7.1/pymchelper/input_output.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/page.py` & `pymchelper-2.7.1/pymchelper/page.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/common.py` & `pymchelper-2.7.1/pymchelper/readers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/fluka.py` & `pymchelper-2.7.1/pymchelper/readers/fluka.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/binary_spec.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/binary_spec.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/general.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/general.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_base.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_base.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bdo2016.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bdo2016.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bdo2019.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bdo2019.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/shieldhit/reader_bin2010.py` & `pymchelper-2.7.1/pymchelper/readers/shieldhit/reader_bin2010.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/readers/topas.py` & `pymchelper-2.7.1/pymchelper/readers/topas.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/run.py` & `pymchelper-2.7.1/pymchelper/run.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/shieldhit/detector/detector_type.py` & `pymchelper-2.7.1/pymchelper/shieldhit/detector/detector_type.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/shieldhit/detector/estimator.py` & `pymchelper-2.7.1/pymchelper/shieldhit/detector/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/shieldhit/detector/fortran_card.py` & `pymchelper-2.7.1/pymchelper/shieldhit/detector/fortran_card.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/shieldhit/detector/geometry.py` & `pymchelper-2.7.1/pymchelper/shieldhit/detector/geometry.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/shieldhit/particle.py` & `pymchelper-2.7.1/pymchelper/shieldhit/particle.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/simulator_type.py` & `pymchelper-2.7.1/pymchelper/simulator_type.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/utils/mcscripter.py` & `pymchelper-2.7.1/pymchelper/utils/mcscripter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/utils/radiotherapy/plan.py` & `pymchelper-2.7.1/pymchelper/utils/radiotherapy/plan.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/utils/runmc.py` & `pymchelper-2.7.1/pymchelper/utils/runmc.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/version.py` & `pymchelper-2.7.1/pymchelper/version.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/common.py` & `pymchelper-2.7.1/pymchelper/writers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/excel.py` & `pymchelper-2.7.1/pymchelper/writers/excel.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/fortranformatter.py` & `pymchelper-2.7.1/pymchelper/writers/fortranformatter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/hdf.py` & `pymchelper-2.7.1/pymchelper/writers/hdf.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/inspector.py` & `pymchelper-2.7.1/pymchelper/writers/inspector.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/json.py` & `pymchelper-2.7.1/pymchelper/writers/json.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/mcpl.py` & `pymchelper-2.7.1/pymchelper/writers/mcpl.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/plots.py` & `pymchelper-2.7.1/pymchelper/writers/plots.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/shieldhit.py` & `pymchelper-2.7.1/pymchelper/writers/shieldhit.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/sparse.py` & `pymchelper-2.7.1/pymchelper/writers/sparse.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/trip98cube.py` & `pymchelper-2.7.1/pymchelper/writers/trip98cube.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/trip98ddd.py` & `pymchelper-2.7.1/pymchelper/writers/trip98ddd.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper/writers/writer.py` & `pymchelper-2.7.1/pymchelper/writers/writer.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper.egg-info/PKG-INFO` & `pymchelper-2.7.1/pymchelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.7.0/pymchelper.egg-info/SOURCES.txt` & `pymchelper-2.7.1/pymchelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymchelper-2.7.0/pymchelper.egg-info/requires.txt` & `pymchelper-2.7.1/pymchelper.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 [:python_version == "3.10"]
 numpy>=1.21
 
 [:python_version == "3.11"]
 numpy>=1.23.3
 
 [:python_version == "3.9"]
-numpy<1.26.0,>=1.20
+numpy<1.27.0,>=1.20
 
 [dicom]
 
 [dicom:python_version < "3.11"]
 pydicom
 
 [dicom:python_version == "3.11"]
 pydicom>=2.3.1
 
 [excel]
 xlwt
 
 [full]
-h5py
 matplotlib
-xlwt
 scipy
+xlwt
+h5py
 hipsterplot
 bashplotlib
 
 [full:platform_system == "Darwin" and (python_version >= "3.10" and python_version < "3.11")]
 pytrip98<3.9.0,>=3.6.1
 
 [full:platform_system == "Darwin" and (python_version >= "3.5" and python_version < "3.10")]
```

### Comparing `pymchelper-2.7.0/setup.py` & `pymchelper-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # |      1.11     | 2.7,  3.4 - 3.5 | linux, mac, win |
 # |      1.10     | 2.7,  3.3 - 3.5 |      linux      |
 # |       1.9     | 2.7,  3.3 - 3.5 |      linux      |
 # |---------------------------------------------------|
 # see https://www.python.org/dev/peps/pep-0508/ for language specification
 install_requires = [
     "numpy>=1.23.3 ; python_version == '3.11'", "numpy>=1.21 ; python_version == '3.10'",
-    "numpy>=1.20,<1.26.0 ; python_version == '3.9'"
+    "numpy>=1.20,<1.27.0 ; python_version == '3.9'"
 ]
 
 setuptools.setup(
     name='pymchelper',
     version=git_version(),
     packages=setuptools.find_packages(where='.', exclude=("tests", "tests.*", "examples")),
     url='https://github.com/DataMedSci/pymchelper',
```

