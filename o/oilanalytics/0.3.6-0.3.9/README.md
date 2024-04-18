# Comparing `tmp/oilanalytics-0.3.6.tar.gz` & `tmp/oilanalytics-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oilanalytics-0.3.6.tar", last modified: Mon Nov  6 12:02:12 2023, max compression
+gzip compressed data, was "oilanalytics-0.3.9.tar", last modified: Wed Nov 15 16:11:12 2023, max compression
```

## Comparing `oilanalytics-0.3.6.tar` & `oilanalytics-0.3.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.557622 oilanalytics-0.3.6/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/notebooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.557622 oilanalytics-0.3.6/oilanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.557622 oilanalytics-0.3.6/oilanalytics/balances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/balances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/balances/balance_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/balances/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/balances/global_oil_balances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/balances/key_agency_comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.557622 oilanalytics-0.3.6/oilanalytics/eia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/eia/eia.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/eia/monthly_drilling_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/eia/steo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/eia/weeklypetreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/energyaspects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/energyaspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/energyaspects/china_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/energyaspects/europe_diesel_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/energyaspects/fsu_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/energyaspects/tars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/euroilstock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/euroilstock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/euroilstock/euroilstock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/geo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/highfreq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/highfreq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/highfreq/ara.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/highfreq/singapore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/iea/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/iea/omr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/jodi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/jodi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/jodi/jodiapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/opec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/opec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/opec/momr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/prices/futures_prices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/oilanalytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/utils/chartutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/utils/eikonutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/oilanalytics/utils/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.557622 oilanalytics-0.3.6/oilanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-06 12:02:12.000000 oilanalytics-0.3.6/oilanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-11-06 12:02:12.000000 oilanalytics-0.3.6/oilanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 12:02:12.000000 oilanalytics-0.3.6/oilanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-06 12:02:12.000000 oilanalytics-0.3.6/oilanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-06 12:02:12.000000 oilanalytics-0.3.6/oilanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 12:02:12.561622 oilanalytics-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_ea_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_eia.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_eia_weekly_rep.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_futures_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_highfreq.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_iea.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_key_agency_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-06 12:01:59.000000 oilanalytics-0.3.6/test/test_opec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/notebooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/balances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/balances/balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/balances/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/balances/global_oil_balances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/balances/key_agency_comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/eia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/eia/eia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/eia/monthly_drilling_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/eia/steo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/eia/weeklypetreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/energyaspects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/energyaspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/energyaspects/china_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/energyaspects/europe_diesel_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/energyaspects/fsu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/energyaspects/tars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/euroilstock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/euroilstock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/euroilstock/euroilstock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/highfreq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/highfreq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/highfreq/ara.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/highfreq/singapore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/iea/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/iea/omr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/jodi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/jodi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/jodi/jodiapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/opec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/opec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/opec/momr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/prices/futures_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/oilanalytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/utils/chartutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/utils/eikonutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/oilanalytics/utils/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.163458 oilanalytics-0.3.9/oilanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-15 16:11:12.000000 oilanalytics-0.3.9/oilanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-11-15 16:11:12.000000 oilanalytics-0.3.9/oilanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 16:11:12.000000 oilanalytics-0.3.9/oilanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-15 16:11:12.000000 oilanalytics-0.3.9/oilanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-15 16:11:12.000000 oilanalytics-0.3.9/oilanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:12.167458 oilanalytics-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_ea_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_eia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_eia_weekly_rep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_futures_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_highfreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_iea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_key_agency_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-15 16:11:03.000000 oilanalytics-0.3.9/test/test_opec.py
```

### Comparing `oilanalytics-0.3.6/oilanalytics/balances/balance_utils.py` & `oilanalytics-0.3.9/oilanalytics/balances/balance_utils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/balances/global_oil_balances.py` & `oilanalytics-0.3.9/oilanalytics/balances/global_oil_balances.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/balances/key_agency_comparisons.py` & `oilanalytics-0.3.9/oilanalytics/balances/key_agency_comparisons.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/eia/eia.py` & `oilanalytics-0.3.9/oilanalytics/eia/eia.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/eia/monthly_drilling_report.py` & `oilanalytics-0.3.9/oilanalytics/eia/monthly_drilling_report.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/eia/steo.py` & `oilanalytics-0.3.9/oilanalytics/eia/steo.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/eia/weeklypetreport.py` & `oilanalytics-0.3.9/oilanalytics/eia/weeklypetreport.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,16 @@
     df = excel_scraper.read_table(
         canada_importa_file_loc, sheet_name="Data 1", skiprows=(0, 2), index_col=0
     )
     return df
 
 
 def modify_level(level0, level1):
-    return [
-        item + "_4wa" if "4-Week Avg" in level1[i] else item
-        for i, item in enumerate(level0)
-    ]
+    return [item + "_4wa" if i < len(level1) and "4-Week Avg" in level1[i] else item for i, item in enumerate(level0)]
+
 
 
 def read_release_date(fileloc):
     ex = excel_scraper.read_excel_file(fileloc)
     d = ex.parse("Contents")
     ind_row = 27
     ind_col = 2
```

### Comparing `oilanalytics-0.3.6/oilanalytics/energyaspects/china_stats.py` & `oilanalytics-0.3.9/oilanalytics/energyaspects/china_stats.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/energyaspects/europe_diesel_balance.py` & `oilanalytics-0.3.9/oilanalytics/energyaspects/europe_diesel_balance.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/energyaspects/fsu_stats.py` & `oilanalytics-0.3.9/oilanalytics/energyaspects/fsu_stats.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/energyaspects/tars.py` & `oilanalytics-0.3.9/oilanalytics/energyaspects/tars.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/euroilstock/euroilstock.py` & `oilanalytics-0.3.9/oilanalytics/euroilstock/euroilstock.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/highfreq/ara.py` & `oilanalytics-0.3.9/oilanalytics/highfreq/ara.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/highfreq/singapore.py` & `oilanalytics-0.3.9/oilanalytics/highfreq/singapore.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/iea/omr.py` & `oilanalytics-0.3.9/oilanalytics/iea/omr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/opec/momr.py` & `oilanalytics-0.3.9/oilanalytics/opec/momr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/prices/futures_prices.py` & `oilanalytics-0.3.9/oilanalytics/prices/futures_prices.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics/utils/chartutils.py` & `oilanalytics-0.3.9/oilanalytics/utils/chartutils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/oilanalytics.egg-info/SOURCES.txt` & `oilanalytics-0.3.9/oilanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/setup.py` & `oilanalytics-0.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="oilanalytics",
-    version="0.3.6",
+    version="0.3.9",
     author="aeorxc",
     description="Utilities for oil analytics",
     url="https://github.com/aeorxc/oilanalytics",
     project_urls={
         "Source": "https://github.com/aeorxc/oilanalytics",
     },
     packages=setuptools.find_packages(),
```

### Comparing `oilanalytics-0.3.6/test/test_eia.py` & `oilanalytics-0.3.9/test/test_eia.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.6/test/test_highfreq.py` & `oilanalytics-0.3.9/test/test_highfreq.py`

 * *Files identical despite different names*

