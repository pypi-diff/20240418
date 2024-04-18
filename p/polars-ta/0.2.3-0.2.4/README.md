# Comparing `tmp/polars_ta-0.2.3.tar.gz` & `tmp/polars_ta-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_ta-0.2.3.tar", last modified: Sat Mar 23 06:09:24 2024, max compression
+gzip compressed data, was "polars_ta-0.2.4.tar", last modified: Thu Apr 18 02:56:55 2024, max compression
```

## Comparing `polars_ta-0.2.3.tar` & `polars_ta-0.2.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.290525 polars_ta-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-23 06:09:12.000000 polars_ta-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-03-23 06:09:24.290525 polars_ta-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-03-23 06:09:12.000000 polars_ta-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.278525 polars_ta-0.2.3/polars_ta/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.278525 polars_ta-0.2.3/polars_ta/candles/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/candles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/candles/cdl1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/candles/cdl1_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/candles/cdl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.282525 polars_ta-0.2.3/polars_ta/performance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/performance/drawdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/performance/returns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.282525 polars_ta-0.2.3/polars_ta/prefix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/cdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/talib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/tdx.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/prefix/wq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.282525 polars_ta-0.2.3/polars_ta/ta/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/price.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/volatility.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/ta/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.282525 polars_ta-0.2.3/polars_ta/talib/
--rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/talib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.286525 polars_ta-0.2.3/polars_ta/tdx/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/over_bought_over_sold.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/pressure_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/tdx/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.286525 polars_ta-0.2.3/polars_ta/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/numba_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/pandas_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/utils/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.290525 polars_ta-0.2.3/polars_ta/wq/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/cross_sectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-23 06:09:12.000000 polars_ta-0.2.3/polars_ta/wq/transformational.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:09:24.290525 polars_ta-0.2.3/polars_ta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-03-23 06:09:24.000000 polars_ta-0.2.3/polars_ta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-23 06:09:24.000000 polars_ta-0.2.3/polars_ta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 06:09:24.000000 polars_ta-0.2.3/polars_ta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-23 06:09:24.000000 polars_ta-0.2.3/polars_ta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-23 06:09:24.000000 polars_ta-0.2.3/polars_ta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-23 06:09:12.000000 polars_ta-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 06:09:24.290525 polars_ta-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 06:09:12.000000 polars_ta-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 02:56:51.000000 polars_ta-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-18 02:56:55.252782 polars_ta-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-18 02:56:51.000000 polars_ta-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/candles/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl1_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/drawdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/returns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/cdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/talib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/tdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/wq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/volatility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/talib/
+-rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/talib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/tdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/over_bought_over_sold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/pressure_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/numba_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/pandas_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/wq/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/cross_sectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/transformational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 02:56:51.000000 polars_ta-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:56:55.252782 polars_ta-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:56:51.000000 polars_ta-0.2.4/setup.py
```

### Comparing `polars_ta-0.2.3/LICENSE` & `polars_ta-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/PKG-INFO` & `polars_ta-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.3
+Version: 0.2.4
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,16 @@
         
 Keywords: polars,expression,talib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: polars>=0.20.7
+Requires-Dist: polars>=0.20.19
+Requires-Dist: polars-ols>=0.3.0
 Requires-Dist: numpy
 Requires-Dist: numba
 Requires-Dist: pandas
 Provides-Extra: talib
 Requires-Dist: TA-Lib; extra == "talib"
 
 # polars_ta
```

### Comparing `polars_ta-0.2.3/README.md` & `polars_ta-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/candles/cdl1.py` & `polars_ta-0.2.4/polars_ta/candles/cdl1.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,20 @@
 def candle_color(open_: Expr, high: Expr, low: Expr, close: Expr) -> Expr:
     """K线颜色"""
     return close >= open_
 
 
 def four_price_doji(open_: Expr, high: Expr, low: Expr, close: Expr) -> Expr:
     """一字"""
-    return low > (high - TA_EPSILON)
+    return low >= (high - TA_EPSILON)
 
 
 def doji(open_: Expr, high: Expr, low: Expr, close: Expr) -> Expr:
     """十字(含一字、T字)"""
-    return (open_ - close).abs() < TA_EPSILON
+    return (open_ - close).abs() <= TA_EPSILON
 
 
 def dragonfly(open_: Expr, high: Expr, low: Expr, close: Expr) -> Expr:
     """正T字"""
     return doji(open_, high, low, close) & (low < close - TA_EPSILON)
```

### Comparing `polars_ta-0.2.3/polars_ta/candles/cdl1_limit.py` & `polars_ta-0.2.4/polars_ta/candles/cdl1_limit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/candles/cdl2.py` & `polars_ta-0.2.4/polars_ta/candles/cdl2.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/noise.py` & `polars_ta-0.2.4/polars_ta/noise.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/performance/returns.py` & `polars_ta-0.2.4/polars_ta/performance/returns.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/prefix/ta.py` & `polars_ta-0.2.4/polars_ta/prefix/ta.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/prefix/talib.py` & `polars_ta-0.2.4/polars_ta/prefix/talib.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/prefix/tdx.py` & `polars_ta-0.2.4/polars_ta/prefix/tdx.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/momentum.py` & `polars_ta-0.2.4/polars_ta/ta/momentum.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/operators.py` & `polars_ta-0.2.4/polars_ta/ta/operators.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/overlap.py` & `polars_ta-0.2.4/polars_ta/ta/overlap.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/statistic.py` & `polars_ta-0.2.4/polars_ta/ta/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/transform.py` & `polars_ta-0.2.4/polars_ta/ta/transform.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/volatility.py` & `polars_ta-0.2.4/polars_ta/ta/volatility.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/ta/volume.py` & `polars_ta-0.2.4/polars_ta/ta/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/talib/__init__.py` & `polars_ta-0.2.4/polars_ta/talib/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/__init__.py` & `polars_ta-0.2.4/polars_ta/tdx/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/_nb.py` & `polars_ta-0.2.4/polars_ta/tdx/_nb.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/arithmetic.py` & `polars_ta-0.2.4/polars_ta/tdx/arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/choice.py` & `polars_ta-0.2.4/polars_ta/tdx/choice.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/energy.py` & `polars_ta-0.2.4/polars_ta/tdx/energy.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/logical.py` & `polars_ta-0.2.4/polars_ta/tdx/logical.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/over_bought_over_sold.py` & `polars_ta-0.2.4/polars_ta/tdx/over_bought_over_sold.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/pressure_support.py` & `polars_ta-0.2.4/polars_ta/tdx/pressure_support.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/reference.py` & `polars_ta-0.2.4/polars_ta/tdx/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return a - b
 
 
 def BARSLASTCOUNT(condition: Expr) -> Expr:
     """Cumulative count of continuous true observations
     统计连续满足条件的周期数"""
     a = condition.cast(Int32).cum_sum()
-    b = when(condition.cast(Boolean)).then(None).otherwise(a).forward_fill().fill_null(0)
+    b = when(~condition.cast(Boolean)).then(a).otherwise(None).forward_fill().fill_null(0)
     return a - b
 
 
 def BARSSINCE(condition: Expr) -> Expr:
     """# of observations since the first time condition was true
     第一次X不为0到现在的天数"""
     a = condition.cum_count()
```

### Comparing `polars_ta-0.2.3/polars_ta/tdx/statistic.py` & `polars_ta-0.2.4/polars_ta/tdx/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/trend.py` & `polars_ta-0.2.4/polars_ta/tdx/trend.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/tdx/volume.py` & `polars_ta-0.2.4/polars_ta/tdx/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/utils/helper.py` & `polars_ta-0.2.4/polars_ta/utils/helper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/utils/numba_.py` & `polars_ta-0.2.4/polars_ta/utils/numba_.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/utils/pandas_.py` & `polars_ta-0.2.4/polars_ta/utils/pandas_.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/utils/pit.py` & `polars_ta-0.2.4/polars_ta/utils/pit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/utils/wrapper.py` & `polars_ta-0.2.4/polars_ta/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/wq/_nb.py` & `polars_ta-0.2.4/polars_ta/wq/_nb.py`

 * *Files 12% similar despite different names*

```diff
@@ -145,7 +145,32 @@
         return out
     a1 = sliding_window_view(x1, window)
     a2 = sliding_window_view(x2, window)
     a3 = sliding_window_view(x3, window)
     for i, (v1, v2, v3) in enumerate(zip(a1, a2, a3)):
         out[i + window - 1] = _triple_corr(v1, v2, v3)
     return out
+
+
+@jit(nopython=True, nogil=True, fastmath=True, cache=True)
+def isnan(x):
+    # https://github.com/numba/numba/issues/2919#issuecomment-747377615
+    if int(x) == -9223372036854775808:
+        return True
+    else:
+        return False
+
+
+@jit(nopython=True, nogil=True, fastmath=True, cache=True)
+def _zip_prod(a, b):
+    for i in range(1, a.shape[0]):
+        if isnan(a[i]):
+            a[i] = a[i - 1] * b[i - 1]
+    return a
+
+
+@jit(nopython=True, nogil=True, fastmath=False, cache=False)
+def _zip_sum(a, b):
+    for i in range(1, a.shape[0]):
+        if isnan(a[i]):
+            a[i] = a[i - 1] + b[i - 1]
+    return a
```

### Comparing `polars_ta-0.2.3/polars_ta/wq/_slow.py` & `polars_ta-0.2.4/polars_ta/wq/_slow.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/wq/arithmetic.py` & `polars_ta-0.2.4/polars_ta/wq/arithmetic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import numpy as np
-from polars import Expr, Series
+from polars import Expr, Series, mean_horizontal
 from polars import reduce, max_horizontal, sum_horizontal, min_horizontal, Int64
 
 
 def abs_(x: Expr) -> Expr:
     if isinstance(x, (Expr, Series)):
         return x.abs()
     else:
         return np.abs(x)
 
 
 def add(a: Expr, b: Expr, *args, filter_: bool = False) -> Expr:
     """Add all inputs (at least 2 inputs required). If filter = true, filter all input NaN to 0 before adding"""
-    _args = [a, b] + list(args)
-
     if filter_:
-        return sum_horizontal(*_args)
-
+        return sum_horizontal(a, b, *args)
+    _args = [a, b] + list(args)
     return reduce(function=lambda acc, x: acc + x, exprs=_args)
 
 
 def arc_cos(x: Expr) -> Expr:
     """If -1 <= x <= 1: arccos(x); else NaN"""
     return x.arccos()
 
@@ -67,17 +65,17 @@
 
 def floor(x: Expr) -> Expr:
     return x.floor()
 
 
 def fraction(x: Expr) -> Expr:
     """This operator removes the whole number part and returns the remaining fraction part with sign."""
-    # return sign(x) * (abs(x) - floor(abs(x)))
-    # return x.sign() * (x.abs() % 1)
-    return x % 1
+    # 按小学时的定义，负数-1.2的整数部分是-2,小数部分是0.8，而这有所不同
+    # return x % 1
+    return x.sign() * (x.abs() % 1)
 
 
 def inverse(x: Expr) -> Expr:
     """1 / x"""
     return 1 / x
 
 
@@ -96,27 +94,24 @@
     """convert simple return to log return
     简单收益率 转 对数收益率"""
     return x.log1p()
 
 
 def max_(a: Expr, b: Expr, *args) -> Expr:
     """Maximum value of all inputs. At least 2 inputs are required."""
-    _args = [a, b] + list(args)
-    return max_horizontal(*_args)
+    return max_horizontal(a, b, *args)
 
 
 def mean(a: Expr, b: Expr, *args) -> Expr:
-    _args = [a, b] + list(args)
-    return sum_horizontal(*_args) / len(_args)
+    return mean_horizontal(a, b, *args)
 
 
 def min_(a: Expr, b: Expr, *args) -> Expr:
     """Maximum value of all inputs. At least 2 inputs are required."""
-    _args = [a, b] + list(args)
-    return min_horizontal(*_args)
+    return min_horizontal(a, b, *args)
 
 
 def mod(x: Expr, y: Expr) -> Expr:
     return x % y
 
 
 def multiply(a: Expr, b: Expr, *args, filter_: bool = False) -> Expr:
@@ -151,14 +146,23 @@
         return x // f * f
 
 
 def s_log_1p(x: Expr) -> Expr:
     return x.abs().log1p() * x.sign()
 
 
+def sigmoid(a: Expr) -> Expr:
+    # a<0
+    # b = a.exp()
+    # return b / (1 + b)
+
+    # a>0
+    return 1 / (1 + (-a).exp())
+
+
 def sign(x: Expr) -> Expr:
     if isinstance(x, (Expr, Series)):
         return x.sign()
     else:
         return np.sign(x)
 
 
@@ -177,14 +181,18 @@
     return x.sin()
 
 
 def sinh(x: Expr) -> Expr:
     return x.sinh()
 
 
+def softsign(a: Expr) -> Expr:
+    return a / (1 + a.abs())
+
+
 def sqrt(x: Expr) -> Expr:
     return x.sqrt()
 
 
 def subtract(a: Expr, b: Expr, *args, filter_: bool = False) -> Expr:
     """x-y. If filter = true, filter all input NaN to 0 before subtracting"""
     _args = [a, b] + list(args)
@@ -203,7 +211,20 @@
     return x.tanh()
 
 
 def truncate(x: Expr) -> Expr:
     """truncate towards zero
     向零取整"""
     return x.cast(Int64)
+
+
+def var(a: Expr, b: Expr, *args) -> Expr:
+    """多列水平方差"""
+    _args = [a, b] + list(args)
+    _mean = mean_horizontal(_args)
+    _sum = sum_horizontal([(expr - _mean) ** 2 for expr in _args])
+    return _sum
+
+
+def std(a: Expr, b: Expr, *args) -> Expr:
+    """多列水平标准差"""
+    return var(a, b, *args).sqrt()
```

### Comparing `polars_ta-0.2.3/polars_ta/wq/cross_sectional.py` & `polars_ta-0.2.4/polars_ta/wq/cross_sectional.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-from polars import Expr
-
-from polars_ta.wq.preprocess import cs_neutralize_demean, cs_standardize_minmax, cs_winsorize_3sigma
-from polars_ta.wq.preprocess import cs_standardize_zscore
-
+import polars_ols as pls
+from polars import Expr, when
+from polars_ols import OLSKwargs
 
 # In the original version, the function names are not prefixed with `cs_`,
 # here we add it to prevent confusion
 # 原版函数名都没有加`cs_`, 这里统一加一防止混淆
 
-def cs_normalize(x: Expr, use_std: bool = False, limit: float = 0.0) -> Expr:
-    """Calculates the mean value of all valid alpha values for a certain date, then subtracts that mean from each element."""
-    if use_std:
-        # we need ddof=1 to match the doc
-        # 这里用ddof=1才能与文档示例的数值对应上
-        r = cs_standardize_zscore(x, ddof=1)
-    else:
-        r = cs_neutralize_demean(x)
 
-    if limit == 0:
-        return r
-    else:
-        return r.clip(-limit, limit)
+_ols_kwargs = OLSKwargs(null_policy='drop', solve_method='svd')
 
 
 def cs_one_side(x: Expr, is_long: bool = True) -> Expr:
     """Shifts all instruments up or down so that the Alpha becomes long-only or short-only
 (if side = short), respectively."""
     # TODO: 这里不确定，需再研究
     # [-1, 0, 1]+1=[0, 1, 2]
@@ -46,23 +33,27 @@
         L = x.clip(lower_bound=0)  # 全正数
         S = x.clip(upper_bound=0)  # 全负数，和还是负数
         return L / L.sum() * long_scale - S / S.sum() * short_scale
     else:
         return x / x.abs().sum() * scale_
 
 
-def cs_scale_down(x: Expr) -> Expr:
-    """Scales all values in each day proportionately between 0 and 1 such that minimum value maps to 0 and maximum value maps to 1. Constant is the offset by which final result is subtracted."""
-    return cs_standardize_minmax(x)
-
-
 def cs_truncate(x: Expr, max_percent: float = 0.01) -> Expr:
     """Operator truncates all values of x to maxPercent. Here, maxPercent is in decimal notation."""
     return x.clip(upper_bound=x.sum() * max_percent)
 
 
-def cs_winsorize(x: Expr, std: float = 4) -> Expr:
-    return cs_winsorize_3sigma(x, std)
+def cs_fill_zero(x: Expr) -> Expr:
+    """截面不全为空时，空值填充为0，反之保持null
+
+    在权重矩阵中使用时。一定要保证所有股票都在，停牌不能被过滤了"""
+    return when(x.is_not_null().sum() == 0).then(x).otherwise(x.fill_null(0))
+
+
+def cs_regression_neut(y: Expr, x: Expr) -> Expr:
+    """一元回归残差"""
+    return pls.compute_least_squares(y, x, add_intercept=True, mode='residuals', ols_kwargs=_ols_kwargs)
 
 
-def cs_zscore(x: Expr) -> Expr:
-    return cs_standardize_zscore(x)
+def cs_regression_proj(y: Expr, x: Expr) -> Expr:
+    """一元回归预测"""
+    return pls.compute_least_squares(y, x, add_intercept=True, mode='predictions', ols_kwargs=_ols_kwargs)
```

### Comparing `polars_ta-0.2.3/polars_ta/wq/logical.py` & `polars_ta-0.2.4/polars_ta/wq/logical.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/polars_ta/wq/preprocess.py` & `polars_ta-0.2.4/polars_ta/wq/preprocess.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 from typing import List
 
 import numpy as np
+import polars_ols as pls
 from polars import Expr, Series, Struct, map_batches
+from polars_ols.least_squares import OLSKwargs
 
 from polars_ta import TA_EPSILON
+from polars_ta.wq.cross_sectional import cs_rank
 
 
-def cs_standardize_zscore(x: Expr, ddof: int = 0) -> Expr:
+# ======================
+# standardize
+def cs_zscore(x: Expr, ddof: int = 0) -> Expr:
     return (x - x.mean()) / x.std(ddof=ddof)
 
 
-def cs_standardize_minmax(x: Expr) -> Expr:
+def cs_minmax(x: Expr) -> Expr:
     a = x.min()
     b = x.max()
     return (x - a) / (b - a + TA_EPSILON)
 
 
-def cs_winsorize_quantile(x: Expr, low_limit: float = 0.025, up_limit: float = 0.995) -> Expr:
+# ======================
+# winsorize
+def cs_quantile(x: Expr, low_limit: float = 0.025, up_limit: float = 0.995) -> Expr:
     a = x.quantile(low_limit)
     b = x.quantile(up_limit)
     return x.clip(lower_bound=a, upper_bound=b)
 
 
-def cs_winsorize_3sigma(x: Expr, n: float = 3.) -> Expr:
+def cs_3sigma(x: Expr, n: float = 3.) -> Expr:
     # fill_nan will seriously reduce speed. So it's more appropriate for users to handle it themselves
     # fill_nan(None) 严重拖慢速度，所以还是由用户自己处理更合适
     a = x.mean()
     b = n * x.std(ddof=0)
     return x.clip(lower_bound=a - b, upper_bound=a + b)
 
 
-def cs_winsorize_mad(x: Expr, n: float = 3., k: float = 1.4826) -> Expr:
+def cs_mad(x: Expr, n: float = 3., k: float = 1.4826) -> Expr:
     # https://en.wikipedia.org/wiki/Median_absolute_deviation
     a = x.median()
     b = (n * k) * (x - a).abs().median()
     return x.clip(lower_bound=a - b, upper_bound=a + b)
 
 
-def cs_neutralize_demean(x: Expr) -> Expr:
+# ======================
+# neutralize
+def cs_demean(x: Expr) -> Expr:
     """demean
 
     Notes
     -----
     Slower than multivariate regression. We need to groupby date and industry here,
     while multivariate regression only needs to add industry dummy variables and then groupby date
 
@@ -49,30 +58,20 @@
     -----
     速度没有多元回归快，因为这里需要按日期行业groupby，
     而多元回归只要添加行业哑变量，然后按日期groupby即可
     """
     return x - x.mean()
 
 
-def cs_neutralize_residual_simple(y: Expr, x: Expr) -> Expr:
-    """simple regression
-    一元回归"""
-    # https://stackoverflow.com/a/74906705/1894479
-    # 一元回归时，这个版本更快，不需再补充常量1
-    # e_i = y_i - a - bx_i
-    #     = y_i - ȳ + bx̄ - bx_i
-    #     = y_i - ȳ - b(x_i - x̄)
-    x_demeaned = x - x.mean()
-    y_demeaned = y - y.mean()
-    x_demeaned_squared = x_demeaned.pow(2)
-    beta = x_demeaned.dot(y_demeaned) / x_demeaned_squared.sum()
-    return y_demeaned - beta * x_demeaned
+# ======================
+# neutralize
+_ols_kwargs = OLSKwargs(null_policy='drop', solve_method='svd')
 
 
-def residual_multiple(cols: List[Series], add_constant: bool) -> Series:
+def _residual_multiple(cols: List[Series], add_constant: bool) -> Series:
     # 将pl.Struct转成list,这样可以实现传正则，其它也转list
     cols = [list(c.struct) if isinstance(c.dtype, Struct) else [c] for c in cols]
     # 二维列表转一维列表，再转np.ndarray
     cols = [i.to_numpy() for p in cols for i in p]
     if add_constant:
         cols += [np.ones_like(cols[0])]
     yx = np.vstack(cols).T
@@ -90,38 +89,55 @@
     # refill
     out = np.empty_like(yx[:, 0])
     out[~mask] = residual
     out[mask] = np.nan
     return Series(out, nan_to_null=True)
 
 
-def cs_neutralize_residual_multiple(y: Expr, *more_x: Expr) -> Expr:
+def cs_resid_(y: Expr, *more_x: Expr) -> Expr:
     """multivariate regression
     多元回归
-
-    Examples
-    --------
-    >>> cs_neutralize_residual_multiple(EP, LOG_MKT_CAP, *cs.expand_selector(df, cs.matches(r"^sw_l1_\d+$")), ONE)
-    >>> cs_neutralize_residual_multiple(EP, LOG_MKT_CAP, pl.struct(r"^sw_l1_\d+$"), ONE)
-
-    Notes
-    -----
-    add a constant column for the intercept
-    常量1，可以通过多输入1列来完成
-    正则列需要通过`pl.struct`传输，比之前整体转`pl.struct`能支持复杂公式
     """
-    return map_batches([y, *more_x], lambda xx: residual_multiple(xx, False))
+    return map_batches([y, *more_x], lambda xx: _residual_multiple(xx, False))
 
 
-def cs_neutralize_residual(y: Expr, *more_x: Expr) -> Expr:
-    """回归"""
-    return cs_neutralize_residual_multiple(y, *more_x)
+def cs_resid(y: Expr, *more_x: Expr) -> Expr:
+    """多元回归取残差"""
+    return pls.compute_least_squares(y, *more_x, mode='residuals', ols_kwargs=_ols_kwargs)
 
 
 def cs_mad_zscore(y: Expr) -> Expr:
     """常用功能简化封装。去极值、标准化"""
-    return cs_standardize_zscore(cs_winsorize_mad(y))
+    return cs_zscore(cs_mad(y))
 
 
 def cs_mad_zscore_resid(y: Expr, *more_x: Expr) -> Expr:
     """常用功能简化封装。去极值、标准化、中性化"""
-    return cs_neutralize_residual_multiple(cs_standardize_zscore(cs_winsorize_mad(y)), *more_x)
+    return cs_resid(cs_zscore(cs_mad(y)), *more_x)
+
+
+def cs_mad_rank(y: Expr) -> Expr:
+    """常用功能简化封装。去极值，排名。
+
+    适合于分层收益V型或倒V的情况"""
+    return cs_rank(cs_mad(y))
+
+
+def cs_mad_rank2(y: Expr, m: float) -> Expr:
+    """非线性处理。去极值，排名，移动峰或谷到零点，然后平方
+
+    适合于分层收益V型或倒V的情况"""
+    return (cs_rank(cs_mad(y)) - m) ** 2
+
+
+def cs_mad_rank2_resid(y: Expr, m: float, *more_x: Expr) -> Expr:
+    """非线性处理。去极值，排名，移动峰或谷到零点，然后平方。回归取残差
+
+    适合于分层收益V型或倒V的情况"""
+    return cs_resid((cs_rank(cs_mad(y)) - m) ** 2, *more_x)
+
+
+def cs_rank2(y: Expr, m: float) -> Expr:
+    """非线性处理。移动峰或谷到零点，然后平方
+
+    适合于分层收益V型或倒V的情况"""
+    return (cs_rank(y) - m) ** 2
```

### Comparing `polars_ta-0.2.3/polars_ta/wq/transformational.py` & `polars_ta-0.2.4/polars_ta/wq/transformational.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return _rank_qcut(x, q)
 
 
 def clamp(x: Expr, lower: float = 0, upper: float = 0, inverse: bool = False, mask: float = None) -> Expr:
     """Limits input value between lower and upper bound in inverse = false mode (which is default). Alternatively, when inverse = true, values between bounds are replaced with mask, while values outside bounds are left as is."""
     if inverse:
         # mask is one of: 'nearest_bound', 'mean', 'NAN' or any floating point number
-        return when((lower < x) & (x < upper)).then(mask).otherwise(x)
+        return when((x < lower) | (x > upper)).then(x).otherwise(mask)
     else:
         return x.clip(lower, upper)
 
 
 def filter_(x: Expr, h: str = "1, 2, 3, 4", t: str = "0.5") -> Expr:
     """Used to filter the value and allows to create filters like linear or exponential decay."""
     raise
@@ -41,53 +41,47 @@
 def keep(x: Expr, f: float, period: int = 5) -> Expr:
     """This operator outputs value x when f changes and continues to do that for “period” days after f stopped changing. After “period” days since last change of f, NaN is output."""
     raise
 
 
 def left_tail(x: Expr, maximum: float = 0) -> Expr:
     """NaN everything greater than maximum, maximum should be constant."""
-    return when(x > maximum).then(None).otherwise(x)
+    return when(x <= maximum).then(x).otherwise(None)
 
 
 def pasteurize(x: Expr) -> Expr:
     """Set to NaN if x is INF or if the underlying instrument is not in the Alpha universe"""
     # TODO: 不在票池中的的功能无法表示
     # TODO: 与purify好像没啥区别
-    return when(x.is_infinite()).then(None).otherwise(x)
+    return when(x.is_finite()).then(x).otherwise(None)
 
 
 def purify(x: Expr) -> Expr:
     """Clear infinities (+inf, -inf) by replacing with NaN."""
-    return when(x.is_infinite()).then(None).otherwise(x)
+    return when(x.is_finite()).then(x).otherwise(None)
 
 
 def fill_nan(x: Expr) -> Expr:
     """fill nan by null
     填充nan为null"""
     return x.fill_nan(None)
 
 
-def fill_infinite(x: Expr) -> Expr:
-    """fill infinite by null
-    填充 +inf, -inf为null
-
-    Notes
-    -----
-    如果要对多列进行处理，需要在所有表达式最后添加`.name.keep()`，由于这不是最后一列，所以只能注释
-    """
-    return when(x.is_infinite()).then(None).otherwise(x)  # .name.keep()
+def fill_zero(x: Expr) -> Expr:
+    """填充null为0"""
+    return x.fill_null(0)
 
 
 def right_tail(x: Expr, minimum: float = 0) -> Expr:
     """NaN everything less than minimum, minimum should be constant."""
-    return when(x < minimum).then(None).otherwise(x)
+    return when(x >= minimum).then(x).otherwise(None)
 
 
 def sigmoid(x: Expr) -> Expr:
     """Returns 1 / (1 + exp(-x))"""
     return 1 / (1 + (-x).exp())
 
 
 def tail(x: Expr, lower: float = 0, upper: float = 0, newval: float = 0) -> Expr:
     """If (x > lower AND x < upper) return newval, else return x. Lower, upper, newval should be constants. """
     # TODO 与clamp一样?
-    return when((lower < x) & (x < upper)).then(newval).otherwise(x)
+    return when((x <= lower) | (x >= upper)).then(x).otherwise(newval)
```

### Comparing `polars_ta-0.2.3/polars_ta.egg-info/PKG-INFO` & `polars_ta-0.2.4/polars_ta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.3
+Version: 0.2.4
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,16 @@
         
 Keywords: polars,expression,talib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: polars>=0.20.7
+Requires-Dist: polars>=0.20.19
+Requires-Dist: polars-ols>=0.3.0
 Requires-Dist: numpy
 Requires-Dist: numba
 Requires-Dist: pandas
 Provides-Extra: talib
 Requires-Dist: TA-Lib; extra == "talib"
 
 # polars_ta
```

### Comparing `polars_ta-0.2.3/polars_ta.egg-info/SOURCES.txt` & `polars_ta-0.2.4/polars_ta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.3/pyproject.toml` & `polars_ta-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 keywords = ["polars", "expression", "talib"]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python"
 ]
 dependencies = [
-    "polars>=0.20.7",
+    "polars>=0.20.19",
+    "polars-ols>=0.3.0",
     "numpy",
     "numba",
     "pandas",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

