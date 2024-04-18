# Comparing `tmp/rx_scripts-0.3.3.tar.gz` & `tmp/rx_scripts-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rx_scripts-0.3.3.tar", last modified: Tue Feb  6 13:43:27 2024, max compression
+gzip compressed data, was "rx_scripts-0.3.4.tar", last modified: Thu Apr 18 14:54:02 2024, max compression
```

## Comparing `rx_scripts-0.3.3.tar` & `rx_scripts-0.3.4.tar`

### file list

```diff
@@ -1,77 +1,91 @@
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      386 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/README.md
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.945977 rx_scripts-0.3.3/jobs/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      287 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/jobs/cdr_copy
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2651 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/jobs/job_copy
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      199 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/jobs/run_copy
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.945977 rx_scripts-0.3.3/scripts/
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2298 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/check_size
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2108 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/check_tuples
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4705 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/copy_tuples
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3143 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/dv_stats
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2079 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/jmanager
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      495 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/kerberos
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2880 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/link_files
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1588 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/link_to_file
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2766 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/print_trees
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2593 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/scripts/tar_plots
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/setup.cfg
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      526 2024-02-06 13:43:22.000000 rx_scripts-0.3.3/setup.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.955977 rx_scripts-0.3.3/src/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       63 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      966 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/atr_mgr.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7314 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/binning.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1337 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/cf_checker.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1362 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/collector.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     5427 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/compare_files.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9441 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/data_splitter.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    17488 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/fit_manager.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    11632 2024-01-22 13:12:12.000000 rx_scripts-0.3.3/src/fitter.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5020 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/ganga_stats.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    15810 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/hep_cl.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2819 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/hep_gb.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1014 2024-01-24 17:01:39.000000 rx_scripts-0.3.3/src/log_store.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10821 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/mcpull.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8901 2024-01-20 15:44:17.000000 rx_scripts-0.3.3/src/model_analyzer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2477 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/ndict.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1901 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/pathfinder.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     8994 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/plot_fit.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4564 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/plotter.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.955977 rx_scripts-0.3.3/src/plotting/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1123 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/plotting/utilities.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      805 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/progress.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/src/rx_scripts.egg-info/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      386 2024-02-06 13:43:27.000000 rx_scripts-0.3.3/src/rx_scripts.egg-info/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1323 2024-02-06 13:43:27.000000 rx_scripts-0.3.3/src/rx_scripts.egg-info/SOURCES.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-02-06 13:43:27.000000 rx_scripts-0.3.3/src/rx_scripts.egg-info/dependency_links.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       85 2024-02-06 13:43:27.000000 rx_scripts-0.3.3/src/rx_scripts.egg-info/requires.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       23 2024-02-06 13:43:27.000000 rx_scripts-0.3.3/src/rx_scripts.egg-info/top_level.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1886 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stat_indep.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.955977 rx_scripts-0.3.3/src/stats/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      959 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/average.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9306 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/correlations.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2192 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/covariance.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1188 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/nll_plot.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2107 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/pdf.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      725 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/stats/utils.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1561 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/style.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2918 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/sweight_serialize.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    22503 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/trgwgt.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)   128595 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/utils.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    44088 2024-01-22 13:22:42.000000 rx_scripts-0.3.3/src/utils_noroot.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2069 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/utils_py2.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3458 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/src/version_management.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/src/zutils/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5430 2024-01-20 13:38:46.000000 rx_scripts-0.3.3/src/zutils/pdf.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    13662 2024-02-04 12:43:53.000000 rx_scripts-0.3.3/src/zutils/plot.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    11448 2024-01-25 12:23:03.000000 rx_scripts-0.3.3/src/zutils/utils.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-06 13:43:27.965977 rx_scripts-0.3.3/tests/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      380 2024-01-24 16:45:14.000000 rx_scripts-0.3.3/tests/test_log_store.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       97 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/tests/test_logger.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4801 2024-01-14 16:15:35.000000 rx_scripts-0.3.3/tests/test_model_analyzer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1109 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/tests/test_nll_plot.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1778 2024-01-20 15:48:15.000000 rx_scripts-0.3.3/tests/test_zdscb.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      395 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/tests/test_zfit_plot.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1348 2024-01-14 12:39:18.000000 rx_scripts-0.3.3/tests/test_zfitter_datatype.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1865 2024-01-14 17:25:42.000000 rx_scripts-0.3.3/tests/test_zshape.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      451 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1679 2024-03-28 15:55:38.000000 rx_scripts-0.3.4/README.md
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.605293 rx_scripts-0.3.4/jobs/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      287 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/jobs/cdr_copy
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2651 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/jobs/job_copy
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      199 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/jobs/run_copy
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.605293 rx_scripts-0.3.4/scripts/
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2298 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/check_size
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2108 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/check_tuples
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4004 2024-03-28 16:05:03.000000 rx_scripts-0.3.4/scripts/copy_tstruc
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4705 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/copy_tuples
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3143 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/dv_stats
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2079 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/jmanager
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1958 2024-03-28 15:55:38.000000 rx_scripts-0.3.4/scripts/job_run_commands
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      495 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/kerberos
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2880 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/link_files
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1588 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/link_to_file
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2766 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/scripts/print_trees
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-03-28 15:55:38.000000 rx_scripts-0.3.4/scripts/submit_run_commands
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3024 2024-03-28 16:16:15.000000 rx_scripts-0.3.4/scripts/tar_plots
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/setup.cfg
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      576 2024-04-18 14:53:30.000000 rx_scripts-0.3.4/setup.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.615293 rx_scripts-0.3.4/src/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       63 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      966 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/atr_mgr.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7314 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/binning.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1337 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/cf_checker.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1362 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/collector.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     5427 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/compare_files.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9441 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/data_splitter.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    17488 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/fit_manager.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    11814 2024-03-28 15:55:38.000000 rx_scripts-0.3.4/src/fitter.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5020 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/ganga_stats.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    15810 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/hep_cl.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2819 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/hep_gb.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1145 2024-04-18 14:43:48.000000 rx_scripts-0.3.4/src/log_store.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10821 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/mcpull.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4199 2024-02-28 16:40:03.000000 rx_scripts-0.3.4/src/misid_check.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8901 2024-01-20 15:44:17.000000 rx_scripts-0.3.4/src/model_analyzer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2477 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/ndict.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1901 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/pathfinder.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     8994 2024-03-01 12:30:47.000000 rx_scripts-0.3.4/src/plot_fit.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4564 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/plotter.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.615293 rx_scripts-0.3.4/src/plotting/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1123 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/plotting/utilities.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      805 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/progress.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/src/rx_scripts.egg-info/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      451 2024-04-18 14:54:02.000000 rx_scripts-0.3.4/src/rx_scripts.egg-info/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1645 2024-04-18 14:54:02.000000 rx_scripts-0.3.4/src/rx_scripts.egg-info/SOURCES.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-18 14:54:02.000000 rx_scripts-0.3.4/src/rx_scripts.egg-info/dependency_links.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      105 2024-04-18 14:54:02.000000 rx_scripts-0.3.4/src/rx_scripts.egg-info/requires.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       13 2024-04-18 14:54:02.000000 rx_scripts-0.3.4/src/rx_scripts.egg-info/top_level.txt
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.615293 rx_scripts-0.3.4/src/scripts_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       63 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/scripts_data/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.615293 rx_scripts-0.3.4/src/scripts_data/misid_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       63 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/scripts_data/misid_data/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)  1063125 2024-02-27 16:25:17.000000 rx_scripts-0.3.4/src/scripts_data/misid_data/bpd0kpienu.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1886 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stat_indep.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.615293 rx_scripts-0.3.4/src/stats/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1095 2024-04-02 04:18:47.000000 rx_scripts-0.3.4/src/stats/average.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9306 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stats/correlations.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2192 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stats/covariance.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1188 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stats/nll_plot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2107 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stats/pdf.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      725 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/stats/utils.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1561 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/style.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2918 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/sweight_serialize.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    22503 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/trgwgt.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)   129002 2024-03-17 13:41:11.000000 rx_scripts-0.3.4/src/utils.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    44088 2024-01-22 13:22:42.000000 rx_scripts-0.3.4/src/utils_noroot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2069 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/utils_py2.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3458 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/src/version_management.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/src/zutils/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5430 2024-01-20 13:38:46.000000 rx_scripts-0.3.4/src/zutils/pdf.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    15706 2024-03-27 17:17:24.000000 rx_scripts-0.3.4/src/zutils/plot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    13157 2024-03-27 17:17:24.000000 rx_scripts-0.3.4/src/zutils/utils.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 14:54:02.625293 rx_scripts-0.3.4/tests/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-04-02 08:38:29.000000 rx_scripts-0.3.4/tests/test_arr_fun.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      766 2024-04-18 14:52:23.000000 rx_scripts-0.3.4/tests/test_log_store.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       97 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/tests/test_logger.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2858 2024-02-27 18:01:29.000000 rx_scripts-0.3.4/tests/test_misid_check.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4801 2024-01-14 16:15:35.000000 rx_scripts-0.3.4/tests/test_model_analyzer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1109 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/tests/test_nll_plot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      416 2024-03-02 14:50:38.000000 rx_scripts-0.3.4/tests/test_pdg_utils.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1747 2024-03-04 11:29:12.000000 rx_scripts-0.3.4/tests/test_plot_hist.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1778 2024-01-20 15:48:15.000000 rx_scripts-0.3.4/tests/test_zdscb.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      399 2024-03-01 12:26:57.000000 rx_scripts-0.3.4/tests/test_zfit_plot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1348 2024-01-14 12:39:18.000000 rx_scripts-0.3.4/tests/test_zfitter_datatype.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1865 2024-01-14 17:25:42.000000 rx_scripts-0.3.4/tests/test_zshape.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      997 2024-03-18 21:08:43.000000 rx_scripts-0.3.4/tests/test_zutils.py
```

### Comparing `rx_scripts-0.3.3/README.md` & `rx_scripts-0.3.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -38,18 +38,23 @@
 
 ```python
 import utils
 ```
 
 for instance.
 
+## Particle kinematics
+
+[Mass hypothesis change](doc/mass_hypthesis_change.md)
+
 ## Statistics
 
 [Covariance calculator](doc/covariance.md)   
 [Negative log likelihood plotter](doc/nll_plt.md)   
+[Pull plotter](doc/pull_plotter.md)
 ## Other utilities
 
 These live in the `zutils/utils.py` module and can be used to:
 
 ### Print PDFs
 
 ```python
@@ -59,14 +64,16 @@
 ```
 where `d_const` is a mapping between the name of the parameter and `[mu, error]`.
 
 ## File system
 
 [Symbolic link maker](doc/link_files.md)
 
-[Held jobs manager](doc/held_jobs.md)
+[On jobs](doc/jobs.md)
 
 [Transfer ntuples to LXPLUS from IHEP](doc/tuple_transfer.md)
 
 [TAR directory sctructure with a given type of files](doc/tar_plots.md)
 
-[Check file size](doc/check_size.md)
+[Check file size](doc/check_size.md)
+
+[Copy files and entire file structure for a given extenson](doc/copy_tstruc.md)
```

### Comparing `rx_scripts-0.3.3/jobs/job_copy` & `rx_scripts-0.3.4/jobs/job_copy`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/check_size` & `rx_scripts-0.3.4/scripts/check_size`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/check_tuples` & `rx_scripts-0.3.4/scripts/check_tuples`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/copy_tuples` & `rx_scripts-0.3.4/scripts/copy_tuples`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/dv_stats` & `rx_scripts-0.3.4/scripts/dv_stats`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/jmanager` & `rx_scripts-0.3.4/scripts/jmanager`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/link_files` & `rx_scripts-0.3.4/scripts/link_files`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/link_to_file` & `rx_scripts-0.3.4/scripts/link_to_file`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/print_trees` & `rx_scripts-0.3.4/scripts/print_trees`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/scripts/tar_plots` & `rx_scripts-0.3.4/scripts/tar_plots`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     echo "2. TAR latter tree and remove the copied tree."
     echo ""
     echo "Args:"
     echo ""
     echo "-s Absolute path to directory containing version directory, e.g. /a/b/c"
     echo "-v Version directory where tree starts, e.g. v3"
     echo "-e Extension(s) of the files that will be copied, e.g. png. Default is png, if using multiple, put them inside quotes"
+    echo "-r Regular expression for paths to skip"
     echo ""
     echo "Example:"
     echo ""
     echo "tar_plots -s /publicfs/lhcb/user/campoverde/weights/comparison -v v1 -e png"
     echo 'tar_plots -s /publicfs/lhcb/user/campoverde/weights/comparison -v v1 -e "png tex"'
 }
 #-----------------------
@@ -30,15 +31,16 @@
 	kill -INT $$
     fi
 }
 #-----------------------
 get_args()
 {
     EXT="png"
-    while getopts :hf:s:v:e: option
+    RGX="none"
+    while getopts :hf:s:v:e:r: option
     do 
 	case "${option}"
 	    in
             h)  
                 display_help
                 exit 0
                 ;;  
@@ -49,19 +51,36 @@
             :)  echo "$0: Arguments needed"
                 display_help
                 exit 1
                 ;;  
 	    s)SRC=${OPTARG};;
 	    v)VER=${OPTARG};;
 	    e)EXT="${OPTARG}";;
+	    r)RGX="${OPTARG}";;
 	esac
     done
     check_var "source path" $SRC
     check_var "version"     $VER      
     check_var "extension"   $EXT      
+    check_var "regex"       $RGX
+}
+#-----------------------
+skip_path()
+{
+    FILE_PATH=$1
+    if [[ "$RGX" == "none" ]];then
+	SKIP_PATH=0
+	return
+    fi
+
+    if [[ $FILE_PATH =~ $RGX ]]; then
+	SKIP_PATH=1
+    else
+	SKIP_PATH=0
+    fi
 }
 #-----------------------
 copy()
 {
     VER=$1
     SRC=$2
     EXT="$3"
@@ -75,14 +94,20 @@
 	    PLOT_DIR=$(dirname $PLOT_PATH)
 	    END_NAM=$(basename $FILE_PATH)
 
 	    mkdir -p $PLOT_DIR
 
 	    TGT_PATH=$PLOT_DIR/$END_NAM
 
+	    skip_path $FILE_PATH
+	    if [[ $SKIP_PATH -eq 1 ]];then
+	        SKIP_PATH=0
+		continue
+	    fi
+
 	    if [[ ! -f $TGT_PATH ]] || [[ $TGT_PATH -ot $FILE_PATH ]];then
 		cp $FILE_PATH $TGT_PATH
 	    fi  
 	done
     done
 }
 #-----------------------
```

### Comparing `rx_scripts-0.3.3/setup.py` & `rx_scripts-0.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 import glob
 
 setup(
         name            ="rx_scripts",
-        version         ='0.3.3',
+        version         ='0.3.4',
         description     ='Generic utilities for data analysis',
         long_description='Package used to store utilities for RX calculation',
         scripts         = glob.glob('scripts/*') + glob.glob('jobs/*'),
-        packages        = ['', 'stats', 'zutils', 'plotting'], 
+        packages        = find_packages(where='src'), 
         package_dir     = {'' : 'src'},
+        package_data    = {'scripts_data' : ['*/*.json']},
         install_requires= open('requirements.txt').read()
         )
```

### Comparing `rx_scripts-0.3.3/src/atr_mgr.py` & `rx_scripts-0.3.4/src/atr_mgr.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/binning.py` & `rx_scripts-0.3.4/src/binning.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/cf_checker.py` & `rx_scripts-0.3.4/src/cf_checker.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/collector.py` & `rx_scripts-0.3.4/src/collector.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/compare_files.py` & `rx_scripts-0.3.4/src/compare_files.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/data_splitter.py` & `rx_scripts-0.3.4/src/data_splitter.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/fit_manager.py` & `rx_scripts-0.3.4/src/fit_manager.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/fitter.py` & `rx_scripts-0.3.4/src/fitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import utils_noroot as utnr
 
-from scipy import stats
+from scipy     import stats
+from log_store import log_store
 
 import numpy
 import zfit
 import pandas as pd
 
 #------------------------------
 class zfitter_gof_error(Exception):
     pass
 #------------------------------
 class zfitter:
-    log=utnr.getLogger('zfitter')
+    log=log_store.add_logger('scripts:zfitter')
     #------------------------------
     def __init__(self, pdf, data):
         self._data_in = data
         self._pdf     = pdf
 
         self._data_zf = None 
         self._obs     = None
@@ -206,16 +207,18 @@
             self.log.info('-' * 30)
             self.log.info(f'{"Low edge":>15}{"High edge":>15}')
             self.log.info('-' * 30)
             for rng in ranges:
                 self.log.info(f'{rng[0]:>15.3e}{rng[1]:>15.3e}')
 
         if self._pdf.is_extended:
+            self.log.info('Using Extended Unbinned Likelihood')
             l_nll = [ zfit.loss.ExtendedUnbinnedNLL(model=self._pdf, data=self._data_zf, constraints=constraints, fit_range=frange) for frange in ranges ]
         else:
+            self.log.info('Using Non-Extended Unbinned Likelihood')
             l_nll = [ zfit.loss.UnbinnedNLL        (model=self._pdf, data=self._data_zf, constraints=constraints, fit_range=frange) for frange in ranges ]
 
         nll = sum(l_nll[1:], l_nll[0])
 
         return nll
     #------------------------------
     def fit(self, ntries=None, pval_threshold = 0.05, d_const={}, ranges=None, l_print_par=[]):
```

### Comparing `rx_scripts-0.3.3/src/ganga_stats.py` & `rx_scripts-0.3.4/src/ganga_stats.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/hep_cl.py` & `rx_scripts-0.3.4/src/hep_cl.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/hep_gb.py` & `rx_scripts-0.3.4/src/hep_gb.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/log_store.py` & `rx_scripts-0.3.4/src/log_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import logzero
 
 from logzero import logger as log
 #------------------------------------------------------------
 class log_store:
     d_logger = {}
     d_levels = {}
+    log_level= logzero.INFO
+    #--------------------------
     @staticmethod
     def add_logger(name=None):
-        if name is None:
+        if   name is None:
             log.error(f'Logger name missing')
             raise
         elif name in log_store.d_logger:
             log.error(f'Logger name {name} already found')
             raise
 
-        level          = logzero.INFO if name not in log_store.d_levels else log_store.d_levels[name] 
+        level          = log_store.log_level if name not in log_store.d_levels else log_store.d_levels[name] 
         logger         = logzero.setup_logger(name=name, level=level)
         log_store.d_logger[name] = logger
 
         return logger
-
+    #--------------------------
     @staticmethod
     def set_level(name, value):
         log_store.d_levels[name] = value
-
+    #--------------------------
     @staticmethod
     def show_loggers():
         log.info(f'{"Name":<20}{"Level":<20}')
         for name, logger in log_store.d_logger.items():
             log.info(f'{name:<20}{logger.level:<20}')
 #------------------------------------------------------------
```

### Comparing `rx_scripts-0.3.3/src/mcpull.py` & `rx_scripts-0.3.4/src/mcpull.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/model_analyzer.py` & `rx_scripts-0.3.4/src/model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/ndict.py` & `rx_scripts-0.3.4/src/ndict.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/pathfinder.py` & `rx_scripts-0.3.4/src/pathfinder.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/plot_fit.py` & `rx_scripts-0.3.4/src/plot_fit.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/plotter.py` & `rx_scripts-0.3.4/src/plotter.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/plotting/utilities.py` & `rx_scripts-0.3.4/src/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/progress.py` & `rx_scripts-0.3.4/src/progress.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/rx_scripts.egg-info/SOURCES.txt` & `rx_scripts-0.3.4/src/rx_scripts.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 README.md
 setup.py
 jobs/cdr_copy
 jobs/job_copy
 jobs/run_copy
 scripts/check_size
 scripts/check_tuples
+scripts/copy_tstruc
 scripts/copy_tuples
 scripts/dv_stats
 scripts/jmanager
+scripts/job_run_commands
 scripts/kerberos
 scripts/link_files
 scripts/link_to_file
 scripts/print_trees
+scripts/submit_run_commands
 scripts/tar_plots
 src/__init__.py
 src/atr_mgr.py
 src/binning.py
 src/cf_checker.py
 src/collector.py
 src/compare_files.py
@@ -23,14 +26,15 @@
 src/fit_manager.py
 src/fitter.py
 src/ganga_stats.py
 src/hep_cl.py
 src/hep_gb.py
 src/log_store.py
 src/mcpull.py
+src/misid_check.py
 src/model_analyzer.py
 src/ndict.py
 src/pathfinder.py
 src/plot_fit.py
 src/plotter.py
 src/progress.py
 src/stat_indep.py
@@ -43,24 +47,32 @@
 src/version_management.py
 src/plotting/utilities.py
 src/rx_scripts.egg-info/PKG-INFO
 src/rx_scripts.egg-info/SOURCES.txt
 src/rx_scripts.egg-info/dependency_links.txt
 src/rx_scripts.egg-info/requires.txt
 src/rx_scripts.egg-info/top_level.txt
+src/scripts_data/__init__.py
+src/scripts_data/misid_data/__init__.py
+src/scripts_data/misid_data/bpd0kpienu.json
 src/stats/average.py
 src/stats/correlations.py
 src/stats/covariance.py
 src/stats/nll_plot.py
 src/stats/pdf.py
 src/stats/utils.py
 src/zutils/pdf.py
 src/zutils/plot.py
 src/zutils/utils.py
+tests/test_arr_fun.py
 tests/test_log_store.py
 tests/test_logger.py
+tests/test_misid_check.py
 tests/test_model_analyzer.py
 tests/test_nll_plot.py
+tests/test_pdg_utils.py
+tests/test_plot_hist.py
 tests/test_zdscb.py
 tests/test_zfit_plot.py
 tests/test_zfitter_datatype.py
-tests/test_zshape.py
+tests/test_zshape.py
+tests/test_zutils.py
```

### Comparing `rx_scripts-0.3.3/src/stat_indep.py` & `rx_scripts-0.3.4/src/stat_indep.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/stats/average.py` & `rx_scripts-0.3.4/src/stats/average.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 #---------------------------------------------
 def average(arr_y, arr_e):
     '''
     Used to average measurements with errors
     Takes: Array of measurements, array of errors
     Returns: Average value, uncertainty, p-value for null hypothesis: all values are compatible with eachother
     '''
+    if isinstance(arr_e, list):
+        arr_e = numpy.array(arr_e)
+
+    if isinstance(arr_y, list):
+        arr_y = numpy.array(arr_y)
+
     nval   = arr_y.size
     arr_x  = numpy.linspace(1, nval, nval)
 
     [avg], [[cov]] = scy_opt.curve_fit(lambda x, b: b, arr_x, arr_y, sigma=arr_e)
     pval           = get_pval(arr_y, avg, arr_e)
 
     err = numpy.sqrt(cov)
```

### Comparing `rx_scripts-0.3.3/src/stats/correlations.py` & `rx_scripts-0.3.4/src/stats/correlations.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/stats/covariance.py` & `rx_scripts-0.3.4/src/stats/covariance.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/stats/nll_plot.py` & `rx_scripts-0.3.4/src/stats/nll_plot.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/stats/pdf.py` & `rx_scripts-0.3.4/src/stats/pdf.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/stats/utils.py` & `rx_scripts-0.3.4/src/stats/utils.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/style.py` & `rx_scripts-0.3.4/src/style.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/sweight_serialize.py` & `rx_scripts-0.3.4/src/sweight_serialize.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/trgwgt.py` & `rx_scripts-0.3.4/src/trgwgt.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/utils.py` & `rx_scripts-0.3.4/src/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,25 +216,27 @@
     l_color.append(3)
     l_color.append(6)
     l_color.append(8)
     l_color.append(39)
     l_color.append(49)
     l_color.append(38)
     l_color.append(46)
+    l_color.append(31)
 
     l_marker.append(20)
     l_marker.append(21)
     l_marker.append(22)
     l_marker.append(23)
     l_marker.append(33)
     l_marker.append(47)
     l_marker.append(34)
     l_marker.append(39)
     l_marker.append(47)
     l_marker.append(49)
+    l_marker.append(41)
 
     l_line.append(1)
     l_line.append(1)
     l_line.append(1)
     l_line.append(1)
     l_line.append(1)
     l_line.append(1)
@@ -1845,14 +1847,22 @@
 
     plotHistograms(l_hist, plotpath, d_opt=d_opt)
 #--------------------------------------------------
 def plot_histograms(l_hist, outpath, d_opt = {}):
     log.visible(f'Saving to: {outpath}')
     plotHistograms(l_hist, outpath, d_opt = d_opt)
 #--------------------------------------------------
+def hist_to_1mcdf(hist):
+    name = hist.GetName()
+    hcum = hist.Clone(f'h_1mcdf_{name}')
+    area = hcum.Integral()
+    hcum.Scale(1./area)
+
+    return hcum.GetCumulative(False)
+#--------------------------------------------------
 def plotHistograms(l_hist, outpath, d_opt = {}):
     for hist in l_hist:
         if not hist.InheritsFrom('TH1'):
             log.error('Object is introduced is not a histogram')
             print(hist)
             raise
 
@@ -1886,61 +1896,64 @@
 
         if 'leg_stats'  in d_opt and d_opt['leg_stats']:
             title = hist.GetTitle()
             area  = get_hist_area(hist) 
             title = '{}, {:.5e}'.format(title, area)
             hist.SetTitle(title)
 
-    
     if "xrange" in d_opt:
         xmin, xmax = d_opt["xrange"]
     else:
         xaxis= l_hist[0].GetXaxis()
         xmin = xaxis.GetXmin()
         xmax = xaxis.GetXmax()
 
-    if 'yrange' in d_opt:
-        ymin, ymax = d_opt['yrange']
-    else:
-        ymax = -sys.float_info.max
-        ymin = +sys.float_info.max
-        for hist in l_hist:
-            yymax = hist.GetYaxis().GetXmax()
-            yymin = hist.GetYaxis().GetXmin()
-
-            ymax = yymax if yymax > ymax else ymax
-            ymin = yymin if yymin < ymin else ymin
-
-        ymax = 1.05 * ymax
-        ymin = 0.95 * ymin if 'miny' not in d_opt else d_opt['miny']
-
-    for hist in l_hist:
-        hist.GetYaxis().SetRangeUser(ymin, ymax)
-
     xname=''
     if "xname" in d_opt:
         xname = d_opt["xname"]
 
     yname=''
     if "yname" in d_opt:
         yname = d_opt["yname"]
 
     if 'normalize' in d_opt and d_opt['normalize']:
         yname = 'Normalized'
 
+    if '1_m_cdf'   in d_opt and d_opt['1_m_cdf']:
+        l_hist = [ hist_to_1mcdf(hist) for hist in l_hist ]
+        yname  = '1 - CDF'
+
     if 'width' in d_opt:
         width=d_opt['width']
     else:
         width=600
 
     if 'height' in d_opt:
         height=d_opt['height']
     else:
         height=600
 
+    if 'yrange' in d_opt:
+        ymin, ymax = d_opt['yrange']
+    else:
+        ymax = -sys.float_info.max
+        ymin = +sys.float_info.max
+        for hist in l_hist:
+            yymax = hist.GetYaxis().GetXmax()
+            yymin = hist.GetYaxis().GetXmin()
+
+            ymax = yymax if yymax > ymax else ymax
+            ymin = yymin if yymin < ymin else ymin
+
+        ymax = 1.05 * ymax if 'maxy' not in d_opt else d_opt['maxy']
+        ymin = 0.95 * ymin if 'miny' not in d_opt else d_opt['miny']
+
+    for hist in l_hist:
+        hist.GetYaxis().SetRangeUser(ymin, ymax)
+
     ran=ROOT.TRandom3(0)
     ranval=ran.Integer(100000000)
     c_hist = ROOT.TCanvas(f'c_hist_{ranval}', '', width, height)
 
     l_sty=['ET0'] * len(l_hist)
     if 'sty' in d_opt and d_opt['sty'] is not None:
         l_sty = d_opt['sty']
@@ -1985,33 +1998,31 @@
         yaxis_r.SetTitle(yname_r)
         yaxis_r.SetTitleSize(0.10)
         yaxis_r.SetTitleOffset(0.6)
 
         min_x = xaxis_r.GetXmin()
         max_x = xaxis_r.GetXmax()
 
-        line=ROOT.TLine(min_x, 1, max_x, 1)
-        line.SetLineColor(1)
-        line.SetLineWidth(2)
-        line.SetLineStyle(6)
-
-        hasline=False
         for h_rat in l_h_rat:
             if 'ymax_r' in d_opt:
                 ymax_r = d_opt['ymax_r']
                 h_rat.SetMaximum(ymax_r)
 
             if 'ymin_r' in d_opt:
                 ymin_r = d_opt['ymin_r']
                 h_rat.SetMinimum(ymin_r)
 
             h_rat.Draw('same')
-            if not hasline:
-                line.Draw()
-                hasline=True
+
+        line=ROOT.TLine(min_x, 1, max_x, 1)
+        line.SetLineColor(1)
+        line.SetLineWidth(2)
+        line.SetLineStyle(6)
+        line.Draw()
+
     elif 'extra_pad' in d_opt:
         obj=d_opt['extra_pad']
         c_hist.Divide(2, 1)
         pad_1=c_hist.cd(1)
         pad_2=c_hist.cd(2)
         obj.Draw()
     else:
@@ -2089,14 +2100,16 @@
         #Upper left
         elif d_opt['legend'] == +2:
             leg=pad_1.BuildLegend(0.2, 0.50, 0.5, 0.90)
         elif d_opt['legend'] == +0.2:
             leg=pad_1.BuildLegend(0.2, 0.70, 0.5, 0.90)
         elif d_opt['legend'] == +20:
             leg=pad_1.BuildLegend(0.2, 0.50, 0.8, 0.90)
+        elif d_opt['legend'] == +21:
+            leg=pad_1.BuildLegend(0.2, 0.65, 0.6, 0.95)
         elif d_opt['legend'] == +30:
             leg=pad_1.BuildLegend(0.2, 0.50, 0.6, 0.90)
         elif d_opt['legend'] == -2:
             leg=pad_1.BuildLegend(0.2, 0.20, 0.5, 0.50)
         else:
             log.error('Invalid legend entry: {}'.format(d_opt['legend']))
             raise
@@ -2125,19 +2138,19 @@
         line.SetLineStyle(2)
         line.SetLineWidth(2)
         line.SetLineColor(color)
         line.Draw()
 
     if 'vline' in d_opt:
         xval, color = d_opt['vline']
-        line = ROOT.TLine(xval, ymin, xval, ymax)
-        line.SetLineColor(color)
-        line.SetLineStyle(2)
-        line.SetLineWidth(2)
-        line.Draw()
+        line_v = ROOT.TLine(xval, ymin, xval, ymax)
+        line_v.SetLineColor(color)
+        line_v.SetLineStyle(2)
+        line_v.SetLineWidth(2)
+        line_v.Draw()
 
     if 'logy'  in d_opt and d_opt['logy']:
         pad_1.SetLogy()
 
     if 'ygrid' in d_opt and d_opt['ygrid']:
         pad_1.SetGridy()
 
@@ -4071,24 +4084,25 @@
     v_col_org = rdf.GetColumnNames()
     l_col_org = [name.c_str() for name in v_col_org ]
     l_col     = []
 
     tmva_rgx  = 'tmva_\d+_\d+'
 
     for col in l_col_org:
-        rgx = d_opt['exclude_re']
-        if   rgx is not None and re.match(rgx, col) and     re.match(tmva_rgx, col):
+        user_rgx = d_opt['exclude_re']
+        if user_rgx is not None and re.match(user_rgx, col):
             log.debug(f'Dropping: {col}')
             continue
-        elif rgx is not None and re.match(rgx, col) and not re.match(tmva_rgx, col):
-            log.warning(f'Dropping: {col}')
+
+        if                          re.match(tmva_rgx, col):
+            log.debug(f'Dropping: {col}')
             continue
-        else:
-            log.debug(f'Picking: {col}')
-            l_col.append(col)
+
+        log.debug(f'Picking: {col}')
+        l_col.append(col)
 
     data  = ak.from_rdataframe(rdf, columns=l_col)
     d_data= { col : data[col] for col in l_col }
 
     if arr_val.dtype == 'object':
         arr_val = arr_val.astype(float)
```

### Comparing `rx_scripts-0.3.3/src/utils_noroot.py` & `rx_scripts-0.3.4/src/utils_noroot.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/utils_py2.py` & `rx_scripts-0.3.4/src/utils_py2.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/version_management.py` & `rx_scripts-0.3.4/src/version_management.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/zutils/pdf.py` & `rx_scripts-0.3.4/src/zutils/pdf.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/src/zutils/plot.py` & `rx_scripts-0.3.4/src/zutils/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         self.binned_data       = None
         self.errors            = []
         self._result           = result
         self._suffix           = suffix
         self._leg              = {}
         self._l_blind          = None
+        self._l_plot_components= None
         self.axs               = None
 
         # zfit.settings.advanced_warnings['extend_wrapped_extended'] = False
         warnings.filterwarnings("ignore")
     #----------------------------------------
     def _data_to_zdata(self, obs, data, weights):
         if isinstance(data, np.ndarray):
@@ -107,17 +108,22 @@
             color="black",
             histtype="errorbar",
             label=self._leg.get("Data", "Data"),
             ax=ax,
         )
         self._get_errors(data_hist, errorbars, nbins)
     #----------------------------------------
-    def _pull_hist(self, pdf_hist, nbins=None):
+    def _pull_hist(self, pdf_hist, nbins, data_yield):
         pdf_values  = pdf_hist.values()
         data_values = self.binned_data.values()
+
+        pdf_tot = sum(pdf_values)
+        pdf_scl = data_yield / pdf_tot
+
+        pdf_values  = [ value * pdf_scl for value in pdf_values ]
         pull_errors = [[], []]
         pulls       = []
 
         for [low, up], pdf_val, dat_val in zip(self.errors, pdf_values, data_values):
             res = 0   if dat_val == 0 else dat_val - pdf_val 
             res = float(res)
             err = low if res      > 0 else up
@@ -128,22 +134,22 @@
 
         hst            = hist.axis.Regular(nbins, self.lower, self.upper, name="pulls")
         pull_hist      = hist.Hist(hst)
         pull_hist[...] = pulls
 
         return pull_hist, pull_errors
     #----------------------------------------
-    def _plot_pulls(self, ax, nbins=100): 
+    def _plot_pulls(self, ax, nbins, data_yield): 
         obs_name   = self.obs.obs[0]
         binning    = zfit.binned.RegularBinning(bins=nbins, start=self.lower, stop=self.upper, name=obs_name)
         binned_obs = zfit.Space(obs_name, binning=binning)
         binned_pdf = zfit.pdf.BinnedFromUnbinnedPDF(self.total_model, binned_obs)
         pdf_hist   = binned_pdf.to_hist()
 
-        pull_hist, pull_errors = self._pull_hist(pdf_hist, nbins=nbins) 
+        pull_hist, pull_errors = self._pull_hist(pdf_hist, nbins, data_yield) 
 
         mplhep.histplot(
             pull_hist,
             color   = "black",
             histtype= "errorbar",
             yerr    = np.array(pull_errors),
             ax      = ax,
@@ -182,21 +188,22 @@
         '''
         pdf = self.total_model
 
         if self._result is not None:
             d_par = {}
             for par, d_val in self._result.params.items():
                 val = d_val['value']
+                name= par if isinstance(par, str) else par.name
                 try:
                     err = d_val['hesse']['error']
                 except:
-                    log.warning('Cannot extract Hesse errors, using zeros')
+                    log.warning(f'Cannot extract {name} Hesse errors, using zeros')
+                    pprint.pprint(d_val)
                     err = 0
 
-                name = par if isinstance(par, str) else par.name
                 d_par[name] = [val, err]
         else:
             s_par = pdf.get_params()
             d_par = {par.name : [par.value(), 0] for par in s_par}
 
         return d_par
     #----------------------------------------
@@ -215,17 +222,21 @@
             if add_pars != 'all' and name not in add_pars:
                 continue
 
             line += f'{name:<20}{val:>10.3e}{"+/-":>5}{err:>10.3e}\n'
         
         plt.text(0.65, 0.75, line, fontsize=12, transform=plt.gcf().transFigure)
     #----------------------------------------
-    def _get_axis(self, add_pars):
+    def _get_axis(self, add_pars, skip_pulls):
+        plt.style.use(mplhep.style.LHCb2)
+        if skip_pulls:
+            _, (ax) = plt.subplots(1)
+            return [ax]
+
         if add_pars is None:
-            plt.style.use(mplhep.style.LHCb2)
             fig       = plt.figure()
             gs        = fig.add_gridspec(nrows=2, ncols=1, hspace=0.1, height_ratios=[4, 1])
             axs       = gs.subplots(sharex=True)
 
             return axs.flat
 
         fig = plt.figure(figsize=(13, 7))
@@ -233,42 +244,66 @@
         ax2 = plt.subplot2grid((4,40),(3, 0), rowspan=1, colspan=25)
         plt.subplots_adjust(hspace=0.2)
 
         self._add_pars_box(add_pars)
 
         return [ax1, ax2]
     #----------------------------------------
+    def _get_component_yield(self, model, par):
+        if model.is_extended:
+            par  = model.get_yield()
+            nevt = float(par.value())
+            return nevt
+
+        yild = self.total_model.get_yield()
+        if yild is None:
+            nevs = self.data_weight_np.sum()
+        else:
+            nevs = yild.value().numpy()
+
+        frac = par.value().numpy()
+
+        return frac * nevs
+    #----------------------------------------
     def _plot_model_components(self, nbins, stacked):
         if not hasattr(self.total_model, 'pdfs'):
             return
 
         y = None
-        for model in self.total_model.pdfs: 
-            if not model.is_extended:
-                continue
+        for model, par in zip(self.total_model.pdfs, self.total_model.params.values()): 
+            nevt = self._get_component_yield(model, par)
 
-            par  = model.get_yield()
-            nevt = float(par.value())
-            ax   = self.axs[0]
+            if model.name in self._l_plot_components:
+                l_model = [ (frc, pdf) for pdf, frc in zip(model.pdfs, model.params.values()) ]
+            else:
+                l_model = [ (1, model)]
 
-            this_y = model.pdf(self.x) * nevt / nbins * (self.upper - self.lower)
+            y=self._plot_components(y, nbins, stacked, nevt, l_model)
+    #----------------------------------------
+    def _plot_components(self, y, nbins, stacked, nevt, l_model):
+        ax   = self.axs[0]
+        for frc, model in l_model:
+            this_y = model.pdf(self.x) * nevt * frc / nbins * (self.upper - self.lower)
 
             if stacked:
                 y = this_y if y is None else y + this_y
             else:
                 y = this_y
 
             if (self._l_blind is not None) and (model.name == self._l_blind[0]):
                 log.debug(f'Blinding: {model.name}')
                 y = self._blind_pdf_val(y)
 
             ax.plot(self.x, y, linestyle='--', label=self._leg.get(model.name, model.name))
+
+        return y
     #----------------------------------------
-    def _plot_model(self, ax, model, yields, nbins=100, linestyle="-"):
-        y = model.pdf(self.x) * yields / nbins * (self.upper - self.lower)
+    def _plot_model(self, ax, model, nbins=100, linestyle='-'):
+        data_yield = self.data_weight_np.sum()
+        y = model.pdf(self.x) * data_yield / nbins * (self.upper - self.lower)
 
         if self._l_blind is not None:
             log.debug(f'Blinding: {model.name}')
             y = self._blind_pdf_val(y)
 
         ax.plot(self.x, y, linestyle, label=self._leg.get(model.name, model.name))
     #----------------------------------------
@@ -297,73 +332,94 @@
                 self.lower, self.upper = plot_range
             except TypeError:
                 log.error(f'plot_range argument is expected to be a tuple with two numeric values')
                 raise TypeError
 
         return np.linspace(self.lower, self.upper, 2000)
     #----------------------------------------
+    def _get_data_yield(self, mas_tup):
+        if mas_tup is None:
+            return self.data_weight_np.sum()
+
+        minx, maxx = mas_tup
+        arr_data   = np.array([self.data_np, self.data_weight_np]).T
+
+        arr_data = arr_data[arr_data[:, 0] > minx]
+        arr_data = arr_data[arr_data[:, 0] < maxx]
+
+        [_, arr_wgt] = arr_data.T
+
+        return arr_wgt.sum()
+    #----------------------------------------
     @utnr.timeit
     def plot(self, 
             stacked           = False, 
             blind             = None, 
             no_data           = False, 
             ranges            = None, 
             nbins: int        = 100, 
             unit: str         = "$\\rm{MeV}/\\it{c}^{2}$", 
             xlabel: str       = "", 
             ylabel: str       = "", 
             d_leg: dict       = {}, 
             plot_range: tuple = None, 
+            plot_components   = [],
             ext_text : str    = None, 
             add_pars          = None, 
             ymax              = None,
-            skip_pulls        = False):
+            skip_pulls        = False,
+            axs               = None,
+            ):
         '''
         stacked (bool): If true will stack the PDFs
         ranges:     List of tuples with ranges if any was used for the fit, e.g. [(0, 3), (7, 10)]
         nbins:      Bin numbers
         unit:       Unit for x axis, default is MeV/c^2
         no_data (bool): If true data won't be plotted as well as pull
         xlabel:     xlabel
         ylabel:     ylabel
         d_leg:      Customize legend
         plot_range: Set plot_range
+        plot_components (list): List of strings, with names of PDFs, which are expected to be sums of PDFs and whose components should be plotted separately 
         ext_text:   Text that can be added to plot
         add_pars (list|str): List of names of parameters to be added or string with value 'all' to add all fit parameters. If this is used, plot won't use LHCb style.
         skip_pulls(bool) : Will not draw pulls if True, default False
         ymax (float) : Optional, if specified will be used to set the maximum in plot 
         blind (list) : Optional, if specified will remove data in given range, e.g. [var , -1, +1] as well as pulls, the PDF named "var" will also be blinded
         '''
+        self._l_plot_components = plot_components
+
         self._leg     = d_leg
         self.x        = self._get_xcoor(plot_range)
-        self.axs      = self._get_axis(add_pars)
+        self.axs      = self._get_axis(add_pars, skip_pulls) if axs is None else axs
         self._l_blind = blind
-        total_entries = self.data_weight_np.sum()
+        total_entries = self._get_data_yield(plot_range) 
 
         if not stacked:
-            self._plot_model(self.axs[0], self.total_model,  total_entries, nbins)
+            self._plot_model(self.axs[0], self.total_model, nbins)
 
         self._plot_model_components(nbins, stacked)
 
         if not no_data:
             self._plot_data(self.axs[0], nbins, ranges)
 
         if not skip_pulls and not no_data:
-            self._plot_pulls(self.axs[1], nbins=nbins)
+            self._plot_pulls(self.axs[1], nbins, total_entries)
 
         text           = self._get_text(ext_text)
         xlabel, ylabel = self._get_labels(xlabel, ylabel, unit, nbins)
 
         self.axs[0].legend(title=text, fontsize=20, title_fontsize=20)
         self.axs[0].set(xlabel=xlabel, ylabel=ylabel)
         self.axs[0].set_xlim([self.lower, self.upper])
 
         if ymax is not None:
             self.axs[0].set_ylim([0, ymax])
 
-        self.axs[1].set(xlabel=xlabel, ylabel="pulls")
-        self.axs[1].set_xlim([self.lower, self.upper])
+        if not skip_pulls:
+            self.axs[1].set(xlabel=xlabel, ylabel="pulls")
+            self.axs[1].set_xlim([self.lower, self.upper])
 
         for ax in self.axs:
             ax.label_outer()
 #----------------------------------------
```

### Comparing `rx_scripts-0.3.3/src/zutils/utils.py` & `rx_scripts-0.3.4/src/zutils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import zfit
 import numpy
+import pprint
 
 import pandas            as pnd
 import matplotlib.pyplot as plt
 import utils_noroot      as utnr
 
 from log_store   import log_store
 from zutils.plot import plot      as zfp
@@ -323,32 +324,73 @@
     pdf   = gauss.create_extended(ne)
 
     dat   = zfit.Data.from_numpy(obs=obs, array=arr_val)
     nll   = zfit.loss.ExtendedUnbinnedNLL(model=pdf, data=dat, fit_range=(mu_v - fit_sig * sg_v, mu_v + fit_sig * sg_v))
 
     minimizer = zfit.minimize.Minuit()
     result    = minimizer.minimize(nll)
-    result.hesse()
+    result.hesse(method='minuit_hesse')
     result.freeze()
 
     mu_v = result.params[f'mu_{ival}']['value']
     sg_v = result.params[f'sg_{ival}']['value']
 
     mu_e = result.params[f'mu_{ival}']['hesse']['error']
     sg_e = result.params[f'sg_{ival}']['hesse']['error']
 
     if plot:
         mu_sg_txt = f'$\mu={mu_v:.3f}\pm{mu_e:.3f}$\n$\sigma={sg_v:.3f}\pm{sg_e:.3f}$'
         mu_sg_txt = f'{var_name}\n{mu_sg_txt}' if var_name is not None else var_name
         obj= zfp(data=dat, model=pdf, result=result)
         obj.plot(nbins=50, ext_text=mu_sg_txt, d_leg={'Gauss_ext' : 'Fit', 'Data' : 'Pull'}, plot_range=(mu_v - 4 * sg_v, mu_v + 4 * sg_v))
 
+        val = f'$\mu={mu_v:.3f}\pm{mu_e:.3f}$'
+        err = f'$\sigma={sg_v:.3f}\pm{sg_e:.3f}$'
+
+        obj.axs[0].legend(title=f'{val}\n{err}')
+
         obj.axs[0].set_ylabel('Entries')
         obj.axs[1].set_xlabel('')
 
         obj.axs[0].axvline(x=mu_v - sg_v, color='red', linestyle=':')
-        obj.axs[0].axvline(x=mu_v     , color='red', linestyle='-')
+        obj.axs[0].axvline(x=mu_v       , color='red', linestyle='-')
         obj.axs[0].axvline(x=mu_v + sg_v, color='red', linestyle=':')
 
     return (mu_v, mu_e), (sg_v, sg_e)
 #-------------------------------------------------------
-
+def freq_one(df, good_val, quantity):
+    sr_qnt = df[quantity]
+    ntot   = len(sr_qnt)
+
+    sr_good= sr_qnt[sr_qnt == good_val]
+    ngood  = len(sr_good)
+
+    return ngood, ntot - ngood
+#-------------------------------------------------------
+def add_labels(arr_x, arr_y1, arr_y2, xoff, yoff, l_color=['blue', 'orange'], form='{:.0f}'):
+    [color_1, color_2] = l_color
+    for x, y1, y2 in zip(arr_x, arr_y1, arr_y2):
+        label_1 = form.format(y1)
+        label_2 = form.format(y2)
+
+        plt.annotate(label_1, (x,y1), fontsize=22, textcoords="offset points", xytext=(xoff,-yoff), color=color_1, ha='center')
+        plt.annotate(label_2, (x,y2), fontsize=22, textcoords="offset points", xytext=(xoff, yoff), color=color_2, ha='center')
+#-------------------------------------------------------
+def plot_qlty(df):
+    cnv_y, cnv_n = freq_one(df, 1, 'converged') 
+    sta_y, sta_n = freq_one(df, 0, 'status') 
+    val_y, val_n = freq_one(df, 1, 'valid') 
+
+    xerr = [0.5, 0.5, 0.5]
+    xval = [1.0, 2.0, 3.0]
+    plt.errorbar(xval, [cnv_y, sta_y, val_y], xerr=xerr, label='Good' , marker='o', linestyle='None')
+    plt.errorbar(xval, [cnv_n, sta_n, val_n], xerr=xerr, label='Bad'  , marker='o', linestyle='None')
+
+    add_labels(xval, [cnv_y, sta_y, val_y], [cnv_n, sta_n, val_n], 40, 20)
+
+    plt.title('Fit quality')
+    plt.grid()
+    plt.legend()
+    plt.ylim(0, 1.2 * len(df))
+    plt.xticks(xval, ['Converged', 'Status', 'Valid'])
+    plt.tight_layout()
+#-------------------------------------------------------
```

### Comparing `rx_scripts-0.3.3/tests/test_model_analyzer.py` & `rx_scripts-0.3.4/tests/test_model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/tests/test_nll_plot.py` & `rx_scripts-0.3.4/tests/test_nll_plot.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/tests/test_zdscb.py` & `rx_scripts-0.3.4/tests/test_zdscb.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/tests/test_zfitter_datatype.py` & `rx_scripts-0.3.4/tests/test_zfitter_datatype.py`

 * *Files identical despite different names*

### Comparing `rx_scripts-0.3.3/tests/test_zshape.py` & `rx_scripts-0.3.4/tests/test_zshape.py`

 * *Files identical despite different names*

