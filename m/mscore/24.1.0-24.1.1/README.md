# Comparing `tmp/mscore-24.1.0.tar.gz` & `tmp/mscore-24.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscore-24.1.0.tar", last modified: Fri Mar 29 16:18:02 2024, max compression
+gzip compressed data, was "mscore-24.1.1.tar", last modified: Thu Apr 18 15:35:15 2024, max compression
```

## Comparing `mscore-24.1.0.tar` & `mscore-24.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.515972 mscore-24.1.0/
--rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-03-29 16:18:02.515972 mscore-24.1.0/PKG-INFO
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7917 2024-03-11 14:02:27.000000 mscore-24.1.0/README.md
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.491972 mscore-24.1.0/mscore/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1224 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       84 2024-03-11 14:02:27.000000 mscore-24.1.0/mscore/__main__.py
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2324 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/activate.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.495972 mscore-24.1.0/mscore/data_variables/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      154 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/data_variables/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20530 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/data_variables/hcc_descriptors.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8462 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/data_variables/hierarchies.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    22046 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/data_variables/variable_dict.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    16379 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/demography_builder.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7889 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/demography_vars_applicator.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    14916 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/file_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8819 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/hcc_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     9761 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/ram_models.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.487972 mscore-24.1.0/mscore/reference_data/
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.503972 mscore-24.1.0/mscore/reference_data/Crosswalks/
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110293 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2221CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110523 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2222CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   121889 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2223CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   112657 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2224CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   111973 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2421CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   112169 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2422CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   124500 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2423CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   115090 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2424CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   100809 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/Crosswalks/F2824CW.TXT
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.511972 mscore-24.1.0/mscore/reference_data/Model_Coefficients/
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-11-03 17:05:55.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-11-03 17:05:55.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    24329 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.511972 mscore-24.1.0/mscore/reference_data/application_tables/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1572021 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/application_tables/application_format_fact.parquet
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    68902 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/application_tables/application_model_coefficient.parquet
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     3585 2024-03-11 13:53:36.000000 mscore-24.1.0/mscore/reference_data/application_tables/application_model_dimension.parquet
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.511972 mscore-24.1.0/mscore/reference_data/model_formats_all_columns/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   663610 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   680986 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1088405 2023-06-23 19:57:48.000000 mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    15685 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/scoring_handler.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.515972 mscore-24.1.0/mscore/utilities/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      941 2024-03-29 16:18:00.000000 mscore-24.1.0/mscore/utilities/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    10798 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/authentication.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     6665 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/utilities/cli.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     4164 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/context.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2015 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/data_models.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    11087 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/data_validation.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1969 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/utilities/file_organizer.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8359 2024-03-29 16:17:59.000000 mscore-24.1.0/mscore/utilities/licensing.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2252 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/log_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2098 2024-03-29 16:18:01.000000 mscore-24.1.0/mscore/utilities/user_models.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-03-29 16:18:02.515972 mscore-24.1.0/mscore.egg-info/
--rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/PKG-INFO
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2611 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/SOURCES.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        1 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/dependency_links.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       52 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/entry_points.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       81 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/requires.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        7 2024-03-29 16:18:02.000000 mscore-24.1.0/mscore.egg-info/top_level.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1192 2024-03-29 16:10:33.000000 mscore-24.1.0/pyproject.toml
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       38 2024-03-29 16:18:02.515972 mscore-24.1.0/setup.cfg
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/
+-rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-04-18 15:35:15.478664 mscore-24.1.1/PKG-INFO
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7917 2024-03-11 14:02:27.000000 mscore-24.1.1/README.md
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.462657 mscore-24.1.1/mscore/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1239 2024-04-18 15:32:27.000000 mscore-24.1.1/mscore/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       84 2024-03-11 14:02:27.000000 mscore-24.1.1/mscore/__main__.py
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2319 2024-04-18 15:32:48.000000 mscore-24.1.1/mscore/activate.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.466658 mscore-24.1.1/mscore/data_variables/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      149 2024-04-18 15:33:20.000000 mscore-24.1.1/mscore/data_variables/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20525 2024-04-18 15:33:28.000000 mscore-24.1.1/mscore/data_variables/hcc_descriptors.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8457 2024-04-18 15:33:49.000000 mscore-24.1.1/mscore/data_variables/hierarchies.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    22040 2024-04-18 15:33:32.000000 mscore-24.1.1/mscore/data_variables/variable_dict.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    16374 2024-04-18 15:32:40.000000 mscore-24.1.1/mscore/demography_builder.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7883 2024-04-18 15:33:15.000000 mscore-24.1.1/mscore/demography_vars_applicator.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    14910 2024-04-18 15:32:52.000000 mscore-24.1.1/mscore/file_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8814 2024-04-18 15:32:32.000000 mscore-24.1.1/mscore/hcc_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     9755 2024-04-18 15:32:56.000000 mscore-24.1.1/mscore/ram_models.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.462657 mscore-24.1.1/mscore/reference_data/
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.466658 mscore-24.1.1/mscore/reference_data/Crosswalks/
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110293 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2221CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110523 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2222CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   121889 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2223CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   112657 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2224CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   111973 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2421CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   112169 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2422CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   124500 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2423CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   115090 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2424CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   100809 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2824CW.TXT
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/Model_Coefficients/
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-11-03 17:05:55.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-11-03 17:05:55.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    24329 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/application_tables/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1572021 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_format_fact.parquet
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    68902 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_model_coefficient.parquet
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     3585 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_model_dimension.parquet
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   663610 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   680986 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1088405 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    15680 2024-04-18 15:32:35.000000 mscore-24.1.1/mscore/scoring_handler.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/mscore/utilities/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      935 2024-04-18 15:34:06.000000 mscore-24.1.1/mscore/utilities/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    10793 2024-04-18 15:34:29.000000 mscore-24.1.1/mscore/utilities/authentication.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     6659 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/cli.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     4159 2024-04-18 15:35:02.000000 mscore-24.1.1/mscore/utilities/context.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2010 2024-04-18 15:34:34.000000 mscore-24.1.1/mscore/utilities/data_models.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    11082 2024-04-18 15:34:45.000000 mscore-24.1.1/mscore/utilities/data_validation.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1964 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/file_organizer.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8354 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/licensing.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2247 2024-04-18 15:34:24.000000 mscore-24.1.1/mscore/utilities/log_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2093 2024-04-18 15:34:19.000000 mscore-24.1.1/mscore/utilities/user_models.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/mscore.egg-info/
+-rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/PKG-INFO
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2611 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/SOURCES.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        1 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/dependency_links.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       52 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/entry_points.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       81 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/requires.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        7 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/top_level.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1192 2024-04-18 15:23:53.000000 mscore-24.1.1/pyproject.toml
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       38 2024-04-18 15:35:15.478664 mscore-24.1.1/setup.cfg
```

### Comparing `mscore-24.1.0/PKG-INFO` & `mscore-24.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscore
-Version: 24.1.0
+Version: 24.1.1
 Summary: MScore: Risk Scores Made Easy
 Home-page: https://github.com/elevendatacorp/mscore.git
 Author: RAM Development Team
 Author-email: RAM Development Team <dev@riskadjustmentmodel.com>
 Project-URL: Homepage, https://riskadjustmentmodel.com/mscore-product
 Project-URL: Bug Tracker, https://github.com/elevendatacorp/mscore/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mscore Version: 24.1.0 Summary: MScore: Risk Scores
+Metadata-Version: 2.1 Name: mscore Version: 24.1.1 Summary: MScore: Risk Scores
 Made Easy Home-page: https://github.com/elevendatacorp/mscore.git Author: RAM
 Development Team Author-email: RAM Development Team
 riskadjustmentmodel.com> Project-URL: Homepage, https://
 riskadjustmentmodel.com/mscore-product Project-URL: Bug Tracker, https://
 github.com/elevendatacorp/mscore/issues Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: pandas Requires-
```

### Comparing `mscore-24.1.0/README.md` & `mscore-24.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/__init__.pye` & `mscore-24.1.1/mscore/__init__.pye`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhRMRbXQ]dEE5Wh=$I`TdD$=p5$S="
-GhN1)"/5XRB!@*+8B3)tO@5"=gtJZu
+GhN16"-i_EB!@*+8B3)cO@5"=gtJZu
 $6oDNn(kHEb!oO2&*.^rjTlY0Va0St
 6'([qq]n9lj3#%qfoH^gVPaUj`_o$U
 .lgVa.=-DT*$0o8]Bi5W&^S.i^,^R)
 ?%k0uHQ1iCWo*IG)>oTUNH?MVC'H:b
-*1&qcPSg&DNgUI`.@cBo2Tjo3jMZk]
+*1&qcPSg&DNgUIa.@cBo2Tjo3jMZk]
 p0'<jAEON<hH=-=.<uCL+./f\$k&ll
 5;Jd4((/5kX-b"?n83Uh_)Bs-n9/YZ
 PgJ:9"V1?g,/(&XK<&m(KN,QRRJlKp
 oH/G:CARoa2-XqIVUsibTA;KeLN4;l
 VS+m_MHUhj`b3t3PkkgZOS:O'N9,M.
 16_^t(N;iPWNoElLCd]4:j(j`=!mu>
 @$8^7E,m&Fp_7PE14%I%h\N!uN$Jk"
@@ -26,15 +26,15 @@
 Q<f>ZZ-J*TntSh$@&Z+MkEdi_eT5IK
 Va^\roiF[PB%_"j$iJ@Q/14/,fnU62
 A=OfEe_b.,EpXCF]l%5'+/l@HQish"
 oROXR9R@r,G&*tdD,0Vq;"cRsRFE%k
 1b"*U>NHNj:jDrlA?Da!B;OFDi'DhZ
 m&msJ%cc2tMsJFGD-=>.-Xq$[!jp#q
 ['o;mNY\3)*jT;@4)1*<`S*8gBtoJg
-EJo.glOju6K`:$`/79\6W>tHf01TB(
-Lb=K+@V+_05Jl:1SDcS)2KoL5_7F+Z
-n[TQ=\b(e=^qDk#d3A-dTP*\g)@<oJ
-4BpE55pB\q0'J#r"?NYa%*A%E\R0J)
-UY%;Z<+4`P_F2U;L<=Hp4E$g`lWHgQ
-+d@udP':#,JGgfJjm&6n/Dh#QhI36d
-IZ5,UW]#R6h>dNU
+EJo.glOjusL&C'6,U##ZW%bmF-;n*(
+gh3PfDKt+Y?EsFGRd>MG*dAWKa/a+i
+kE'sfY4\'#jK:P4cthr:VL,VU7iB$f
+4^H)q80Vq%0`@Id*Hd9:'@X7O]hEo8
+Un'Q"6"c!efgs$egQ,/m.W=I/\PQ#3
+.Cb-&Ncl+DT82Jerhc>7.G$&GbAOCI
+eX7+$prN49QP%FJa8"d%rIU:f[eg%)
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/activate.pye` & `mscore-24.1.1/mscore/activate.pye`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhQA+]%H'4j8/jI2qe12^=muT!)i\#g].<S
-GhN2$##Y2O+;l8u8C']%S#[F-ns>E0lNZ5k
+GhN1u#$(JS+;l8u8C']%S#[F-ns>E0lNZ5k
 >qRmh8)9i2<LII4l,p`%P0Ki_</sfX3:H6`
 %.ORmVKT&J_G.rcO?W^pI0/#gJJ!!JVSeAL
 "I\2hrh!K*ikN*<Yu*Z[@:sl5*$s(o#ihR6
 s&$U!QCk]!]DJ208-21bUlllEI\m,Rj"rRi
 &>YU:?gOE!dR\7<%ON0ur&NiWk:Gp@'91]4
 3-[7[j*>#EKHM[`=8g8+bR!-A(\='@rZbFZ
 8br.#.D.i>TIoo%nP,Feer82W:=Mc#biDdT
@@ -57,9 +57,9 @@
 2Ig@NMGfJob"YASKa`)^I6^1V&V-HR8`Kce
 <!6K^bqaqS5I,GRTj]7so08li^fZdq.f5'<
 c)CnXA!dQJ*_4)Ok6^a4Wi,3"#E4'TII-Jt
 c]p]u=SC&a\=H]aRGt^=KVg6PUVFRoV<j!/
 i,E$;s$4M#BE[D0EQ((D6BMktDVsBbJe""i
 4Dd"]N#QuZ0<9X_][*^tjRA`u2k=YT.X=V8
 ^WM!I#(&_gUiC<VeDL!:.f</\^m]d3A\T^D
-END0d8luTnGU*]*4TGH^
+END0dKV^V7;?-[s
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/data_variables/hcc_descriptors.pye` & `mscore-24.1.1/mscore/data_variables/hcc_descriptors.pye`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhV1[SX-t)/[p)+rkUJh*eY@2!'UMja8c2?
-GhN0!55rBb&1GNW[YnYE:dnsD\rRfhm/qF\
+GhN2s4T`Ke&1GNW[YnYE:dnsD\rRfhm/qF\
 $QK#"o6#u(9rL#UD1V!:6:4J%A7*W9&RZqb
 RBZ^1be7_m3oiF/<^6R&XSF;0"b<3p3+9S$
 eFRckD-e)_2DT7f,n`8DJ5F4ZVnCsN%I*Lu
 ;C=u1bVU\^LUpolp^feL6.luEf+$Q_`q!7.
 j+5IfnJ>HId)a2-Ie`%cRP_(9=EkV,LhT2f
 6/YF6OPXY]L%BIBH!.9S'[0YA./CX12+8ZP
 m+=MtPWM=Wd(s!g2HDndm5FBK]^DdJCe.Eh
@@ -562,10 +562,10 @@
 "'*g5=*I3lY$'rQO%N<8F+lQ?5;DLe/P-u%
 C;?#/'6L%^RgajdY*JTWTo1gd1!hjji_>*%
 dZ32*`4$g-_PKn4h`\p!#5/RE@0>nbj\EC'
 ^#(j(U`OO4q>+:PhK>'n2\4T%>'A\0#>'e)
 m2.GPQEGM%V<E3Vgf(`@,`Q=5W>`1cGZ>fl
 R;/"R?e_IgHZ4A4m;O]Lj?S1O$TAFS,@<^9
 \7ujXK$nt['?%jIj%R;'7[(F4ku4[0W"u$U
-9h\65`pt"[64;h^$#t5[P+$.5N-J>4mVhq%
-mKnm?qeF,]
+9h\65`pt"[64;h^$#t5[P+$.5N-J>4mVhsI
+k%2KI
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/data_variables/hierarchies.pye` & `mscore-24.1.1/mscore/data_variables/hierarchies.pye`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhQqrH23GNGD>q@)!A+p7a,!83k,A_
-GhN0e)7nth&1Hj6^BaJ$e[R.5V@HR'
+GhN0a)8>7l&1Hj6^BaJ$e[R.5V@HR'
 @C.n`(H.Qa"(B:jDO-:g^2lWRn[4_P
 9ZoC!Q#'ruI=>EWIX+nWFN8$8naama
 7nt:ZDgB\\fF9(0\H/5!In$,__iL!=
 *s=ZgZ#pHF6EesqTOLF$EHpV?BE51B
 `.k6Rq[1%&6k[TYBVT78MNV"#UJ98Q
 jOpn\/),;e08#PQ0;5aD)Y9Gb[-+c-
 :q*.:=9Q(.8X4`4<Po*OJ.06G#1i[/
@@ -265,9 +265,9 @@
 %R4X%ggfacTh.+1[t+';UGV`gq++D:
 p(/@<Q,lpT]!?]X;RmXA4q<LjfUUI.
 %pCmp1+jUo.pqEN@8UPI/+*66?;+.7
 ql@-%3-R,<a)]ch-uXpS6+iIMc&/Qt
 L3RU)ke98shj8khc4?sgK6Cgi/7Lf7
 ;t3(ND31[BEHeOub:KP#iX'&KMt*EZ
 dqAB>q.sjK*=&!Ce_+rW=sV<"%9Wo9
-<P@%mXDpi(E(gFV1F0Lr0]iTR-'2qD
+<P@%mXDpi(E(gFV1F0MkFd6`a
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/data_variables/variable_dict.pye` & `mscore-24.1.1/mscore/data_variables/variable_dict.pye`

 * *Files 2% similar despite different names*

```diff
@@ -679,15 +679,15 @@
 T%>BN[Y0KW.aI`XA%<1Lj$@_kQc>1b
 he*..aBA\8@.1-3<Xlah-ZrK!10[fT
 A?KGRd@I'-WSPUucP(JA:#a>n++0^A
 !/*BkOMXmITpRhCDE\Gj?b)86/^,a\
 Hjd>db8;<pY`e4rf](siSAj@o*Z=)s
 ZHn57B2i6N4<:\V?r=CHs8>[*fo3k(
 ]`gN?"cg&\pt0_EF+(f[8,e+-n(@F%
-4NVXn-l'm(!D*@$rV#6c2m(*1e0*pk
+4NVXn-l'm(!C[($rV#6c2m(*1e0*pk
 (b/i@h$@`,04g-!n')'34"jBDWYa.8
 ?Edt(\l:TL1#.UAc4"p<CRgX5r1dp_
 gtGJ:ARX>8)tMHt.)eXums<7M6%$@J
 QPi_)$7[:OahQJ%b)K:,L1Z]?'4KWu
 >KdJmYhc[&.<&NtImBjq]BteE\e7UO
 g<+[JNW_`m#jln;_7QS%[N:Au01t()
 fjH&!9Vjel"k$LY6INm;Zk4_@'b>-d
@@ -703,10 +703,9 @@
 Vedtk-Bi.&OMm^[$o=Z^El>0Xg:6nj
 T;i0jHn\O::O0Bi=P6MR::Pjo,rRn,
 [>m+nBa-[j0g7r:H$eot&q2DPEOdC$
 LumbG)i?<"5;jV?;#.BaESZ&%Ik5#u
 e9+-gB3o"_m$%.aU$tncBe]cH-,Gu1
 kQB;lV4k:eI)LH9'3LWYLI[]M4%)ak
 SqeEpGGt[ro!H/$$+Y+!NRY"@RMdQ4
-.7NMU?Q%\tCtk(o@-a[QiEA[K*/_`8
-mo9>f
+.7NMU?Q%\tCtk(o@-a[QiKO^.mJHqa
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/demography_builder.pye` & `mscore-24.1.1/mscore/demography_builder.pye`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhQB?p:Y+al%N&@fTP]p'45G\!(`ag'`\46
-GhN100q-Be-Lq)%cWrT'G.C_+>0rBPI/1c1
+GhN1,0qQZi-Lq)%cWrT'G.C_+>0rBPI/1c1
 H'K[(3aiX]@O%poA(lOoOu"NQ>-`!il&7#`
 DY?^5;sRK4M*&Z(!aj[5ntUd:pT]&_9N>Eb
 SnP0"(M<Nn;q=TR&UmQ1OE+a&T@m8g.VR5e
 &T(0-nHHDGWClS!Ej&!maS9&]P!Bdbo"lKb
 gGb&lqdiHdksRpu[]/+@!(Yk>jA]3EhJ0.X
 S.epRUE=-H8BuN#j?n^Gf68QEO1+H"/%6)%
 _]7tl3Nup=`T4N&SqF%Q/Z[l*aN%Z4ZU)Tm
@@ -447,9 +447,9 @@
 <Lc.j><S,P=i5^CO=k^qf;[=8[.S<$oKL>$
 G2_8W<e'oIq0@n?dPiY(8-+8$Q0Z*^\bPa]
 \IJ`W\U'Sq7_[6H2-9%mbrB(g.\^oe1M%ou
 SAedakBB&ug@Rd5i)XqtGFE+W>_\>mLi9o:
 F,Ar"$pCL^VY/@l^'GCVSn&HY8@HU-Qa<!?
 %l%K2dbg>;3`Ff,!1-PZGM1CUm0S:\;K"<&
 ,OXF9b>!Xufp;f76gCFKha[9Jld=UkSukJS
-W(2Va3=6#D`om4^MqXM+O=NM/,B,#Y.7TZ`
+W(2Va3=6#D`om4^MqXM+O=NMmbQO6r
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/demography_vars_applicator.pye` & `mscore-24.1.1/mscore/demography_vars_applicator.pye`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhQBaH?X,(D9mttCK#%*S/.Ck!(a!n-NF,H
-GhN1d(M;m6nW+&QH:hffVMs>qR132.i1FYP
+GhN1`(M`0:nW+&QH:hffVMs>qR132.i1FYP
 EfFSYn\g)5QFSZkXIrjG!"U48h,Sm1:'%Cg
 b=Op*kh'H/<j34Mlg1mBkqL9+V@g<`DRr1B
 HR(3*r&(E\-Upn$q[#&Yrr/>*G0)qir]SWp
 BmS)`pMYiR"',ESruhUn1FB#(#o1?Q/mTAO
 [BQ1AZhTl25)Mso+%BC]3lOl?YTf%_GjB&*
 ;IL?YBAOg+<,"BAs')b+LNNZsJX0-=-!-0e
 9b5hcgE#IY'#Z4m_2&F<,e-NoAUt'fQd'o+
@@ -211,10 +211,9 @@
 O#_LtBdh;_P-.9ss*CqN69c!p)1B9c]H;nj
 R]s5$<^;bb2lPd:l8XV1rPh5(pKh,GB7qqs
 <Hj.^">moB\+<R9hW+KGFE>2j'uuk;0>t+0
 MBq9He_+agZJOR4f.d];US'NZF"kRt-Xh'V
 Igh7hOQ%$X3?!%X-+(n(Ac-CWBr2Bj5Q22"
 h"LrA[MgGRcbpd\gRc#;+\YTbZ(r@DE<1`S
 -g!L%7.>9Mk>@H.[,mesSQT@hedQ5:?(!fk
-VDbqX5":BaKj@+NP!MeeZ7a"Dif$\$!>Tjj
-iapS:
+VDbqX5":BaKj@+NP!MeeZ7a"Dif$YUQW;Eq
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/file_handler.pye` & `mscore-24.1.1/mscore/file_handler.pye`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhV3"rOk>!eG(&VCjEX-:WFCS44=F;
-GhN2</320C)smmIPbU56H"A@D<s*BF
+GhN28/3VHG)smmIPbU56H"A@D<s*BF
 QIqfpMh0UhgF<p(O2ELgbFFgD@$[Om
 o/%^pSl(T1$#YQBD[.$)g.e>?@%S?Y
 CjN:s%ZY*'4+h@;&CVX*$^tD]YAVK*
 55,X]r;.c7l&G7La-75:8oVu*!AY^%
 O*X]!Z_\2ec3I%b_Os.H>pj'N'm`p=
 `ksV/jhj8%-MH-_"hSp4T@ZN$Pu%^F
 J=3M,o6Iq^B>*]?Q9)Zr&Woj8K.C8a
@@ -473,10 +473,9 @@
 M\b)oI$'"#r@K=(VU^"Vf-Xe'_q$mL
 aNllg05p.[-T.'jZteD/`!hMC%*uWb
 "'mIXN;mMTW8=k0__dkm2k91F7B6fX
 \uWH(-_!G40ia6`5'N>'`!)dZ`rnu:
 2,6E"*GmI'&R(=Y'+?u[UX*Z`hp':4
 *NbkHQ\'Rbp5TAS*"5<2I]DUQ2[f.g
 K9Klhj4Lj5ge5N(G<49nJhZ3t/cp(U
-S(?@c$LoG<rHob/UsJ(i6Q(l96<FUe
-:B1@p
+S(?@c$LoG<rHob/UsJ(iNAY3:/cYkO
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/hcc_handler.pye` & `mscore-24.1.1/mscore/hcc_handler.pye`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhP5=qc*9L^stO`3R^X5V"G&p8#-A_
-GhN1")Q;c"-<WM<>eG2W]?L:I;3]dT
+GhN0s)Q`&&-<WM<>eG2W]?L:I;3]dT
 IdmIDq$k2BeYpk#8]BgajGsT)0!S.E
 o6sj2`#t:[CY4ZaN)4>FQ]u=X(X#aj
 [gP2Z`58;c$BKE.$R+$K9-7mN_ZDdu
 @nVcKamlOp\$O]k?ZkS^^=YSIZ@D*0
 ;,1U_LOhkUn'3,(foe;H8X&ji89&O9
 i_L@njhPtq_S-r[Q\9af4C=namQdP5
 :F":Tka#7t`H2]JSucBb-)ZZUp=b6C
@@ -277,9 +277,9 @@
 dIMF'k!<d7&fm:eqDt'Xb.X/^1*in?
 /UH/B5iq7F"H_d/.G^nfk1X(k``8Qm
 BXOYnC!d`B</u`mk!jNQCPEk!eB`EN
 BXf8F$i`4fU"1cGGl[B;>!!!64#9W0
 _2pkS8cY$&GlDg<P)/I6\CN]PEU[[A
 Lsb/Y9!Z3I4=H9#ZP*!oC2YgbK=F6i
 bdY-&]d=@X[CEFL_gTaC2ZVLHrk13p
-L=U\?9KE#R*Amfs
+L)>aC)Me@n
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/ram_models.pye` & `mscore-24.1.1/mscore/ram_models.pye`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhW&dkGeETHD,W@DVO$TR+4e0!*+[XZ2ak)
-GhN0h*Ok$\$WDgA;f]%@76p))9$Sf3m=+@T
+GhN0d*P:<`$WDgA;f]%@76p))9$Sf3m=+@T
 Q?*50#B@7ulW.g^IQ<&`]^JlIKs07339j5-
 RoQSY\/1qW%tk6i0/6'+>Z9?CW\2Ll\dhtA
 [g9U#$5)m3"@PNgFGXZGihj&R!4fO:$lW7O
 :Be6M.-4loH`a5m$]4)#JE35)aXK#L)b-d%
 .Jg_:*7j=`)>4lW5,nT:JE<3TTe`&DC+OtO
 \GYTlV.ok*n\]EIP3ff\^I\(.$g5'JqfRpG
 m`/Y/97Go#6-aJ?B=X<Hb;>j@??Emq]I/-L
@@ -263,10 +263,9 @@
 TTr;pY?EA4k-4DR=j*+'\%%GMkA6O7"gA$R
 B_]N@"Pk*B!UGRVPl!UbF6Xui`J5GZCkP/r
 IfrL:`V'@rph16P0#?k_<cg*"?qm_P$4HY8
 R8>JNQPlZ9&H:UP<.(jK.JO]cqmRMgV!I%=
 aClTVr@1>_Jq<QOkBZ*.\'\F-E8q'U\J[N#
 bk\]fo+IBYNa?@7<jg=R#]/U>LN[D)g"2^`
 9%Q^nDXHc("eco'-&%ajpWMeKej.Q,YFbuC
-9@Gs#;a.mgrkhG7LoUNFcG`LCocrhCj'AQp
-)P`Pt
+9@Gs#;a.mgrkhG7LoUNFcG`LCock[7@A"YA
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2221CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2221CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2222CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2222CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2223CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2223CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2224CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2224CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2421CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2421CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2422CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2422CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2423CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2423CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2424CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2424CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Crosswalks/F2824CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2824CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/application_tables/application_format_fact.parquet` & `mscore-24.1.1/mscore/reference_data/application_tables/application_format_fact.parquet`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/application_tables/application_model_coefficient.parquet` & `mscore-24.1.1/mscore/reference_data/application_tables/application_model_coefficient.parquet`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/application_tables/application_model_dimension.parquet` & `mscore-24.1.1/mscore/reference_data/application_tables/application_model_dimension.parquet`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/mscore/scoring_handler.pye` & `mscore-24.1.1/mscore/scoring_handler.pye`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhNO;f)!#CGkr,*f[>guZWh\U4YI%"
-GhN0=0B1@<*d/B!Z0FIJcM\!EI;p'u
+GhN090BUX@*d/B!Z0FIJcM\!EI;p'u
 i$"_WA(t\/rJ+`MOX-=CQ!Q!K4eH/8
 ca@8q<e9Pm.ha6@I0k8269KaaE0?H;
 XD`!mW@V-0\V>`U/29Kf>AOs:_L`p!
 ARB_VHHT-qj-#sUHWrQ`ipgb7EVQ+(
 !lE;N+7A7trjDWPF.%kM!Ek(rEARdF
 K`8hjcfLb>>scke@kqgb00RQXD@[<+
 2pb6Rc?u7u!3"9a-j<\dV/Y>qgR[F!
@@ -498,9 +498,9 @@
 rtW$m>;9`mr#OTj8:MKgN8hRm$#A1c
 9^TMeCSPae!7Tu?p-a$+.:-HXAHp/b
 )Qh'@DBqVf"Ibr\2Z[@n9@fDS9]kdh
 ]nLI+QJGpqfQ4J-H%S1>Bq$t!,Tb=G
 GMTag!VERZJjDHPN0E=VR)",H`>diS
 /mP*ECD3UX_</E^"*r.Ar^n!d@?d\c
 gZQ95qjlVAk`XKrOTdX167qPjRs"Ne
-Ii1p"dIZ?sm$k$gRK3MZgrsL36/Bh(
+Ii1p"dIZ?sm$k$gRK3Li$qe\\
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/utilities/__init__.pye` & `mscore-24.1.1/mscore/utilities/__init__.pye`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhQrgF+\t]q+oR7I`NlhpO@8l!)T?qLB%;S
-GhN1F!egO7Td:GRHQ$p*BG;<d-!3#NFi1nq
+GhN1B!f6g;Td:GRHQ$p*BG;<d-!3#NFi1nq
 k!)[HQ=G*4K`jna96bXTZ1uAg[,E5o:O-m4
 ^C[UmW<t3X7Pb:q$8=qpe4KeWF_sG%XT5Zo
 G+@@YqO!FS`O"bb<#m'h@1m`L]3%_cIAbQN
 2a%[tS9Rr!,h#L=mgLf$]Y]t:YWYO\`9TGp
 b+93n!lOc_TTlcD/mg/Za`)oo3K1Se6[\\4
 :qE+d1nal0D^hCEUFK^1.NZbPmI+d+,oEm!
 -<&i^;5U9C"XUjKcK&P/hV%+2^]O<2?FZ0k
@@ -18,10 +18,9 @@
 &Bmp>=Dcq8Y&,CiEApQ5PN3$+.[c]_?Y`Ms
 Q9s^sg0(pA_X]0U\FV",0KAb!\V41s$Iu#5
 b0al\O`p%3lJMDU=EM+!1@?=W?I?)fOatds
 m\])Fh(e1g9it8.RkC=4(;^of=G!B$,B3`2
 *Y`*Wh"KXP)%aY2m0jf42aZ;7OhI2/!PEb<
 X:0/Ha^I9;V)b0+VRU[hFGeT"Z-6J3g@`4?
 TK]!u@(u'G=hSWA`1Yc"UQU*gMOj\;CCjp'
-pmL\o!$p\d&k<&7YBt=.T8pisMBN%MDjm`m
-5e6pq
+pmL\o!$p\d&k<&7YBt=.T8pisMXRY55Q:]`
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/utilities/authentication.pye` & `mscore-24.1.1/mscore/utilities/authentication.pye`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhSY=:uW.VfK@?'?'n^-S*"np4DG*8
-GhN0s+KXIgNHJI%4rVUc\p,$Cje>1;
+GhN0o+L'akNHJI%4rVUc\p,$Cje>1;
 QDZORr;VcCMKEMOU-8Q+:j4UpM4NRW
 M+VeP,P%pjd6/8/EKP0n!=d2;d+uT)
 F=\@Zq*^bHH1_nfQ@F6gl:8/.nZ,6e
 Psu7FP[V1<6b0$`9/W5oOB4?A3pElj
 43]*@6Eh%2<"YVE<;&;tGEQ7@9@.1?
 [9b((H5ShecQ#;#nJ$Zc.d(snZ@'^[
 b*U!rGt,@g]a,IIK;>_e,PfM8.)1<o
@@ -340,10 +340,10 @@
 3POhuF3[m^a!Ooj.T[`hkGdOV,4"RN
 r2&D$')-U%+XhQF)&c&[(3=IT+Qe*8
 3^IN*9/>4OdEacsQCEekD0p"m_ni<D
 Z*0BiR,e05p8^(74k#_&JCEUE$gcZ]
 'ttkgFVjqPXZ4/]*YkGUfATr\!/Yfc
 Y#S&#_kH\,OOsCHO2q*\6RtrP%gIto
 CL:;+NGD@gLg5;)P*8S1N14]H+rIo)
-#h(LaeSi*M/^9Sa19:8B$EG-S<)cQl
-TV';c&(1FX
+#h(LaeSi*M/^9Sa19:8B$EG-S<18cF
+%ZCAf
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/utilities/cli.pye` & `mscore-24.1.1/mscore/utilities/cli.pye`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhR3kqD2dEA+Pa3>tpKmE](<.!(n(5jo>A]
-GhN2T'-Z^,\>,sTjeZXlh)Y3XVM0G;@@>_2
+GhN2P'.*!0\>,sTjeZXlh)Y3XVM0G;@@>_2
 nd=l2Y!rD)dY<-Oba8ItTlte'W,28r<h&Re
 p9MV'08^4lBY>;r;%;#[lmA*dLQ@Nce)^TJ
 Z*jme)e2,[luFt<LIce'P&No@?sT*d[L?bR
 0B5?FMYN12/?)O.=M!OhB@n$>fAtP&Np/%<
 VAiZtp)X=H@DE))O"c&TfZCR8L0YndW$&Ni
 _6TbAjfebT^B$f(V#V*tY(:nH*l5]TcsjE-
 HiaBl(Q`J7&%b)k[_A"H@5+CuP+rS]%<)il
@@ -177,10 +177,9 @@
 ZmGRHA,Vq6T3e/u;%"hB2h-Rc2?Tn,:df)#
 QI"N9%IGIS(5(=)MYJ+Z6HlE^pUX&l&K%>U
 L'+YsHrI41HCiX>1aW]Lc&DbQm%LN7&1dH2
 G+[f!BOW&[)psl9H.H&Ya+uqo76o']@n?eU
 Vb211D"q9ij#dJlM)Zb%]J+=LSRN,8a*sji
 0?WG=.X:FsnUuJoa/W/aZ.`QoEoqE!6lDKA
 U87,RER)8endM!-\*3%H6q$>%&q2Phm1$BX
-M;cgjCPkbu2V>)+lmlfhV:%(+5ec&pFkR\k
-K`D)Q
+M;cgjCPkbu2V>)+lmlfhV:%(+N`S[,;#gRr
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/utilities/context.pye` & `mscore-24.1.1/mscore/utilities/context.pye`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhU>?;d8XQQg;"Jb3dbKDD`I81,K0K
-GhN0c%(u0@pkBQAkg*W^AMZ=?/+JI1
+GhN0_%)DHDpkBQAkg*W^AMZ=?/+JI1
 eOPm(n*ZAM>A0B_3i%j.1p/.qecBc-
 1hi=Ydm.5_*;1ZkC3^Q?3J:#P<Fc!1
 l01+.\[jX`k>n)r[H0WnOdY6DQgqk!
 G&LhU#JK7P`Y"VK_1U;fkl^`)k,1+;
 dD\]1'<H^j%/+_K&P4`iggS/1@7Q<V
 f;$WHn\R&-d@_?>=(5dgGWII,If.+\
 ]lJtkD'ii.mK(\=M8i0_hB_K60EmA&
@@ -126,10 +126,10 @@
 "I(U]*SnT9"eZZ3_6hX!PC\Ea!]?GU
 CO?t<L2N727d>FK@V<sd!$!$G?qT7:
 8aq5!I$t2QkRq1V#?!pT>U4DoF;lbe
 D6ttdK;]oW[(][2_(4CPaN6J3"e2j:
 Q#WjMb=_(3+o)NC\;9C?fsLrk;RA%V
 ^V/I[h6/'@O%L4d6=.VMUnUkLm(OO4
 3cWsVMK.U?.jdb.[dJ[2!*+EOX@Ic6
-rs6gGS#ZX*+mDOp[;BMaW+;M)-M^i<
-2&Rfo-7&Wl
+rs6gGS#ZX*+mDOp[;BMaW+;M)-9%$,
+,T?^`
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/utilities/data_models.pye` & `mscore-24.1.1/mscore/utilities/data_models.pye`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhQ),^:@q.cJ[cKQ[eC6^]!d;!(JLGFT;CA
-GhN26"[Dk8Ug%Z3geuMG47_7JU/cR;Q"P_D
+GhN22"[i.<Ug%Z3geuMG47_7JU/cR;Q"P_D
 Lka=g`Y9Eb0k&nMH_m'])TaAHgKal%,UK5r
 Ko;#[(*@TCf.2h^>m]/+)CVqW',ns`KEc$/
 ZZ;6!3EF#K*UhbU"KQ#&7eq%\SJQRUOCnI?
 $b?sKQor3kCn)@JD0)dZ2U)>W]%U7AYr;Cr
 Tfu:GmphZ+_isLV[[K="j33`bSiW>o0YB]E
 :^79>]tr;Sh,80\jl:a^;R8+/aY\$4Vie4[
 SlWS<E`%L\ha@Euep8nB%5jji\BC=Y0&][b
@@ -48,9 +48,9 @@
 7e?loJr*NJ1GFjN,QYh1mSQVba4Wr,]BcE8
 g=u@5l7IE8p!eY\*-Tlj\=pl-19VR+W'"B9
 2]cVeTSSeW%')LbcNSrIecq<m42:!Gns-E[
 .'#A5'gFWs/A0!C"[g]4hGgG5r(k;EFg=@m
 &)<tB>CQOe?$oC9qNEq1>&C7>Mcf8:`#>T:
 0s*RYSgdg-oo1ieh/;9jbdk79cVej$R+&c;
 9W_sg>s!WVXQ;Wt:H<rXrK!Gf/NCDO>hkNd
-Zs#MSAeXUC'K)#to\pG+YWr"*DNt5KL"<@+
+Zs#MSAeXUC'K)#to\pG+YWk"gC=L6'
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/utilities/data_validation.pye` & `mscore-24.1.1/mscore/utilities/data_validation.pye`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhR3R<XNkqs*opgh7[n'F4JeA!'?5H\,ZL/
-GhN0n+gKl)oY^_u^?H@8nB!1BP6NiD^d^6'
+GhN0j+gp/-oY^_u^?H@8nB!1BP6NiD^d^6'
 (UFGC89j^XJ:n;/":rghVT7AMlHtUo@ScHo
 8V=tB9bP6!0'3AZk46UF7AZ=0FROi,PQ;$j
 Ym#B@R6UI;85H=\B'p&GPo[1;i%R%I^,q+Q
 ,G3o)[us^/#RJcf1S2)k%%*o$CnIR5H*o\M
 kk"T-\I8>dNnn$ZHh14KPu'@;C9CL+<+iCU
 _:dWgo:$/!mdT3@3k?7,F$f2M['(+3B/_i$
 $mG.V>G77G;1alnTJmrYDl4$h`7l#V_X!VL
@@ -300,9 +300,9 @@
 JJ'1+qERTm\_ZHRR\lA8$OJ8r?S)Dk^,O-#
 #!!crJT_nVmU9O\ks\u1fR@?'(;m[`>8-MX
 ;1%j:2scRAg_[2jPK>,*Zh;5cI+*)dR>qVJ
 J=ket!S/3]oSjdKEe/6o$H>GC(R,tqa<7[T
 .&29M8rpPh3m!&b^+Bbb+U!l]U;9j`q*8;%
 #=ks"F,3Rh&:hb\6UaiiKIsuC'a[ZN3sP_/
 :D(&?!lg:+:YmAHqLKNHPfn+6Gq#%R]?f,@
-BqOWQ8MpTsSlFA2nAgQU_4Q,jC<(ar/H>bN
+BqOWQ8MpTsSlFA2nAgQU%n#3FhuE`W
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/utilities/file_organizer.pye` & `mscore-24.1.1/mscore/utilities/file_organizer.pye`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhW&,2l60."hsX<RHse3-!nUl!)-Q$m/R+d
-GhN1f"_@JPeL%`cG-j#[:1t)gEkD:#T`c!;
+GhN1b"_dbTeL%`cG-j#[:1t)gEkD:#T`c!;
 O@:h:!WpR=>'YfA/qBYm.s/s:7@g9@MfsFJ
 e8ps^Iu)rQP@/q1g&t0@Q!mM_FVbg&I:f'n
 \MpPF#SGWP?nS`(NATo6hH"`e(2/5glY$,b
 g+#,nf(1\M0@nO$\-*%2Ei3mrf7T:O/;kd@
 N`9T+4;L(-1n?h*b]u1JlHS39h;^N(NfJPs
 =7rDM>WUoU3tKF9WnGn;-7k10#:&geeD%`p
 `+rWa=YP>-(nZ\@&aj(TGiV_bM7MI$k4PNq
@@ -47,9 +47,9 @@
 m^:=EQ=,FFW(?\S37:052!pj9=)niMnSq:B
 \_H/O2`[f!dZfTJqa&.a*3sC-V,X_@+d#W`
 \:mq#!(l,#SLLGJ:h",SOXJSPS9>J(fbt<'
 fLlY$p>UI<GcM"h<&kX.Bdn9sE"9@I*/D'$
 puIAkQ>Q"k74C4nhkC-:aoteOO?R#%(!U:-
 Kr,J!$\sV1GiY[r_C0u!aUFV5d[`3POfK]g
 jB'Z6ij[Z;9Z.6d^9s;T.)(Sb2b0_X32%>A
-@Juh`oL_sZ@8+tCPL)X4_rLdt
+@Juh`oL_sZ@=gE\_*e8'
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore/utilities/licensing.pye` & `mscore-24.1.1/mscore/utilities/licensing.pye`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhQYe:Gku[.:@)_II==Lg[$Ej/b92Q
-GhN2h(_,Z?Va=Ub>?"D$DBq6h&u(`g
+GhN2d(_PrCVa=Ub>?"D$DBq6h&u(`g
 4#X":E<?V.iq*;T58:9LVcA7Fp&.mW
 mh,A["aBT0"4B?f1o1'^<[?AB^QB*,
 +c#KK-e2`=<kb?c%Jhgd<U$?2bY[iN
 CQ)GrB.gar9">`17ea)U*&mot'2>dT
 ;;3jj@<iWYmad_>=5FQ/J/4N!^OopD
 >L_2?>Fp?KM\YmAH7K[KP@??l-nq?0
 F8Q1td_]5=Y"qLAEEBhr2]&6oUAcB<
@@ -262,9 +262,9 @@
 qtVi_1BdT1UHiJ@0Ro0I]E>suUlJ3U
 X\l:uiM<0/4OL:9C@D@VIspd0qFEt\
 )GcTV^5;UMjV/eIR/O0=1-[F]PcYDl
 q`Bm#-`2[jW)*q^':WXYJ8Jf]T(N?G
 L/;:AFPJ-WH61%Chqa]];R):S_PFVM
 ag@Q<\`5-HZCnPM@6*-KI3Af]5haY!
 gY^Nk/PCsI"]^3,d%ik^ZI`P@Wn/("
-j+IXrp939,d6(u]H2mpF
+j+IXr3-(s9KE(uP
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/utilities/log_handler.pye` & `mscore-24.1.1/mscore/utilities/log_handler.pye`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 --BEGIN SOURCEDEFENDER FILE---
 GhTd0IE(W&^1)@hQ,@mj>ru0i6oP@Q
-GhN1G#(ua7^dZ4:C6>diMZkQX\Wd&C
+GhN1C#)E$;^dZ4:C6>diMZkQX\Wd&C
 YSiQKcC33>R@H]mjfmGS]V>:R_>$\c
 L8beV?+TVal*>([W.1cne0&n2G'\30
 NYdD:Mep*Gr9DkaW=N)-$Q%"_D$fIj
 XnX&p8\,o^Ejn`aq!.#&)K`Y4pH.GI
 &p1GoUbOT=2kLuqrp@L[X)(S5Bf#<H
 bV+#O+&3%1_R$nJ$Z[FCD+)s\`;AP;
 4O]Su_+&BpNW!/O=qq8`N;q-s@3^F;
@@ -65,9 +65,9 @@
 /e&OL0/Rg$&[$gkBX<Z;%<`.^UCVe<
 NYA!6UDF7]4E!nHFB0m]h9fh'%\]FP
 nm+B*.V!?KI^j<Hq$5'N$f0JF/c<U[
 8*1I3pYu2oNTJ&r_k&<'Jhrqdp]U[_
 Z`Qq7JqY/;QVoC64!TJ*A,QjX8=cn^
 Xclhi.p)t5jj:7sj'g+T%b17g(?*J#
 .[AAYh=l9fT"G?1\W*;k[gPjhC(m:)
-OB!hkgN*fbO=a%'HoQ?N
+OB!hkgN18T#WM/O
 ---END SOURCEDEFENDER FILE----
```

### Comparing `mscore-24.1.0/mscore/utilities/user_models.pye` & `mscore-24.1.1/mscore/utilities/user_models.pye`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -----BEGIN SOURCEDEFENDER FILE-----
 GhW%0f[DS6W(h-FXlOsR/G(k%!)31or;Zft
-GhN2t"TeH5am0lL8?UI.6q<L(ZtPCDI?5">
+GhN2p"U4`9am0lL8?UI.6q<L(ZtPCDI?5">
 #VX&R:SGr*q3bg<A1&NYgGV'7$'qPg(B.en
 .g@X[.E+se3DV1):g'oK4nQIg**qBQpbHu"
 'Y>#<ccVG=!bf&7rgb@l*gb@,!7m+fod"NP
 %H>,29(@h=]9-ApbF0mZj614\E=t!ZCut2T
 RK',\[<4\-!rUX?@9]3noF9$3p^q:8pV%n1
 RD]$Q2(?Z1J&3\OUV;_eBVqk)=m2^AF0"Zo
 )Cejh.fm25om1&;\aP?bhhPn>R55`Vd!f=s
@@ -50,10 +50,10 @@
 Wg:sg7l:)M,Mb=X6%s,2SP8s\ciSANmh!hq
 5UhS4("#)\O9N-FH=&AlrVQsET#$$Y);cGK
 580Q-oEcf>Q/IA0ND`<DTPL?r+n=PA9n$4m
 2nG#206KuP0=l=rELT%.N3hZZ1V![sWd>fO
 Vm`F'ON%+?6s'4MeO,/nQVP/raL:I[SYlL8
 n2PQ=Oao.k)_G4u3J#9!fGK]KKYHh"n@8#(
 K!;67FB[$S7\"("d[O")J_*F`lT%Mnq*B#b
-0_:-jH1D=Ch8&P.bnn\L,HHbI,)V-R^B35u
-3)k#,VZ6\s
+0_:-jH1D=Ch8&P.bnn\L,HHbI,)V-REA2VB
+NW9%Z
 ------END SOURCEDEFENDER FILE------
```

### Comparing `mscore-24.1.0/mscore.egg-info/PKG-INFO` & `mscore-24.1.1/mscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscore
-Version: 24.1.0
+Version: 24.1.1
 Summary: MScore: Risk Scores Made Easy
 Home-page: https://github.com/elevendatacorp/mscore.git
 Author: RAM Development Team
 Author-email: RAM Development Team <dev@riskadjustmentmodel.com>
 Project-URL: Homepage, https://riskadjustmentmodel.com/mscore-product
 Project-URL: Bug Tracker, https://github.com/elevendatacorp/mscore/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mscore Version: 24.1.0 Summary: MScore: Risk Scores
+Metadata-Version: 2.1 Name: mscore Version: 24.1.1 Summary: MScore: Risk Scores
 Made Easy Home-page: https://github.com/elevendatacorp/mscore.git Author: RAM
 Development Team Author-email: RAM Development Team
 riskadjustmentmodel.com> Project-URL: Homepage, https://
 riskadjustmentmodel.com/mscore-product Project-URL: Bug Tracker, https://
 github.com/elevendatacorp/mscore/issues Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: pandas Requires-
```

### Comparing `mscore-24.1.0/mscore.egg-info/SOURCES.txt` & `mscore-24.1.1/mscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscore-24.1.0/pyproject.toml` & `mscore-24.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mscore"
-version = "24.1.0"
+version = "24.1.1"
 dependencies = [
   "pandas",
   "pyarrow",
   "numpy",
   "requests",
   "getmac",
   "cython",
```

