# Comparing `tmp/tiskitpy-0.5.tar.gz` & `tmp/tiskitpy-0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiskitpy-0.5.tar", last modified: Thu Apr 18 08:43:57 2024, max compression
+gzip compressed data, was "tiskitpy-0.5rc1.tar", last modified: Mon Jan 15 18:38:34 2024, max compression
```

## Comparing `tiskitpy-0.5.tar` & `tiskitpy-0.5rc1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.548550 tiskitpy-0.5/
--rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskitpy-0.5/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)       83 2024-04-18 08:41:48.000000 tiskitpy-0.5/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     2471 2024-04-18 08:43:57.548243 tiskitpy-0.5/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1661 2024-04-18 08:41:48.000000 tiskitpy-0.5/README.md
--rw-r--r--   0 crawford   (501) admin       (80)       38 2024-04-18 08:43:57.548651 tiskitpy-0.5/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     1486 2024-04-18 08:42:25.000000 tiskitpy-0.5/setup.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.517427 tiskitpy-0.5/tiskitpy/
--rw-r--r--   0 crawford   (501) admin       (80)     2559 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     7173 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/clean_rotator.py
--rw-r--r--   0 crawford   (501) admin       (80)     1897 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/cleaned_stream.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.521020 tiskitpy-0.5/tiskitpy/data_cleaner/
--rw-r--r--   0 crawford   (501) admin       (80)      171 2024-04-18 08:41:48.000000 tiskitpy-0.5/tiskitpy/data_cleaner/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    17324 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/data_cleaner/data_cleaner_tf.py
--rw-r--r--   0 crawford   (501) admin       (80)     5807 2024-04-18 08:41:48.000000 tiskitpy-0.5/tiskitpy/data_cleaner/rf_list.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.523556 tiskitpy-0.5/tiskitpy/decimate/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskitpy-0.5/tiskitpy/decimate/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      184 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/ToDo.md
--rw-r--r--   0 crawford   (501) admin       (80)     1678 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.535787 tiskitpy-0.5/tiskitpy/decimate/__pycache__/
--rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     1871 2023-07-11 20:46:27.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4980 2022-12-16 15:51:31.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     5197 2024-03-14 09:50:19.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)    13928 2022-12-14 10:39:43.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)    14859 2024-03-30 18:46:41.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     7662 2024-03-04 13:29:30.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskitpy-0.5/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc
--rwxr-xr-x   0 crawford   (501) admin       (80)    20984 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/decimate/decimator.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     7968 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/decimate/fir_filter.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.538508 tiskitpy-0.5/tiskitpy/decimate/sac_fir/
--rw-r--r--   0 crawford   (501) admin       (80)      845 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec2
--rw-r--r--   0 crawford   (501) admin       (80)     1218 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec3
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec4
--rw-r--r--   0 crawford   (501) admin       (80)     1866 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec5
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec6
--rw-r--r--   0 crawford   (501) admin       (80)     1898 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec7
--rw-r--r--   0 crawford   (501) admin       (80)       18 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/decimate/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.539404 tiskitpy-0.5/tiskitpy/fir_corr/
--rw-r--r--   0 crawford   (501) admin       (80)       39 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/fir_corr/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    12281 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/fir_corr/fir2caus.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     4766 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/logger.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2295 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/read_mseed.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.540438 tiskitpy-0.5/tiskitpy/response_functions/
--rw-r--r--   0 crawford   (501) admin       (80)      133 2024-04-18 08:41:48.000000 tiskitpy-0.5/tiskitpy/response_functions/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    26927 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/response_functions/response_functions.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.543058 tiskitpy-0.5/tiskitpy/rptransient/
--rw-r--r--   0 crawford   (501) admin       (80)       85 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    23785 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/dirac_comb.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    10790 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/periodic_transient.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3155 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/transients.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3244 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       21 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/rptransient/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.545284 tiskitpy-0.5/tiskitpy/spectral_density/
--rw-r--r--   0 crawford   (501) admin       (80)     2840 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/spectral_density/Peterson_noise_model.py
--rw-r--r--   0 crawford   (501) admin       (80)      125 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/spectral_density/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    74382 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/spectral_density/spectral_density.py
--rw-r--r--   0 crawford   (501) admin       (80)     4174 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/spectral_density/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       18 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/spectral_density/version.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    20747 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/time_spans.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.547465 tiskitpy-0.5/tiskitpy/utils/
--rw-r--r--   0 crawford   (501) admin       (80)      219 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/utils/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    17645 2024-04-18 08:41:49.000000 tiskitpy-0.5/tiskitpy/utils/clean_sequence.py
--rw-r--r--   0 crawford   (501) admin       (80)     2209 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/utils/functions.py
--rw-r--r--   0 crawford   (501) admin       (80)    12134 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/utils/seis_rotate.py
--rw-r--r--   0 crawford   (501) admin       (80)     2811 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/utils/stream_synchronize.py
--rw-r--r--   0 crawford   (501) admin       (80)       20 2024-04-18 08:42:25.000000 tiskitpy-0.5/tiskitpy/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-04-18 08:43:57.519887 tiskitpy-0.5/tiskitpy.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     2471 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     2368 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)      146 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       50 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        9 2024-04-18 08:43:57.000000 tiskitpy-0.5/tiskitpy.egg-info/top_level.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.193991 tiskitpy-0.5rc1/
+-rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskitpy-0.5rc1/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       83 2023-07-13 06:27:46.000000 tiskitpy-0.5rc1/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     2474 2024-01-15 18:38:34.193181 tiskitpy-0.5rc1/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1661 2023-07-13 07:39:52.000000 tiskitpy-0.5rc1/README.md
+-rw-r--r--   0 crawford   (501) admin       (80)       38 2024-01-15 18:38:34.194231 tiskitpy-0.5rc1/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     1404 2023-07-13 08:51:24.000000 tiskitpy-0.5rc1/setup.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.130317 tiskitpy-0.5rc1/tiskitpy/
+-rw-r--r--   0 crawford   (501) admin       (80)     2128 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7239 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/clean_rotator.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1368 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/cleaned_stream.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.134999 tiskitpy-0.5rc1/tiskitpy/data_cleaner/
+-rw-r--r--   0 crawford   (501) admin       (80)      171 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/data_cleaner/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    16955 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/data_cleaner/data_cleaner_tf.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5807 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/data_cleaner/rf_list.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.141809 tiskitpy-0.5rc1/tiskitpy/decimate/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskitpy-0.5rc1/tiskitpy/decimate/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      184 2021-06-11 13:44:08.000000 tiskitpy-0.5rc1/tiskitpy/decimate/ToDo.md
+-rw-r--r--   0 crawford   (501) admin       (80)     1678 2021-06-24 09:28:18.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.164343 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/
+-rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1871 2023-07-11 20:46:27.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4980 2022-12-16 15:51:31.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4903 2024-01-15 18:07:40.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13928 2022-12-14 10:39:43.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13932 2024-01-15 18:05:56.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     7573 2024-01-15 18:05:56.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     5735 2024-01-15 18:08:05.000000 tiskitpy-0.5rc1/tiskitpy/decimate/decimate_SDS.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    18847 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/decimate/decimator.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     7730 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/decimate/fir_filter.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.170029 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/
+-rw-r--r--   0 crawford   (501) admin       (80)      845 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec2
+-rw-r--r--   0 crawford   (501) admin       (80)     1218 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec3
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec4
+-rw-r--r--   0 crawford   (501) admin       (80)     1866 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec5
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec6
+-rw-r--r--   0 crawford   (501) admin       (80)     1898 2012-02-01 20:07:02.000000 tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec7
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2021-06-07 17:29:05.000000 tiskitpy-0.5rc1/tiskitpy/decimate/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.172053 tiskitpy-0.5rc1/tiskitpy/fir_corr/
+-rw-r--r--   0 crawford   (501) admin       (80)       39 2022-07-06 10:50:29.000000 tiskitpy-0.5rc1/tiskitpy/fir_corr/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    12281 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/fir_corr/fir2caus.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3699 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/logger.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2295 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/read_mseed.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.173877 tiskitpy-0.5rc1/tiskitpy/response_functions/
+-rw-r--r--   0 crawford   (501) admin       (80)      133 2023-07-13 06:37:56.000000 tiskitpy-0.5rc1/tiskitpy/response_functions/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    26837 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/response_functions/response_functions.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.180379 tiskitpy-0.5rc1/tiskitpy/rptransient/
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2022-05-04 22:13:23.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    23785 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/dirac_comb.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    10790 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/periodic_transient.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3155 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/transients.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3244 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       21 2021-12-09 22:15:36.000000 tiskitpy-0.5rc1/tiskitpy/rptransient/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.187426 tiskitpy-0.5rc1/tiskitpy/spectral_density/
+-rw-r--r--   0 crawford   (501) admin       (80)     2840 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/spectral_density/Peterson_noise_model.py
+-rw-r--r--   0 crawford   (501) admin       (80)      125 2024-01-11 12:13:30.000000 tiskitpy-0.5rc1/tiskitpy/spectral_density/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    67421 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/spectral_density/spectral_density.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4174 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/spectral_density/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2022-01-06 11:06:02.000000 tiskitpy-0.5rc1/tiskitpy/spectral_density/version.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    20127 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/time_spans.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.192267 tiskitpy-0.5rc1/tiskitpy/utils/
+-rw-r--r--   0 crawford   (501) admin       (80)      300 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/utils/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    17645 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/utils/clean_sequence.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1845 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/utils/functions.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11915 2024-01-15 17:48:29.000000 tiskitpy-0.5rc1/tiskitpy/utils/seis_rotate.py
+-rw-r--r--   0 crawford   (501) admin       (80)       25 2024-01-15 18:02:25.000000 tiskitpy-0.5rc1/tiskitpy/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2024-01-15 18:38:34.133285 tiskitpy-0.5rc1/tiskitpy.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     2474 2024-01-15 18:38:33.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     2365 2024-01-15 18:38:34.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2024-01-15 18:38:33.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       78 2024-01-15 18:38:33.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       50 2024-01-15 18:38:33.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        9 2024-01-15 18:38:33.000000 tiskitpy-0.5rc1/tiskitpy.egg-info/top_level.txt
```

### Comparing `tiskitpy-0.5/LICENSE.txt` & `tiskitpy-0.5rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/PKG-INFO` & `tiskitpy-0.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiskitpy
-Version: 0.5
+Version: 0.5rc1
 Summary: TIme Series toolKIT
 Home-page: https://github.com/WayneCrawford/tiskitpy
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `tiskitpy-0.5/README.md` & `tiskitpy-0.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/setup.py` & `tiskitpy-0.5rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     url="https://github.com/WayneCrawford/tiskitpy",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=['obspy>=1.3.0','PyYAML', 'numpy', 'scipy', 'matplotlib',
                       'xarray'],
     entry_points={
          'console_scripts': [
-            'tiskitpy_decimate_SDS=tiskitpy.scripts.decimate_SDS:main', 
-            'tiskitpy_get_SDS_inventory=tiskitpy.scripts.get_SDS_inventory:main'
+            'tiskitpy_decimate_SDS=tiskitpy.decimate.decimate_SDS:main'
          ]
     },
     python_requires='>=3.8',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
```

### Comparing `tiskitpy-0.5/tiskitpy/__init__.py` & `tiskitpy-0.5rc1/tiskitpy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,39 +25,29 @@
 
 - ``fir2caus`` : Transform zero-phase data to minimum phase (only works
     for LCHEAPO loggers, need to update to calculate/work for any
     zero-phase filter)
 - ``read_MSEED`` : Read MSEED data, even if the file is too big (> 2 GB)
     for obspy's read() function
 - ``Peterson_noise_model`` : Return the Peterson High and Low Noise Models
-- ``stream_synchronize`` : Return a synchronized stream (all traces have
-    same starttime and endtime).  Raises ValueError if not all streams have
-    the same sample_rate
-- ``stream_unmask`` : unmasks data in a stream, interpolating to fill any gaps
 
 Command-line programs
 =========================
 
-Use the `-h` option for help
-
 - ``tiskitpy_decimate_SDS`` : Decimate data stored in a SeisComp Data Structure
-  database.
-- ``tiskitpy_get_SDS_inventory``: Return the inventory corresponding to a
-  SeisComp Data Structure database, using the FDSN Station webservice
+    database.
+    Inserts the data into the same database and creates a new StationXML file
+    (based on an existing StationXML file for the input database)
 """
 from .clean_rotator import CleanRotator
 from .cleaned_stream import CleanedStream
+from .logger import init_logger
 from .data_cleaner import DataCleaner, RFList
 from .decimate import Decimator
 from .rptransient import PeriodicTransient
 from .spectral_density import SpectralDensity, Peterson_noise_model
 from .time_spans import TimeSpans
 from .response_functions import ResponseFunctions
-# Functions
 from .read_mseed import read_MSEED
 from .fir_corr import fir2caus
-from .utils import stream_synchronize, stream_unmask
-# These are only here for tests, there is probably a better way to access/hide them
-from .logger import init_logger
 from .utils import CleanSequence
-
 # from .utils import remove_cleaner_string, CleanerString, CleanSequence
```

### Comparing `tiskitpy-0.5/tiskitpy/clean_rotator.py` & `tiskitpy-0.5rc1/tiskitpy/clean_rotator.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,45 +37,44 @@
         uselogvar(bool): use logarithm of variance as metric
         filt_band (tuple): lower, upper frequency limits of band to filter data
                 before calculating rotation
         save_eq_file (bool): Passed onto TimeSpans.from_eqs()
     Attributes:
         angle (float): angle by which Z (or Z-X-Y) was rotated
         azimuth (float): azimuth by which Z (or Z-X-Y) was rotated
-        variance_reduction (float): amount by which variance was reduced during
-            calculation (0 to 1)
     """
 
     def __init__(self, stream, avoid_spans=None, plot=False, quickTest=False,
                  remove_eq=True, uselogvar=False, verbose=True,
                  filt_band=(0.001, 0.01), save_eq_file=True):
         """
         Calculate rotation angles needed to minimize noise on vertical channel
+
         """
         ignore_spans = self._make_eq_spans(
             remove_eq, stream[0].stats, verbose, save_eq_file
         )
         if avoid_spans is not None:
             ignore_spans += avoid_spans
         filtstream = self._filtstream(stream, filt_band)
         srData = SeisRotate(filtstream)
-        (ang, azi, var_red) = srData.calc_zrotate_opt(
-            ignore_spans=ignore_spans, uselogvar=uselogvar
+        (ang, azi) = srData.calc_zrotate_opt(
+            verbose=verbose, ignore_spans=ignore_spans, uselogvar=uselogvar
         )
+        if verbose:
+            logger.info(f"    Best angle= azimuth is ({ang:.2f}, {azi:.2f})")
         self.angle = ang
         self.azimuth = azi
-        self.variance_reduction = var_red
-        if verbose:
-            logger.info(self.__str__())
         if plot:
             self._plot_filtered_stream(stream, filt_band)
 
     def __str__(self):
-        return "CleanRotator: angle, azimuth, var_red = {:5.2f}, {:6.1f}, {:3.2f}".format(
-            self.angle, self.azimuth, self.variance_reduction)
+        return "CleanRotator: angle, azimuth = {:.2f}, {:.1f} degrees".format(
+            self.angle, self.azimuth
+        )
 
     def _filtstream(self, stream, filt_band):
         """Filter data to tilt noise band for best Angle calc"""
         filtstream = stream.copy()
         filtstream.detrend("demean")
         filtstream.detrend("linear")
         filtstream.filter(
@@ -111,32 +110,28 @@
         trace_view_Z = viewstream.select(component="Z")[0]
         trace_view_rot_Z = view_rot.select(component="Z")[0]
         rotZchan = trace_view_rot_Z.stats.channel
         rotZchan = rotZchan[0] + "R" + rotZchan[2]
         compare_stream = Stream([trace_view_Z, trace_view_rot_Z])
         compare_stream.plot(equal_scale=True, method="full")
 
-    def apply(self, stream, horiz_too=False, rot_limit=20.):
+    def apply(self, stream, horiz_too=False):
         """
         Rotates vertical channel to minimize noise
 
         Arguments:
             stream (Stream): data, must have \\*Z, \\*[1|N] and \\*[2|E]
                 channels
             horiz_too: (bool) rotate horizontals also (use if you believe
                 channels are truly orthogonal, probably a bad idea anyway
                 as long as we use a 2-value rotation)
-            rot_limit (float): Do not rotate if self.angle greater then this value
         Returns:
             strm_rot (Stream): rotated stream
         """
         seis_stream, other_stream = SeisRotate.separate_streams(stream)
-        if self.angle > rot_limit:
-            logger.warning(f'{self.angle=} > {rot_limit=}, not rotating!')
-            return stream
         srData = SeisRotate(stream)
         srData.zrotate(self.angle, self.azimuth, horiz_too)
         srData.Z = CS.tag(srData.Z, TRANS_CODE)
         if other_stream is None:
             return CleanedStream(srData.stream())
         else:
             return CleanedStream(srData.stream() + other_stream)
@@ -174,7 +169,21 @@
             (float): angle by which Z (or Z-X-Y) was rotated
             (float): azimuth by which Z (or Z-X-Y) was rotated
     """
     obj = CleanRotator(stream, avoid_spans, plot, quickTest, remove_eq,
                        uselogvar, verbose, filt_band)
     return obj.apply(stream), obj.rot_angle, obj.rot_azimuth
 
+
+# def extract_corr_z(evstream, tf_name):
+#     """
+#     Return a corrected stream from ATACR EventStream
+#
+#     Args:
+#         evstream (:class:`obstools.atacr.EventStream`):
+#         tf_name (str): transfer function key
+#     Returns:
+#         outstream (Stream): corrected Z stream
+#     """
+#     stream = evstream.sth.select(component='Z').copy()
+#     stream[0].data = evstream.correct[tf_name].flatten()
+#     return stream
```

### Comparing `tiskitpy-0.5/tiskitpy/data_cleaner/data_cleaner_tf.py` & `tiskitpy-0.5rc1/tiskitpy/data_cleaner/data_cleaner_tf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from obspy.core.stream import Stream
 from matplotlib import pyplot as plt
 
 from ..response_functions import ResponseFunctions
 from ..spectral_density import SpectralDensity
 from .rf_list import RFList
 from ..cleaned_stream import CleanedStream
-from ..utils import CleanSequence as CS, stream_synchronize, stream_unmask
+from ..utils import CleanSequence as CS
 from tiskitpy.logger import init_logger
 
 logger = init_logger()
 
 
 class DataCleaner:
     """
@@ -164,75 +164,71 @@
                 domain, time_domain is much slower)
         Returns:
             stream (:class:`obspy.core.stream.Stream`): corrected data
 
         Assumes frequency response function is for counts, not resp_corrected data.
         """
         assert isinstance(stream, Stream)
-        
-        stream = stream_unmask(stream)
+
         # Make sure that the array is not masked
-        # if np.any([np.ma.count_masked(tr.data) for tr in stream]):
-        #     logger.warning('Unmasking masked data (usually a gap or overlap)')
-        #     stream = stream.split().merge(fill_value='interpolate')
+        if np.any([np.ma.count_masked(tr.data) for tr in stream]):
+            logger.warning('Unmasking masked data (usually a gap or overlap)')
+            stream = stream.split().merge(fill_value='interpolate')
 
         out_stream = CleanedStream(stream)
 
         if in_time_domain is True:
             logger.warning("Correcting traces in the time domain: VERY SLOW")
         else:
             logger.info("Correcting traces in the frequency domain")
 
         for rfs in self.RFList:
             in_id = rfs.input_channel_id
             for out_id in rfs.output_channel_ids:
-                # print(f'{out_stream=}, {in_id=}, {out_id=}')
                 in_trace = out_stream.select(id=in_id)[0]
                 out_trace = out_stream.select(id=out_id)[0]
                 out_stream.remove(out_trace)
                 out_trace = self._correct_trace(
-                    in_trace, out_trace,
-                    rfs.freqs, rfs.corrector_wrt_counts(out_id),
-                    in_time_domain
+                    in_trace,
+                    out_trace,
+                    rfs.freqs,
+                    rfs.corrector_wrt_counts(out_id),
+                    in_time_domain,
                 )
                 out_trace = CS.tag(out_trace, in_trace.id)
                 out_stream += out_trace
         return out_stream
 
     def plot(self):
         """
         Plot data cleaning frequency response functions
         """
         self.RFList.plot()
 
-    def _correct_trace(self, in_trace, out_trace, f, rf, in_time_domain=False,
-                       max_reject_sync=0.01):
+    def _correct_trace(self, in_trace, out_trace, f, rf, in_time_domain=False):
         """
         Correct a trace using an input trace and a frequency response function
 
         Note that the frequency response function should be between the trace's units
 
         Args:
             in_trace (:class: `obspy.core.trace.Trace`): input trace
             out_trace (:class: `obspy.core.trace.Trace`): original output trace
             f (:class:`numpy.ndarray`): frequencies
             rf (:class:`numpy.ndarray`): frequency response function between the input
                 and output traces (counts/count)
             in_time_domain (bool): do correction in time domain
-            max_reject_sync (float): max_reject for stream_synchronize()
 
         Returns:
             out_trace_corrected (:class:`obspy.core.trace.Trace`): corrected
                 output trace
         """
-        stream = stream_synchronize(Stream([in_trace, out_trace]), max_reject_sync)
-        in_trace, out_trace = stream[0], stream[1]
-        # self._validate_streams_synchronized(in_trace, out_trace)
-        # in_trace = in_trace.copy()
-        # out_trace = out_trace.copy()
+        self._validate_streams_synchronized(in_trace, out_trace)
+        in_trace = in_trace.copy()
+        out_trace = out_trace.copy()
         in_trace.detrend("linear")
         out_trace.detrend("linear")
         if in_time_domain:
             return self._correct_trace_time(in_trace, out_trace, f, rf)
         else:
             return self._correct_trace_freq(in_trace, out_trace, f, rf)
```

### Comparing `tiskitpy-0.5/tiskitpy/data_cleaner/rf_list.py` & `tiskitpy-0.5rc1/tiskitpy/data_cleaner/rf_list.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/.DS_Store` & `tiskitpy-0.5rc1/tiskitpy/decimate/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__init__.py` & `tiskitpy-0.5rc1/tiskitpy/decimate/__init__.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-39.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jan 23 16:15:58 2024 UTC, .py size: 6379 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,325 +1,307 @@
-00000000: 610d 0d0a 0000 0000 3ee6 af65 eb18 0000  a.......>..e....
+00000000: 610d 0d0a 0000 0000 6874 a565 6816 0000  a.......ht.eh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000020: 0003 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6406  ..d.d.l.m.Z...d.
 00000060: 6407 6c08 6d09 5a09 0100 6408 6409 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 6d0c 5a0c 0100 650b 8300 5a0a  m.Z.m.Z...e...Z.
-00000080: 640a 640b 8400 5a0d 640c 640d 8400 5a0e  d.d...Z.d.d...Z.
-00000090: 640e 640f 8400 5a0f 6410 6411 8400 5a10  d.d...Z.d.d...Z.
-000000a0: 6412 6413 8400 5a11 6402 5300 2914 7a6a  d.d...Z.d.S.).zj
-000000b0: 0a53 6372 6970 7420 746f 2064 6563 696d  .Script to decim
-000000c0: 6174 6520 5344 5320 6461 7461 2c20 7374  ate SDS data, st
-000000d0: 7566 6620 6e65 7720 6368 616e 6e65 6c73  uff new channels
-000000e0: 2069 6e74 6f20 7468 6520 5344 5320 7374   into the SDS st
-000000f0: 7275 6374 7572 650a 616e 6420 7265 7475  ructure.and retu
-00000100: 726e 2074 6865 206d 6f64 6966 6965 6420  rn the modified 
-00000110: 696e 7665 6e74 6f72 790a e900 0000 004e  inventory......N
-00000120: 2901 da04 5061 7468 2901 da04 7265 6164  )...Path)...read
-00000130: 2901 da0e 7265 6164 5f69 6e76 656e 746f  )...read_invento
-00000140: 7279 e901 0000 0029 01da 0944 6563 696d  ry.....)...Decim
-00000150: 6174 6f72 e902 0000 0029 02da 0b69 6e69  ator.....)...ini
-00000160: 745f 6c6f 6767 6572 da14 6368 616e 6765  t_logger..change
-00000170: 5f63 6f6e 736f 6c65 5f6c 6576 656c 6302  _console_levelc.
-00000180: 0000 0000 0000 0000 0000 001e 0000 0012  ................
-00000190: 0000 0043 0000 0073 6803 0000 7c00 6a00  ...C...sh...|.j.
-000001a0: 6401 7500 7210 6402 7d02 6e04 6403 7d02  d.u.r.d.}.n.d.}.
-000001b0: 7401 7402 7c02 8302 0100 7403 6404 7c02  t.t.|.....t.d.|.
-000001c0: 9b02 9d02 8301 0100 7404 7c00 6a05 8301  ........t.|.j...
-000001d0: 7d03 7406 7c00 6a07 8301 7d04 7c00 6a08  }.t.|.j...}.|.j.
-000001e0: 7c04 6a09 1b00 7d05 7406 a00a 6405 7c00  |.j...}.t...d.|.
-000001f0: 6a08 a102 7d06 7406 a00a 6405 7c05 a102  j...}.t...d.|...
-00000200: 7d07 7402 a00b 6406 a00c 7c05 7c07 a102  }.t...d...|.|...
-00000210: a101 0100 7c06 7c07 6b02 728e 740d 6407  ....|.|.k.r.t.d.
-00000220: 7c06 9b00 9d02 8301 8201 6408 6409 8400  |.........d.d...
-00000230: 7c03 a00e a100 4400 8301 4400 9002 5dc0  |.....D...D...].
-00000240: 7d08 7c08 6a0f 7d09 7402 a00b 640a 7c09  }.|.j.}.t...d.|.
-00000250: 9b02 9d02 a101 0100 640b 6409 8400 7c08  ........d.d...|.
-00000260: a00e a100 4400 8301 4400 9002 5d90 7d0a  ....D...D...].}.
-00000270: 7c0a 6a0f 7d0b 7402 a00b 640c 7c0b 9b02  |.j.}.t...d.|...
-00000280: 9d02 a101 0100 640d 6409 8400 7c0a a00e  ......d.d...|...
-00000290: a100 4400 8301 4400 9002 5d60 7d0c 7c0c  ..D...D...]`}.|.
-000002a0: 6a0f 7d0d 7402 a00b 640e 7c0d 9b02 9d02  j.}.t...d.|.....
-000002b0: a101 0100 640f 6409 8400 7c0c a00e a100  ....d.d...|.....
-000002c0: 4400 8301 4400 9002 5d30 7d0e 7c0e 6a0f  D...D...]0}.|.j.
-000002d0: 7d0f 7c0f 6410 1900 7c06 6b02 9001 7362  }.|.d...|.k...sb
-000002e0: 7402 a00b 6411 7c0f 9b02 6412 7c06 9b00  t...d.|...d.|...
-000002f0: 6413 9d05 a101 0100 9001 712a 6e84 7410  d.........q*n.t.
-00000300: 7c01 7c0b 7c0d 7c0f a011 6414 a101 6410  |.|.|.|...d...d.
-00000310: 1900 8304 9001 7394 7402 a012 6411 7c0f  ......s.t...d.|.
-00000320: 9b02 6415 9d03 a101 0100 9001 712a 6e52  ..d.........q*nR
-00000330: 7413 7c01 7c0b 7c0d 7c0f a011 6414 a101  t.|.|.|.|...d...
-00000340: 6410 1900 8304 7c00 6a08 6b02 9001 73d4  d.....|.j.k...s.
-00000350: 7402 a00b 6411 7c0f 9b02 6416 7c00 6a08  t...d.|...d.|.j.
-00000360: 9b00 6413 9d05 a101 0100 9001 712a 6e12  ..d.........q*n.
-00000370: 7402 a00b 6411 7c0f 9b02 6417 9d03 a101  t...d.|...d.....
-00000380: 0100 7c0c 7c07 7c0f 6418 6419 8502 1900  ..|.|.|.d.d.....
-00000390: 1700 1b00 7d10 7c10 a014 a100 0100 7402  ....}.|.......t.
-000003a0: a00b 641a a00c 7c10 6a0f a101 a101 0100  ..d...|.j.......
-000003b0: 7415 7c0e a016 641b 7c0f 9b00 641c 9d03  t.|...d.|...d...
-000003c0: a101 8301 7d11 7402 a00b 641d 7417 7c11  ....}.t...d.t.|.
-000003d0: 8301 641e 9b04 641f 9d03 a101 0100 7c11  ..d...d.......|.
-000003e0: 4400 9001 5d04 7d12 7418 7419 7c12 8301  D...].}.t.t.|...
-000003f0: 6420 8302 7d13 7c13 6410 1900 6a1a 6a1b  d ..}.|.d...j.j.
-00000400: 7c04 6a09 1600 6410 6b02 9002 7292 740d  |.j...d.k...r.t.
-00000410: 6421 7c13 6410 1900 6a1a 6a1b 9b00 6422  d!|.d...j.j...d"
-00000420: 7c04 6a09 9b00 6423 9d05 8301 0100 7c13  |.j...d#......|.
-00000430: 6410 1900 6a1a 6a1c 7c00 6a08 6b03 9002  d...j.j.|.j.k...
-00000440: 72c2 7402 a012 7419 7c12 8301 9b00 6424  r.t...t.|.....d$
-00000450: 7c00 6a08 9b00 6425 9d04 a101 0100 7419  |.j...d%......t.
-00000460: 7c12 6a0f 8301 a011 6414 a101 5c07 7d14  |.j.....d...\.}.
-00000470: 7d15 7d16 7d17 7d18 7d19 7d1a 7401 7402  }.}.}.}.}.}.t.t.
-00000480: 6402 8302 0100 7c04 a01d 7c13 a101 7d1b  d.....|...|...}.
-00000490: 7401 7402 7c02 8302 0100 7c07 7c17 6418  t.t.|.....|.|.d.
-000004a0: 6419 8502 1900 1700 7d1c 7c14 9b00 6414  d.......}.|...d.
-000004b0: 7c15 9b00 6414 7c16 9b00 6414 7c1c 9b00  |...d.|...d.|...
-000004c0: 6414 7c18 9b00 6414 7c19 9b00 6414 7c1a  d.|...d.|...d.|.
-000004d0: 9b00 9d0d 7d1d 7c1b a01e 7c10 7c1d 1b00  ....}.|...|.|...
-000004e0: 6420 a102 0100 9002 7146 7c04 a01f 7c01  d ......qF|...|.
-000004f0: 7c13 a102 7d01 9001 712a 71fc 71ce 71a0  |...}...q*q.q.q.
-00000500: 7c01 5300 2926 6196 0100 000a 2020 2020  |.S.)&a.....    
-00000510: 5468 6520 6d61 696e 2066 756e 6374 696f  The main functio
-00000520: 6e0a 0a20 2020 2053 686f 756c 6420 656e  n..    Should en
-00000530: 7375 7265 2063 6f6e 7469 6e75 6974 7920  sure continuity 
-00000540: 6163 726f 7373 2064 6179 2061 6e64 2079  across day and y
-00000550: 6561 7220 626f 756e 6461 7269 6573 2e0a  ear boundaries..
-00000560: 2020 2020 4375 7272 656e 746c 7920 6a75      Currently ju
-00000570: 7374 2063 6865 636b 7320 6966 2074 6865  st checks if the
-00000580: 2072 6571 7565 7374 6564 2064 6563 696d   requested decim
-00000590: 6174 696f 6e20 6973 2061 6e20 696e 7465  ation is an inte
-000005a0: 6772 616c 2064 6976 6973 6f72 0a20 2020  gral divisor.   
-000005b0: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
-000005c0: 6461 7927 7320 7361 6d70 6c65 7320 616e  day's samples an
-000005d0: 6420 7265 7475 726e 7320 616e 2065 7272  d returns an err
-000005e0: 6f72 2069 6620 6e6f 740a 2020 2020 4f6e  or if not.    On
-000005f0: 6c79 2077 6f72 6b73 2066 6f72 2062 726f  ly works for bro
-00000600: 6164 2d62 616e 6420 6368 616e 6e65 6c73  ad-band channels
-00000610: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00000620: 2020 2020 6172 6773 2028 3a63 6c61 7373      args (:class
-00000630: 3a20 6172 6770 6172 7365 293a 2043 6f6d  : argparse): Com
-00000640: 6d61 6e64 206c 696e 6520 6172 6775 6d65  mand line argume
-00000650: 6e74 730a 2020 2020 2020 2020 696e 7620  nts.        inv 
-00000660: 283a 636c 6173 733a 606f 6273 7079 2e63  (:class:`obspy.c
-00000670: 6f72 652e 696e 7665 6e74 6f72 792e 496e  ore.inventory.In
-00000680: 7665 6e74 6f72 7960 293a 2073 7461 7469  ventory`): stati
-00000690: 6f6e 2069 6e76 656e 746f 7279 0a20 2020  on inventory.   
-000006a0: 2054 da07 5741 524e 494e 47da 0544 4542   T..WARNING..DEB
-000006b0: 5547 7a10 6c6f 6767 696e 675f 6465 6661  UGz.logging_defa
-000006c0: 756c 743d da01 427a 3b6f 7574 7075 7420  ult=..Bz;output 
-000006d0: 7361 6d70 6c69 6e67 2072 6174 6520 7769  sampling rate wi
-000006e0: 6c6c 2062 6520 7b3a 677d 2073 7073 2c20  ll be {:g} sps, 
-000006f0: 6261 6e64 2063 6f64 6520 7769 6c6c 2062  band code will b
-00000700: 6520 7b7d 7a25 6964 656e 7469 6361 6c20  e {}z%identical 
-00000710: 696e 7075 7420 2620 6f75 7470 7574 2062  input & output b
-00000720: 616e 6420 636f 6465 733a 2063 0100 0000  and codes: c....
-00000730: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000740: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
-00000750: 017c 01a0 00a1 0072 047c 0191 0271 0453  .|.....r.|...q.S
-00000760: 00a9 00a9 01da 0669 735f 6469 72a9 02da  .......is_dir...
-00000770: 022e 30da 0178 720d 0000 0072 0d00 0000  ..0..xr....r....
-00000780: fa4c 2f55 7365 7273 2f63 7261 7766 6f72  .L/Users/crawfor
-00000790: 642f 5f57 6f72 6b2f 5072 6f67 7261 6d6d  d/_Work/Programm
-000007a0: 696e 672f 7469 736b 6974 7079 2f74 6973  ing/tiskitpy/tis
-000007b0: 6b69 7470 792f 6465 6369 6d61 7465 2f64  kitpy/decimate/d
-000007c0: 6563 696d 6174 655f 5344 532e 7079 da0a  ecimate_SDS.py..
-000007d0: 3c6c 6973 7463 6f6d 703e 2e00 0000 f300  <listcomp>......
-000007e0: 0000 007a 2064 6563 696d 6174 655f 5344  ...z decimate_SD
-000007f0: 532e 3c6c 6f63 616c 733e 2e3c 6c69 7374  S.<locals>.<list
-00000800: 636f 6d70 3e7a 0b20 7965 6172 5f6e 616d  comp>z. year_nam
-00000810: 653d 6301 0000 0000 0000 0000 0000 0002  e=c.............
-00000820: 0000 0004 0000 0053 0000 0073 1800 0000  .......S...s....
-00000830: 6700 7c00 5d10 7d01 7c01 a000 a100 7204  g.|.].}.|.....r.
-00000840: 7c01 9102 7104 5300 720d 0000 0072 0e00  |...q.S.r....r..
-00000850: 0000 7210 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000860: 0072 1300 0000 7214 0000 0031 0000 0072  .r....r....1...r
-00000870: 1500 0000 7a0a 096e 6574 5f6e 616d 653d  ....z..net_name=
-00000880: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000890: 0004 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
-000008a0: 7c00 5d10 7d01 7c01 a000 a100 7204 7c01  |.].}.|.....r.|.
-000008b0: 9102 7104 5300 720d 0000 0072 0e00 0000  ..q.S.r....r....
-000008c0: 7210 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-000008d0: 1300 0000 7214 0000 0034 0000 0072 1500  ....r....4...r..
-000008e0: 0000 7a0b 0909 7374 615f 6e61 6d65 3d63  ..z...sta_name=c
-000008f0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000900: 0400 0000 5300 0000 7318 0000 0067 007c  ....S...s....g.|
-00000910: 005d 107d 017c 01a0 00a1 0072 047c 0191  .].}.|.....r.|..
-00000920: 0271 0453 0072 0d00 0000 720e 0000 0072  .q.S.r....r....r
-00000930: 1000 0000 720d 0000 0072 0d00 0000 7213  ....r....r....r.
-00000940: 0000 0072 1400 0000 3700 0000 7215 0000  ...r....7...r...
-00000950: 0072 0100 0000 7a0c 0909 0963 6861 5f6e  .r....z....cha_n
-00000960: 616d 653d 7a0f 3a20 6261 6e64 5f63 6f64  ame=z.: band_cod
-00000970: 6520 213d 207a 0a2c 2073 6b69 7070 696e  e != z., skippin
-00000980: 67da 012e 7a1c 3a20 6e6f 7420 696e 2069  g...z.: not in i
-00000990: 6e76 656e 746f 7279 2c20 736b 6970 7069  nventory, skippi
-000009a0: 6e67 7a17 3a20 696e 7620 7361 6d70 6c69  ngz.: inv sampli
-000009b0: 6e67 2072 6174 6520 213d 207a 0c3a 2070  ng rate != z.: p
-000009c0: 726f 6365 7373 696e 6772 0500 0000 4e7a  rocessingr....Nz
-000009d0: 2409 0909 0943 7265 6174 696e 6720 6f75  $....Creating ou
-000009e0: 7470 7574 2063 6861 6e6e 656c 2064 6972  tput channel dir
-000009f0: 2022 7b7d 227a 022a 2e7a 022e 2a7a 0409   "{}"z.*.z..*z..
-00000a00: 0909 09da 0164 7a11 2066 696c 6573 2074  .....dz. files t
-00000a10: 6f20 7072 6f63 6573 73da 054d 5345 4544  o process..MSEED
-00000a20: 7a15 6461 7927 7320 7374 7265 616d 206c  z.day's stream l
-00000a30: 656e 6774 6820 287a 2129 2069 7320 6e6f  ength (z!) is no
-00000a40: 7420 6469 7669 7369 626c 6520 6279 2064  t divisible by d
-00000a50: 6563 696d 6174 6f72 2028 fa01 297a 2020  ecimator (..)z  
-00000a60: 6669 7273 7420 626c 6f63 6b27 7320 7361  first block's sa
-00000a70: 6d70 6c69 6e67 2072 6174 6520 213d 207a  mpling rate != z
-00000a80: 0d2c 2073 6b69 7070 696e 672e 2e2e 2920  ., skipping...) 
-00000a90: da05 7175 6965 7472 0900 0000 da06 6c6f  ..quietr......lo
-00000aa0: 6767 6572 da05 7072 696e 7472 0200 0000  gger..printr....
-00000ab0: da08 5344 535f 726f 6f74 7206 0000 00da  ..SDS_rootr.....
-00000ac0: 0d64 6563 696d 5f66 6163 746f 7273 da11  .decim_factors..
-00000ad0: 696e 7075 745f 7361 6d70 6c65 5f72 6174  input_sample_rat
-00000ae0: 65da 1164 6563 696d 6174 696f 6e5f 6661  e..decimation_fa
-00000af0: 6374 6f72 da0d 6765 745f 6261 6e64 5f63  ctor..get_band_c
-00000b00: 6f64 65da 0469 6e66 6fda 0666 6f72 6d61  ode..info..forma
-00000b10: 74da 0a56 616c 7565 4572 726f 72da 0769  t..ValueError..i
-00000b20: 7465 7264 6972 da04 6e61 6d65 da0f 5f63  terdir..name.._c
-00000b30: 6861 6e6e 656c 5f69 6e5f 696e 76da 0573  hannel_in_inv..s
-00000b40: 706c 6974 da07 7761 726e 696e 67da 0f5f  plit..warning.._
-00000b50: 6368 5f73 616d 706c 655f 7261 7465 da05  ch_sample_rate..
-00000b60: 6d6b 6469 72da 046c 6973 74da 0467 6c6f  mkdir..list..glo
-00000b70: 62da 036c 656e 7203 0000 00da 0373 7472  b..lenr......str
-00000b80: da05 7374 6174 73da 046e 7074 73da 0d73  ..stats..npts..s
-00000b90: 616d 706c 696e 675f 7261 7465 da08 6465  ampling_rate..de
-00000ba0: 6369 6d61 7465 da05 7772 6974 65da 1075  cimate..write..u
-00000bb0: 7064 6174 655f 696e 7665 6e74 6f72 7929  pdate_inventory)
-00000bc0: 1eda 0461 7267 73da 0369 6e76 5a0f 6c6f  ...args..invZ.lo
-00000bd0: 6767 696e 675f 6465 6661 756c 7472 1d00  gging_defaultr..
-00000be0: 0000 da09 6465 6369 6d61 746f 725a 126f  ....decimatorZ.o
-00000bf0: 7574 7075 745f 7361 6d70 6c65 5f72 6174  utput_sample_rat
-00000c00: 65da 0c69 6e5f 6261 6e64 5f63 6f64 655a  e..in_band_codeZ
-00000c10: 0d6f 7574 5f62 616e 645f 636f 6465 5a08  .out_band_codeZ.
-00000c20: 7965 6172 5f64 6972 5a09 7965 6172 5f6e  year_dirZ.year_n
-00000c30: 616d 655a 076e 6574 5f64 6972 5a08 6e65  ameZ.net_dirZ.ne
-00000c40: 745f 6e61 6d65 5a07 7374 615f 6469 725a  t_nameZ.sta_dirZ
-00000c50: 0873 7461 5f6e 616d 655a 0763 6861 5f64  .sta_nameZ.cha_d
-00000c60: 6972 5a08 6368 615f 6e61 6d65 5a0b 6f75  irZ.cha_nameZ.ou
-00000c70: 745f 6368 615f 6469 72da 0566 696c 6573  t_cha_dir..files
-00000c80: da01 66da 0673 7472 6561 6dda 036e 6574  ..f..stream..net
-00000c90: da03 7374 61da 036c 6f63 5a03 6963 68da  ..sta..locZ.ich.
-00000ca0: 0374 7970 da02 7972 da02 6479 5a08 645f  .typ..yr..dyZ.d_
-00000cb0: 7374 7265 616d 5a03 6f63 685a 086f 7574  streamZ.ochZ.out
-00000cc0: 666e 616d 6572 0d00 0000 720d 0000 0072  fnamer....r....r
-00000cd0: 1300 0000 da0c 6465 6369 6d61 7465 5f53  ......decimate_S
-00000ce0: 4453 1100 0000 7384 0000 0000 0d0a 0106  DS....s.........
-00000cf0: 0204 010a 010e 010a 010a 010c 010e 010c  ................
-00000d00: 0108 0104 ff06 0208 010e 0218 0106 0110  ................
-00000d10: 0118 0106 0110 0118 0106 0110 0118 0106  ................
-00000d20: 010e 0118 0106 011a 0112 0106 0120 011a  ............. ..
-00000d30: 0106 0212 0114 0108 0108 0104 ff06 0216  ................
-00000d40: 0118 010a 010e 0118 0102 0110 0204 fe06  ................
-00000d50: ff04 0414 0104 010a 0104 ff06 ff04 031e  ................
-00000d60: 020a 010a 010a 0210 012c 0114 0116 0172  .........,.....r
-00000d70: 4300 0000 6304 0000 0000 0000 0000 0000  C...c...........
-00000d80: 0004 0000 0006 0000 0043 0000 0073 1800  .........C...s..
-00000d90: 0000 7400 7c00 6a01 7c01 7c02 7c03 6401  ..t.|.j.|.|.|.d.
-00000da0: 8d03 8301 6402 6b04 5300 a903 4e29 03da  ....d.k.S...N)..
-00000db0: 076e 6574 776f 726b da07 7374 6174 696f  .network..statio
-00000dc0: 6eda 0763 6861 6e6e 656c 7201 0000 0029  n..channelr....)
-00000dd0: 0272 2e00 0000 da06 7365 6c65 6374 2904  .r......select).
-00000de0: 7237 0000 0072 3d00 0000 723e 0000 00da  r7...r=...r>....
-00000df0: 0363 6861 720d 0000 0072 0d00 0000 7213  .char....r....r.
-00000e00: 0000 0072 2700 0000 6100 0000 7302 0000  ...r'...a...s...
-00000e10: 0000 0172 2700 0000 6304 0000 0000 0000  ...r'...c.......
-00000e20: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00000e30: 0073 2200 0000 7c00 6a00 7c01 7c02 7c03  .s"...|.j.|.|.|.
-00000e40: 6401 8d03 6402 1900 6402 1900 6402 1900  d...d...d...d...
-00000e50: 7d04 7c04 6a01 5300 7244 0000 0029 0272  }.|.j.S.rD...).r
-00000e60: 4800 0000 da0b 7361 6d70 6c65 5f72 6174  H.....sample_rat
-00000e70: 6529 0572 3700 0000 723d 0000 0072 3e00  e).r7...r=...r>.
-00000e80: 0000 7249 0000 005a 0663 6869 6e66 6f72  ..rI...Z.chinfor
-00000e90: 0d00 0000 720d 0000 0072 1300 0000 722a  ....r....r....r*
-00000ea0: 0000 0064 0000 0073 0400 0000 0001 1c01  ...d...s........
-00000eb0: 722a 0000 0063 0100 0000 0000 0000 0000  r*...c..........
-00000ec0: 0000 0300 0000 0400 0000 4300 0000 7348  ..........C...sH
-00000ed0: 0000 0074 007c 006a 0164 0183 027d 0174  ...t.|.j.d...}.t
-00000ee0: 027c 007c 0183 027d 017c 006a 0364 0275  .|.|...}.|.j.d.u
-00000ef0: 0072 307c 006a 01a0 0464 0364 04a1 027d  .r0|.j...d.d...}
-00000f00: 026e 067c 006a 037d 027c 016a 057c 0264  .n.|.j.}.|.j.|.d
-00000f10: 0164 058d 0201 0064 0253 0029 067a 8d0a  .d.....d.S.).z..
-00000f20: 2020 2020 4170 706c 6965 7320 6465 6369      Applies deci
-00000f30: 6d61 7465 5f53 4453 2077 6865 6e20 7468  mate_SDS when th
-00000f40: 6520 696e 7665 6e74 6f72 7920 6973 2069  e inventory is i
-00000f50: 6e20 6120 5374 6174 696f 6e58 4d4c 2066  n a StationXML f
-00000f60: 696c 650a 0a20 2020 2041 7267 733a 0a20  ile..    Args:. 
-00000f70: 2020 2020 2020 2061 7267 7320 283a 636c         args (:cl
-00000f80: 6173 733a 2061 7267 7061 7273 6529 3a20  ass: argparse): 
-00000f90: 436f 6d6d 616e 6420 6c69 6e65 2061 7267  Command line arg
-00000fa0: 756d 656e 7473 0a0a 2020 2020 da0a 5354  uments..    ..ST
-00000fb0: 4154 494f 4e58 4d4c 4e7a 042e 786d 6c7a  ATIONXMLNz..xmlz
-00000fc0: 0a5f 6465 6369 6d2e 786d 6c29 0172 2300  ._decim.xml).r#.
-00000fd0: 0000 2906 7204 0000 00da 0869 6e76 5f66  ..).r......inv_f
-00000fe0: 696c 6572 4300 0000 da0b 6f75 7470 7574  ilerC.....output
-00000ff0: 5f66 696c 65da 0772 6570 6c61 6365 7234  _file..replacer4
-00001000: 0000 0029 0372 3600 0000 7237 0000 00da  ...).r6...r7....
-00001010: 026f 6672 0d00 0000 720d 0000 0072 1300  .ofr....r....r..
-00001020: 0000 da17 6465 6369 6d61 7465 5f53 4453  ....decimate_SDS
-00001030: 5f53 7461 7469 6f6e 584d 4c69 0000 0073  _StationXMLi...s
-00001040: 0c00 0000 0008 0c01 0a01 0a01 1002 0601  ................
-00001050: 7250 0000 0063 0000 0000 0000 0000 0000  rP...c..........
-00001060: 0000 0200 0000 0700 0000 4300 0000 738a  ..........C...s.
-00001070: 0000 0074 006a 0164 0164 028d 017d 007c  ...t.j.d.d...}.|
-00001080: 006a 0264 0364 0464 058d 0201 007c 006a  .j.d.d.d.....|.j
-00001090: 0264 0664 0764 058d 0201 007c 006a 0264  .d.d.d.....|.j.d
-000010a0: 0874 0364 0964 0a8d 0301 007c 006a 0264  .t.d.d.....|.j.d
-000010b0: 0b74 0464 0c67 0064 0da2 0164 0e64 0f8d  .t.d.g.d...d.d..
-000010c0: 0501 007c 006a 0264 1064 1164 0064 1264  ...|.j.d.d.d.d.d
-000010d0: 138d 0401 007c 006a 0264 1464 1564 1664  .....|.j.d.d.d.d
-000010e0: 1764 1864 198d 0501 007c 00a0 05a1 007d  .d.d.....|.....}
-000010f0: 0174 067c 0183 0101 0064 0053 0029 1a4e  .t.|.....d.S.).N
-00001100: 7a38 496e 7365 7274 2064 6563 696d 6174  z8Insert decimat
-00001110: 6564 2063 6861 6e6e 656c 7320 616e 6420  ed channels and 
-00001120: 6372 6561 7465 206e 6577 2053 7461 7469  create new Stati
-00001130: 6f6e 584d 4c20 6669 6c65 2901 da0b 6465  onXML file)...de
-00001140: 7363 7269 7074 696f 6e72 1d00 0000 7a12  scriptionr....z.
-00001150: 5344 5320 726f 6f74 2064 6972 6563 746f  SDS root directo
-00001160: 7279 2901 da04 6865 6c70 724c 0000 007a  ry)...helprL...z
-00001170: 0f53 7461 7469 6f6e 584d 4c20 6669 6c65  .StationXML file
-00001180: 721f 0000 007a 2d50 726f 6365 7373 206f  r....z-Process o
-00001190: 6e6c 7920 6368 616e 6e65 6c73 2068 6176  nly channels hav
-000011a0: 696e 6720 7468 6973 2073 616d 706c 6520  ing this sample 
-000011b0: 7261 7465 2902 da04 7479 7065 7252 0000  rate)...typerR..
-000011c0: 0072 1e00 0000 fa01 2b29 0672 0700 0000  .r......+).r....
-000011d0: e903 0000 00e9 0400 0000 e905 0000 00e9  ................
-000011e0: 0600 0000 e907 0000 007a 2553 6571 7565  .........z%Seque
-000011f0: 6e63 6520 6f66 2064 6563 696d 6174 696f  nce of decimatio
-00001200: 6e20 6661 6374 6f72 7320 746f 2075 7365  n factors to use
-00001210: 2904 7253 0000 00da 056e 6172 6773 da07  ).rS.....nargs..
-00001220: 6368 6f69 6365 7372 5200 0000 7a04 2d2d  choicesrR...z.--
-00001230: 6f66 724d 0000 007a 4a4f 7574 7075 7420  ofrM...zJOutput 
-00001240: 5374 6174 696f 6e58 4d4c 2066 696c 656e  StationXML filen
-00001250: 616d 6520 2864 6566 6175 6c74 203d 2069  ame (default = i
-00001260: 6e66 696c 652e 7265 706c 6163 6528 272e  nfile.replace('.
-00001270: 786d 6c27 2c20 275f 6465 6369 6d2e 786d  xml', '_decim.xm
-00001280: 6c27 2929 03da 0464 6573 74da 0764 6566  l'))...dest..def
-00001290: 6175 6c74 7252 0000 007a 022d 717a 072d  aultrR...z.-qz.-
-000012a0: 2d71 7569 6574 da0a 7374 6f72 655f 7472  -quiet..store_tr
-000012b0: 7565 467a 1d53 7570 7072 6573 7320 696e  ueFz.Suppress in
-000012c0: 666f 726d 6174 696f 6e20 6d65 7373 6167  formation messag
-000012d0: 6573 2903 da06 6163 7469 6f6e 725d 0000  es)...actionr]..
-000012e0: 0072 5200 0000 2907 da08 6172 6770 6172  .rR...)...argpar
-000012f0: 7365 da0e 4172 6775 6d65 6e74 5061 7273  se..ArgumentPars
-00001300: 6572 da0c 6164 645f 6172 6775 6d65 6e74  er..add_argument
-00001310: da05 666c 6f61 74da 0369 6e74 da0a 7061  ..float..int..pa
-00001320: 7273 655f 6172 6773 7250 0000 0029 02da  rse_argsrP...)..
-00001330: 0670 6172 7365 7272 3600 0000 720d 0000  .parserr6...r...
-00001340: 0072 0d00 0000 7213 0000 00da 046d 6169  .r....r......mai
-00001350: 6e7a 0000 0073 2c00 0000 0001 0401 02ff  nz...s,.........
-00001360: 0603 0e01 0601 02ff 0602 0801 02ff 0602  ................
-00001370: 0a01 0601 02fe 0603 0a01 02ff 0603 0a01  ................
-00001380: 04ff 0602 0801 7267 0000 0029 12da 075f  ......rg...)..._
-00001390: 5f64 6f63 5f5f 7260 0000 00da 0770 6174  _doc__r`.....pat
-000013a0: 686c 6962 7202 0000 00da 116f 6273 7079  hlibr......obspy
-000013b0: 2e63 6f72 652e 7374 7265 616d 7203 0000  .core.streamr...
-000013c0: 00da 146f 6273 7079 2e63 6f72 652e 696e  ...obspy.core.in
-000013d0: 7665 6e74 6f72 7972 0400 0000 7238 0000  ventoryr....r8..
-000013e0: 0072 0600 0000 721b 0000 0072 0800 0000  .r....r....r....
-000013f0: 7209 0000 0072 4300 0000 7227 0000 0072  r....rC...r'...r
-00001400: 2a00 0000 7250 0000 0072 6700 0000 720d  *...rP...rg...r.
-00001410: 0000 0072 0d00 0000 720d 0000 0072 1300  ...r....r....r..
-00001420: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001430: 7318 0000 0004 0408 010c 020c 010c 020c  s...............
-00001440: 0110 0206 0308 5008 0308 0508 11         ......P......
+00000070: 6d0b 5a0b 0100 650b 8300 5a0a 640a 640b  m.Z...e...Z.d.d.
+00000080: 8400 5a0c 6410 640c 640d 8401 5a0d 640e  ..Z.d.d.d...Z.d.
+00000090: 640f 8400 5a0e 6402 5300 2911 7a6a 0a53  d...Z.d.S.).zj.S
+000000a0: 6372 6970 7420 746f 2064 6563 696d 6174  cript to decimat
+000000b0: 6520 5344 5320 6461 7461 2c20 7374 7566  e SDS data, stuf
+000000c0: 6620 6e65 7720 6368 616e 6e65 6c73 2069  f new channels i
+000000d0: 6e74 6f20 7468 6520 5344 5320 7374 7275  nto the SDS stru
+000000e0: 6374 7572 650a 616e 6420 7265 7475 726e  cture.and return
+000000f0: 2074 6865 206d 6f64 6966 6965 6420 696e   the modified in
+00000100: 7665 6e74 6f72 790a e900 0000 004e 2901  ventory......N).
+00000110: da04 5061 7468 2901 da04 7265 6164 2901  ..Path)...read).
+00000120: da0e 7265 6164 5f69 6e76 656e 746f 7279  ..read_inventory
+00000130: e901 0000 0029 01da 0944 6563 696d 6174  .....)...Decimat
+00000140: 6f72 e902 0000 0029 01da 0b69 6e69 745f  or.....)...init_
+00000150: 6c6f 6767 6572 6304 0000 0000 0000 0000  loggerc.........
+00000160: 0000 001b 0000 0012 0000 0043 0000 0073  ...........C...s
+00000170: 8e02 0000 7400 7c00 8301 7d00 7401 7c03  ....t.|...}.t.|.
+00000180: 8301 7d04 7c02 7c04 6a02 1b00 7d05 7401  ..}.|.|.j...}.t.
+00000190: a003 6401 7c02 a102 7d06 7401 a003 6401  ..d.|...}.t...d.
+000001a0: 7c05 a102 7d07 7404 a005 6402 a006 7c05  |...}.t...d...|.
+000001b0: 7c07 a102 a101 0100 7c06 7c07 6b02 725a  |.......|.|.k.rZ
+000001c0: 7407 6403 7c06 9b00 9d02 8301 8201 6404  t.d.|.........d.
+000001d0: 6405 8400 7c00 a008 a100 4400 8301 4400  d...|.....D...D.
+000001e0: 9002 5d1a 7d08 7404 a005 6406 7409 7c08  ..].}.t...d.t.|.
+000001f0: 6a0a 8301 9b00 9d02 a101 0100 6407 6405  j...........d.d.
+00000200: 8400 7c08 a008 a100 4400 8301 4400 9001  ..|.....D...D...
+00000210: 5dea 7d09 7404 a005 6408 7409 7c09 6a0a  ].}.t...d.t.|.j.
+00000220: 8301 9b00 9d02 a101 0100 6409 6405 8400  ..........d.d...
+00000230: 7c09 a008 a100 4400 8301 4400 9001 5dba  |.....D...D...].
+00000240: 7d0a 7404 a005 640a 7409 7c0a 6a0a 8301  }.t...d.t.|.j...
+00000250: 9b00 9d02 a101 0100 640b 6405 8400 7c0a  ........d.d...|.
+00000260: a008 a100 4400 8301 4400 9001 5d8a 7d0b  ....D...D...].}.
+00000270: 7404 a005 640c 7409 7c0b 6a0a 8301 9b00  t...d.t.|.j.....
+00000280: 9d02 a101 0100 7c0b 6a0a 7d0c 7c0c 640d  ......|.j.}.|.d.
+00000290: 1900 7c06 6b02 9001 7328 71f6 7c0a 7c07  ..|.k...s(q.|.|.
+000002a0: 7c0c 640e 640f 8502 1900 1700 1b00 7d0d  |.d.d.........}.
+000002b0: 7c0d a00b a100 0100 7404 a005 6410 a006  |.......t...d...
+000002c0: 7c0d 6a0a a101 a101 0100 740c 7c0b a00d  |.j.......t.|...
+000002d0: 6411 7c0c 9b00 6412 9d03 a101 8301 7d0e  d.|...d.......}.
+000002e0: 7404 a005 6413 740e 7c0e 8301 6414 9b04  t...d.t.|...d...
+000002f0: 6415 9d03 a101 0100 7c0e 4400 5dec 7d0f  d.......|.D.].}.
+00000300: 740f 7409 7c0f 8301 6416 8302 7d10 7c10  t.t.|...d...}.|.
+00000310: 640d 1900 6a10 6a11 7c04 6a02 1600 640d  d...j.j.|.j...d.
+00000320: 6b02 9001 72d2 7407 6417 7c10 640d 1900  k...r.t.d.|.d...
+00000330: 6a10 6a11 9b00 6418 7c04 6a02 9b00 6419  j.j...d.|.j...d.
+00000340: 9d05 8301 0100 7c10 640d 1900 6a10 6a12  ......|.d...j.j.
+00000350: 7c02 6b03 9001 72fe 7404 a013 7409 7c0f  |.k...r.t...t.|.
+00000360: 8301 9b00 641a 7c02 9b00 641b 9d04 a101  ....d.|...d.....
+00000370: 0100 7409 7c0f 6a0a 8301 a014 641c a101  ..t.|.j.....d...
+00000380: 5c07 7d11 7d12 7d13 7d14 7d15 7d16 7d17  \.}.}.}.}.}.}.}.
+00000390: 7c04 a015 7c10 a101 7d18 7c07 7c14 640e  |...|...}.|.|.d.
+000003a0: 640f 8502 1900 1700 7d19 7c11 9b00 641c  d.......}.|...d.
+000003b0: 7c12 9b00 641c 7c13 9b00 641c 7c19 9b00  |...d.|...d.|...
+000003c0: 641c 7c15 9b00 641c 7c16 9b00 641c 7c17  d.|...d.|...d.|.
+000003d0: 9b00 9d0d 7d1a 7c18 a016 7c0d 7c1a 1b00  ....}.|...|.|...
+000003e0: 6416 a102 0100 9001 7188 7c04 a017 7c01  d.......q.|...|.
+000003f0: 7c10 a102 7d01 71f6 71c8 719a 716c 7c01  |...}.q.q.q.ql|.
+00000400: 5300 291d 6130 0200 000a 2020 2020 5468  S.).a0....    Th
+00000410: 6520 6d61 696e 2066 756e 6374 696f 6e0a  e main function.
+00000420: 0a20 2020 2053 686f 756c 6420 656e 7375  .    Should ensu
+00000430: 7265 2063 6f6e 7469 6e75 6974 7920 6163  re continuity ac
+00000440: 726f 7373 2064 6179 2061 6e64 2079 6561  ross day and yea
+00000450: 7220 626f 756e 6461 7269 6573 2e0a 2020  r boundaries..  
+00000460: 2020 4375 7272 656e 746c 7920 6a75 7374    Currently just
+00000470: 2063 6865 636b 7320 6966 2074 6865 2072   checks if the r
+00000480: 6571 7565 7374 6564 2064 6563 696d 6174  equested decimat
+00000490: 696f 6e20 6973 2061 6e20 696e 7465 6772  ion is an integr
+000004a0: 616c 2064 6976 6973 6f72 0a20 2020 206f  al divisor.    o
+000004b0: 6620 7468 6520 6375 7272 656e 7420 6461  f the current da
+000004c0: 7927 7320 7361 6d70 6c65 7320 616e 6420  y's samples and 
+000004d0: 7265 7475 726e 7320 616e 2065 7272 6f72  returns an error
+000004e0: 2069 6620 6e6f 740a 2020 2020 4f6e 6c79   if not.    Only
+000004f0: 2077 6f72 6b73 2066 6f72 2062 726f 6164   works for broad
+00000500: 2d62 616e 6420 6368 616e 6e65 6c73 0a0a  -band channels..
+00000510: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000520: 2020 5344 535f 726f 6f74 2028 7374 7220    SDS_root (str 
+00000530: 6f72 2050 6174 6829 3a20 5344 5320 726f  or Path): SDS ro
+00000540: 6f74 2064 6972 6563 746f 7279 0a20 2020  ot directory.   
+00000550: 2020 2020 2069 6e76 2028 3a63 6c61 7373       inv (:class
+00000560: 3a60 6f62 7370 792e 636f 7265 2e69 6e76  :`obspy.core.inv
+00000570: 656e 746f 7279 2e49 6e76 656e 746f 7279  entory.Inventory
+00000580: 6029 3a20 7374 6174 696f 6e20 696e 7665  `): station inve
+00000590: 6e74 6f72 790a 2020 2020 2020 2020 696e  ntory.        in
+000005a0: 7075 745f 7361 6d70 6c65 5f72 6174 6520  put_sample_rate 
+000005b0: 2866 6c6f 6174 293a 2073 616d 706c 6520  (float): sample 
+000005c0: 7261 7465 206f 6620 6461 7461 2074 6f20  rate of data to 
+000005d0: 7072 6f63 6573 730a 2020 2020 2020 2020  process.        
+000005e0: 6465 6369 6d5f 6c69 7374 2028 6c69 7374  decim_list (list
+000005f0: 293a 206c 6973 7420 6f66 2064 6563 696d  ): list of decim
+00000600: 6174 696f 6e20 6661 6374 6f72 7320 2869  ation factors (i
+00000610: 6e74 6567 6572 7320 6265 7477 6565 6e0a  ntegers between.
+00000620: 2020 2020 2020 2020 2020 2020 3220 616e              2 an
+00000630: 6420 3729 0a20 2020 20da 0142 7a3b 6f75  d 7).    ..Bz;ou
+00000640: 7470 7574 2073 616d 706c 696e 6720 7261  tput sampling ra
+00000650: 7465 2077 696c 6c20 6265 207b 3a67 7d20  te will be {:g} 
+00000660: 7370 732c 2062 616e 6420 636f 6465 2077  sps, band code w
+00000670: 696c 6c20 6265 207b 7d7a 2569 6465 6e74  ill be {}z%ident
+00000680: 6963 616c 2069 6e70 7574 2026 206f 7574  ical input & out
+00000690: 7075 7420 6261 6e64 2063 6f64 6573 3a20  put band codes: 
+000006a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000006b0: 0004 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
+000006c0: 7c00 5d10 7d01 7c01 a000 a100 7204 7c01  |.].}.|.....r.|.
+000006d0: 9102 7104 5300 a900 a901 da06 6973 5f64  ..q.S.......is_d
+000006e0: 6972 a902 da02 2e30 da01 7872 0a00 0000  ir.....0..xr....
+000006f0: 720a 0000 00fa 4c2f 5573 6572 732f 6372  r.....L/Users/cr
+00000700: 6177 666f 7264 2f5f 576f 726b 2f50 726f  awford/_Work/Pro
+00000710: 6772 616d 6d69 6e67 2f74 6973 6b69 7470  gramming/tiskitp
+00000720: 792f 7469 736b 6974 7079 2f64 6563 696d  y/tiskitpy/decim
+00000730: 6174 652f 6465 6369 6d61 7465 5f53 4453  ate/decimate_SDS
+00000740: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e2b  .py..<listcomp>+
+00000750: 0000 00f3 0000 0000 7a20 6465 6369 6d61  ........z decima
+00000760: 7465 5f53 4453 2e3c 6c6f 6361 6c73 3e2e  te_SDS.<locals>.
+00000770: 3c6c 6973 7463 6f6d 703e 7a06 2079 6561  <listcomp>z. yea
+00000780: 723d 6301 0000 0000 0000 0000 0000 0002  r=c.............
+00000790: 0000 0004 0000 0053 0000 0073 1800 0000  .......S...s....
+000007a0: 6700 7c00 5d10 7d01 7c01 a000 a100 7204  g.|.].}.|.....r.
+000007b0: 7c01 9102 7104 5300 720a 0000 0072 0b00  |...q.S.r....r..
+000007c0: 0000 720d 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+000007d0: 0072 1000 0000 7211 0000 002d 0000 0072  .r....r....-...r
+000007e0: 1200 0000 7a05 096e 6574 3d63 0100 0000  ....z..net=c....
+000007f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000800: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
+00000810: 017c 01a0 00a1 0072 047c 0191 0271 0453  .|.....r.|...q.S
+00000820: 0072 0a00 0000 720b 0000 0072 0d00 0000  .r....r....r....
+00000830: 720a 0000 0072 0a00 0000 7210 0000 0072  r....r....r....r
+00000840: 1100 0000 2f00 0000 7212 0000 007a 0a09  ..../...r....z..
+00000850: 0973 7461 7469 6f6e 3d63 0100 0000 0000  .station=c......
+00000860: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00000870: 0000 7318 0000 0067 007c 005d 107d 017c  ..s....g.|.].}.|
+00000880: 01a0 00a1 0072 047c 0191 0271 0453 0072  .....r.|...q.S.r
+00000890: 0a00 0000 720b 0000 0072 0d00 0000 720a  ....r....r....r.
+000008a0: 0000 0072 0a00 0000 7210 0000 0072 1100  ...r....r....r..
+000008b0: 0000 3100 0000 7212 0000 007a 0b09 0909  ..1...r....z....
+000008c0: 6368 616e 6e65 6c3d 7201 0000 0072 0500  channel=r....r..
+000008d0: 0000 4e7a 2409 0909 0943 7265 6174 696e  ..Nz$....Creatin
+000008e0: 6720 6f75 7470 7574 2063 6861 6e6e 656c  g output channel
+000008f0: 2064 6972 2022 7b7d 227a 022a 2e7a 022e   dir "{}"z.*.z..
+00000900: 2a7a 0409 0909 09da 0164 7a11 2066 696c  *z.......dz. fil
+00000910: 6573 2074 6f20 7072 6f63 6573 73da 054d  es to process..M
+00000920: 5345 4544 7a15 6461 7927 7320 7374 7265  SEEDz.day's stre
+00000930: 616d 206c 656e 6774 6820 287a 2129 2069  am length (z!) i
+00000940: 7320 6e6f 7420 6469 7669 7369 626c 6520  s not divisible 
+00000950: 6279 2064 6563 696d 6174 6f72 2028 fa01  by decimator (..
+00000960: 297a 2020 6669 7273 7420 626c 6f63 6b27  )z  first block'
+00000970: 7320 7361 6d70 6c69 6e67 2072 6174 6520  s sampling rate 
+00000980: 213d 207a 0d2c 2073 6b69 7070 696e 672e  != z., skipping.
+00000990: 2e2e da01 2e29 1872 0200 0000 7206 0000  .....).r....r...
+000009a0: 00da 1164 6563 696d 6174 696f 6e5f 6661  ...decimation_fa
+000009b0: 6374 6f72 da0d 6765 745f 6261 6e64 5f63  ctor..get_band_c
+000009c0: 6f64 65da 066c 6f67 6765 72da 0469 6e66  ode..logger..inf
+000009d0: 6fda 0666 6f72 6d61 74da 0a56 616c 7565  o..format..Value
+000009e0: 4572 726f 72da 0769 7465 7264 6972 da03  Error..iterdir..
+000009f0: 7374 72da 046e 616d 65da 056d 6b64 6972  str..name..mkdir
+00000a00: da04 6c69 7374 da04 676c 6f62 da03 6c65  ..list..glob..le
+00000a10: 6e72 0300 0000 da05 7374 6174 73da 046e  nr......stats..n
+00000a20: 7074 73da 0d73 616d 706c 696e 675f 7261  pts..sampling_ra
+00000a30: 7465 da07 7761 726e 696e 67da 0573 706c  te..warning..spl
+00000a40: 6974 da08 6465 6369 6d61 7465 da05 7772  it..decimate..wr
+00000a50: 6974 65da 1075 7064 6174 655f 696e 7665  ite..update_inve
+00000a60: 6e74 6f72 7929 1bda 0853 4453 5f72 6f6f  ntory)...SDS_roo
+00000a70: 74da 0369 6e76 da11 696e 7075 745f 7361  t..inv..input_sa
+00000a80: 6d70 6c65 5f72 6174 65da 0a64 6563 696d  mple_rate..decim
+00000a90: 5f6c 6973 74da 0964 6563 696d 6174 6f72  _list..decimator
+00000aa0: 5a12 6f75 7470 7574 5f73 616d 706c 655f  Z.output_sample_
+00000ab0: 7261 7465 da0c 696e 5f62 616e 645f 636f  rate..in_band_co
+00000ac0: 6465 5a0d 6f75 745f 6261 6e64 5f63 6f64  deZ.out_band_cod
+00000ad0: 655a 0879 6561 725f 6469 725a 076e 6574  eZ.year_dirZ.net
+00000ae0: 5f64 6972 5a07 7374 615f 6469 725a 0763  _dirZ.sta_dirZ.c
+00000af0: 6861 5f64 6972 5a08 6368 615f 6e61 6d65  ha_dirZ.cha_name
+00000b00: 5a0b 6f75 745f 6368 615f 6469 72da 0566  Z.out_cha_dir..f
+00000b10: 696c 6573 da01 66da 0673 7472 6561 6dda  iles..f..stream.
+00000b20: 036e 6574 da03 7374 61da 036c 6f63 5a03  .net..sta..locZ.
+00000b30: 6963 68da 0374 7970 da02 7972 da02 6479  ich..typ..yr..dy
+00000b40: 5a08 645f 7374 7265 616d 5a03 6f63 685a  Z.d_streamZ.ochZ
+00000b50: 086f 7574 666e 616d 6572 0a00 0000 720a  .outfnamer....r.
+00000b60: 0000 0072 1000 0000 da0c 6465 6369 6d61  ...r......decima
+00000b70: 7465 5f53 4453 1100 0000 7362 0000 0000  te_SDS....sb....
+00000b80: 1008 0108 010a 010c 010c 0108 0104 ff06  ................
+00000b90: 0208 010e 0218 0116 0118 0116 0118 0116  ................
+00000ba0: 0118 0116 0106 010e 0102 0114 0108 0108  ................
+00000bb0: 0104 ff06 0216 0118 0108 010e 0118 0102  ................
+00000bc0: 0110 0204 fe06 ff04 0412 0104 010a 0102  ................
+00000bd0: ff06 ff04 031e 010a 0110 012c 0114 0114  ...........,....
+00000be0: 0172 3b00 0000 6305 0000 0000 0000 0000  .r;...c.........
+00000bf0: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
+00000c00: 3e00 0000 7400 7c01 6401 8302 7d05 7401  >...t.|.d...}.t.
+00000c10: 7c00 7c05 7c02 7c03 8304 7d05 7c04 6402  |.|.|.|...}.|.d.
+00000c20: 7500 722c 7c01 a002 6403 6404 a102 7d04  u.r,|...d.d...}.
+00000c30: 7c05 6a03 7c04 6401 6405 8d02 0100 6402  |.j.|.d.d.....d.
+00000c40: 5300 2906 6113 0200 000a 2020 2020 4170  S.).a.....    Ap
+00000c50: 706c 6965 7320 6465 6369 6d61 7465 5f53  plies decimate_S
+00000c60: 4453 2077 6865 6e20 7468 6520 696e 7665  DS when the inve
+00000c70: 6e74 6f72 7920 6973 2069 6e20 6120 5374  ntory is in a St
+00000c80: 6174 696f 6e58 4d4c 2066 696c 650a 0a20  ationXML file.. 
+00000c90: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000ca0: 2053 4453 5f72 6f6f 7420 2873 7472 206f   SDS_root (str o
+00000cb0: 7220 5061 7468 293a 2053 4453 2072 6f6f  r Path): SDS roo
+00000cc0: 7420 6469 7265 6374 6f72 790a 2020 2020  t directory.    
+00000cd0: 2020 2020 696e 765f 6669 6c65 2028 7374      inv_file (st
+00000ce0: 7220 6f72 2050 6174 6829 3a20 5061 7468  r or Path): Path
+00000cf0: 2074 6f20 5374 6174 696f 6e58 4d4c 2066   to StationXML f
+00000d00: 696c 650a 2020 2020 2020 2020 696e 7075  ile.        inpu
+00000d10: 745f 7361 6d70 6c65 5f72 6174 6520 2866  t_sample_rate (f
+00000d20: 6c6f 6174 293a 2073 616d 706c 6520 7261  loat): sample ra
+00000d30: 7465 206f 6620 6461 7461 2074 6f20 7072  te of data to pr
+00000d40: 6f63 6573 730a 2020 2020 2020 2020 6465  ocess.        de
+00000d50: 6369 6d5f 6c69 7374 2028 6c69 7374 293a  cim_list (list):
+00000d60: 206c 6973 7420 6f66 2064 6563 696d 6174   list of decimat
+00000d70: 696f 6e20 6661 6374 6f72 7320 2869 6e74  ion factors (int
+00000d80: 6567 6572 7320 6265 7477 6565 6e0a 2020  egers between.  
+00000d90: 2020 2020 2020 2020 2020 3220 616e 6420            2 and 
+00000da0: 3729 0a20 2020 2020 2020 206f 7574 7075  7).        outpu
+00000db0: 745f 6669 6c65 2028 7374 7229 3a20 6f75  t_file (str): ou
+00000dc0: 7470 7574 2053 7461 7469 6f6e 584d 4c20  tput StationXML 
+00000dd0: 6669 6c65 6e61 6d65 2028 4e6f 6e65 203d  filename (None =
+00000de0: 3e20 0a20 2020 2020 2020 2020 2020 2069  > .            i
+00000df0: 6e66 696c 652e 7265 706c 6163 6528 272e  nfile.replace('.
+00000e00: 786d 6c27 2c20 275f 6465 6369 6d2e 786d  xml', '_decim.xm
+00000e10: 6c27 2929 0a0a 2020 2020 5468 6520 6f75  l'))..    The ou
+00000e20: 7470 7574 2053 7461 7469 6f6e 584d 4c20  tput StationXML 
+00000e30: 6669 6c65 2077 696c 6c20 6861 7665 2074  file will have t
+00000e40: 6865 2073 7566 6669 7820 2060 5f64 6563  he suffix  `_dec
+00000e50: 696d 2e78 6d6c 600a 2020 2020 da0a 5354  im.xml`.    ..ST
+00000e60: 4154 494f 4e58 4d4c 4e7a 042e 786d 6c7a  ATIONXMLNz..xmlz
+00000e70: 0a5f 6465 6369 6d2e 786d 6c29 0172 1b00  ._decim.xml).r..
+00000e80: 0000 2904 7204 0000 0072 3b00 0000 da07  ..).r....r;.....
+00000e90: 7265 706c 6163 6572 2a00 0000 2906 722c  replacer*...).r,
+00000ea0: 0000 00da 0869 6e76 5f66 696c 6572 2e00  .....inv_filer..
+00000eb0: 0000 722f 0000 00da 0b6f 7574 7075 745f  ..r/.....output_
+00000ec0: 6669 6c65 722d 0000 0072 0a00 0000 720a  filer-...r....r.
+00000ed0: 0000 0072 1000 0000 da17 6465 6369 6d61  ...r......decima
+00000ee0: 7465 5f53 4453 5f53 7461 7469 6f6e 584d  te_SDS_StationXM
+00000ef0: 4c50 0000 0073 0a00 0000 0010 0a01 0e01  LP...s..........
+00000f00: 0801 0c01 7240 0000 0063 0000 0000 0000  ....r@...c......
+00000f10: 0000 0000 0000 0200 0000 0700 0000 4300  ..............C.
+00000f20: 0000 739a 0000 0074 006a 0164 0164 028d  ..s....t.j.d.d..
+00000f30: 017d 007c 006a 0264 0364 0464 058d 0201  .}.|.j.d.d.d....
+00000f40: 007c 006a 0264 0664 0764 058d 0201 007c  .|.j.d.d.d.....|
+00000f50: 006a 0264 0874 0364 0964 0a8d 0301 007c  .j.d.t.d.d.....|
+00000f60: 006a 0264 0b74 0464 0c67 0064 0da2 0164  .j.d.t.d.g.d...d
+00000f70: 0e64 0f8d 0501 007c 006a 0264 1064 1164  .d.....|.j.d.d.d
+00000f80: 0064 1264 138d 0401 007c 006a 0264 1464  .d.d.....|.j.d.d
+00000f90: 1564 1664 1764 188d 0401 007c 00a0 05a1  .d.d.d.....|....
+00000fa0: 007d 0174 067c 016a 077c 016a 087c 016a  .}.t.|.j.|.j.|.j
+00000fb0: 097c 016a 0a7c 016a 0b83 0501 0064 0053  .|.j.|.j.....d.S
+00000fc0: 0029 194e 7a38 496e 7365 7274 2064 6563  .).Nz8Insert dec
+00000fd0: 696d 6174 6564 2063 6861 6e6e 656c 7320  imated channels 
+00000fe0: 616e 6420 6372 6561 7465 206e 6577 2053  and create new S
+00000ff0: 7461 7469 6f6e 584d 4c20 6669 6c65 2901  tationXML file).
+00001000: da0b 6465 7363 7269 7074 696f 6e72 2c00  ..descriptionr,.
+00001010: 0000 7a12 5344 5320 726f 6f74 2064 6972  ..z.SDS root dir
+00001020: 6563 746f 7279 2901 da04 6865 6c70 723e  ectory)...helpr>
+00001030: 0000 007a 0f53 7461 7469 6f6e 584d 4c20  ...z.StationXML 
+00001040: 6669 6c65 722e 0000 007a 2d50 726f 6365  filer....z-Proce
+00001050: 7373 206f 6e6c 7920 6368 616e 6e65 6c73  ss only channels
+00001060: 2068 6176 696e 6720 7468 6973 2073 616d   having this sam
+00001070: 706c 6520 7261 7465 2902 da04 7479 7065  ple rate)...type
+00001080: 7242 0000 00da 0c64 6563 696d 5f66 6163  rB.....decim_fac
+00001090: 746f 72fa 012b 2906 7207 0000 00e9 0300  tor..+).r.......
+000010a0: 0000 e904 0000 00e9 0500 0000 e906 0000  ................
+000010b0: 00e9 0700 0000 7a26 5365 7175 656e 6365  ......z&Sequence
+000010c0: 206f 6620 6465 6369 6d61 7469 6f6e 2066   of decimation f
+000010d0: 6163 746f 7273 2074 6f20 7573 6529 2904  actors to use)).
+000010e0: 7243 0000 00da 056e 6172 6773 da07 6368  rC.....nargs..ch
+000010f0: 6f69 6365 7372 4200 0000 7a04 2d2d 6f66  oicesrB...z.--of
+00001100: 723f 0000 007a 4a4f 7574 7075 7420 5374  r?...zJOutput St
+00001110: 6174 696f 6e58 4d4c 2066 696c 656e 616d  ationXML filenam
+00001120: 6520 2864 6566 6175 6c74 203d 2069 6e66  e (default = inf
+00001130: 696c 652e 7265 706c 6163 6528 272e 786d  ile.replace('.xm
+00001140: 6c27 2c20 275f 6465 6369 6d2e 786d 6c27  l', '_decim.xml'
+00001150: 2929 03da 0464 6573 74da 0764 6566 6175  ))...dest..defau
+00001160: 6c74 7242 0000 007a 022d 717a 072d 2d71  ltrB...z.-qz.--q
+00001170: 7569 6574 da0a 7374 6f72 655f 7472 7565  uiet..store_true
+00001180: 7a1d 5375 7070 7265 7373 2069 6e66 6f72  z.Suppress infor
+00001190: 6d61 7469 6f6e 206d 6573 7361 6765 7329  mation messages)
+000011a0: 02da 0661 6374 696f 6e72 4200 0000 290c  ...actionrB...).
+000011b0: da08 6172 6770 6172 7365 da0e 4172 6775  ..argparse..Argu
+000011c0: 6d65 6e74 5061 7273 6572 da0c 6164 645f  mentParser..add_
+000011d0: 6172 6775 6d65 6e74 da05 666c 6f61 74da  argument..float.
+000011e0: 0369 6e74 da0a 7061 7273 655f 6172 6773  .int..parse_args
+000011f0: 7240 0000 0072 2c00 0000 723e 0000 0072  r@...r,...r>...r
+00001200: 2e00 0000 7244 0000 0072 3f00 0000 2902  ....rD...r?...).
+00001210: da06 7061 7273 6572 da04 6172 6773 720a  ..parser..argsr.
+00001220: 0000 0072 0a00 0000 7210 0000 00da 046d  ...r....r......m
+00001230: 6169 6e67 0000 0073 3200 0000 0001 0401  aing...s2.......
+00001240: 02ff 0603 0e01 0601 02ff 0602 0801 02ff  ................
+00001250: 0602 0a01 0601 02fe 0603 0a01 02ff 0603  ................
+00001260: 0a01 02ff 0602 0801 0a01 0801 04fe 7259  ..............rY
+00001270: 0000 0029 014e 290f da07 5f5f 646f 635f  ...).N)...__doc_
+00001280: 5f72 5100 0000 da07 7061 7468 6c69 6272  _rQ.....pathlibr
+00001290: 0200 0000 da11 6f62 7370 792e 636f 7265  ......obspy.core
+000012a0: 2e73 7472 6561 6d72 0300 0000 da14 6f62  .streamr......ob
+000012b0: 7370 792e 636f 7265 2e69 6e76 656e 746f  spy.core.invento
+000012c0: 7279 7204 0000 0072 3000 0000 7206 0000  ryr....r0...r...
+000012d0: 0072 1900 0000 7208 0000 0072 3b00 0000  .r....r....r;...
+000012e0: 7240 0000 0072 5900 0000 720a 0000 0072  r@...rY...r....r
+000012f0: 0a00 0000 720a 0000 0072 1000 0000 da08  ....r....r......
+00001300: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
+00001310: 0004 0408 010c 020c 010c 020c 010c 0206  ................
+00001320: 0308 4000 ff0a 17                        ..@....
```

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar 30 18:46:35 2024 UTC, .py size: 20984 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0b5e 0866 f851 0000  a........^.f.Q..
+00000000: 610d 0d0a 0000 0000 ed6f a565 9f49 0000  a........o.e.I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6402 6c09 5a09 6401 6402 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6401 6406 6c0b 6d0c 5a0c 0100 6401  Z.d.d.l.m.Z...d.
@@ -69,15 +69,15 @@
 00000440: 0000 7211 0000 0029 01da 0473 656c 66a9  ..r....)...self.
 00000450: 0072 1400 0000 fa49 2f55 7365 7273 2f63  .r.....I/Users/c
 00000460: 7261 7766 6f72 642f 5f57 6f72 6b2f 5072  rawford/_Work/Pr
 00000470: 6f67 7261 6d6d 696e 672f 7469 736b 6974  ogramming/tiskit
 00000480: 7079 2f74 6973 6b69 7470 792f 6465 6369  py/tiskitpy/deci
 00000490: 6d61 7465 2f64 6563 696d 6174 6f72 2e70  mate/decimator.p
 000004a0: 79da 1164 6563 696d 6174 696f 6e5f 6661  y..decimation_fa
-000004b0: 6374 6f72 3c00 0000 7302 0000 0000 037a  ctor<...s......z
+000004b0: 6374 6f72 3400 0000 7302 0000 0000 037a  ctor4...s......z
 000004c0: 1b44 6563 696d 6174 6f72 2e64 6563 696d  .Decimator.decim
 000004d0: 6174 696f 6e5f 6661 6374 6f72 5463 0300  ation_factorTc..
 000004e0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
 000004f0: 0000 4300 0000 733a 0000 007c 027c 005f  ..C...s:...|.|._
 00000500: 0074 017c 0174 0283 0272 1a7c 00a0 037c  .t.|.t...r.|...|
 00000510: 01a1 0153 0074 017c 0174 0483 0272 2e7c  ...S.t.|.t...r.|
 00000520: 00a0 057c 01a1 0153 0074 0664 0183 0182  ...|...S.t.d....
@@ -102,828 +102,770 @@
 00000650: 6365 4e29 07da 0a6b 6565 705f 6474 7970  ceN)...keep_dtyp
 00000660: 65da 0a69 7369 6e73 7461 6e63 6572 0700  e..isinstancer..
 00000670: 0000 da0b 5f72 756e 5f73 7472 6561 6d72  ...._run_streamr
 00000680: 0800 0000 da0a 5f72 756e 5f74 7261 6365  ......_run_trace
 00000690: da09 5479 7065 4572 726f 7229 0372 1300  ..TypeError).r..
 000006a0: 0000 da04 6461 7461 7217 0000 0072 1400  ....datar....r..
 000006b0: 0000 7214 0000 0072 1500 0000 da08 6465  ..r....r......de
-000006c0: 6369 6d61 7465 4100 0000 730c 0000 0000  cimateA...s.....
+000006c0: 6369 6d61 7465 3900 0000 730c 0000 0000  cimate9...s.....
 000006d0: 0906 010a 010a 010a 010a 027a 1244 6563  ...........z.Dec
 000006e0: 696d 6174 6f72 2e64 6563 696d 6174 654e  imator.decimateN
-000006f0: 6306 0000 0000 0000 0000 0000 000e 0000  c...............
-00000700: 000a 0000 0043 0000 0073 ae01 0000 7c01  .....C...s....|.
+000006f0: 6305 0000 0000 0000 0000 0000 0008 0000  c...............
+00000700: 0009 0000 0043 0000 0073 8400 0000 7c01  .....C...s....|.
 00000710: a000 a100 7d01 7c02 6401 7501 7220 6402  ....}.|.d.u.r d.
-00000720: 6403 8400 7c02 4400 8301 7d06 6e0e 6404  d...|.D...}.n.d.
-00000730: 6403 8400 7c01 4400 8301 7d06 7c06 4400  d...|.D...}.|.D.
-00000740: 9001 5d74 7d07 7c00 6a01 7c01 7c07 6a02  ..]t}.|.j.|.|.j.
-00000750: 7c07 6a03 7c07 6a04 7c07 6a05 7c03 6405  |.j.|.j.|.j.|.d.
-00000760: 6406 8d07 7d08 7c08 6a06 7c07 6a07 6b02  d...}.|.j.|.j.k.
-00000770: 736c 7408 6407 8301 8201 7c00 6a09 7c08  slt.d.....|.j.|.
-00000780: 7c07 6a02 7c07 6a03 7c04 6408 8d04 0100  |.j.|.j.|.d.....
-00000790: 7c07 6a02 9b00 6409 7c07 6a03 9b00 6409  |.j...d.|.j...d.
-000007a0: 7c07 6a04 9b00 7c08 6a0a 9b00 9d06 7d09  |.j...|.j.....}.
-000007b0: 7c08 6a0a 7c07 6a05 6b02 72c4 740b a00c  |.j.|.j.k.r.t...
-000007c0: 640a 7c09 9b00 640b 9d03 a101 0100 7132  d.|...d.......q2
-000007d0: 6e7c 740d 7c01 6a0e 7c07 6a02 7c07 6a03  n|t.|.j.|.j.|.j.
-000007e0: 7c07 6a04 7c08 6a0a 640c 8d04 8301 640d  |.j.|.j.d.....d.
-000007f0: 6b04 9001 7240 640e 7d0a 7c05 640f 7500  k...r@d.}.|.d.u.
-00000800: 9001 7228 740b a00f 7c0a 9b00 6410 7c09  ..r(t...|...d.|.
-00000810: 9b00 6411 9d04 a101 0100 7c01 6a10 7c07  ..d.......|.j.|.
-00000820: 6a02 7c07 6a03 7c07 6a04 7c08 6a0a 640c  j.|.j.|.j.|.j.d.
-00000830: 8d04 7d01 6e18 740b a00f 7c0a 9b00 6410  ..}.n.t...|...d.
-00000840: 7c09 9b00 640b 9d04 a101 0100 7132 6405  |...d.......q2d.
-00000850: 7d0b 7c01 4400 5d48 7d0c 7c0c 6a0a 7c07  }.|.D.]H}.|.j.|.
-00000860: 6a02 6b02 9001 735e 9001 7148 7c0c 4400  j.k...s^..qH|.D.
-00000870: 5d2a 7d0d 7c0d 6a0a 7c07 6a03 6b02 9001  ]*}.|.j.|.j.k...
-00000880: 7262 7c0d 6a11 a012 7c08 a101 0100 640f  rb|.j...|.....d.
-00000890: 7d0b 0100 9001 7148 9001 7162 9001 7148  }.....qH..qb..qH
-000008a0: 7c0b 640f 7501 7232 7408 6412 7c09 9b00  |.d.u.r2t.d.|...
-000008b0: 9d02 8301 8201 7132 7c01 5300 2913 6175  ......q2|.S.).au
-000008c0: 0200 000a 2020 2020 2020 2020 5570 6461  ....        Upda
-000008d0: 7465 2069 6e76 656e 746f 7279 2066 6f72  te inventory for
-000008e0: 2063 6861 6e6e 656c 7320 666f 756e 6420   channels found 
-000008f0: 696e 2073 7472 6561 6d0a 0a20 2020 2020  in stream..     
-00000900: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000910: 2020 2020 2069 6e76 2028 3a63 6c61 7373       inv (:class
-00000920: 3a60 6f62 7370 792e 636f 7265 2e65 7665  :`obspy.core.eve
-00000930: 6e74 732e 696e 7665 6e74 6f72 792e 496e  nts.inventory.In
-00000940: 7665 6e74 6f72 7960 293a 2069 6e76 656e  ventory`): inven
-00000950: 746f 7279 0a20 2020 2020 2020 2020 2020  tory.           
-00000960: 2073 7420 283a 636c 6173 733a 606f 6273   st (:class:`obs
-00000970: 7079 2e63 6f72 652e 7374 7265 616d 2e53  py.core.stream.S
-00000980: 7472 6561 6d60 293a 2064 6174 6120 7374  tream`): data st
-00000990: 7265 616d 2028 7573 6564 2074 6f0a 2020  ream (used to.  
-000009a0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000009b0: 7465 726d 696e 6520 6e65 742f 7374 612f  termine net/sta/
-000009c0: 6368 616e 2f6c 6f63 2063 6f64 6573 292e  chan/loc codes).
-000009d0: 2020 4966 204e 6f6e 652c 2077 696c 6c20    If None, will 
-000009e0: 7570 6461 7465 0a20 2020 2020 2020 2020  update.         
-000009f0: 2020 2020 2020 2065 7665 7279 2063 6861         every cha
-00000a00: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
-00000a10: 206e 6f72 6d61 6c69 7a65 5f66 6972 7320   normalize_firs 
-00000a20: 2862 6f6f 6c29 3a20 6e6f 726d 616c 697a  (bool): normaliz
-00000a30: 6520 4649 5220 6368 616e 6e65 6c73 2074  e FIR channels t
-00000a40: 6861 7420 6172 656e 2774 2061 6c72 6561  hat aren't alrea
-00000a50: 6479 0a20 2020 2020 2020 2020 2020 2069  dy.            i
-00000a60: 6e76 5f66 6f72 6365 5f6f 7665 7277 7269  nv_force_overwri
-00000a70: 7465 2028 626f 6f6c 293a 2049 6620 7468  te (bool): If th
-00000a80: 6520 7461 7267 6574 2063 6861 6e6e 656c  e target channel
-00000a90: 2073 6565 645f 6964 2061 6c72 6561 6479   seed_id already
-00000aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ab0: 2065 7869 7374 7320 2861 6e64 2069 7427   exists (and it'
-00000ac0: 7320 6e6f 7420 7468 6520 736f 7572 6365  s not the source
-00000ad0: 2063 6861 6e6e 656c 2073 6565 645f 6964   channel seed_id
-00000ae0: 292c 206f 7665 7277 7269 7465 2069 740a  ), overwrite it.
-00000af0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00000b00: 3a0a 2020 2020 2020 2020 2020 2020 6f62  :.            ob
-00000b10: 7370 7920 696e 7665 6e74 6f72 7920 7769  spy inventory wi
-00000b20: 7468 206e 6577 2063 6861 6e6e 656c 730a  th new channels.
-00000b30: 2020 2020 2020 2020 4e63 0100 0000 0000          Nc......
-00000b40: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-00000b50: 0000 7312 0000 0067 007c 005d 0a7d 017c  ..s....g.|.].}.|
-00000b60: 016a 0091 0271 0453 0072 1400 0000 2901  .j...q.S.r....).
-00000b70: da05 7374 6174 73a9 02da 022e 30da 0274  ..stats.....0..t
-00000b80: 7272 1400 0000 7214 0000 0072 1500 0000  rr....r....r....
-00000b90: da0a 3c6c 6973 7463 6f6d 703e 6700 0000  ..<listcomp>g...
-00000ba0: f300 0000 007a 2e44 6563 696d 6174 6f72  .....z.Decimator
-00000bb0: 2e75 7064 6174 655f 696e 7665 6e74 6f72  .update_inventor
-00000bc0: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
-00000bd0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00000be0: 0000 0400 0000 0c00 0000 5300 0000 7342  ..........S...sB
-00000bf0: 0000 0067 007c 005d 3a7d 017c 0144 005d  ...g.|.]:}.|.D.]
-00000c00: 307d 027c 0244 005d 267d 0374 0074 017c  0}.|.D.]&}.t.t.|
-00000c10: 016a 027c 026a 027c 036a 037c 036a 027c  .j.|.j.|.j.|.j.|
-00000c20: 036a 0464 008d 0564 018d 0191 0471 1471  .j.d...d.....q.q
-00000c30: 0c71 0453 0029 0229 05da 076e 6574 776f  .q.S.).)...netwo
-00000c40: 726b da07 7374 6174 696f 6eda 086c 6f63  rk..station..loc
-00000c50: 6174 696f 6eda 0763 6861 6e6e 656c da0d  ation..channel..
-00000c60: 7361 6d70 6c69 6e67 5f72 6174 6529 01da  sampling_rate)..
-00000c70: 0668 6561 6465 7229 0572 0900 0000 da04  .header).r......
-00000c80: 6469 6374 da04 636f 6465 da0d 6c6f 6361  dict..code..loca
-00000c90: 7469 6f6e 5f63 6f64 65da 0b73 616d 706c  tion_code..sampl
-00000ca0: 655f 7261 7465 2904 7220 0000 00da 036e  e_rate).r .....n
-00000cb0: 6574 da03 7374 61da 0263 6872 1400 0000  et..sta..chr....
-00000cc0: 7214 0000 0072 1500 0000 7222 0000 0069  r....r....r"...i
-00000cd0: 0000 0073 1800 0000 060a 0201 0801 08f5  ...s............
-00000ce0: 0201 0201 0401 0401 0401 0401 04fb 04ff  ................
-00000cf0: 4629 0672 2400 0000 7225 0000 0072 2600  F).r$...r%...r&.
-00000d00: 0000 7227 0000 00da 0e6e 6f72 6d61 6c69  ..r'.....normali
-00000d10: 7a65 5f66 6972 73da 0d69 6e73 6572 745f  ze_firs..insert_
-00000d20: 696e 5f69 6e76 7a2f 6461 7461 2061 6e64  in_invz/data and
-00000d30: 206d 6574 6164 6174 6120 7361 6d70 6c69   metadata sampli
-00000d40: 6e67 2072 6174 6573 2061 7265 2064 6966  ng rates are dif
-00000d50: 6665 7265 6e74 21a9 0372 2e00 0000 722f  ferent!..r....r/
-00000d60: 0000 00da 0571 7569 6574 da01 2e7a 2d4e  .....quiet...z-N
-00000d70: 6577 2063 6861 6e6e 656c 2068 6173 2073  ew channel has s
-00000d80: 616d 6520 636f 6465 2061 7320 736f 7572  ame code as sour
-00000d90: 6365 2063 6861 6e6e 656c 2028 7a0c 292c  ce channel (z.),
-00000da0: 2072 656a 6563 7465 6421 a904 7224 0000   rejected!..r$..
-00000db0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00000dc0: 7201 0000 007a 334e 6577 2063 6861 6e6e  r....z3New chann
-00000dd0: 656c 2068 6173 2073 616d 6520 7365 6564  el has same seed
-00000de0: 5f69 6420 6173 2061 6e20 6578 6973 7469  _id as an existi
-00000df0: 6e67 2063 6861 6e6e 656c 54fa 0220 287a  ng channelT.. (z
-00000e00: 0f29 2c20 6f76 6572 7772 6974 696e 6721  .), overwriting!
-00000e10: 7a18 4469 6420 6e6f 7420 6669 6e64 2061  z.Did not find a
-00000e20: 2068 6f6d 6520 666f 7220 2913 da04 636f   home for )...co
-00000e30: 7079 da12 5f64 7570 6c69 6361 7465 5f63  py.._duplicate_c
-00000e40: 6861 6e6e 656c 7224 0000 0072 2500 0000  hannelr$...r%...
-00000e50: 7226 0000 0072 2700 0000 722d 0000 0072  r&...r'...r-...r
-00000e60: 2800 0000 da0a 5661 6c75 6545 7272 6f72  (.....ValueError
-00000e70: da0c 5f6d 6f64 6966 795f 6368 616e 722b  .._modify_chanr+
-00000e80: 0000 00da 066c 6f67 6765 72da 0565 7272  .....logger..err
-00000e90: 6f72 da03 6c65 6eda 0673 656c 6563 74da  or..len..select.
-00000ea0: 0777 6172 6e69 6e67 da06 7265 6d6f 7665  .warning..remove
-00000eb0: da08 6368 616e 6e65 6c73 da06 6170 7065  ..channels..appe
-00000ec0: 6e64 290e 7213 0000 00da 0369 6e76 da02  nd).r......inv..
-00000ed0: 7374 7231 0000 0072 3400 0000 5a13 696e  str1...r4...Z.in
-00000ee0: 765f 666f 7263 655f 6f76 6572 7772 6974  v_force_overwrit
-00000ef0: 655a 0a73 7461 7473 5f6c 6973 7472 1e00  eZ.stats_listr..
-00000f00: 0000 da07 6e65 775f 6368 61da 0773 6565  ....new_cha..see
-00000f10: 645f 6964 5a0b 626f 696c 6572 706c 6174  d_idZ.boilerplat
-00000f20: 65da 0861 7070 656e 6465 6472 2e00 0000  e..appendedr....
-00000f30: 722f 0000 0072 1400 0000 7214 0000 0072  r/...r....r....r
-00000f40: 1500 0000 da10 7570 6461 7465 5f69 6e76  ......update_inv
-00000f50: 656e 746f 7279 5200 0000 736c 0000 0000  entoryR...sl....
-00000f60: 1308 0108 0110 0206 0a02 f606 0e0a 0104  ................
-00000f70: 0102 0104 0104 0104 0104 0102 0102 f906  ................
-00000f80: 090c 0102 0102 ff04 0204 010c ff06 0320  ............... 
-00000f90: 010c 0206 0102 ff0a 0204 010e 0108 ff06  ................
-00000fa0: 0102 ff06 0204 010a 0116 010c 0108 ff08  ................
-00000fb0: 0316 0102 0204 0108 010e 0104 0108 010e  ................
-00000fc0: 010c 0104 010e 0108 0110 017a 1a44 6563  ...........z.Dec
-00000fd0: 696d 6174 6f72 2e75 7064 6174 655f 696e  imator.update_in
-00000fe0: 7665 6e74 6f72 79da 012a 6308 0000 0000  ventory..*c.....
-00000ff0: 0000 0000 0000 000e 0000 000b 0000 0043  ...............C
-00001000: 0000 0073 7400 0000 7c01 a000 a100 7d01  ...st...|.....}.
-00001010: 7c01 6a01 7c02 7c03 7c05 7c04 6401 8d04  |.j.|.|.|.|.d...
-00001020: 7d08 7c08 4400 5d50 7d09 7c09 4400 5d46  }.|.D.]P}.|.D.]F
-00001030: 7d0a 7c0a a000 a100 7d0b 7c0b 4400 5d34  }.|.....}.|.D.]4
-00001040: 7d0c 7c00 6a02 7c01 7c09 6a03 7c0a 6a03  }.|.j.|.|.j.|.j.
-00001050: 7c0c 6a04 7c0c 6a03 7c07 6402 8d06 7d0d  |.j.|.j.|.d...}.
-00001060: 7c00 6a05 7c0d 7c02 7c03 7c06 6403 8d04  |.j.|.|.|.|.d...
-00001070: 0100 7136 7126 711e 7c01 5300 2904 6104  ..q6q&q.|.S.).a.
-00001080: 0300 000a 2020 2020 2020 2020 5570 6461  ....        Upda
-00001090: 7465 2069 6e76 656e 746f 7279 2062 6173  te inventory bas
-000010a0: 6564 206f 6e20 6e65 7477 6f72 6b2c 2073  ed on network, s
-000010b0: 7461 7469 6f6e 2c20 6368 616e 6e65 6c20  tation, channel 
-000010c0: 616e 6420 6c6f 6361 7469 6f6e 2063 6f64  and location cod
-000010d0: 6573 0a0a 2020 2020 2020 2020 4172 6773  es..        Args
-000010e0: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-000010f0: 7620 283a 636c 6173 733a 606f 6273 7079  v (:class:`obspy
-00001100: 2e63 6f72 652e 6576 656e 7473 2e69 6e76  .core.events.inv
-00001110: 656e 746f 7279 2e49 6e76 656e 746f 7279  entory.Inventory
-00001120: 6029 3a20 696e 7665 6e74 6f72 790a 2020  `): inventory.  
-00001130: 2020 2020 2020 2020 2020 6e65 7477 6f72            networ
-00001140: 6b20 2873 7472 293a 2046 4453 4e20 6e65  k (str): FDSN ne
-00001150: 7477 6f72 6b20 636f 6465 0a20 2020 2020  twork code.     
-00001160: 2020 2020 2020 2073 7461 7469 6f6e 2028         station (
-00001170: 7374 7229 3a20 7374 6174 696f 6e20 636f  str): station co
-00001180: 6465 0a20 2020 2020 2020 2020 2020 2063  de.            c
-00001190: 6861 6e6e 656c 2028 7374 7229 3a20 6368  hannel (str): ch
-000011a0: 616e 6e65 6c20 636f 6465 0a20 2020 2020  annel code.     
-000011b0: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
-000011c0: 2873 7472 293a 2046 4453 4e20 6c6f 6361  (str): FDSN loca
-000011d0: 7469 6f6e 2063 6f64 650a 2020 2020 2020  tion code.      
-000011e0: 2020 2020 2020 7175 6965 7420 2862 6f6f        quiet (boo
-000011f0: 6c29 3a20 446f 206e 6f74 2073 6179 2077  l): Do not say w
-00001200: 6861 7420 6368 616e 6e65 6c28 7329 2077  hat channel(s) w
-00001210: 6173 2063 6861 6e67 6564 0a20 2020 2020  as changed.     
-00001220: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-00001230: 5f66 6972 7320 2862 6f6f 6c29 3a20 6e6f  _firs (bool): no
-00001240: 726d 616c 697a 6520 4649 5220 6368 616e  rmalize FIR chan
-00001250: 6e65 736c 2074 6861 7420 6172 656e 2774  nesl that aren't
-00001260: 2061 6c72 6561 6479 0a0a 2020 2020 2020   already..      
-00001270: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00001280: 2020 2020 2020 206e 6577 696e 763a 2069         newinv: i
-00001290: 6e76 2028 3a63 6c61 7373 3a60 6f62 7370  nv (:class:`obsp
-000012a0: 792e 636f 7265 2e65 7665 6e74 732e 696e  y.core.events.in
-000012b0: 7665 6e74 6f72 792e 496e 7665 6e74 6f72  ventory.Inventor
-000012c0: 7960 293a 0a20 2020 2020 2020 2020 2020  y`):.           
-000012d0: 2020 2020 2075 7064 6174 6564 2069 6e76       updated inv
-000012e0: 656e 746f 7279 0a0a 2020 2020 2020 2020  entory..        
-000012f0: 6e65 7477 6f72 6b2c 2073 7461 7469 6f6e  network, station
-00001300: 2c20 6368 616e 6e65 6c20 616e 6420 6c6f  , channel and lo
-00001310: 6361 7469 6f6e 2063 6f64 6573 2061 7265  cation codes are
-00001320: 2027 2a27 2062 7920 6465 6661 756c 742c   '*' by default,
-00001330: 0a20 2020 2020 2020 206d 6179 2069 6e63  .        may inc
-00001340: 6c75 6465 2077 696c 6463 6172 6473 2061  lude wildcards a
-00001350: 7320 7370 6563 6966 6965 6420 696e 206f  s specified in o
-00001360: 6273 7079 2e63 6f72 652e 7374 7265 616d  bspy.core.stream
-00001370: 2e53 7472 6561 6d2e 7365 6c65 6374 0a20  .Stream.select. 
-00001380: 2020 2020 2020 2072 3600 0000 2901 7231         r6...).r1
-00001390: 0000 0072 3300 0000 2906 7238 0000 0072  ...r3...).r8...r
-000013a0: 3f00 0000 7239 0000 0072 2b00 0000 722c  ?...r9...r+...r,
-000013b0: 0000 0072 3b00 0000 290e 7213 0000 0072  ...r;...).r....r
-000013c0: 4400 0000 7224 0000 0072 2500 0000 7227  D...r$...r%...r'
-000013d0: 0000 0072 2600 0000 7234 0000 0072 3100  ...r&...r4...r1.
-000013e0: 0000 5a0c 696e 765f 7365 6c65 6374 6564  ..Z.inv_selected
-000013f0: 722e 0000 0072 2f00 0000 5a07 6f6c 645f  r....r/...Z.old_
-00001400: 7374 61da 0363 6861 7246 0000 0072 1400  sta..charF...r..
-00001410: 0000 7214 0000 0072 1500 0000 da1a 7570  ..r....r......up
-00001420: 6461 7465 5f69 6e76 656e 746f 7279 5f66  date_inventory_f
-00001430: 726f 6d5f 6e73 6c63 a500 0000 732e 0000  rom_nslc....s...
-00001440: 0000 1608 0104 0102 0102 0102 0102 fc06  ................
-00001450: 0608 0108 0108 0108 0104 0102 0104 0104  ................
-00001460: 0104 0104 0102 fa06 0804 0108 ff0c 037a  ...............z
-00001470: 2444 6563 696d 6174 6f72 2e75 7064 6174  $Decimator.updat
-00001480: 655f 696e 7665 6e74 6f72 795f 6672 6f6d  e_inventory_from
-00001490: 5f6e 736c 6363 0200 0000 0000 0000 0000  _nslcc..........
-000014a0: 0000 0200 0000 0400 0000 4300 0000 730e  ..........C...s.
-000014b0: 0100 0074 007c 0083 0164 016b 0372 1c74  ...t.|...d.k.r.t
-000014c0: 0164 027c 009b 0264 039d 0383 0182 017c  .d.|...d.......|
-000014d0: 0064 0476 0072 ae7c 0164 056b 0572 3064  .d.v.r.|.d.k.r0d
-000014e0: 0653 007c 0164 076b 0572 3c64 0853 007c  .S.|.d.k.r<d.S.|
-000014f0: 0164 096b 0572 4864 0a53 007c 0164 0b6b  .d.k.rHd.S.|.d.k
-00001500: 0572 5464 0c53 007c 0164 016b 0472 6064  .rTd.S.|.d.k.r`d
-00001510: 0d53 007c 0164 0e6b 0472 6c64 0f53 007c  .S.|.d.k.rld.S.|
-00001520: 0164 106b 0472 7864 1153 007c 0164 126b  .d.k.rxd.S.|.d.k
-00001530: 0472 8464 1353 007c 0164 146b 0572 9064  .r.d.S.|.d.k.r.d
-00001540: 1553 007c 0164 166b 0572 9c64 1753 007c  .S.|.d.k.r.d.S.|
-00001550: 0164 186b 0572 a864 1953 0064 1a53 006e  .d.k.r.d.S.d.S.n
-00001560: 5c7c 0064 1b76 0090 0072 fa7c 0164 056b  \|.d.v...r.|.d.k
-00001570: 0572 c464 1c53 007c 0164 076b 0572 d064  .r.d.S.|.d.k.r.d
-00001580: 1d53 007c 0164 096b 0572 dc64 1e53 007c  .S.|.d.k.r.d.S.|
-00001590: 0164 0b6b 0590 0072 ea64 1f53 0074 02a0  .d.k...r.d.S.t..
-000015a0: 0364 20a1 0101 0064 2153 006e 1074 0464  .d ....d!S.n.t.d
-000015b0: 227c 009b 0064 239d 0383 0182 0164 2453  "|...d#......d$S
-000015c0: 0029 257a dd0a 2020 2020 2020 2020 5265  .)%z..        Re
-000015d0: 7475 726e 2074 6865 2063 6861 6e6e 656c  turn the channel
-000015e0: 2062 616e 6420 636f 6465 2062 6173 6564   band code based
-000015f0: 206f 6e20 616e 2069 6e70 7574 2062 616e   on an input ban
-00001600: 645f 636f 6465 0a0a 2020 2020 2020 2020  d_code..        
-00001610: 3a70 6172 616d 2069 6e5f 6261 6e64 5f63  :param in_band_c
-00001620: 6f64 653a 2069 6e70 7574 2062 616e 6420  ode: input band 
-00001630: 636f 6465 2028 2742 2720 6966 2063 7574  code ('B' if cut
-00001640: 6f66 6620 3e20 3130 732c 0a20 2020 2020  off > 10s,.     
-00001650: 2020 2020 2020 2027 5327 206f 7468 6572         'S' other
-00001660: 7769 7365 290a 2020 2020 2020 2020 3a70  wise).        :p
-00001670: 6172 616d 2073 616d 706c 655f 7261 7465  aram sample_rate
-00001680: 3a20 696e 7075 7420 7361 6d70 6c65 2072  : input sample r
-00001690: 6174 6520 2873 7073 290a 2020 2020 2020  ate (sps).      
-000016a0: 2020 720c 0000 007a 0e22 696e 5f62 616e    r....z."in_ban
-000016b0: 645f 636f 6465 3d7a 1c22 2069 7320 6d6f  d_code=z." is mo
-000016c0: 7265 2074 6861 6e20 6f6e 6520 6368 6172  re than one char
-000016d0: 6163 7465 725a 0c46 4348 424d 4c56 5552  acterZ.FCHBMLVUR
-000016e0: 5054 5169 e803 0000 da01 46e9 fa00 0000  PTQi......F.....
-000016f0: da01 43e9 5000 0000 da01 48e9 0a00 0000  ..C.P.....H.....
-00001700: da01 42da 014d 6733 3333 3333 33d3 3fda  ..B..Mg333333.?.
-00001710: 014c 67b8 1e85 eb51 b89e 3fda 0156 67fa  .Lg....Q..?..Vg.
-00001720: 7e6a bc74 9368 3fda 0155 672d 431c ebe2  ~j.t.h?..Ug-C...
-00001730: 361a 3fda 0152 67f1 68e3 88b5 f8e4 3eda  6.?..Rg.h.....>.
-00001740: 0150 678d edb5 a0f7 c6b0 3eda 0154 da01  .Pg.......>..T..
-00001750: 515a 0447 4445 53da 0147 da01 44da 0145  QZ.GDES..G..D..E
-00001760: da01 537a 2853 686f 7274 2070 6572 696f  ..Sz(Short perio
-00001770: 6420 7365 6e73 6f72 2073 616d 706c 6520  d sensor sample 
-00001780: 7261 7465 203c 2031 3020 7370 73da 0158  rate < 10 sps..X
-00001790: 7a19 556e 6b6e 6f77 6e20 6261 6e64 2062  z.Unknown band b
-000017a0: 6173 6520 636f 6465 3a20 22fa 0122 4e29  ase code: ".."N)
-000017b0: 0572 3e00 0000 723a 0000 00da 0877 6172  .r>...r:.....war
-000017c0: 6e69 6e67 73da 0477 6172 6e72 1b00 0000  nings..warnr....
-000017d0: 2902 da0c 696e 5f62 616e 645f 636f 6465  )...in_band_code
-000017e0: 722d 0000 0072 1400 0000 7214 0000 0072  r-...r....r....r
-000017f0: 1500 0000 da0d 6765 745f 6261 6e64 5f63  ......get_band_c
-00001800: 6f64 65d3 0000 0073 4c00 0000 0009 0c01  ode....sL.......
-00001810: 1001 0801 0801 0401 0801 0401 0801 0401  ................
-00001820: 0801 0401 0801 0401 0801 0401 0801 0401  ................
-00001830: 0801 0401 0801 0401 0801 0401 0801 0402  ................
-00001840: 0601 0a01 0801 0401 0801 0401 0801 0401  ................
-00001850: 0a01 0402 0a01 0602 7a17 4465 6369 6d61  ........z.Decima
-00001860: 746f 722e 6765 745f 6261 6e64 5f63 6f64  tor.get_band_cod
-00001870: 6563 0400 0000 0000 0000 0000 0000 0400  ec..............
-00001880: 0000 0700 0000 4300 0000 7334 0000 007c  ......C...s4...|
-00001890: 017c 00a0 007c 017c 02a1 026b 0372 2874  .|...|.|...k.r(t
-000018a0: 01a0 0264 017c 019b 0064 027c 029b 0064  ...d.|...d.|...d
-000018b0: 039d 05a1 0101 007c 00a0 007c 017c 03a1  .......|...|.|..
-000018c0: 0253 0029 047a cc0a 2020 2020 2020 2020  .S.).z..        
-000018d0: 5265 7475 726e 2074 6865 2063 6861 6e6e  Return the chann
-000018e0: 656c 2062 616e 6420 636f 6465 0a0a 2020  el band code..  
-000018f0: 2020 2020 2020 3a70 6172 616d 2069 6e5f        :param in_
-00001900: 6261 6e64 5f63 6f64 653a 2069 6e70 7574  band_code: input
-00001910: 2062 616e 6420 636f 6465 0a20 2020 2020   band code.     
-00001920: 2020 203a 7061 7261 6d20 696e 5f73 616d     :param in_sam
-00001930: 706c 655f 7261 7465 3a20 696e 7075 7420  ple_rate: input 
-00001940: 7361 6d70 6c65 2072 6174 6520 2873 7073  sample rate (sps
-00001950: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
-00001960: 206f 7574 5f73 616d 706c 655f 7261 7465   out_sample_rate
-00001970: 3a20 6f75 7470 7574 2073 616d 706c 6520  : output sample 
-00001980: 7261 7465 2028 7370 7329 0a20 2020 2020  rate (sps).     
-00001990: 2020 207a 1149 6e70 7574 2062 616e 6420     z.Input band 
-000019a0: 636f 6465 2028 7a27 2920 646f 6573 206e  code (z') does n
-000019b0: 6f74 206d 6174 6368 2020 696e 7075 7420  ot match  input 
-000019c0: 7361 6d70 6c69 6e67 2072 6174 6520 28fa  sampling rate (.
-000019d0: 0129 2903 7265 0000 0072 6200 0000 7263  .)).re...rb...rc
-000019e0: 0000 0029 0472 1300 0000 7264 0000 005a  ...).r....rd...Z
-000019f0: 0e69 6e5f 7361 6d70 6c65 5f72 6174 655a  .in_sample_rateZ
-00001a00: 0f6f 7574 5f73 616d 706c 655f 7261 7465  .out_sample_rate
-00001a10: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00001a20: 125f 6765 745f 6e65 775f 6261 6e64 5f63  ._get_new_band_c
-00001a30: 6f64 6506 0100 0073 0e00 0000 0009 1001  ode....s........
-00001a40: 0401 0801 02ff 06ff 0404 7a1c 4465 6369  ..........z.Deci
-00001a50: 6d61 746f 722e 5f67 6574 5f6e 6577 5f62  mator._get_new_b
-00001a60: 616e 645f 636f 6465 da00 6306 0000 0000  and_code..c.....
-00001a70: 0000 0000 0000 0009 0000 000b 0000 0043  ...............C
-00001a80: 0000 0073 8800 0000 6401 a000 7c02 7c03  ...s....d...|.|.
-00001a90: 7c01 6a01 7c01 6a02 6704 a101 7d06 7c01  |.j.|.j.g...}.|.
-00001aa0: 6a03 7d07 7c00 a004 7c01 7c07 a102 0100  j.}.|...|.|.....
-00001ab0: 7c00 a005 7c01 7c07 a102 0100 7c01 0400  |...|.|.....|...
-00001ac0: 6a03 7c00 6a06 1d00 0200 5f03 6401 a000  j.|.j....._.d...
-00001ad0: 7c02 7c03 7c01 6a01 7c01 6a02 6704 a101  |.|.|.j.|.j.g...
-00001ae0: 7d08 7407 a008 6402 7c06 9b00 6403 7c07  }.t...d.|...d.|.
-00001af0: 6404 9b04 6405 7c08 9b00 6403 7c01 6a03  d...d.|...d.|.j.
-00001b00: 6404 9b04 6406 9d09 a101 0100 6407 5300  d...d.......d.S.
-00001b10: 2908 619e 0100 000a 2020 2020 2020 2020  ).a.....        
-00001b20: 6d6f 6469 6679 2072 6570 6f6e 7365 2061  modify reponse a
-00001b30: 6e64 206e 616d 6520 6f66 2061 2063 6861  nd name of a cha
-00001b40: 6e6e 656c 2074 6f20 636f 7272 6573 706f  nnel to correspo
-00001b50: 6e64 2074 6f20 6465 6369 6d61 7469 6f6e  nd to decimation
-00001b60: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00001b70: 2020 2020 2020 2020 2020 2020 6368 6120              cha 
-00001b80: 283a 636c 6173 733a 606f 6273 7079 2e63  (:class:`obspy.c
-00001b90: 6f72 652e 696e 7665 6e74 6f72 792e 6368  ore.inventory.ch
-00001ba0: 616e 6e65 6c60 293a 206f 7269 6769 6e61  annel`): origina
-00001bb0: 6c20 6368 616e 6e65 6c0a 2020 2020 2020  l channel.      
-00001bc0: 2020 2020 2020 6e65 7420 2873 7472 293a        net (str):
-00001bd0: 206e 6574 776f 726b 2063 6f64 6520 286a   network code (j
-00001be0: 7573 7420 666f 7220 636c 6561 7265 7220  ust for clearer 
-00001bf0: 7072 6f67 7265 7373 2070 7269 6e74 6f75  progress printou
-00001c00: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
-00001c10: 7461 2028 7374 7229 3a20 7374 6174 696f  ta (str): statio
-00001c20: 6e20 636f 6465 2028 6a75 7374 2066 6f72  n code (just for
-00001c30: 2063 6c65 6172 6572 2070 726f 6772 6573   clearer progres
-00001c40: 7320 7072 696e 746f 7574 290a 2020 2020  s printout).    
-00001c50: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
-00001c60: 655f 6669 7273 2028 626f 6f6c 293a 206e  e_firs (bool): n
-00001c70: 6f72 6d61 6c69 7a65 7320 616e 7920 4649  ormalizes any FI
-00001c80: 5220 6368 616e 6e65 6c20 7468 6174 2069  R channel that i
-00001c90: 736e 2774 0a20 2020 2020 2020 2020 2020  sn't.           
-00001ca0: 2020 2020 2061 6c72 6561 6479 0a20 2020       already.   
-00001cb0: 2020 2020 2072 3500 0000 7a16 6368 616e       r5...z.chan
-00001cc0: 6e65 6c20 6d6f 6469 6669 6564 2066 726f  nel modified fro
-00001cd0: 6d20 7237 0000 00da 0167 7a09 2073 7073  m r7.....gz. sps
-00001ce0: 2920 746f 207a 0620 7370 7329 204e 2909  ) to z. sps) N).
-00001cf0: da04 6a6f 696e 722c 0000 0072 2b00 0000  ..joinr,...r+...
-00001d00: 722d 0000 00da 185f 6164 645f 696e 7374  r-....._add_inst
-00001d10: 7275 6d65 6e74 5f72 6573 706f 6e73 65da  rument_response.
-00001d20: 105f 6368 616e 6765 5f63 6861 6e5f 6c6f  ._change_chan_lo
-00001d30: 6372 1600 0000 723c 0000 00da 0469 6e66  cr....r<.....inf
-00001d40: 6f29 0972 1300 0000 724b 0000 0072 2e00  o).r....rK...r..
-00001d50: 0000 722f 0000 0072 3100 0000 7234 0000  ..r/...r1...r4..
-00001d60: 005a 0b6f 6c64 5f73 6565 645f 6964 da11  .Z.old_seed_id..
-00001d70: 696e 7075 745f 7361 6d70 6c65 5f72 6174  input_sample_rat
-00001d80: 6572 4700 0000 7214 0000 0072 1400 0000  erG...r....r....
-00001d90: 7215 0000 0072 3b00 0000 1601 0000 731e  r....r;.......s.
-00001da0: 0000 0000 0c16 0206 010c 010c 0110 0116  ................
-00001db0: 0106 0102 ff04 0104 ff04 0202 fe04 0206  ................
-00001dc0: fe7a 1644 6563 696d 6174 6f72 2e5f 6d6f  .z.Decimator._mo
-00001dd0: 6469 6679 5f63 6861 6e63 0100 0000 0000  dify_chanc......
-00001de0: 0000 0000 0000 0200 0000 0600 0000 0300  ................
-00001df0: 0000 733e 0100 007c 006a 006a 0144 0090  ..s>...|.j.j.D..
-00001e00: 015d 2e7d 0174 027c 0174 0383 0272 be7c  .].}.t.|.t...r.|
-00001e10: 016a 0464 016b 0272 2e74 057c 016a 0683  .j.d.k.r.t.|.j..
-00001e20: 0189 006e 567c 016a 0464 026b 0272 4864  ...nV|.j.d.k.rHd
-00001e30: 0374 057c 016a 0683 0114 0089 006e 3c7c  .t.|.j.......n<|
-00001e40: 016a 0464 046b 0272 7464 0374 057c 016a  .j.d.k.rtd.t.|.j
-00001e50: 0664 0564 0685 0219 0083 0114 007c 016a  .d.d.........|.j
-00001e60: 0664 0619 0017 0089 006e 1074 0764 077c  .d.......n.t.d.|
-00001e70: 016a 049b 009d 0283 0182 0174 0888 0064  .j.........t...d
-00001e80: 0818 0083 0164 096b 0472 bc74 09a0 0a64  .....d.k.r.t...d
-00001e90: 0a88 009b 0064 0b9d 03a1 0101 0087 0066  .....d.........f
-00001ea0: 0164 0c64 0d84 087c 016a 0644 0083 017c  .d.d...|.j.D...|
-00001eb0: 015f 0671 0874 027c 0174 0b83 0272 0874  ._.q.t.|.t...r.t
-00001ec0: 057c 016a 0c83 0164 0e6b 0272 ec74 057c  .|.j...d.k.r.t.|
-00001ed0: 016a 0d83 0189 0088 0064 0e6b 0272 ea71  .j.......d.k.r.q
-00001ee0: 086e 1474 057c 016a 0d83 0174 057c 016a  .n.t.|.j...t.|.j
-00001ef0: 0c83 011b 0089 0074 0888 0064 0818 0083  .......t...d....
-00001f00: 0164 096b 0472 0874 09a0 0a64 0f88 009b  .d.k.r.t...d....
-00001f10: 0064 0b9d 03a1 0101 0087 0066 0164 1064  .d.........f.d.d
-00001f20: 0d84 087c 016a 0d44 0083 017c 015f 0d71  ...|.j.D...|._.q
-00001f30: 0864 0553 0029 117a a80a 2020 2020 2020  .d.S.).z..      
-00001f40: 2020 5665 7269 6669 6573 2026 2c20 6966    Verifies &, if
-00001f50: 206e 6565 6465 642c 206e 6f72 6d61 6c69   needed, normali
-00001f60: 7a65 7320 6368 616e 6e65 6c27 7320 4649  zes channel's FI
-00001f70: 5220 6f72 2043 6f65 6666 6963 6965 6e74  R or Coefficient
-00001f80: 7320 636f 6566 6673 0a0a 2020 2020 2020  s coeffs..      
-00001f90: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00001fa0: 2020 2020 6368 6120 283a 636c 6173 733a      cha (:class:
-00001fb0: 606f 6273 7079 2e63 6f72 652e 696e 7665  `obspy.core.inve
-00001fc0: 6e74 6f72 792e 6368 616e 6e65 6c60 293a  ntory.channel`):
-00001fd0: 2063 6861 6e6e 656c 0a20 2020 2020 2020   channel.       
-00001fe0: 20da 044e 4f4e 45da 0445 5645 4e72 0e00   ..NONE..EVENr..
-00001ff0: 0000 da03 4f44 444e e9ff ffff ff7a 2255  ....ODDN.....z"U
-00002000: 6e6b 6e6f 776e 2046 4952 2063 6f65 6666  nknown FIR coeff
-00002010: 6963 6965 6e74 2073 796d 6d65 7472 793a  icient symmetry:
-00002020: 2072 0c00 0000 677b 14ae 47e1 7a84 3f7a   r....g{..G.z.?z
-00002030: 1f44 4543 494d 4154 4f52 3a20 5375 6d20  .DECIMATOR: Sum 
-00002040: 6f66 2046 4952 2063 6f65 6666 7320 3d20  of FIR coeffs = 
-00002050: 7a0d 2c20 6e6f 726d 616c 697a 696e 6763  z., normalizingc
-00002060: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002070: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
-00002080: 005d 0c7d 017c 0188 001b 0091 0271 0453  .].}.|.......q.S
-00002090: 0072 1400 0000 7214 0000 00a9 0272 2000  .r....r......r .
-000020a0: 0000 da01 78a9 015a 0963 6f65 6666 5f73  ....x..Z.coeff_s
-000020b0: 756d 7214 0000 0072 1500 0000 7222 0000  umr....r....r"..
-000020c0: 0046 0100 0073 0400 0000 0601 02ff 7a2d  .F...s........z-
-000020d0: 4465 6369 6d61 746f 722e 5f6e 6f72 6d61  Decimator._norma
-000020e0: 6c69 7a65 5f66 6972 732e 3c6c 6f63 616c  lize_firs.<local
-000020f0: 733e 2e3c 6c69 7374 636f 6d70 3e72 0100  s>.<listcomp>r..
-00002100: 0000 7a35 4445 4349 4d41 544f 523a 2073  ..z5DECIMATOR: s
-00002110: 756d 286e 756d 6572 6174 6f72 2063 6f65  um(numerator coe
-00002120: 6666 7329 2f73 756d 2864 656e 6f6d 2063  ffs)/sum(denom c
-00002130: 6f65 6666 7329 203d 2063 0100 0000 0000  oeffs) = c......
-00002140: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-00002150: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
-00002160: 0188 001b 0091 0271 0453 0072 1400 0000  .......q.S.r....
-00002170: 7214 0000 0072 7300 0000 7275 0000 0072  r....rs...ru...r
-00002180: 1400 0000 7215 0000 0072 2200 0000 5401  ....r....r"...T.
-00002190: 0000 7223 0000 0029 0eda 0872 6573 706f  ..r#...)...respo
-000021a0: 6e73 65da 0f72 6573 706f 6e73 655f 7374  nse..response_st
-000021b0: 6167 6573 7218 0000 0072 0a00 0000 da08  agesr....r......
-000021c0: 7379 6d6d 6574 7279 da03 7375 6dda 0c63  symmetry..sum..c
-000021d0: 6f65 6666 6963 6965 6e74 7372 3a00 0000  oefficientsr:...
-000021e0: da03 6162 7372 3c00 0000 726d 0000 0072  ..absr<...rm...r
-000021f0: 0b00 0000 da0b 6465 6e6f 6d69 6e61 746f  ......denominato
-00002200: 72da 096e 756d 6572 6174 6f72 2902 724b  r..numerator).rK
-00002210: 0000 005a 0373 7467 7214 0000 0072 7500  ...Z.stgr....ru.
-00002220: 0000 7215 0000 00da 0f5f 6e6f 726d 616c  ..r......_normal
-00002230: 697a 655f 6669 7273 2d01 0000 7340 0000  ize_firs-...s@..
-00002240: 0000 080e 010a 010a 010c 010a 0110 010a  ................
-00002250: 021e ff04 0402 010a ff04 0310 0106 0102  ................
-00002260: ff0a 020a 0104 ff0a 020a 010e 010a 0108  ................
-00002270: 0104 0214 0210 0104 0102 0102 ff06 ff04  ................
-00002280: 037a 1944 6563 696d 6174 6f72 2e5f 6e6f  .z.Decimator._no
-00002290: 726d 616c 697a 655f 6669 7273 6304 0000  rmalize_firsc...
-000022a0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-000022b0: 0043 0000 0073 2000 0000 7c00 a000 7c01  .C...s ...|...|.
-000022c0: 6a01 7c01 6a02 7c02 7c03 a104 5c02 7c01  j.|.j.|.|...\.|.
-000022d0: 5f01 7c01 5f02 6401 5300 2902 611c 0100  _.|._.d.S.).a...
-000022e0: 000a 2020 2020 2020 2020 4368 616e 6765  ..        Change
-000022f0: 2063 6861 6e6e 656c 2028 6f72 206c 6f63   channel (or loc
-00002300: 6174 696f 6e29 2063 6f64 6520 696e 2070  ation) code in p
-00002310: 6c61 6365 2c20 6163 636f 7264 696e 6720  lace, according 
-00002320: 746f 2064 6563 696d 6174 696f 6e0a 0a20  to decimation.. 
-00002330: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-00002340: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-00002350: 6120 2849 6e76 656e 746f 7279 2e43 6861  a (Inventory.Cha
-00002360: 6e6e 656c 2920 6368 616e 6e65 6c20 746f  nnel) channel to
-00002370: 2062 6520 6d6f 6469 6669 6564 2028 696e   be modified (in
-00002380: 2070 6c61 6365 290a 2020 2020 2020 2020   place).        
-00002390: 2020 2020 696e 5f73 7220 2866 6c6f 6174      in_sr (float
-000023a0: 293a 2069 6e70 7574 2073 616d 706c 6520  ): input sample 
-000023b0: 7261 7465 0a20 2020 2020 2020 2020 2020  rate.           
-000023c0: 2061 766f 6964 5f63 6f64 6573 2028 6c69   avoid_codes (li
-000023d0: 7374 293a 2063 6861 6e6e 656c 3a6c 6f63  st): channel:loc
-000023e0: 6174 696f 6e20 636f 6465 7320 746f 2061  ation codes to a
-000023f0: 766f 6964 0a20 2020 2020 2020 204e 2903  void.        N).
-00002400: da0d 5f67 6574 5f63 6861 6e5f 6c6f 6372  .._get_chan_locr
-00002410: 2b00 0000 722c 0000 0029 0472 1300 0000  +...r,...).r....
-00002420: 724b 0000 00da 0569 6e5f 7372 da0b 6176  rK.....in_sr..av
-00002430: 6f69 645f 636f 6465 7372 1400 0000 7214  oid_codesr....r.
-00002440: 0000 0072 1500 0000 726c 0000 0056 0100  ...r....rl...V..
-00002450: 0073 0600 0000 0009 0401 0cff 7a1a 4465  .s..........z.De
-00002460: 6369 6d61 746f 722e 5f63 6861 6e67 655f  cimator._change_
-00002470: 6368 616e 5f6c 6f63 6305 0000 0000 0000  chan_locc.......
-00002480: 0000 0000 000a 0000 0008 0000 0043 0000  .............C..
-00002490: 0073 c400 0000 7c00 6a00 6401 6b02 7212  .s....|.j.d.k.r.
-000024a0: 7401 6402 8301 8201 7c03 7c00 6a00 1b00  t.d.....|.|.j...
-000024b0: 7d05 7c00 a002 7c01 6403 1900 7c03 7c05  }.|...|.d...|.|.
-000024c0: a103 7d06 7c06 7c01 6401 6404 8502 1900  ..}.|.|.d.d.....
-000024d0: 1700 7d07 7c07 7c01 6b02 7274 7a14 7403  ..}.|.|.k.rtz.t.
-000024e0: 7c02 8301 6401 1700 6405 9b04 7d08 5700  |...d...d...}.W.
-000024f0: 7178 0400 7404 7970 0100 0100 0100 6406  qx..t.yp......d.
-00002500: 7d08 5900 7178 3000 6e04 7c02 7d08 7c04  }.Y.qx0.n.|.}.|.
-00002510: 4400 5d3a 7d09 7c07 7c09 a005 6407 a101  D.]:}.|.|...d...
-00002520: 6403 1900 6b02 727c 7c08 7c09 a005 6407  d...k.r||.|...d.
-00002530: a101 6401 1900 6b02 727c 7403 7c08 8301  ..d...k.r|t.|...
-00002540: 6401 1700 6405 9b04 7d08 717c 717c 71bc  d...d...}.q|q|q.
-00002550: 7178 7c07 7c08 6602 5300 2908 618f 0100  qx|.|.f.S.).a...
-00002560: 000a 2020 2020 2020 2020 4765 7420 6e65  ..        Get ne
-00002570: 7720 6368 616e 6e65 6c20 286f 7220 6c6f  w channel (or lo
-00002580: 6329 2063 6f64 6573 2066 726f 6d20 6f6c  c) codes from ol
-00002590: 6420 636f 6465 7320 616e 6420 6465 6369  d codes and deci
-000025a0: 6d61 7469 6f6e 2066 6163 746f 720a 0a20  mation factor.. 
-000025b0: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-000025c0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-000025d0: 615f 636f 6465 3a20 696e 7075 7420 6368  a_code: input ch
-000025e0: 616e 6e65 6c20 636f 6465 0a20 2020 2020  annel code.     
-000025f0: 2020 2020 2020 206c 6f63 5f63 6f64 653a         loc_code:
-00002600: 2069 6e70 7574 206c 6f63 6174 696f 6e20   input location 
-00002610: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
-00002620: 2069 6e5f 7372 3a20 696e 7075 7420 7361   in_sr: input sa
-00002630: 6d70 6c69 6e67 2072 6174 650a 2020 2020  mpling rate.    
-00002640: 2020 2020 2020 2020 6176 6f69 645f 636f          avoid_co
-00002650: 6465 7320 286c 6973 7429 3a20 6368 616e  des (list): chan
-00002660: 6e65 6c3a 6c6f 6361 7469 6f6e 2063 6f64  nel:location cod
-00002670: 6573 2074 6f20 6176 6f69 640a 0a20 2020  es to avoid..   
-00002680: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00002690: 2020 2020 2020 2020 2020 7475 706c 653a            tuple:
-000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026b0: 206e 6577 5f63 6861 6e5f 636f 6465 2028   new_chan_code (
-000026c0: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
-000026d0: 2020 2020 206e 6577 5f6c 6f63 5f63 6f64       new_loc_cod
-000026e0: 6520 2873 7472 290a 2020 2020 2020 2020  e (str).        
-000026f0: 720c 0000 007a 1044 6563 696d 6174 696f  r....z.Decimatio
-00002700: 6e20 3d3d 2031 2172 0100 0000 4eda 0330  n == 1!r....N..0
-00002710: 3264 5a02 3031 fa01 3a29 0672 1600 0000  2dZ.01..:).r....
-00002720: 723a 0000 0072 6700 0000 da03 696e 74da  r:...rg.....int.
-00002730: 0945 7863 6570 7469 6f6e da05 7370 6c69  .Exception..spli
-00002740: 7429 0a72 1300 0000 5a08 6368 615f 636f  t).r....Z.cha_co
-00002750: 6465 5a08 6c6f 635f 636f 6465 7280 0000  deZ.loc_coder...
-00002760: 0072 8100 0000 5a06 6f75 745f 7372 5a0d  .r....Z.out_srZ.
-00002770: 6e65 775f 6261 6e64 5f63 6f64 655a 0c6e  new_band_codeZ.n
-00002780: 6577 5f63 6861 5f63 6f64 655a 0c6e 6577  ew_cha_codeZ.new
-00002790: 5f6c 6f63 5f63 6f64 65da 0163 7214 0000  _loc_code..cr...
-000027a0: 0072 1400 0000 7215 0000 0072 7f00 0000  .r....r....r....
-000027b0: 6301 0000 7328 0000 0000 0f0a 0108 010a  c...s(..........
-000027c0: 0112 0110 0108 0202 0114 010c 010c 0204  ................
-000027d0: 0308 0210 ff02 0210 fe02 0410 0104 0104  ................
-000027e0: 017a 1744 6563 696d 6174 6f72 2e5f 6765  .z.Decimator._ge
-000027f0: 745f 6368 616e 5f6c 6f63 6303 0000 0000  t_chan_locc.....
-00002800: 0000 0000 0000 0007 0000 0009 0000 0043  ...............C
-00002810: 0000 0073 b000 0000 7c01 6a00 6a01 6401  ...s....|.j.j.d.
-00002820: 1900 6a02 7d03 7c00 6a03 4400 5d40 7d04  ..j.}.|.j.D.]@}.
-00002830: 7404 a005 7c04 a101 7d05 7c03 6402 3700  t...|...}.|.d.7.
-00002840: 7d03 7c01 6a00 6a01 a006 7c05 a007 7c02  }.|.j.j...|...|.
-00002850: 7c03 7c01 6a00 6a01 6401 1900 6a08 a103  |.|.j.j.d...j...
-00002860: a101 0100 7c02 7c04 1d00 7d02 7114 7a0e  ....|.|...}.q.z.
-00002870: 7c01 6a00 a009 a100 0100 5700 6e46 0400  |.j.......W.nF..
-00002880: 740a 79aa 0100 0100 0100 7c01 6a00 6a0b  t.y.......|.j.j.
-00002890: 6a0c 7d06 7c06 a00d a100 6403 6b02 72a6  j.}.|.....d.k.r.
-000028a0: 6404 7c01 6a00 6a0b 5f0c 7c01 6a00 a009  d.|.j.j._.|.j...
-000028b0: a100 0100 7c06 7c01 6a00 6a0b 5f0c 5900  ....|.|.j.j._.Y.
-000028c0: 6e02 3000 6405 5300 2906 7a6b 0a20 2020  n.0.d.S.).zk.   
-000028d0: 2020 2020 2041 7070 656e 6420 2064 6563       Append  dec
-000028e0: 696d 6174 696f 6e20 6f62 6a65 6374 2773  imation object's
-000028f0: 2069 6e73 7472 756d 656e 7420 7265 7370   instrument resp
-00002900: 6f6e 7365 2074 6f20 616e 2065 7869 7374  onse to an exist
-00002910: 696e 670a 2020 2020 2020 2020 6368 616e  ing.        chan
-00002920: 6e65 6c27 7320 7265 7370 6f6e 7365 0a20  nel's response. 
-00002930: 2020 2020 2020 2072 7200 0000 720c 0000         rr...r...
-00002940: 00da 0250 417a 034d 2f53 4e29 0e72 7600  ...PAz.M/SN).rv.
-00002950: 0000 7277 0000 00da 1573 7461 6765 5f73  ..rw.....stage_s
-00002960: 6571 7565 6e63 655f 6e75 6d62 6572 7211  equence_numberr.
-00002970: 0000 0072 0d00 0000 da08 6672 6f6d 5f53  ...r......from_S
-00002980: 4143 7243 0000 005a 0874 6f5f 6f62 7370  ACrC...Z.to_obsp
-00002990: 79da 0c6f 7574 7075 745f 756e 6974 73da  y..output_units.
-000029a0: 1f72 6563 616c 6375 6c61 7465 5f6f 7665  .recalculate_ove
-000029b0: 7261 6c6c 5f73 656e 7369 7469 7669 7479  rall_sensitivity
-000029c0: 7285 0000 00da 1669 6e73 7472 756d 656e  r......instrumen
-000029d0: 745f 7365 6e73 6974 6976 6974 79da 0b69  t_sensitivity..i
-000029e0: 6e70 7574 5f75 6e69 7473 da05 7570 7065  nput_units..uppe
-000029f0: 7229 0772 1300 0000 724b 0000 0072 6e00  r).r....rK...rn.
-00002a00: 0000 da0c 7374 6167 655f 6e75 6d62 6572  ....stage_number
-00002a10: da01 64da 0a66 6972 5f66 696c 7465 72da  ..d..fir_filter.
-00002a20: 0369 5f75 7214 0000 0072 1400 0000 7215  .i_ur....r....r.
-00002a30: 0000 0072 6b00 0000 8b01 0000 7326 0000  ...rk.......s&..
-00002a40: 0000 050e 010a 010a 0108 0108 0104 0104  ................
-00002a50: 010c fe02 ff04 050a 0102 010e 010c 010a  ................
-00002a60: 010c 010a 010a 017a 2244 6563 696d 6174  .......z"Decimat
-00002a70: 6f72 2e5f 6164 645f 696e 7374 7275 6d65  or._add_instrume
-00002a80: 6e74 5f72 6573 706f 6e73 6563 0200 0000  nt_responsec....
-00002a90: 0000 0000 0000 0000 0500 0000 0600 0000  ................
-00002aa0: 4300 0000 7366 0000 0074 007c 0174 0183  C...sf...t.|.t..
-00002ab0: 0273 1274 0264 0183 0182 017c 01a0 03a1  .s.t.d.....|....
-00002ac0: 007d 0267 007d 037c 026a 0444 005d 147d  .}.g.}.|.j.D.].}
-00002ad0: 047c 03a0 057c 00a0 067c 04a1 01a1 0101  .|...|...|......
-00002ae0: 0071 247c 037c 025f 0474 07a0 0864 02a0  .q$|.|._.t...d..
-00002af0: 0964 0364 0484 007c 0244 0083 01a1 01a1  .d.d...|.D......
-00002b00: 0101 007c 02a0 0aa1 0001 007c 0253 0029  ...|.......|.S.)
-00002b10: 057a 270a 2020 2020 2020 2020 4465 6369  .z'.        Deci
-00002b20: 6d61 7465 206f 6273 7079 2053 7472 6561  mate obspy Strea
-00002b30: 6d0a 2020 2020 2020 2020 7a24 696e 7075  m.        z$inpu
-00002b40: 7420 7374 7265 616d 2069 7320 6e6f 7420  t stream is not 
-00002b50: 616e 206f 6273 7079 2053 7472 6561 6d21  an obspy Stream!
-00002b60: 7a17 4e65 7720 6461 7461 2068 6173 207b  z.New data has {
-00002b70: 7d20 7361 6d70 6c65 7363 0100 0000 0000  } samplesc......
-00002b80: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-00002b90: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
-00002ba0: 016a 006a 0191 0271 0453 0072 1400 0000  .j.j...q.S.r....
-00002bb0: 2902 721c 0000 00da 0473 697a 6572 1f00  ).r......sizer..
-00002bc0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00002bd0: 0072 2200 0000 ae01 0000 7304 0000 0006  .r".......s.....
-00002be0: 0102 ff7a 2944 6563 696d 6174 6f72 2e5f  ...z)Decimator._
-00002bf0: 7275 6e5f 7374 7265 616d 2e3c 6c6f 6361  run_stream.<loca
-00002c00: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 290b  ls>.<listcomp>).
-00002c10: 7218 0000 0072 0700 0000 723a 0000 0072  r....r....r:...r
-00002c20: 3800 0000 da06 7472 6163 6573 7243 0000  8.....tracesrC..
-00002c30: 0072 1a00 0000 723c 0000 0072 6d00 0000  .r....r<...rm...
-00002c40: da06 666f 726d 6174 da06 7665 7269 6679  ..format..verify
-00002c50: 2905 7213 0000 00da 0673 7472 6561 6d72  ).r......streamr
-00002c60: 4500 0000 5a05 6e65 7774 7272 2100 0000  E...Z.newtrr!...
-00002c70: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00002c80: 1900 0000 a301 0000 7318 0000 0000 040a  ........s.......
-00002c90: 0108 0108 0104 010a 0112 0106 010e 0102  ................
-00002ca0: ff0a 0208 017a 1544 6563 696d 6174 6f72  .....z.Decimator
-00002cb0: 2e5f 7275 6e5f 7374 7265 616d 6302 0000  ._run_streamc...
-00002cc0: 0000 0000 0000 0000 0008 0000 0007 0000  ................
-00002cd0: 0043 0000 0073 ec00 0000 7400 7c01 7401  .C...s....t.|.t.
-00002ce0: 8302 7312 7402 6401 8301 8201 7c01 6a03  ..s.t.d.....|.j.
-00002cf0: 6a04 7d02 7c01 a005 a100 7d03 7c03 6a06  j.}.|.....}.|.j.
-00002d00: 6a07 7d04 7408 a009 6402 a00a 7c04 7c04  j.}.t...d...|.|.
-00002d10: 7c00 6a0b 1b00 7c00 6a0b a103 a101 0100  |.j...|.j.......
-00002d20: 740c a00c a100 7d05 7c00 6a0d 4400 5d2a  t.....}.|.j.D.]*
-00002d30: 7d06 740e a00f 7c06 a101 7d07 7c07 a010  }.t...|...}.|...
-00002d40: 7c03 6a03 a101 7c03 5f03 7c03 6a11 7c06  |.j...|._.|.j.|.
-00002d50: 6403 6404 8d02 0100 7154 7c00 6a12 6403  d.d.....qT|.j.d.
-00002d60: 7500 72a4 7c03 6a03 6a04 7c02 6b02 73a4  u.r.|.j.j.|.k.s.
-00002d70: 7c03 6a03 a013 7c02 a101 7c03 5f03 7c00  |.j...|...|._.|.
-00002d80: a014 7c03 6a06 6a15 7c03 6a06 6a16 7c03  ..|.j.j.|.j.j.|.
-00002d90: 6a06 6a07 7c00 6a0b 1400 a103 5c02 7c03  j.j.|.j.....\.|.
-00002da0: 6a06 5f15 7c03 6a06 5f16 7408 a009 6405  j._.|.j._.t...d.
-00002db0: a00a 740c a00c a100 7c05 1800 a101 a101  ..t.....|.......
-00002dc0: 0100 7c03 5300 2906 7a26 0a20 2020 2020  ..|.S.).z&.     
-00002dd0: 2020 2044 6563 696d 6174 6520 6f62 7370     Decimate obsp
-00002de0: 7920 5472 6163 650a 2020 2020 2020 2020  y Trace.        
-00002df0: 7a22 696e 7075 7420 7472 6163 6520 6973  z"input trace is
-00002e00: 206e 6f74 2061 6e20 6f62 7370 7920 5472   not an obspy Tr
-00002e10: 6163 6521 7a30 4465 6369 6d61 7469 6e67  ace!z0Decimating
-00002e20: 2064 6174 6120 6672 6f6d 207b 3a67 7d20   data from {:g} 
-00002e30: 746f 207b 3a67 7d20 487a 2028 7b3a 647d  to {:g} Hz ({:d}
-00002e40: 7829 2e2e 2e20 5429 01da 096e 6f5f 6669  x)... T)...no_fi
-00002e50: 6c74 6572 7a13 546f 6f6b 207b 3a2e 3166  lterz.Took {:.1f
-00002e60: 7d20 7365 636f 6e64 7329 1772 1800 0000  } seconds).r....
-00002e70: 7208 0000 0072 3a00 0000 721c 0000 00da  r....r:...r.....
-00002e80: 0564 7479 7065 7238 0000 0072 1e00 0000  .dtyper8...r....
-00002e90: 7228 0000 0072 3c00 0000 726d 0000 0072  r(...r<...rm...r
-00002ea0: 9600 0000 7216 0000 00da 0474 696d 6572  ....r......timer
-00002eb0: 1100 0000 720d 0000 0072 8a00 0000 da08  ....r....r......
-00002ec0: 636f 6e76 6f6c 7665 721d 0000 0072 1700  convolver....r..
-00002ed0: 0000 da06 6173 7479 7065 727f 0000 0072  ....astyper....r
-00002ee0: 2700 0000 7226 0000 0029 0872 1300 0000  '...r&...).r....
-00002ef0: da05 7472 6163 6572 9a00 0000 7221 0000  ..tracer....r!..
-00002f00: 00da 0273 72da 0374 6963 7291 0000 0072  ...sr..ticr....r
-00002f10: 9200 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00002f20: 0000 0072 1a00 0000 b301 0000 732e 0000  ...r........s...
-00002f30: 0000 040a 0108 0108 0108 0108 0108 010a  ................
-00002f40: 0104 fe06 0308 010a 010a 010e 0110 0116  ................
-00002f50: 010e 0104 0106 0106 010c fd10 0418 017a  ...............z
-00002f60: 1444 6563 696d 6174 6f72 2e5f 7275 6e5f  .Decimator._run_
-00002f70: 7472 6163 6563 0100 0000 0000 0000 0000  tracec..........
-00002f80: 0000 0a00 0000 0800 0000 0300 0000 730a  ..............s.
-00002f90: 0100 0074 0074 0174 0283 0083 0183 01a0  ...t.t.t........
-00002fa0: 03a1 006a 047d 0164 017c 0064 029b 049d  ...j.}.d.|.d....
-00002fb0: 027d 027c 01a0 057c 02a1 017d 0374 067c  .}.|...|...}.t.|
-00002fc0: 0383 0164 036b 0273 3e74 0764 0483 0182  ...d.k.s>t.d....
-00002fd0: 0174 087c 0383 018f 687d 047c 04a0 09a1  .t.|....h}.|....
-00002fe0: 0001 007c 04a0 09a1 00a0 0aa1 007d 0574  ...|.........}.t
-00002ff0: 0b7c 0564 0519 0083 0189 0074 0c7c 0564  .|.d.......t.|.d
-00003000: 0319 0083 017d 0667 007d 077c 04a0 0da1  .....}.g.}.|....
-00003010: 0044 005d 1e7d 087c 0787 0066 0164 0664  .D.].}.|...f.d.d
-00003020: 0784 087c 08a0 0aa1 0044 0083 0117 007d  ...|.....D.....}
-00003030: 0771 8057 0064 0804 0004 0083 0301 006e  .q.W.d.........n
-00003040: 1031 0073 b430 0001 0001 0001 0059 0001  .1.s.0.......Y..
-00003050: 0074 067c 0783 017c 066b 0273 de74 0e64  .t.|...|.k.s.t.d
-00003060: 09a0 0f74 067c 0783 017c 06a1 0283 0182  ...t.|...|......
-00003070: 0174 067c 0783 0164 0318 007d 097c 0764  .t.|...d...}.|.d
-00003080: 0a64 0564 0a85 0319 007c 0717 007d 0774  .d.d.....|...}.t
-00003090: 107c 077c 0964 0364 0b83 0453 0029 0c7a  .|.|.d.d...S.).z
-000030a0: 2a0a 2020 2020 2020 2020 5265 7475 726e  *.        Return
-000030b0: 7320 6120 5341 4320 4649 5220 6669 6c74  s a SAC FIR filt
-000030c0: 6572 0a20 2020 2020 2020 20da 0364 6563  er.        ..dec
-000030d0: 7291 0000 0072 0c00 0000 7a23 5341 4320  r....r....z#SAC 
-000030e0: 6669 6c74 6572 2066 696c 6520 227b 6662  filter file "{fb
-000030f0: 6173 657d 2220 6e6f 7420 666f 756e 6472  ase}" not foundr
-00003100: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00003110: 0002 0000 0004 0000 0013 0000 0073 1800  .............s..
-00003120: 0000 6700 7c00 5d10 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-00003130: 8800 1b00 9102 7104 5300 7214 0000 0029  ......q.S.r....)
-00003140: 01da 0566 6c6f 6174 7273 0000 00a9 01da  ...floatrs......
-00003150: 0764 6976 6973 6f72 7214 0000 0072 1500  .divisorr....r..
-00003160: 0000 7222 0000 00dd 0100 0072 2300 0000  ..r".......r#...
-00003170: 7a2b 4465 6369 6d61 746f 722e 5f72 6561  z+Decimator._rea
-00003180: 645f 4649 525f 5341 432e 3c6c 6f63 616c  d_FIR_SAC.<local
-00003190: 733e 2e3c 6c69 7374 636f 6d70 3e4e 7a32  s>.<listcomp>Nz2
-000031a0: 4649 5220 6c65 6e67 7468 2069 7320 6469  FIR length is di
-000031b0: 6666 6572 656e 7420 6672 6f6d 2074 6861  fferent from tha
-000031c0: 7420 7374 6174 6564 3a20 7b7d 2021 3d20  t stated: {} != 
-000031d0: 7b7d 7272 0000 0072 6800 0000 2911 7205  {}rr...rh...).r.
-000031e0: 0000 0072 0300 0000 7204 0000 00da 0772  ...r....r......r
-000031f0: 6573 6f6c 7665 da06 7061 7265 6e74 da04  esolve..parent..
-00003200: 676c 6f62 723e 0000 00da 094e 616d 6545  globr>.....NameE
-00003210: 7272 6f72 da04 6f70 656e da08 7265 6164  rror..open..read
-00003220: 6c69 6e65 7286 0000 0072 a200 0000 7284  liner....r....r.
-00003230: 0000 00da 0972 6561 646c 696e 6573 da0c  .....readlines..
-00003240: 5275 6e74 696d 6545 7272 6f72 7296 0000  RuntimeErrorr...
-00003250: 0072 0d00 0000 290a da0a 6465 6369 6d61  .r....)...decima
-00003260: 7469 6f6e da08 6261 7365 5f64 6972 5a05  tion..base_dirZ.
-00003270: 6662 6173 65da 0866 696c 656e 616d 65da  fbase..filename.
-00003280: 0166 da01 415a 076e 436f 6566 6673 da06  .f..AZ.nCoeffs..
-00003290: 636f 6566 6673 da04 6c69 6e65 da05 6465  coeffs..line..de
-000032a0: 6c61 7972 1400 0000 72a3 0000 0072 1500  layr....r....r..
-000032b0: 0000 da0d 5f72 6561 645f 4649 525f 5341  ...._read_FIR_SA
-000032c0: 43cd 0100 0073 2c00 0000 0004 1401 0c01  C....s,.........
-000032d0: 0a01 0c01 0801 0a01 0801 0c01 0c01 0c01  ................
-000032e0: 0401 0c01 3a01 0c01 0201 0401 08ff 02ff  ....:...........
-000032f0: 0405 0c01 1201 7a17 4465 6369 6d61 746f  ......z.Decimato
-00003300: 722e 5f72 6561 645f 4649 525f 5341 4363  r._read_FIR_SACc
-00003310: 0800 0000 0000 0000 0000 0000 0e00 0000  ................
-00003320: 0a00 0000 4300 0000 733a 0100 0067 007d  ....C...s:...g.}
-00003330: 0867 007d 097c 016a 0044 005d 907d 0a74  .g.}.|.j.D.].}.t
-00003340: 01a0 017c 0a6a 02a0 03a1 007c 02a0 03a1  ...|.j.....|....
-00003350: 00a1 0273 2a71 0e7c 0a6a 0444 005d 6c7d  ...s*q.|.j.D.]l}
-00003360: 0b74 01a0 017c 0b6a 02a0 03a1 007c 03a0  .t...|.j.....|..
-00003370: 03a1 00a1 0273 4c71 307c 0b6a 0544 005d  .....sLq0|.j.D.]
-00003380: 487d 0c74 01a0 017c 0c6a 06a0 03a1 007c  H}.t...|.j.....|
-00003390: 04a0 03a1 00a1 0273 6e71 5274 01a0 017c  .......snqRt...|
-000033a0: 0c6a 02a0 03a1 007c 05a0 03a1 00a1 0273  .j.....|.......s
-000033b0: 8671 527c 08a0 077c 0ba1 0101 007c 09a0  .qR|...|.....|..
-000033c0: 077c 0ca1 0101 0071 5271 3071 0e74 087c  .|.....qRq0q.t.|
-000033d0: 0883 0164 016b 0272 d274 0964 027c 029b  ...d.k.r.t.d.|..
-000033e0: 0064 037c 039b 0064 037c 049b 0064 037c  .d.|...d.|...d.|
-000033f0: 059b 0064 049d 0983 0182 0164 0553 0074  ...d.......d.S.t
-00003400: 087c 0883 0164 066b 0472 f874 0964 07a0  .|...d.k.r.t.d..
-00003410: 0a74 087c 0883 017c 027c 037c 047c 05a1  .t.|...|.|.|.|..
-00003420: 0583 0182 017c 0664 0875 0090 0172 107c  .....|.d.u...r.|
-00003430: 00a0 0b7c 0964 0119 00a1 0101 007c 0964  ...|.d.......|.d
-00003440: 0119 00a0 0ca1 007d 0d7c 0764 0875 0090  .......}.|.d.u..
-00003450: 0172 367c 0864 0119 006a 05a0 077c 0da1  .r6|.d...j...|..
-00003460: 0101 007c 0d53 0029 0961 c301 0000 0a20  ...|.S.).a..... 
-00003470: 2020 2020 2020 2052 6574 7572 6e20 5374         Return St
-00003480: 6174 696f 6e20 2620 4368 616e 6e65 6c20  ation & Channel 
-00003490: 6d61 7463 6869 6e67 206e 6574 776f 726b  matching network
-000034a0: 2c20 7374 6174 696f 6e2c 206c 6f63 6174  , station, locat
-000034b0: 696f 6e2c 2063 6861 6e6e 656c 0a0a 2020  ion, channel..  
-000034c0: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
-000034d0: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
-000034e0: 776f 726b 2028 7374 7229 3a20 6e65 7477  work (str): netw
-000034f0: 6f72 6b20 636f 6465 0a20 2020 2020 2020  ork code.       
-00003500: 2020 2020 2073 7461 7469 6f6e 2028 7374       station (st
-00003510: 7229 3a20 7374 6174 696f 6e20 636f 6465  r): station code
-00003520: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00003530: 6174 696f 6e20 2873 7472 293a 206c 6f63  ation (str): loc
-00003540: 6174 696f 6e20 636f 6465 0a20 2020 2020  ation code.     
-00003550: 2020 2020 2020 2063 6861 6e6e 656c 2028         channel (
-00003560: 7374 7229 3a20 6368 616e 6e65 6c20 636f  str): channel co
-00003570: 6465 0a20 2020 2020 2020 2020 2020 206e  de.            n
-00003580: 6f72 6d61 6c69 7a65 5f66 6972 7320 2862  ormalize_firs (b
-00003590: 6f6f 6c29 3a20 6e6f 726d 616c 697a 6573  ool): normalizes
-000035a0: 2061 6e79 2046 4952 2063 6861 6e6e 656c   any FIR channel
-000035b0: 2074 6861 7420 6973 6e27 740a 2020 2020   that isn't.    
-000035c0: 2020 2020 2020 2020 2020 2020 616c 7265              alre
-000035d0: 6164 790a 0a20 2020 2020 2020 2052 6574  ady..        Ret
-000035e0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000035f0: 2020 2843 6861 6e6e 656c 293a 2064 7570    (Channel): dup
-00003600: 6c69 6361 7465 206f 6620 666f 756e 6420  licate of found 
-00003610: 6368 616e 6e65 6c2c 2072 6561 6479 2074  channel, ready t
-00003620: 6f20 6d6f 6469 6679 0a20 2020 2020 2020  o modify.       
-00003630: 2072 0100 0000 7a12 7472 6163 6520 7761   r....z.trace wa
-00003640: 7665 666f 726d 6964 2022 7235 0000 007a  veformid "r5...z
-00003650: 1822 206e 6f74 2066 6f75 6e64 2069 6e20  ." not found in 
-00003660: 696e 7665 6e74 6f72 7929 024e 4e72 0c00  inventory).NNr..
-00003670: 0000 7a29 7b3a 647d 2073 7461 7469 6f6e  ..z){:d} station
-00003680: 2d63 6861 6e6e 656c 7320 6d61 7463 6865  -channels matche
-00003690: 6420 7b7d 2e7b 7d2e 7b7d 2e7b 7d54 290d  d {}.{}.{}.{}T).
-000036a0: da08 6e65 7477 6f72 6b73 da07 666e 6d61  ..networks..fnma
-000036b0: 7463 6872 2b00 0000 728f 0000 00da 0873  tchr+...r......s
-000036c0: 7461 7469 6f6e 7372 4200 0000 722c 0000  tationsrB...r,..
-000036d0: 0072 4300 0000 723e 0000 0072 3a00 0000  .rC...r>...r:...
-000036e0: 7296 0000 0072 7e00 0000 7238 0000 0029  r....r~...r8...)
-000036f0: 0e72 1300 0000 7244 0000 0072 2400 0000  .r....rD...r$...
-00003700: 7225 0000 0072 2600 0000 7227 0000 0072  r%...r&...r'...r
-00003710: 3100 0000 7232 0000 0072 b800 0000 7242  1...r2...r....rB
-00003720: 0000 0072 2e00 0000 722f 0000 0072 4b00  ...r....r/...rK.
-00003730: 0000 7246 0000 0072 1400 0000 7214 0000  ..rF...r....r...
-00003740: 0072 1500 0000 7239 0000 00ea 0100 0073  .r....r9.......s
-00003750: 4800 0000 0012 0401 0401 0a02 1601 0201  H...............
-00003760: 0a01 1601 0201 0a01 0401 0eff 0403 0201  ................
-00003770: 1601 0201 0a01 1001 0c01 1001 02ff 0401  ................
-00003780: 02ff 0a02 0401 0c01 0201 0401 0eff 02ff  ................
-00003790: 0405 0a01 0e01 0c01 0a01 1001 7a1c 4465  ............z.De
-000037a0: 6369 6d61 746f 722e 5f64 7570 6c69 6361  cimator._duplica
-000037b0: 7465 5f63 6861 6e6e 656c 2901 5429 044e  te_channel).T).N
-000037c0: 4646 4629 0672 4a00 0000 724a 0000 0072  FFF).rJ...rJ...r
-000037d0: 4a00 0000 724a 0000 0046 4629 0472 6800  J...rJ...FF).rh.
-000037e0: 0000 7268 0000 0046 4629 0246 5429 19da  ..rh...FF).FT)..
-000037f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00003800: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00003810: 655f 5fda 075f 5f64 6f63 5f5f da04 6c69  e__..__doc__..li
-00003820: 7374 da0f 5f5f 616e 6e6f 7461 7469 6f6e  st..__annotation
-00003830: 735f 5f72 1200 0000 da04 626f 6f6c da08  s__r......bool..
-00003840: 7072 6f70 6572 7479 7216 0000 0072 1d00  propertyr....r..
-00003850: 0000 7249 0000 0072 4c00 0000 da0c 7374  ..rI...rL.....st
-00003860: 6174 6963 6d65 7468 6f64 7265 0000 0072  aticmethodre...r
-00003870: 6700 0000 723b 0000 0072 7e00 0000 726c  g...r;...r~...rl
-00003880: 0000 0072 7f00 0000 726b 0000 0072 1900  ...r....rk...r..
-00003890: 0000 721a 0000 0072 b500 0000 7239 0000  ..r....r....r9..
-000038a0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
-000038b0: 7215 0000 0072 1000 0000 2700 0000 733c  r....r....'...s<
-000038c0: 0000 000a 0204 0a08 010c 0802 010a 040a  ................
-000038d0: 1200 0100 fe0a 5300 0100 0100 fe0a 2e02  ......S.........
-000038e0: 010a 3208 1000 0100 ff0a 1702 010a 280c  ..2...........(.
-000038f0: 0d0c 2808 1808 1008 1a08 1e00 0100 fe72  ..(............r
-00003900: 1000 0000 291a 72bc 0000 0072 9b00 0000  ....).r....r....
-00003910: da0b 6461 7461 636c 6173 7365 7372 0200  ..dataclassesr..
-00003920: 0000 da07 696e 7370 6563 7472 0300 0000  ....inspectr....
-00003930: 7204 0000 00da 0770 6174 686c 6962 7205  r......pathlibr.
-00003940: 0000 0072 6200 0000 72b7 0000 00da 056e  ...rb...r......n
-00003950: 756d 7079 7206 0000 00da 116f 6273 7079  umpyr......obspy
-00003960: 2e63 6f72 652e 7374 7265 616d 7207 0000  .core.streamr...
-00003970: 0072 0800 0000 da10 6f62 7370 792e 636f  .r......obspy.co
-00003980: 7265 2e74 7261 6365 7209 0000 00da 146f  re.tracer......o
-00003990: 6273 7079 2e63 6f72 652e 696e 7665 6e74  bspy.core.invent
-000039a0: 6f72 7972 0a00 0000 720b 0000 0072 9200  oryr....r....r..
-000039b0: 0000 720d 0000 0072 3c00 0000 720f 0000  ..r....r<...r...
-000039c0: 0072 1000 0000 7214 0000 0072 1400 0000  .r....r....r....
-000039d0: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
-000039e0: 756c 653e 0200 0000 731e 0000 0004 1008  ule>....s.......
-000039f0: 020c 0110 010c 0108 0108 030c 0110 010c  ................
-00003a00: 0110 030c 010c 0206 0302 01              ...........
+00000720: 6403 8400 7c02 4400 8301 7d05 6e0e 6404  d...|.D...}.n.d.
+00000730: 6403 8400 7c01 4400 8301 7d05 7c05 4400  d...|.D...}.|.D.
+00000740: 5d4c 7d06 7c00 6a01 7c01 7c06 6a02 7c06  ]L}.|.j.|.|.j.|.
+00000750: 6a03 7c06 6a04 7c06 6a05 7c03 6405 8d06  j.|.j.|.j.|.d...
+00000760: 7d07 7c07 6a06 7c06 6a07 6b02 7368 7408  }.|.j.|.j.k.sht.
+00000770: 6406 8301 8201 7c00 6a09 7c07 7c06 6a02  d.....|.j.|.|.j.
+00000780: 7c06 6a03 7c04 6407 8d04 0100 7132 7c01  |.j.|.d.....q2|.
+00000790: 5300 2908 61ce 0100 000a 2020 2020 2020  S.).a.....      
+000007a0: 2020 5570 6461 7465 2069 6e76 656e 746f    Update invento
+000007b0: 7279 2066 6f72 2063 6861 6e6e 656c 7320  ry for channels 
+000007c0: 666f 756e 6420 696e 2073 7472 6561 6d0a  found in stream.
+000007d0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000007e0: 2020 2020 2020 2020 2020 2069 6e76 2028             inv (
+000007f0: 3a63 6c61 7373 3a60 6f62 7370 792e 636f  :class:`obspy.co
+00000800: 7265 2e65 7665 6e74 732e 696e 7665 6e74  re.events.invent
+00000810: 6f72 792e 496e 7665 6e74 6f72 7960 293a  ory.Inventory`):
+00000820: 2069 6e76 656e 746f 7279 0a20 2020 2020   inventory.     
+00000830: 2020 2020 2020 2073 7420 283a 636c 6173         st (:clas
+00000840: 733a 606f 6273 7079 2e63 6f72 652e 7374  s:`obspy.core.st
+00000850: 7265 616d 2e53 7472 6561 6d60 293a 2064  ream.Stream`): d
+00000860: 6174 6120 7374 7265 616d 2028 7573 6564  ata stream (used
+00000870: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00000880: 2020 2020 6465 7465 726d 696e 6520 6e65      determine ne
+00000890: 742f 7374 612f 6368 616e 2f6c 6f63 2063  t/sta/chan/loc c
+000008a0: 6f64 6573 292e 2020 4966 204e 6f6e 652c  odes).  If None,
+000008b0: 2077 696c 6c20 7570 6461 7465 0a20 2020   will update.   
+000008c0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+000008d0: 7279 2063 6861 6e6e 656c 0a20 2020 2020  ry channel.     
+000008e0: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
+000008f0: 5f66 6972 7320 2862 6f6f 6c29 3a20 6e6f  _firs (bool): no
+00000900: 726d 616c 697a 6520 4649 5220 6368 616e  rmalize FIR chan
+00000910: 6e65 6c73 2074 6861 7420 6172 656e 2774  nels that aren't
+00000920: 2061 6c72 6561 6479 0a0a 2020 2020 2020   already..      
+00000930: 2020 3a20 7265 7475 726e 733a 206f 6273    : returns: obs
+00000940: 7079 2069 6e76 656e 746f 7279 2077 6974  py inventory wit
+00000950: 6820 6e65 7720 6368 616e 6e65 6c73 0a20  h new channels. 
+00000960: 2020 2020 2020 204e 6301 0000 0000 0000         Nc.......
+00000970: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00000980: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
+00000990: 6a00 9102 7104 5300 7214 0000 0029 01da  j...q.S.r....)..
+000009a0: 0573 7461 7473 a902 da02 2e30 da02 7472  .stats.....0..tr
+000009b0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+000009c0: 0a3c 6c69 7374 636f 6d70 3e5b 0000 00f3  .<listcomp>[....
+000009d0: 0000 0000 7a2e 4465 6369 6d61 746f 722e  ....z.Decimator.
+000009e0: 7570 6461 7465 5f69 6e76 656e 746f 7279  update_inventory
+000009f0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000a00: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00000a10: 0004 0000 000c 0000 0053 0000 0073 4200  .........S...sB.
+00000a20: 0000 6700 7c00 5d3a 7d01 7c01 4400 5d30  ..g.|.]:}.|.D.]0
+00000a30: 7d02 7c02 4400 5d26 7d03 7400 7401 7c01  }.|.D.]&}.t.t.|.
+00000a40: 6a02 7c02 6a02 7c03 6a03 7c03 6a02 7c03  j.|.j.|.j.|.j.|.
+00000a50: 6a04 6400 8d05 6401 8d01 9104 7114 710c  j.d...d.....q.q.
+00000a60: 7104 5300 2902 2905 da07 6e65 7477 6f72  q.S.).)...networ
+00000a70: 6bda 0773 7461 7469 6f6e da08 6c6f 6361  k..station..loca
+00000a80: 7469 6f6e da07 6368 616e 6e65 6cda 0d73  tion..channel..s
+00000a90: 616d 706c 696e 675f 7261 7465 2901 da06  ampling_rate)...
+00000aa0: 6865 6164 6572 2905 7209 0000 00da 0464  header).r......d
+00000ab0: 6963 74da 0463 6f64 65da 0d6c 6f63 6174  ict..code..locat
+00000ac0: 696f 6e5f 636f 6465 da0b 7361 6d70 6c65  ion_code..sample
+00000ad0: 5f72 6174 6529 0472 2000 0000 da03 6e65  _rate).r .....ne
+00000ae0: 74da 0373 7461 da02 6368 7214 0000 0072  t..sta..chr....r
+00000af0: 1400 0000 7215 0000 0072 2200 0000 5d00  ....r....r"...].
+00000b00: 0000 7318 0000 0006 0a02 0108 0108 f502  ..s.............
+00000b10: 0102 0104 0104 0104 0104 0104 fb04 ff29  ...............)
+00000b20: 0572 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00000b30: 7227 0000 00da 0e6e 6f72 6d61 6c69 7a65  r'.....normalize
+00000b40: 5f66 6972 737a 2f64 6174 6120 616e 6420  _firsz/data and 
+00000b50: 6d65 7461 6461 7461 2073 616d 706c 696e  metadata samplin
+00000b60: 6720 7261 7465 7320 6172 6520 6469 6666  g rates are diff
+00000b70: 6572 656e 7421 a903 722e 0000 0072 2f00  erent!..r....r/.
+00000b80: 0000 da05 7175 6965 7429 0ada 0463 6f70  ....quiet)...cop
+00000b90: 79da 125f 6475 706c 6963 6174 655f 6368  y.._duplicate_ch
+00000ba0: 616e 6e65 6c72 2400 0000 7225 0000 0072  annelr$...r%...r
+00000bb0: 2600 0000 7227 0000 0072 2d00 0000 7228  &...r'...r-...r(
+00000bc0: 0000 00da 0a56 616c 7565 4572 726f 72da  .....ValueError.
+00000bd0: 0c5f 6d6f 6469 6679 5f63 6861 6e29 0872  ._modify_chan).r
+00000be0: 1300 0000 da03 696e 76da 0273 7472 3100  ......inv..str1.
+00000bf0: 0000 7233 0000 005a 0a73 7461 7473 5f6c  ..r3...Z.stats_l
+00000c00: 6973 7472 1e00 0000 da07 6e65 775f 6368  istr......new_ch
+00000c10: 6172 1400 0000 7214 0000 0072 1500 0000  ar....r....r....
+00000c20: da10 7570 6461 7465 5f69 6e76 656e 746f  ..update_invento
+00000c30: 7279 4a00 0000 732e 0000 0000 0f08 0108  ryJ...s.........
+00000c40: 0110 0206 0a02 f606 0e08 0104 0102 0104  ................
+00000c50: 0104 0104 0104 0102 fa06 080c 0102 0102  ................
+00000c60: ff04 0304 010c ff08 037a 1a44 6563 696d  .........z.Decim
+00000c70: 6174 6f72 2e75 7064 6174 655f 696e 7665  ator.update_inve
+00000c80: 6e74 6f72 79da 012a 6308 0000 0000 0000  ntory..*c.......
+00000c90: 0000 0000 000e 0000 000b 0000 0043 0000  .............C..
+00000ca0: 0073 7400 0000 7c01 a000 a100 7d01 7c01  .st...|.....}.|.
+00000cb0: 6a01 7c02 7c03 7c05 7c04 6401 8d04 7d08  j.|.|.|.|.d...}.
+00000cc0: 7c08 4400 5d50 7d09 7c09 4400 5d46 7d0a  |.D.]P}.|.D.]F}.
+00000cd0: 7c0a a000 a100 7d0b 7c0b 4400 5d34 7d0c  |.....}.|.D.]4}.
+00000ce0: 7c00 6a02 7c01 7c09 6a03 7c0a 6a03 7c0c  |.j.|.|.j.|.j.|.
+00000cf0: 6a04 7c0c 6a03 7c07 6402 8d06 7d0d 7c00  j.|.j.|.d...}.|.
+00000d00: 6a05 7c0d 7c02 7c03 7c06 6403 8d04 0100  j.|.|.|.|.d.....
+00000d10: 7136 7126 711e 7c01 5300 2904 6104 0300  q6q&q.|.S.).a...
+00000d20: 000a 2020 2020 2020 2020 5570 6461 7465  ..        Update
+00000d30: 2069 6e76 656e 746f 7279 2062 6173 6564   inventory based
+00000d40: 206f 6e20 6e65 7477 6f72 6b2c 2073 7461   on network, sta
+00000d50: 7469 6f6e 2c20 6368 616e 6e65 6c20 616e  tion, channel an
+00000d60: 6420 6c6f 6361 7469 6f6e 2063 6f64 6573  d location codes
+00000d70: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00000d80: 2020 2020 2020 2020 2020 2020 696e 7620              inv 
+00000d90: 283a 636c 6173 733a 606f 6273 7079 2e63  (:class:`obspy.c
+00000da0: 6f72 652e 6576 656e 7473 2e69 6e76 656e  ore.events.inven
+00000db0: 746f 7279 2e49 6e76 656e 746f 7279 6029  tory.Inventory`)
+00000dc0: 3a20 696e 7665 6e74 6f72 790a 2020 2020  : inventory.    
+00000dd0: 2020 2020 2020 2020 6e65 7477 6f72 6b20          network 
+00000de0: 2873 7472 293a 2046 4453 4e20 6e65 7477  (str): FDSN netw
+00000df0: 6f72 6b20 636f 6465 0a20 2020 2020 2020  ork code.       
+00000e00: 2020 2020 2073 7461 7469 6f6e 2028 7374       station (st
+00000e10: 7229 3a20 7374 6174 696f 6e20 636f 6465  r): station code
+00000e20: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00000e30: 6e6e 656c 2028 7374 7229 3a20 6368 616e  nnel (str): chan
+00000e40: 6e65 6c20 636f 6465 0a20 2020 2020 2020  nel code.       
+00000e50: 2020 2020 206c 6f63 6174 696f 6e20 2873       location (s
+00000e60: 7472 293a 2046 4453 4e20 6c6f 6361 7469  tr): FDSN locati
+00000e70: 6f6e 2063 6f64 650a 2020 2020 2020 2020  on code.        
+00000e80: 2020 2020 7175 6965 7420 2862 6f6f 6c29      quiet (bool)
+00000e90: 3a20 446f 206e 6f74 2073 6179 2077 6861  : Do not say wha
+00000ea0: 7420 6368 616e 6e65 6c28 7329 2077 6173  t channel(s) was
+00000eb0: 2063 6861 6e67 6564 0a20 2020 2020 2020   changed.       
+00000ec0: 2020 2020 206e 6f72 6d61 6c69 7a65 5f66       normalize_f
+00000ed0: 6972 7320 2862 6f6f 6c29 3a20 6e6f 726d  irs (bool): norm
+00000ee0: 616c 697a 6520 4649 5220 6368 616e 6e65  alize FIR channe
+00000ef0: 736c 2074 6861 7420 6172 656e 2774 2061  sl that aren't a
+00000f00: 6c72 6561 6479 0a0a 2020 2020 2020 2020  lready..        
+00000f10: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000f20: 2020 2020 206e 6577 696e 763a 2069 6e76       newinv: inv
+00000f30: 2028 3a63 6c61 7373 3a60 6f62 7370 792e   (:class:`obspy.
+00000f40: 636f 7265 2e65 7665 6e74 732e 696e 7665  core.events.inve
+00000f50: 6e74 6f72 792e 496e 7665 6e74 6f72 7960  ntory.Inventory`
+00000f60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00000f70: 2020 2075 7064 6174 6564 2069 6e76 656e     updated inven
+00000f80: 746f 7279 0a0a 2020 2020 2020 2020 6e65  tory..        ne
+00000f90: 7477 6f72 6b2c 2073 7461 7469 6f6e 2c20  twork, station, 
+00000fa0: 6368 616e 6e65 6c20 616e 6420 6c6f 6361  channel and loca
+00000fb0: 7469 6f6e 2063 6f64 6573 2061 7265 2027  tion codes are '
+00000fc0: 2a27 2062 7920 6465 6661 756c 742c 0a20  *' by default,. 
+00000fd0: 2020 2020 2020 206d 6179 2069 6e63 6c75         may inclu
+00000fe0: 6465 2077 696c 6463 6172 6473 2061 7320  de wildcards as 
+00000ff0: 7370 6563 6966 6965 6420 696e 206f 6273  specified in obs
+00001000: 7079 2e63 6f72 652e 7374 7265 616d 2e53  py.core.stream.S
+00001010: 7472 6561 6d2e 7365 6c65 6374 0a20 2020  tream.select.   
+00001020: 2020 2020 2029 0472 2400 0000 7225 0000       ).r$...r%..
+00001030: 0072 2600 0000 7227 0000 0029 0172 3100  .r&...r'...).r1.
+00001040: 0000 7232 0000 0029 0672 3400 0000 da06  ..r2...).r4.....
+00001050: 7365 6c65 6374 7235 0000 0072 2b00 0000  selectr5...r+...
+00001060: 722c 0000 0072 3700 0000 290e 7213 0000  r,...r7...).r...
+00001070: 0072 3800 0000 7224 0000 0072 2500 0000  .r8...r$...r%...
+00001080: 7227 0000 0072 2600 0000 7233 0000 0072  r'...r&...r3...r
+00001090: 3100 0000 5a0c 696e 765f 7365 6c65 6374  1...Z.inv_select
+000010a0: 6564 722e 0000 0072 2f00 0000 5a07 6f6c  edr....r/...Z.ol
+000010b0: 645f 7374 61da 0363 6861 723a 0000 0072  d_sta..char:...r
+000010c0: 1400 0000 7214 0000 0072 1500 0000 da1a  ....r....r......
+000010d0: 7570 6461 7465 5f69 6e76 656e 746f 7279  update_inventory
+000010e0: 5f66 726f 6d5f 6e73 6c63 7d00 0000 732e  _from_nslc}...s.
+000010f0: 0000 0000 1608 0104 0102 0102 0102 0102  ................
+00001100: fc06 0608 0108 0108 0108 0104 0102 0104  ................
+00001110: 0104 0104 0104 0102 fa06 0804 0108 ff0c  ................
+00001120: 037a 2444 6563 696d 6174 6f72 2e75 7064  .z$Decimator.upd
+00001130: 6174 655f 696e 7665 6e74 6f72 795f 6672  ate_inventory_fr
+00001140: 6f6d 5f6e 736c 6363 0200 0000 0000 0000  om_nslcc........
+00001150: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00001160: 730e 0100 0074 007c 0083 0164 016b 0372  s....t.|...d.k.r
+00001170: 1c74 0164 027c 009b 0264 039d 0383 0182  .t.d.|...d......
+00001180: 017c 0064 0476 0072 ae7c 0164 056b 0572  .|.d.v.r.|.d.k.r
+00001190: 3064 0653 007c 0164 076b 0572 3c64 0853  0d.S.|.d.k.r<d.S
+000011a0: 007c 0164 096b 0572 4864 0a53 007c 0164  .|.d.k.rHd.S.|.d
+000011b0: 0b6b 0572 5464 0c53 007c 0164 016b 0472  .k.rTd.S.|.d.k.r
+000011c0: 6064 0d53 007c 0164 0e6b 0472 6c64 0f53  `d.S.|.d.k.rld.S
+000011d0: 007c 0164 106b 0472 7864 1153 007c 0164  .|.d.k.rxd.S.|.d
+000011e0: 126b 0472 8464 1353 007c 0164 146b 0572  .k.r.d.S.|.d.k.r
+000011f0: 9064 1553 007c 0164 166b 0572 9c64 1753  .d.S.|.d.k.r.d.S
+00001200: 007c 0164 186b 0572 a864 1953 0064 1a53  .|.d.k.r.d.S.d.S
+00001210: 006e 5c7c 0064 1b76 0090 0072 fa7c 0164  .n\|.d.v...r.|.d
+00001220: 056b 0572 c464 1c53 007c 0164 076b 0572  .k.r.d.S.|.d.k.r
+00001230: d064 1d53 007c 0164 096b 0572 dc64 1e53  .d.S.|.d.k.r.d.S
+00001240: 007c 0164 0b6b 0590 0072 ea64 1f53 0074  .|.d.k...r.d.S.t
+00001250: 02a0 0364 20a1 0101 0064 2153 006e 1074  ...d ....d!S.n.t
+00001260: 0464 227c 009b 0064 239d 0383 0182 0164  .d"|...d#......d
+00001270: 2453 0029 257a dd0a 2020 2020 2020 2020  $S.)%z..        
+00001280: 5265 7475 726e 2074 6865 2063 6861 6e6e  Return the chann
+00001290: 656c 2062 616e 6420 636f 6465 2062 6173  el band code bas
+000012a0: 6564 206f 6e20 616e 2069 6e70 7574 2062  ed on an input b
+000012b0: 616e 645f 636f 6465 0a0a 2020 2020 2020  and_code..      
+000012c0: 2020 3a70 6172 616d 2069 6e5f 6261 6e64    :param in_band
+000012d0: 5f63 6f64 653a 2069 6e70 7574 2062 616e  _code: input ban
+000012e0: 6420 636f 6465 2028 2742 2720 6966 2063  d code ('B' if c
+000012f0: 7574 6f66 6620 3e20 3130 732c 0a20 2020  utoff > 10s,.   
+00001300: 2020 2020 2020 2020 2027 5327 206f 7468           'S' oth
+00001310: 6572 7769 7365 290a 2020 2020 2020 2020  erwise).        
+00001320: 3a70 6172 616d 2073 616d 706c 655f 7261  :param sample_ra
+00001330: 7465 3a20 696e 7075 7420 7361 6d70 6c65  te: input sample
+00001340: 2072 6174 6520 2873 7073 290a 2020 2020   rate (sps).    
+00001350: 2020 2020 720c 0000 007a 0e22 696e 5f62      r....z."in_b
+00001360: 616e 645f 636f 6465 3d7a 1c22 2069 7320  and_code=z." is 
+00001370: 6d6f 7265 2074 6861 6e20 6f6e 6520 6368  more than one ch
+00001380: 6172 6163 7465 725a 0c46 4348 424d 4c56  aracterZ.FCHBMLV
+00001390: 5552 5054 5169 e803 0000 da01 46e9 fa00  URPTQi......F...
+000013a0: 0000 da01 43e9 5000 0000 da01 48e9 0a00  ....C.P.....H...
+000013b0: 0000 da01 42da 014d 6733 3333 3333 33d3  ....B..Mg333333.
+000013c0: 3fda 014c 67b8 1e85 eb51 b89e 3fda 0156  ?..Lg....Q..?..V
+000013d0: 67fa 7e6a bc74 9368 3fda 0155 672d 431c  g.~j.t.h?..Ug-C.
+000013e0: ebe2 361a 3fda 0152 67f1 68e3 88b5 f8e4  ..6.?..Rg.h.....
+000013f0: 3eda 0150 678d edb5 a0f7 c6b0 3eda 0154  >..Pg.......>..T
+00001400: da01 515a 0447 4445 53da 0147 da01 44da  ..QZ.GDES..G..D.
+00001410: 0145 da01 537a 2853 686f 7274 2070 6572  .E..Sz(Short per
+00001420: 696f 6420 7365 6e73 6f72 2073 616d 706c  iod sensor sampl
+00001430: 6520 7261 7465 203c 2031 3020 7370 73da  e rate < 10 sps.
+00001440: 0158 7a19 556e 6b6e 6f77 6e20 6261 6e64  .Xz.Unknown band
+00001450: 2062 6173 6520 636f 6465 3a20 22fa 0122   base code: ".."
+00001460: 4e29 05da 036c 656e 7236 0000 00da 0877  N)...lenr6.....w
+00001470: 6172 6e69 6e67 73da 0477 6172 6e72 1b00  arnings..warnr..
+00001480: 0000 2902 da0c 696e 5f62 616e 645f 636f  ..)...in_band_co
+00001490: 6465 722d 0000 0072 1400 0000 7214 0000  der-...r....r...
+000014a0: 0072 1500 0000 da0d 6765 745f 6261 6e64  .r......get_band
+000014b0: 5f63 6f64 65ab 0000 0073 4c00 0000 0009  _code....sL.....
+000014c0: 0c01 1001 0801 0801 0401 0801 0401 0801  ................
+000014d0: 0401 0801 0401 0801 0401 0801 0401 0801  ................
+000014e0: 0401 0801 0401 0801 0401 0801 0401 0801  ................
+000014f0: 0402 0601 0a01 0801 0401 0801 0401 0801  ................
+00001500: 0401 0a01 0402 0a01 0602 7a17 4465 6369  ..........z.Deci
+00001510: 6d61 746f 722e 6765 745f 6261 6e64 5f63  mator.get_band_c
+00001520: 6f64 6563 0400 0000 0000 0000 0000 0000  odec............
+00001530: 0400 0000 0700 0000 4300 0000 7334 0000  ........C...s4..
+00001540: 007c 017c 00a0 007c 017c 02a1 026b 0372  .|.|...|.|...k.r
+00001550: 2874 01a0 0264 017c 019b 0064 027c 029b  (t...d.|...d.|..
+00001560: 0064 039d 05a1 0101 007c 00a0 007c 017c  .d.......|...|.|
+00001570: 03a1 0253 0029 047a cc0a 2020 2020 2020  ...S.).z..      
+00001580: 2020 5265 7475 726e 2074 6865 2063 6861    Return the cha
+00001590: 6e6e 656c 2062 616e 6420 636f 6465 0a0a  nnel band code..
+000015a0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+000015b0: 6e5f 6261 6e64 5f63 6f64 653a 2069 6e70  n_band_code: inp
+000015c0: 7574 2062 616e 6420 636f 6465 0a20 2020  ut band code.   
+000015d0: 2020 2020 203a 7061 7261 6d20 696e 5f73       :param in_s
+000015e0: 616d 706c 655f 7261 7465 3a20 696e 7075  ample_rate: inpu
+000015f0: 7420 7361 6d70 6c65 2072 6174 6520 2873  t sample rate (s
+00001600: 7073 290a 2020 2020 2020 2020 3a70 6172  ps).        :par
+00001610: 616d 206f 7574 5f73 616d 706c 655f 7261  am out_sample_ra
+00001620: 7465 3a20 6f75 7470 7574 2073 616d 706c  te: output sampl
+00001630: 6520 7261 7465 2028 7370 7329 0a20 2020  e rate (sps).   
+00001640: 2020 2020 207a 1149 6e70 7574 2062 616e       z.Input ban
+00001650: 6420 636f 6465 2028 7a27 2920 646f 6573  d code (z') does
+00001660: 206e 6f74 206d 6174 6368 2020 696e 7075   not match  inpu
+00001670: 7420 7361 6d70 6c69 6e67 2072 6174 6520  t sampling rate 
+00001680: 28fa 0129 2903 7259 0000 0072 5600 0000  (..)).rY...rV...
+00001690: 7257 0000 0029 0472 1300 0000 7258 0000  rW...).r....rX..
+000016a0: 005a 0e69 6e5f 7361 6d70 6c65 5f72 6174  .Z.in_sample_rat
+000016b0: 655a 0f6f 7574 5f73 616d 706c 655f 7261  eZ.out_sample_ra
+000016c0: 7465 7214 0000 0072 1400 0000 7215 0000  ter....r....r...
+000016d0: 00da 125f 6765 745f 6e65 775f 6261 6e64  ..._get_new_band
+000016e0: 5f63 6f64 65de 0000 0073 0e00 0000 0009  _code....s......
+000016f0: 1001 0401 0801 02ff 06ff 0404 7a1c 4465  ............z.De
+00001700: 6369 6d61 746f 722e 5f67 6574 5f6e 6577  cimator._get_new
+00001710: 5f62 616e 645f 636f 6465 da00 6306 0000  _band_code..c...
+00001720: 0000 0000 0000 0000 0007 0000 000a 0000  ................
+00001730: 0043 0000 0073 7e00 0000 7400 a001 6401  .C...s~...t...d.
+00001740: a002 6402 a003 7c02 7c03 7c01 6a04 7c01  ..d...|.|.|.j.|.
+00001750: 6a05 6704 a101 7c01 6a06 a102 a101 0100  j.g...|.j.......
+00001760: 7c01 6a06 7d06 7c00 a007 7c01 7c06 a102  |.j.}.|...|.|...
+00001770: 0100 7c00 a008 7c01 7c06 a102 0100 7c01  ..|...|.|.....|.
+00001780: 0400 6a06 7c00 6a09 1d00 0200 5f06 7400  ..j.|.j....._.t.
+00001790: a001 6403 a002 6402 a003 7c02 7c03 7c01  ..d...d...|.|.|.
+000017a0: 6a04 7c01 6a05 6704 a101 7c01 6a06 a102  j.|.j.g...|.j...
+000017b0: a101 0100 6404 5300 2905 619e 0100 000a  ....d.S.).a.....
+000017c0: 2020 2020 2020 2020 6d6f 6469 6679 2072          modify r
+000017d0: 6570 6f6e 7365 2061 6e64 206e 616d 6520  eponse and name 
+000017e0: 6f66 2061 2063 6861 6e6e 656c 2074 6f20  of a channel to 
+000017f0: 636f 7272 6573 706f 6e64 2074 6f20 6465  correspond to de
+00001800: 6369 6d61 7469 6f6e 0a0a 2020 2020 2020  cimation..      
+00001810: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00001820: 2020 2020 6368 6120 283a 636c 6173 733a      cha (:class:
+00001830: 606f 6273 7079 2e63 6f72 652e 696e 7665  `obspy.core.inve
+00001840: 6e74 6f72 792e 6368 616e 6e65 6c60 293a  ntory.channel`):
+00001850: 206f 7269 6769 6e61 6c20 6368 616e 6e65   original channe
+00001860: 6c0a 2020 2020 2020 2020 2020 2020 6e65  l.            ne
+00001870: 7420 2873 7472 293a 206e 6574 776f 726b  t (str): network
+00001880: 2063 6f64 6520 286a 7573 7420 666f 7220   code (just for 
+00001890: 636c 6561 7265 7220 7072 6f67 7265 7373  clearer progress
+000018a0: 2070 7269 6e74 6f75 7429 0a20 2020 2020   printout).     
+000018b0: 2020 2020 2020 2073 7461 2028 7374 7229         sta (str)
+000018c0: 3a20 7374 6174 696f 6e20 636f 6465 2028  : station code (
+000018d0: 6a75 7374 2066 6f72 2063 6c65 6172 6572  just for clearer
+000018e0: 2070 726f 6772 6573 7320 7072 696e 746f   progress printo
+000018f0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+00001900: 6e6f 726d 616c 697a 655f 6669 7273 2028  normalize_firs (
+00001910: 626f 6f6c 293a 206e 6f72 6d61 6c69 7a65  bool): normalize
+00001920: 7320 616e 7920 4649 5220 6368 616e 6e65  s any FIR channe
+00001930: 6c20 7468 6174 2069 736e 2774 0a20 2020  l that isn't.   
+00001940: 2020 2020 2020 2020 2020 2020 2061 6c72               alr
+00001950: 6561 6479 0a20 2020 2020 2020 207a 2163  eady.        z!c
+00001960: 6861 6e6e 656c 206d 6f64 6966 6965 6420  hannel modified 
+00001970: 6672 6f6d 207b 7d20 287b 7d20 7370 7329  from {} ({} sps)
+00001980: da01 2e7a 1074 6f20 7b7d 2028 7b3a 677d  ...z.to {} ({:g}
+00001990: 2073 7073 294e 290a da06 6c6f 6767 6572   sps)N)...logger
+000019a0: da04 696e 666f da06 666f 726d 6174 da04  ..info..format..
+000019b0: 6a6f 696e 722c 0000 0072 2b00 0000 722d  joinr,...r+...r-
+000019c0: 0000 00da 185f 6164 645f 696e 7374 7275  ....._add_instru
+000019d0: 6d65 6e74 5f72 6573 706f 6e73 65da 105f  ment_response.._
+000019e0: 6368 616e 6765 5f63 6861 6e5f 6c6f 6372  change_chan_locr
+000019f0: 1600 0000 2907 7213 0000 0072 3e00 0000  ....).r....r>...
+00001a00: 722e 0000 0072 2f00 0000 7231 0000 0072  r....r/...r1...r
+00001a10: 3300 0000 da11 696e 7075 745f 7361 6d70  3.....input_samp
+00001a20: 6c65 5f72 6174 6572 1400 0000 7214 0000  le_rater....r...
+00001a30: 0072 1500 0000 7237 0000 00ee 0000 0073  .r....r7.......s
+00001a40: 1800 0000 000c 0801 1401 04fe 0603 0601  ................
+00001a50: 0c01 0c01 1001 0801 1401 04fe 7a16 4465  ............z.De
+00001a60: 6369 6d61 746f 722e 5f6d 6f64 6966 795f  cimator._modify_
+00001a70: 6368 616e 6301 0000 0000 0000 0000 0000  chanc...........
+00001a80: 0002 0000 0006 0000 0003 0000 0073 3e01  .............s>.
+00001a90: 0000 7c00 6a00 6a01 4400 9001 5d2e 7d01  ..|.j.j.D...].}.
+00001aa0: 7402 7c01 7403 8302 72be 7c01 6a04 6401  t.|.t...r.|.j.d.
+00001ab0: 6b02 722e 7405 7c01 6a06 8301 8900 6e56  k.r.t.|.j.....nV
+00001ac0: 7c01 6a04 6402 6b02 7248 6403 7405 7c01  |.j.d.k.rHd.t.|.
+00001ad0: 6a06 8301 1400 8900 6e3c 7c01 6a04 6404  j.......n<|.j.d.
+00001ae0: 6b02 7274 6403 7405 7c01 6a06 6405 6406  k.rtd.t.|.j.d.d.
+00001af0: 8502 1900 8301 1400 7c01 6a06 6406 1900  ........|.j.d...
+00001b00: 1700 8900 6e10 7407 6407 7c01 6a04 9b00  ....n.t.d.|.j...
+00001b10: 9d02 8301 8201 7408 8800 6408 1800 8301  ......t...d.....
+00001b20: 6409 6b04 72bc 7409 a00a 640a 8800 9b00  d.k.r.t...d.....
+00001b30: 640b 9d03 a101 0100 8700 6601 640c 640d  d.........f.d.d.
+00001b40: 8408 7c01 6a06 4400 8301 7c01 5f06 7108  ..|.j.D...|._.q.
+00001b50: 7402 7c01 740b 8302 7208 7405 7c01 6a0c  t.|.t...r.t.|.j.
+00001b60: 8301 640e 6b02 72ec 7405 7c01 6a0d 8301  ..d.k.r.t.|.j...
+00001b70: 8900 8800 640e 6b02 72ea 7108 6e14 7405  ....d.k.r.q.n.t.
+00001b80: 7c01 6a0d 8301 7405 7c01 6a0c 8301 1b00  |.j...t.|.j.....
+00001b90: 8900 7408 8800 6408 1800 8301 6409 6b04  ..t...d.....d.k.
+00001ba0: 7208 7409 a00a 640f 8800 9b00 640b 9d03  r.t...d.....d...
+00001bb0: a101 0100 8700 6601 6410 640d 8408 7c01  ......f.d.d...|.
+00001bc0: 6a0d 4400 8301 7c01 5f0d 7108 6405 5300  j.D...|._.q.d.S.
+00001bd0: 2911 7aa8 0a20 2020 2020 2020 2056 6572  ).z..        Ver
+00001be0: 6966 6965 7320 262c 2069 6620 6e65 6564  ifies &, if need
+00001bf0: 6564 2c20 6e6f 726d 616c 697a 6573 2063  ed, normalizes c
+00001c00: 6861 6e6e 656c 2773 2046 4952 206f 7220  hannel's FIR or 
+00001c10: 436f 6566 6669 6369 656e 7473 2063 6f65  Coefficients coe
+00001c20: 6666 730a 0a20 2020 2020 2020 2041 7267  ffs..        Arg
+00001c30: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00001c40: 6861 2028 3a63 6c61 7373 3a60 6f62 7370  ha (:class:`obsp
+00001c50: 792e 636f 7265 2e69 6e76 656e 746f 7279  y.core.inventory
+00001c60: 2e63 6861 6e6e 656c 6029 3a20 6368 616e  .channel`): chan
+00001c70: 6e65 6c0a 2020 2020 2020 2020 da04 4e4f  nel.        ..NO
+00001c80: 4e45 da04 4556 454e 720e 0000 00da 034f  NE..EVENr......O
+00001c90: 4444 4ee9 ffff ffff 7a22 556e 6b6e 6f77  DDN.....z"Unknow
+00001ca0: 6e20 4649 5220 636f 6566 6669 6369 656e  n FIR coefficien
+00001cb0: 7420 7379 6d6d 6574 7279 3a20 720c 0000  t symmetry: r...
+00001cc0: 0067 7b14 ae47 e17a 843f 7a1f 4445 4349  .g{..G.z.?z.DECI
+00001cd0: 4d41 544f 523a 2053 756d 206f 6620 4649  MATOR: Sum of FI
+00001ce0: 5220 636f 6566 6673 203d 207a 0d2c 206e  R coeffs = z., n
+00001cf0: 6f72 6d61 6c69 7a69 6e67 6301 0000 0000  ormalizingc.....
+00001d00: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00001d10: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+00001d20: 7c01 8800 1b00 9102 7104 5300 7214 0000  |.......q.S.r...
+00001d30: 0072 1400 0000 a902 7220 0000 00da 0178  .r......r .....x
+00001d40: a901 5a09 636f 6566 665f 7375 6d72 1400  ..Z.coeff_sumr..
+00001d50: 0000 7215 0000 0072 2200 0000 1e01 0000  ..r....r".......
+00001d60: 7304 0000 0006 0102 ff7a 2d44 6563 696d  s........z-Decim
+00001d70: 6174 6f72 2e5f 6e6f 726d 616c 697a 655f  ator._normalize_
+00001d80: 6669 7273 2e3c 6c6f 6361 6c73 3e2e 3c6c  firs.<locals>.<l
+00001d90: 6973 7463 6f6d 703e 7201 0000 007a 3544  istcomp>r....z5D
+00001da0: 4543 494d 4154 4f52 3a20 7375 6d28 6e75  ECIMATOR: sum(nu
+00001db0: 6d65 7261 746f 7220 636f 6566 6673 292f  merator coeffs)/
+00001dc0: 7375 6d28 6465 6e6f 6d20 636f 6566 6673  sum(denom coeffs
+00001dd0: 2920 3d20 6301 0000 0000 0000 0000 0000  ) = c...........
+00001de0: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
+00001df0: 0000 6700 7c00 5d0c 7d01 7c01 8800 1b00  ..g.|.].}.|.....
+00001e00: 9102 7104 5300 7214 0000 0072 1400 0000  ..q.S.r....r....
+00001e10: 7269 0000 0072 6b00 0000 7214 0000 0072  ri...rk...r....r
+00001e20: 1500 0000 7222 0000 002c 0100 0072 2300  ....r"...,...r#.
+00001e30: 0000 290e da08 7265 7370 6f6e 7365 da0f  ..)...response..
+00001e40: 7265 7370 6f6e 7365 5f73 7461 6765 7372  response_stagesr
+00001e50: 1800 0000 720a 0000 00da 0873 796d 6d65  ....r......symme
+00001e60: 7472 79da 0373 756d da0c 636f 6566 6669  try..sum..coeffi
+00001e70: 6369 656e 7473 7236 0000 00da 0361 6273  cientsr6.....abs
+00001e80: 725e 0000 0072 5f00 0000 720b 0000 00da  r^...r_...r.....
+00001e90: 0b64 656e 6f6d 696e 6174 6f72 da09 6e75  .denominator..nu
+00001ea0: 6d65 7261 746f 7229 0272 3e00 0000 5a03  merator).r>...Z.
+00001eb0: 7374 6772 1400 0000 726b 0000 0072 1500  stgr....rk...r..
+00001ec0: 0000 da0f 5f6e 6f72 6d61 6c69 7a65 5f66  ...._normalize_f
+00001ed0: 6972 7305 0100 0073 4000 0000 0008 0e01  irs....s@.......
+00001ee0: 0a01 0a01 0c01 0a01 1001 0a02 1eff 0404  ................
+00001ef0: 0201 0aff 0403 1001 0601 02ff 0a02 0a01  ................
+00001f00: 04ff 0a02 0a01 0e01 0a01 0801 0402 1402  ................
+00001f10: 1001 0401 0201 02ff 06ff 0403 7a19 4465  ............z.De
+00001f20: 6369 6d61 746f 722e 5f6e 6f72 6d61 6c69  cimator._normali
+00001f30: 7a65 5f66 6972 7363 0400 0000 0000 0000  ze_firsc........
+00001f40: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00001f50: 7320 0000 007c 00a0 007c 016a 017c 016a  s ...|...|.j.|.j
+00001f60: 027c 027c 03a1 045c 027c 015f 017c 015f  .|.|...\.|._.|._
+00001f70: 0264 0153 0029 0261 1c01 0000 0a20 2020  .d.S.).a.....   
+00001f80: 2020 2020 2043 6861 6e67 6520 6368 616e       Change chan
+00001f90: 6e65 6c20 286f 7220 6c6f 6361 7469 6f6e  nel (or location
+00001fa0: 2920 636f 6465 2069 6e20 706c 6163 652c  ) code in place,
+00001fb0: 2061 6363 6f72 6469 6e67 2074 6f20 6465   according to de
+00001fc0: 6369 6d61 7469 6f6e 0a0a 2020 2020 2020  cimation..      
+00001fd0: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00001fe0: 2020 2020 2020 2020 2063 6861 2028 496e           cha (In
+00001ff0: 7665 6e74 6f72 792e 4368 616e 6e65 6c29  ventory.Channel)
+00002000: 2063 6861 6e6e 656c 2074 6f20 6265 206d   channel to be m
+00002010: 6f64 6966 6965 6420 2869 6e20 706c 6163  odified (in plac
+00002020: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00002030: 6e5f 7372 2028 666c 6f61 7429 3a20 696e  n_sr (float): in
+00002040: 7075 7420 7361 6d70 6c65 2072 6174 650a  put sample rate.
+00002050: 2020 2020 2020 2020 2020 2020 6176 6f69              avoi
+00002060: 645f 636f 6465 7320 286c 6973 7429 3a20  d_codes (list): 
+00002070: 6368 616e 6e65 6c3a 6c6f 6361 7469 6f6e  channel:location
+00002080: 2063 6f64 6573 2074 6f20 6176 6f69 640a   codes to avoid.
+00002090: 2020 2020 2020 2020 4e29 03da 0d5f 6765          N)..._ge
+000020a0: 745f 6368 616e 5f6c 6f63 722b 0000 0072  t_chan_locr+...r
+000020b0: 2c00 0000 2904 7213 0000 0072 3e00 0000  ,...).r....r>...
+000020c0: da05 696e 5f73 72da 0b61 766f 6964 5f63  ..in_sr..avoid_c
+000020d0: 6f64 6573 7214 0000 0072 1400 0000 7215  odesr....r....r.
+000020e0: 0000 0072 6300 0000 2e01 0000 7306 0000  ...rc.......s...
+000020f0: 0000 0904 010c ff7a 1a44 6563 696d 6174  .......z.Decimat
+00002100: 6f72 2e5f 6368 616e 6765 5f63 6861 6e5f  or._change_chan_
+00002110: 6c6f 6363 0500 0000 0000 0000 0000 0000  locc............
+00002120: 0a00 0000 0800 0000 4300 0000 73c4 0000  ........C...s...
+00002130: 007c 006a 0064 016b 0272 1274 0164 0283  .|.j.d.k.r.t.d..
+00002140: 0182 017c 037c 006a 001b 007d 057c 00a0  ...|.|.j...}.|..
+00002150: 027c 0164 0319 007c 037c 05a1 037d 067c  .|.d...|.|...}.|
+00002160: 067c 0164 0164 0485 0219 0017 007d 077c  .|.d.d.......}.|
+00002170: 077c 016b 0272 747a 1474 037c 0283 0164  .|.k.rtz.t.|...d
+00002180: 0117 0064 059b 047d 0857 0071 7804 0074  ...d...}.W.qx..t
+00002190: 0479 7001 0001 0001 0064 067d 0859 0071  .yp......d.}.Y.q
+000021a0: 7830 006e 047c 027d 087c 0444 005d 3a7d  x0.n.|.}.|.D.]:}
+000021b0: 097c 077c 09a0 0564 07a1 0164 0319 006b  .|.|...d...d...k
+000021c0: 0272 7c7c 087c 09a0 0564 07a1 0164 0119  .r||.|...d...d..
+000021d0: 006b 0272 7c74 037c 0883 0164 0117 0064  .k.r|t.|...d...d
+000021e0: 059b 047d 0871 7c71 7c71 bc71 787c 077c  ...}.q|q|q.qx|.|
+000021f0: 0866 0253 0029 0861 8f01 0000 0a20 2020  .f.S.).a.....   
+00002200: 2020 2020 2047 6574 206e 6577 2063 6861       Get new cha
+00002210: 6e6e 656c 2028 6f72 206c 6f63 2920 636f  nnel (or loc) co
+00002220: 6465 7320 6672 6f6d 206f 6c64 2063 6f64  des from old cod
+00002230: 6573 2061 6e64 2064 6563 696d 6174 696f  es and decimatio
+00002240: 6e20 6661 6374 6f72 0a0a 2020 2020 2020  n factor..      
+00002250: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00002260: 2020 2020 2020 2020 2063 6861 5f63 6f64           cha_cod
+00002270: 653a 2069 6e70 7574 2063 6861 6e6e 656c  e: input channel
+00002280: 2063 6f64 650a 2020 2020 2020 2020 2020   code.          
+00002290: 2020 6c6f 635f 636f 6465 3a20 696e 7075    loc_code: inpu
+000022a0: 7420 6c6f 6361 7469 6f6e 2063 6f64 650a  t location code.
+000022b0: 2020 2020 2020 2020 2020 2020 696e 5f73              in_s
+000022c0: 723a 2069 6e70 7574 2073 616d 706c 696e  r: input samplin
+000022d0: 6720 7261 7465 0a20 2020 2020 2020 2020  g rate.         
+000022e0: 2020 2061 766f 6964 5f63 6f64 6573 2028     avoid_codes (
+000022f0: 6c69 7374 293a 2063 6861 6e6e 656c 3a6c  list): channel:l
+00002300: 6f63 6174 696f 6e20 636f 6465 7320 746f  ocation codes to
+00002310: 2061 766f 6964 0a0a 2020 2020 2020 2020   avoid..        
+00002320: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00002330: 2020 2020 2074 7570 6c65 3a0a 2020 2020       tuple:.    
+00002340: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00002350: 6368 616e 5f63 6f64 6520 2873 7472 290a  chan_code (str).
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 6e65 775f 6c6f 635f 636f 6465 2028 7374  new_loc_code (st
+00002380: 7229 0a20 2020 2020 2020 2072 0c00 0000  r).        r....
+00002390: 7a10 4465 6369 6d61 7469 6f6e 203d 3d20  z.Decimation == 
+000023a0: 3121 7201 0000 004e da03 3032 645a 0230  1!r....N..02dZ.0
+000023b0: 31fa 013a 2906 7216 0000 0072 3600 0000  1..:).r....r6...
+000023c0: 725b 0000 00da 0369 6e74 da09 4578 6365  r[.....int..Exce
+000023d0: 7074 696f 6eda 0573 706c 6974 290a 7213  ption..split).r.
+000023e0: 0000 005a 0863 6861 5f63 6f64 655a 086c  ...Z.cha_codeZ.l
+000023f0: 6f63 5f63 6f64 6572 7600 0000 7277 0000  oc_coderv...rw..
+00002400: 005a 066f 7574 5f73 725a 0d6e 6577 5f62  .Z.out_srZ.new_b
+00002410: 616e 645f 636f 6465 5a0c 6e65 775f 6368  and_codeZ.new_ch
+00002420: 615f 636f 6465 5a0c 6e65 775f 6c6f 635f  a_codeZ.new_loc_
+00002430: 636f 6465 da01 6372 1400 0000 7214 0000  code..cr....r...
+00002440: 0072 1500 0000 7275 0000 003b 0100 0073  .r....ru...;...s
+00002450: 2800 0000 000f 0a01 0801 0a01 1201 1001  (...............
+00002460: 0802 0201 1401 0c01 0c02 0403 0802 10ff  ................
+00002470: 0202 10fe 0204 1001 0401 0401 7a17 4465  ............z.De
+00002480: 6369 6d61 746f 722e 5f67 6574 5f63 6861  cimator._get_cha
+00002490: 6e5f 6c6f 6363 0300 0000 0000 0000 0000  n_locc..........
+000024a0: 0000 0700 0000 0800 0000 4300 0000 73a4  ..........C...s.
+000024b0: 0000 007c 016a 006a 0164 0119 006a 027d  ...|.j.j.d...j.}
+000024c0: 037c 006a 0344 005d 347d 0474 04a0 057c  .|.j.D.]4}.t...|
+000024d0: 04a1 017d 057c 0364 0237 007d 037c 016a  ...}.|.d.7.}.|.j
+000024e0: 006a 01a0 067c 05a0 077c 027c 03a1 02a1  .j...|...|.|....
+000024f0: 0101 007c 027c 041d 007d 0271 147a 0e7c  ...|.|...}.q.z.|
+00002500: 016a 00a0 08a1 0001 0057 006e 4604 0074  .j.......W.nF..t
+00002510: 0979 9e01 0001 0001 007c 016a 006a 0a6a  .y.......|.j.j.j
+00002520: 0b7d 067c 06a0 0ca1 0064 036b 0272 9a64  .}.|.....d.k.r.d
+00002530: 047c 016a 006a 0a5f 0b7c 016a 00a0 08a1  .|.j.j._.|.j....
+00002540: 0001 007c 067c 016a 006a 0a5f 0b59 006e  ...|.|.j.j._.Y.n
+00002550: 0230 0064 0553 0029 067a 630a 2020 2020  .0.d.S.).zc.    
+00002560: 2020 2020 4170 7065 6e64 2020 6465 6369      Append  deci
+00002570: 6d61 7469 6f6e 206f 626a 6563 7427 7320  mation object's 
+00002580: 696e 7374 7275 6d65 6e74 2072 6573 706f  instrument respo
+00002590: 6e73 6520 746f 2061 6e20 6578 6973 7469  nse to an existi
+000025a0: 6e67 2063 6861 6e6e 656c 2773 2072 6573  ng channel's res
+000025b0: 706f 6e73 650a 2020 2020 2020 2020 7268  ponse.        rh
+000025c0: 0000 0072 0c00 0000 da02 5041 7a03 4d2f  ...r......PAz.M/
+000025d0: 534e 290d 726c 0000 0072 6d00 0000 da15  SN).rl...rm.....
+000025e0: 7374 6167 655f 7365 7175 656e 6365 5f6e  stage_sequence_n
+000025f0: 756d 6265 7272 1100 0000 720d 0000 00da  umberr....r.....
+00002600: 0866 726f 6d5f 5341 43da 0661 7070 656e  .from_SAC..appen
+00002610: 645a 0874 6f5f 6f62 7370 79da 1f72 6563  dZ.to_obspy..rec
+00002620: 616c 6375 6c61 7465 5f6f 7665 7261 6c6c  alculate_overall
+00002630: 5f73 656e 7369 7469 7669 7479 727b 0000  _sensitivityr{..
+00002640: 00da 1669 6e73 7472 756d 656e 745f 7365  ...instrument_se
+00002650: 6e73 6974 6976 6974 79da 0b69 6e70 7574  nsitivity..input
+00002660: 5f75 6e69 7473 da05 7570 7065 7229 0772  _units..upper).r
+00002670: 1300 0000 723e 0000 0072 6400 0000 da0c  ....r>...rd.....
+00002680: 7374 6167 655f 6e75 6d62 6572 da01 64da  stage_number..d.
+00002690: 0a66 6972 5f66 696c 7465 72da 0369 5f75  .fir_filter..i_u
+000026a0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000026b0: 6200 0000 6301 0000 7320 0000 0000 040e  b...c...s ......
+000026c0: 010a 010a 0108 0108 010a ff04 030a 0102  ................
+000026d0: 010e 010c 010a 010c 010a 010a 017a 2244  .............z"D
+000026e0: 6563 696d 6174 6f72 2e5f 6164 645f 696e  ecimator._add_in
+000026f0: 7374 7275 6d65 6e74 5f72 6573 706f 6e73  strument_respons
+00002700: 6563 0200 0000 0000 0000 0000 0000 0500  ec..............
+00002710: 0000 0600 0000 4300 0000 7366 0000 0074  ......C...sf...t
+00002720: 007c 0174 0183 0273 1274 0264 0183 0182  .|.t...s.t.d....
+00002730: 017c 01a0 03a1 007d 0267 007d 037c 026a  .|.....}.g.}.|.j
+00002740: 0444 005d 147d 047c 03a0 057c 00a0 067c  .D.].}.|...|...|
+00002750: 04a1 01a1 0101 0071 247c 037c 025f 0474  .......q$|.|._.t
+00002760: 07a0 0864 02a0 0964 0364 0484 007c 0244  ...d...d.d...|.D
+00002770: 0083 01a1 01a1 0101 007c 02a0 0aa1 0001  .........|......
+00002780: 007c 0253 0029 057a 270a 2020 2020 2020  .|.S.).z'.      
+00002790: 2020 4465 6369 6d61 7465 206f 6273 7079    Decimate obspy
+000027a0: 2053 7472 6561 6d0a 2020 2020 2020 2020   Stream.        
+000027b0: 7a24 696e 7075 7420 7374 7265 616d 2069  z$input stream i
+000027c0: 7320 6e6f 7420 616e 206f 6273 7079 2053  s not an obspy S
+000027d0: 7472 6561 6d21 7a17 4e65 7720 6461 7461  tream!z.New data
+000027e0: 2068 6173 207b 7d20 7361 6d70 6c65 7363   has {} samplesc
+000027f0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002800: 0300 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00002810: 005d 0c7d 017c 016a 006a 0191 0271 0453  .].}.|.j.j...q.S
+00002820: 0072 1400 0000 2902 721c 0000 00da 0473  .r....).r......s
+00002830: 697a 6572 1f00 0000 7214 0000 0072 1400  izer....r....r..
+00002840: 0000 7215 0000 0072 2200 0000 8301 0000  ..r....r".......
+00002850: 7304 0000 0006 0102 ff7a 2944 6563 696d  s........z)Decim
+00002860: 6174 6f72 2e5f 7275 6e5f 7374 7265 616d  ator._run_stream
+00002870: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00002880: 6f6d 703e 290b 7218 0000 0072 0700 0000  omp>).r....r....
+00002890: 7236 0000 0072 3400 0000 da06 7472 6163  r6...r4.....trac
+000028a0: 6573 7281 0000 0072 1a00 0000 725e 0000  esr....r....r^..
+000028b0: 0072 5f00 0000 7260 0000 00da 0676 6572  .r_...r`.....ver
+000028c0: 6966 7929 0572 1300 0000 da06 7374 7265  ify).r......stre
+000028d0: 616d 7239 0000 005a 056e 6577 7472 7221  amr9...Z.newtrr!
+000028e0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+000028f0: 0000 7219 0000 0078 0100 0073 1800 0000  ..r....x...s....
+00002900: 0004 0a01 0801 0801 0401 0a01 1201 0601  ................
+00002910: 0e01 02ff 0a02 0801 7a15 4465 6369 6d61  ........z.Decima
+00002920: 746f 722e 5f72 756e 5f73 7472 6561 6d63  tor._run_streamc
+00002930: 0200 0000 0000 0000 0000 0000 0800 0000  ................
+00002940: 0700 0000 4300 0000 73ec 0000 0074 007c  ....C...s....t.|
+00002950: 0174 0183 0273 1274 0264 0183 0182 017c  .t...s.t.d.....|
+00002960: 016a 036a 047d 027c 01a0 05a1 007d 037c  .j.j.}.|.....}.|
+00002970: 036a 066a 077d 0474 08a0 0964 02a0 0a7c  .j.j.}.t...d...|
+00002980: 047c 047c 006a 0b1b 007c 006a 0ba1 03a1  .|.|.j...|.j....
+00002990: 0101 0074 0ca0 0ca1 007d 057c 006a 0d44  ...t.....}.|.j.D
+000029a0: 005d 2a7d 0674 0ea0 0f7c 06a1 017d 077c  .]*}.t...|...}.|
+000029b0: 07a0 107c 036a 03a1 017c 035f 037c 036a  ...|.j...|._.|.j
+000029c0: 117c 0664 0364 048d 0201 0071 547c 006a  .|.d.d.....qT|.j
+000029d0: 1264 0375 0072 a47c 036a 036a 047c 026b  .d.u.r.|.j.j.|.k
+000029e0: 0273 a47c 036a 03a0 137c 02a1 017c 035f  .s.|.j...|...|._
+000029f0: 037c 00a0 147c 036a 066a 157c 036a 066a  .|...|.j.j.|.j.j
+00002a00: 167c 036a 066a 077c 006a 0b14 00a1 035c  .|.j.j.|.j.....\
+00002a10: 027c 036a 065f 157c 036a 065f 1674 08a0  .|.j._.|.j._.t..
+00002a20: 0964 05a0 0a74 0ca0 0ca1 007c 0518 00a1  .d...t.....|....
+00002a30: 01a1 0101 007c 0353 0029 067a 260a 2020  .....|.S.).z&.  
+00002a40: 2020 2020 2020 4465 6369 6d61 7465 206f        Decimate o
+00002a50: 6273 7079 2054 7261 6365 0a20 2020 2020  bspy Trace.     
+00002a60: 2020 207a 2269 6e70 7574 2074 7261 6365     z"input trace
+00002a70: 2069 7320 6e6f 7420 616e 206f 6273 7079   is not an obspy
+00002a80: 2054 7261 6365 217a 3044 6563 696d 6174   Trace!z0Decimat
+00002a90: 696e 6720 6461 7461 2066 726f 6d20 7b3a  ing data from {:
+00002aa0: 677d 2074 6f20 7b3a 677d 2048 7a20 287b  g} to {:g} Hz ({
+00002ab0: 3a64 7d78 292e 2e2e 2054 2901 da09 6e6f  :d}x)... T)...no
+00002ac0: 5f66 696c 7465 727a 1354 6f6f 6b20 7b3a  _filterz.Took {:
+00002ad0: 2e31 667d 2073 6563 6f6e 6473 2917 7218  .1f} seconds).r.
+00002ae0: 0000 0072 0800 0000 7236 0000 0072 1c00  ...r....r6...r..
+00002af0: 0000 da05 6474 7970 6572 3400 0000 721e  ....dtyper4...r.
+00002b00: 0000 0072 2800 0000 725e 0000 0072 5f00  ...r(...r^...r_.
+00002b10: 0000 7260 0000 0072 1600 0000 da04 7469  ..r`...r......ti
+00002b20: 6d65 7211 0000 0072 0d00 0000 7280 0000  mer....r....r...
+00002b30: 00da 0863 6f6e 766f 6c76 6572 1d00 0000  ...convolver....
+00002b40: 7217 0000 00da 0661 7374 7970 6572 7500  r......astyperu.
+00002b50: 0000 7227 0000 0072 2600 0000 2908 7213  ..r'...r&...).r.
+00002b60: 0000 00da 0574 7261 6365 728f 0000 0072  .....tracer....r
+00002b70: 2100 0000 da02 7372 da03 7469 6372 8700  !.....sr..ticr..
+00002b80: 0000 7288 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00002b90: 0072 1500 0000 721a 0000 0088 0100 0073  .r....r........s
+00002ba0: 2e00 0000 0004 0a01 0801 0801 0801 0801  ................
+00002bb0: 0801 0a01 04fe 0603 0801 0a01 0a01 0e01  ................
+00002bc0: 1001 1601 0e01 0401 0601 0601 0cfd 1004  ................
+00002bd0: 1801 7a14 4465 6369 6d61 746f 722e 5f72  ..z.Decimator._r
+00002be0: 756e 5f74 7261 6365 6301 0000 0000 0000  un_tracec.......
+00002bf0: 0000 0000 000a 0000 0008 0000 0003 0000  ................
+00002c00: 0073 0a01 0000 7400 7401 7402 8300 8301  .s....t.t.t.....
+00002c10: 8301 a003 a100 6a04 7d01 6401 7c00 6402  ......j.}.d.|.d.
+00002c20: 9b04 9d02 7d02 7c01 a005 7c02 a101 7d03  ....}.|...|...}.
+00002c30: 7406 7c03 8301 6403 6b02 733e 7407 6404  t.|...d.k.s>t.d.
+00002c40: 8301 8201 7408 7c03 8301 8f68 7d04 7c04  ....t.|....h}.|.
+00002c50: a009 a100 0100 7c04 a009 a100 a00a a100  ......|.........
+00002c60: 7d05 740b 7c05 6405 1900 8301 8900 740c  }.t.|.d.......t.
+00002c70: 7c05 6403 1900 8301 7d06 6700 7d07 7c04  |.d.....}.g.}.|.
+00002c80: a00d a100 4400 5d1e 7d08 7c07 8700 6601  ....D.].}.|...f.
+00002c90: 6406 6407 8408 7c08 a00a a100 4400 8301  d.d...|.....D...
+00002ca0: 1700 7d07 7180 5700 6408 0400 0400 8303  ..}.q.W.d.......
+00002cb0: 0100 6e10 3100 73b4 3000 0100 0100 0100  ..n.1.s.0.......
+00002cc0: 5900 0100 7406 7c07 8301 7c06 6b02 73de  Y...t.|...|.k.s.
+00002cd0: 740e 6409 a00f 7406 7c07 8301 7c06 a102  t.d...t.|...|...
+00002ce0: 8301 8201 7406 7c07 8301 6403 1800 7d09  ....t.|...d...}.
+00002cf0: 7c07 640a 6405 640a 8503 1900 7c07 1700  |.d.d.d.....|...
+00002d00: 7d07 7410 7c07 7c09 6403 640b 8304 5300  }.t.|.|.d.d...S.
+00002d10: 290c 7a2a 0a20 2020 2020 2020 2052 6574  ).z*.        Ret
+00002d20: 7572 6e73 2061 2053 4143 2046 4952 2066  urns a SAC FIR f
+00002d30: 696c 7465 720a 2020 2020 2020 2020 da03  ilter.        ..
+00002d40: 6465 6372 8700 0000 720c 0000 007a 2353  decr....r....z#S
+00002d50: 4143 2066 696c 7465 7220 6669 6c65 2022  AC filter file "
+00002d60: 7b66 6261 7365 7d22 206e 6f74 2066 6f75  {fbase}" not fou
+00002d70: 6e64 7201 0000 0063 0100 0000 0000 0000  ndr....c........
+00002d80: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00002d90: 7318 0000 0067 007c 005d 107d 0174 007c  s....g.|.].}.t.|
+00002da0: 0183 0188 001b 0091 0271 0453 0072 1400  .........q.S.r..
+00002db0: 0000 2901 da05 666c 6f61 7472 6900 0000  ..)...floatri...
+00002dc0: a901 da07 6469 7669 736f 7272 1400 0000  ....divisorr....
+00002dd0: 7215 0000 0072 2200 0000 b201 0000 7223  r....r".......r#
+00002de0: 0000 007a 2b44 6563 696d 6174 6f72 2e5f  ...z+Decimator._
+00002df0: 7265 6164 5f46 4952 5f53 4143 2e3c 6c6f  read_FIR_SAC.<lo
+00002e00: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002e10: 4e7a 3246 4952 206c 656e 6774 6820 6973  Nz2FIR length is
+00002e20: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+00002e30: 7468 6174 2073 7461 7465 643a 207b 7d20  that stated: {} 
+00002e40: 213d 207b 7d72 6800 0000 725c 0000 0029  != {}rh...r\...)
+00002e50: 1172 0500 0000 7203 0000 0072 0400 0000  .r....r....r....
+00002e60: da07 7265 736f 6c76 65da 0670 6172 656e  ..resolve..paren
+00002e70: 74da 0467 6c6f 6272 5500 0000 da09 4e61  t..globrU.....Na
+00002e80: 6d65 4572 726f 72da 046f 7065 6eda 0872  meError..open..r
+00002e90: 6561 646c 696e 6572 7c00 0000 7297 0000  eadliner|...r...
+00002ea0: 0072 7a00 0000 da09 7265 6164 6c69 6e65  .rz.....readline
+00002eb0: 73da 0c52 756e 7469 6d65 4572 726f 7272  s..RuntimeErrorr
+00002ec0: 6000 0000 720d 0000 0029 0ada 0a64 6563  `...r....)...dec
+00002ed0: 696d 6174 696f 6eda 0862 6173 655f 6469  imation..base_di
+00002ee0: 725a 0566 6261 7365 da08 6669 6c65 6e61  rZ.fbase..filena
+00002ef0: 6d65 da01 66da 0141 5a07 6e43 6f65 6666  me..f..AZ.nCoeff
+00002f00: 73da 0663 6f65 6666 73da 046c 696e 65da  s..coeffs..line.
+00002f10: 0564 656c 6179 7214 0000 0072 9800 0000  .delayr....r....
+00002f20: 7215 0000 00da 0d5f 7265 6164 5f46 4952  r......_read_FIR
+00002f30: 5f53 4143 a201 0000 732c 0000 0000 0414  _SAC....s,......
+00002f40: 010c 010a 010c 0108 010a 0108 010c 010c  ................
+00002f50: 010c 0104 010c 013a 010c 0102 0104 0108  .......:........
+00002f60: ff02 ff04 050c 0112 017a 1744 6563 696d  .........z.Decim
+00002f70: 6174 6f72 2e5f 7265 6164 5f46 4952 5f53  ator._read_FIR_S
+00002f80: 4143 6307 0000 0000 0000 0000 0000 000d  ACc.............
+00002f90: 0000 000a 0000 0043 0000 0073 3001 0000  .......C...s0...
+00002fa0: 6700 7d07 6700 7d08 7c01 6a00 4400 5d90  g.}.g.}.|.j.D.].
+00002fb0: 7d09 7401 a001 7c09 6a02 a003 a100 7c02  }.t...|.j.....|.
+00002fc0: a003 a100 a102 732a 710e 7c09 6a04 4400  ......s*q.|.j.D.
+00002fd0: 5d6c 7d0a 7401 a001 7c0a 6a02 a003 a100  ]l}.t...|.j.....
+00002fe0: 7c03 a003 a100 a102 734c 7130 7c0a 6a05  |.......sLq0|.j.
+00002ff0: 4400 5d48 7d0b 7401 a001 7c0b 6a06 a003  D.]H}.t...|.j...
+00003000: a100 7c04 a003 a100 a102 736e 7152 7401  ..|.......snqRt.
+00003010: a001 7c0b 6a02 a003 a100 7c05 a003 a100  ..|.j.....|.....
+00003020: a102 7386 7152 7c07 a007 7c0a a101 0100  ..s.qR|...|.....
+00003030: 7c08 a007 7c0b a101 0100 7152 7130 710e  |...|.....qRq0q.
+00003040: 7408 7c07 8301 6401 6b02 72d2 7409 6402  t.|...d.k.r.t.d.
+00003050: 7c02 9b00 6403 7c03 9b00 6403 7c04 9b00  |...d.|...d.|...
+00003060: 6403 7c05 9b00 6404 9d09 8301 8201 6405  d.|...d.......d.
+00003070: 5300 7408 7c07 8301 6406 6b04 72f8 7409  S.t.|...d.k.r.t.
+00003080: 6407 a00a 7408 7c07 8301 7c02 7c03 7c04  d...t.|...|.|.|.
+00003090: 7c05 a105 8301 8201 7c06 6408 7500 9001  |.......|.d.u...
+000030a0: 7210 7c00 a00b 7c08 6401 1900 a101 0100  r.|...|.d.......
+000030b0: 7c08 6401 1900 a00c a100 7d0c 7c07 6401  |.d.......}.|.d.
+000030c0: 1900 6a05 a007 7c0c a101 0100 7c0c 5300  ..j...|.....|.S.
+000030d0: 2909 61c3 0100 000a 2020 2020 2020 2020  ).a.....        
+000030e0: 5265 7475 726e 2053 7461 7469 6f6e 2026  Return Station &
+000030f0: 2043 6861 6e6e 656c 206d 6174 6368 696e   Channel matchin
+00003100: 6720 6e65 7477 6f72 6b2c 2073 7461 7469  g network, stati
+00003110: 6f6e 2c20 6c6f 6361 7469 6f6e 2c20 6368  on, location, ch
+00003120: 616e 6e65 6c0a 0a20 2020 2020 2020 2041  annel..        A
+00003130: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+00003140: 2020 2020 2020 6e65 7477 6f72 6b20 2873        network (s
+00003150: 7472 293a 206e 6574 776f 726b 2063 6f64  tr): network cod
+00003160: 650a 2020 2020 2020 2020 2020 2020 7374  e.            st
+00003170: 6174 696f 6e20 2873 7472 293a 2073 7461  ation (str): sta
+00003180: 7469 6f6e 2063 6f64 650a 2020 2020 2020  tion code.      
+00003190: 2020 2020 2020 6c6f 6361 7469 6f6e 2028        location (
+000031a0: 7374 7229 3a20 6c6f 6361 7469 6f6e 2063  str): location c
+000031b0: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+000031c0: 6368 616e 6e65 6c20 2873 7472 293a 2063  channel (str): c
+000031d0: 6861 6e6e 656c 2063 6f64 650a 2020 2020  hannel code.    
+000031e0: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
+000031f0: 655f 6669 7273 2028 626f 6f6c 293a 206e  e_firs (bool): n
+00003200: 6f72 6d61 6c69 7a65 7320 616e 7920 4649  ormalizes any FI
+00003210: 5220 6368 616e 6e65 6c20 7468 6174 2069  R channel that i
+00003220: 736e 2774 0a20 2020 2020 2020 2020 2020  sn't.           
+00003230: 2020 2020 2061 6c72 6561 6479 0a0a 2020       already..  
+00003240: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00003250: 2020 2020 2020 2020 2020 2028 4368 616e             (Chan
+00003260: 6e65 6c29 3a20 6475 706c 6963 6174 6520  nel): duplicate 
+00003270: 6f66 2066 6f75 6e64 2063 6861 6e6e 656c  of found channel
+00003280: 2c20 7265 6164 7920 746f 206d 6f64 6966  , ready to modif
+00003290: 790a 2020 2020 2020 2020 7201 0000 007a  y.        r....z
+000032a0: 1274 7261 6365 2077 6176 6566 6f72 6d69  .trace waveformi
+000032b0: 6420 2272 5d00 0000 7a18 2220 6e6f 7420  d "r]...z." not 
+000032c0: 666f 756e 6420 696e 2069 6e76 656e 746f  found in invento
+000032d0: 7279 2902 4e4e 720c 0000 007a 297b 3a64  ry).NNr....z){:d
+000032e0: 7d20 7374 6174 696f 6e2d 6368 616e 6e65  } station-channe
+000032f0: 6c73 206d 6174 6368 6564 207b 7d2e 7b7d  ls matched {}.{}
+00003300: 2e7b 7d2e 7b7d 5429 0dda 086e 6574 776f  .{}.{}T)...netwo
+00003310: 726b 73da 0766 6e6d 6174 6368 722b 0000  rks..fnmatchr+..
+00003320: 0072 8500 0000 da08 7374 6174 696f 6e73  .r......stations
+00003330: da08 6368 616e 6e65 6c73 722c 0000 0072  ..channelsr,...r
+00003340: 8100 0000 7255 0000 0072 3600 0000 7260  ....rU...r6...r`
+00003350: 0000 0072 7400 0000 7234 0000 0029 0d72  ...rt...r4...).r
+00003360: 1300 0000 7238 0000 0072 2400 0000 7225  ....r8...r$...r%
+00003370: 0000 0072 2600 0000 7227 0000 0072 3100  ...r&...r'...r1.
+00003380: 0000 72ad 0000 0072 ae00 0000 722e 0000  ..r....r....r...
+00003390: 0072 2f00 0000 723e 0000 0072 3a00 0000  .r/...r>...r:...
+000033a0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000033b0: 3500 0000 bf01 0000 7346 0000 0000 1104  5.......sF......
+000033c0: 0104 010a 0216 0102 010a 0116 0102 010a  ................
+000033d0: 0104 010e ff04 0302 0116 0102 010a 0110  ................
+000033e0: 010c 0110 0102 ff04 0102 ff0a 0204 010c  ................
+000033f0: 0102 0104 010e ff02 ff04 050a 010e 010c  ................
+00003400: 0110 017a 1c44 6563 696d 6174 6f72 2e5f  ...z.Decimator._
+00003410: 6475 706c 6963 6174 655f 6368 616e 6e65  duplicate_channe
+00003420: 6c29 0154 2903 4e46 4629 0672 3c00 0000  l).T).NFF).r<...
+00003430: 723c 0000 0072 3c00 0000 723c 0000 0046  r<...r<...r<...F
+00003440: 4629 0472 5c00 0000 725c 0000 0046 4629  F).r\...r\...FF)
+00003450: 0146 2919 da08 5f5f 6e61 6d65 5f5f da0a  .F)...__name__..
+00003460: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00003470: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00003480: 5fda 046c 6973 74da 0f5f 5f61 6e6e 6f74  _..list..__annot
+00003490: 6174 696f 6e73 5f5f 7212 0000 00da 0462  ations__r......b
+000034a0: 6f6f 6cda 0870 726f 7065 7274 7972 1600  ool..propertyr..
+000034b0: 0000 721d 0000 0072 3b00 0000 723f 0000  ..r....r;...r?..
+000034c0: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
+000034d0: 5900 0000 725b 0000 0072 3700 0000 7274  Y...r[...r7...rt
+000034e0: 0000 0072 6300 0000 7275 0000 0072 6200  ...rc...ru...rb.
+000034f0: 0000 7219 0000 0072 1a00 0000 72aa 0000  ..r....r....r...
+00003500: 0072 3500 0000 7214 0000 0072 1400 0000  .r5...r....r....
+00003510: 7214 0000 0072 1500 0000 7210 0000 0025  r....r....r....%
+00003520: 0000 0073 3800 0000 0a02 040a 0801 0c02  ...s8...........
+00003530: 0201 0a04 0a12 00ff 0a33 0001 0001 00fe  .........3......
+00003540: 0a2e 0201 0a32 0810 0001 00ff 0a17 0201  .....2..........
+00003550: 0a28 0c0d 0c28 0815 0810 081a 081e 00ff  .(...(..........
+00003560: 7210 0000 0029 1a72 b200 0000 7290 0000  r....).r....r...
+00003570: 00da 0b64 6174 6163 6c61 7373 6573 7202  ...dataclassesr.
+00003580: 0000 00da 0769 6e73 7065 6374 7203 0000  .....inspectr...
+00003590: 0072 0400 0000 da07 7061 7468 6c69 6272  .r......pathlibr
+000035a0: 0500 0000 7256 0000 0072 ac00 0000 da05  ....rV...r......
+000035b0: 6e75 6d70 7972 0600 0000 da11 6f62 7370  numpyr......obsp
+000035c0: 792e 636f 7265 2e73 7472 6561 6d72 0700  y.core.streamr..
+000035d0: 0000 7208 0000 00da 106f 6273 7079 2e63  ..r......obspy.c
+000035e0: 6f72 652e 7472 6163 6572 0900 0000 da14  ore.tracer......
+000035f0: 6f62 7370 792e 636f 7265 2e69 6e76 656e  obspy.core.inven
+00003600: 746f 7279 720a 0000 0072 0b00 0000 7288  toryr....r....r.
+00003610: 0000 0072 0d00 0000 725e 0000 0072 0f00  ...r....r^...r..
+00003620: 0000 7210 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00003630: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
+00003640: 6475 6c65 3e02 0000 0073 1e00 0000 0410  dule>....s......
+00003650: 0801 0c01 1001 0c01 0801 0802 0c01 1001  ................
+00003660: 0c01 1003 0c01 0c02 0603 0201            ............
```

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar  4 13:29:11 2024 UTC, .py size: 7968 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a7cc e565 201f 0000  a..........e ...
+00000000: 610d 0d0a 0000 0000 ed6f a565 321e 0000  a........o.e2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6402 6c06 5a07 6401 6402 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6401 6406 6c0f  m.Z.m.Z...d.d.l.
@@ -23,15 +23,15 @@
 00000160: 0000 0040 0000 0073 8000 0000 6500 5a01  ...@...s....e.Z.
 00000170: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
 00000180: 3c00 6403 5a06 6507 6505 6404 3c00 6405  <.d.Z.e.e.d.<.d.
 00000190: 5a08 6507 6505 6406 3c00 6407 5a09 650a  Z.e.e.d.<.d.Z.e.
 000001a0: 6505 6408 3c00 650b 641a 640a 640b 8401  e.d.<.e.d.d.d...
 000001b0: 8301 5a0c 640c 640d 8400 5a0d 640e 640f  ..Z.d.d...Z.d.d.
 000001c0: 8400 5a0e 6410 6411 8400 5a0f 6412 6413  ..Z.d.d...Z.d.d.
-000001d0: 8400 5a10 641b 6415 6416 8401 5a11 641c  ..Z.d.d.d...Z.d.
+000001d0: 8400 5a10 641b 6414 6415 8401 5a11 641c  ..Z.d.d.d...Z.d.
 000001e0: 6418 6419 8401 5a12 6417 5300 291d da09  d.d...Z.d.S.)...
 000001f0: 4649 5246 696c 7465 727a 2043 7265 6174  FIRFilterz Creat
 00000200: 6520 616e 6420 696d 706c 656d 656e 7420  e and implement 
 00000210: 4649 5220 6669 6c74 6572 73da 0663 6f65  FIR filters..coe
 00000220: 6666 7372 0100 0000 da06 6f66 6673 6574  ffsr......offset
 00000230: e901 0000 00da 0564 6563 696d da00 da04  .......decim....
 00000240: 6e61 6d65 5463 0300 0000 0000 0000 0000  nameTc..........
@@ -214,266 +214,261 @@
 00000d50: 6d65 4572 726f 7229 0272 3c00 0000 da0d  meError).r<.....
 00000d60: 7379 6d6d 6574 7279 5f63 6f64 6572 1700  symmetry_coder..
 00000d70: 0000 7217 0000 0072 1f00 0000 da0f 5f61  ..r....r......_a
 00000d80: 7070 6c79 5f73 796d 6d65 7472 7960 0000  pply_symmetry`..
 00000d90: 0073 1000 0000 0004 0801 0401 0801 1a01  .s..............
 00000da0: 0801 1a02 1001 7a19 4649 5246 696c 7465  ......z.FIRFilte
 00000db0: 722e 5f61 7070 6c79 5f73 796d 6d65 7472  r._apply_symmetr
-00000dc0: 7946 6304 0000 0000 0000 0000 0000 0005  yFc.............
-00000dd0: 0000 0011 0000 0043 0000 0073 5e00 0000  .......C...s^...
-00000de0: 6401 7d04 7c03 6402 7501 7224 7c03 6403  d.}.|.d.u.r$|.d.
-00000df0: 6404 8502 1900 a000 a100 6401 6b02 7224  d.........d.k.r$
-00000e00: 7c03 7d04 7401 7c02 6405 6406 7c04 6407  |.}.t.|.d.d.|.d.
-00000e10: 7c04 6407 6408 7c00 6a02 7c00 6a03 7c01  |.d.d.|.j.|.j.|.
-00000e20: 7c00 6a04 7c00 6a05 7c00 6a05 7c01 1b00  |.j.|.j.|.j.|...
-00000e30: 7c00 6a05 7c01 1b00 6409 8d0f 5300 290a  |.j.|...d...S.).
-00000e40: 7a32 0a20 2020 2020 2020 2052 6574 7572  z2.        Retur
-00000e50: 6e20 616e 206f 6273 7079 2046 4952 5265  n an obspy FIRRe
-00000e60: 7370 6f6e 7365 5374 6167 650a 2020 2020  sponseStage.    
-00000e70: 2020 2020 da05 636f 756e 7446 4e72 1300      ..countFNr..
-00000e80: 0000 720d 0000 0072 0100 0000 7a0e 6469  ..r....r....z.di
-00000e90: 6769 7461 6c20 636f 756e 7473 7242 0000  gital countsrB..
-00000ea0: 0029 0fda 1573 7461 6765 5f73 6571 7565  .)...stage_seque
-00000eb0: 6e63 655f 6e75 6d62 6572 da0a 7374 6167  nce_number..stag
-00000ec0: 655f 6761 696e da14 7374 6167 655f 6761  e_gain..stage_ga
-00000ed0: 696e 5f66 7265 7175 656e 6379 da0b 696e  in_frequency..in
-00000ee0: 7075 745f 756e 6974 73da 1769 6e70 7574  put_units..input
-00000ef0: 5f75 6e69 7473 5f64 6573 6372 6970 7469  _units_descripti
-00000f00: 6f6e da0c 6f75 7470 7574 5f75 6e69 7473  on..output_units
-00000f10: da18 6f75 7470 7574 5f75 6e69 7473 5f64  ..output_units_d
-00000f20: 6573 6372 6970 7469 6f6e da08 7379 6d6d  escription..symm
-00000f30: 6574 7279 7210 0000 00da 0c63 6f65 6666  etryr......coeff
-00000f40: 6963 6965 6e74 73da 1c64 6563 696d 6174  icients..decimat
-00000f50: 696f 6e5f 696e 7075 745f 7361 6d70 6c65  ion_input_sample
-00000f60: 5f72 6174 65da 1164 6563 696d 6174 696f  _rate..decimatio
-00000f70: 6e5f 6661 6374 6f72 da11 6465 6369 6d61  n_factor..decima
-00000f80: 7469 6f6e 5f6f 6666 7365 74da 1064 6563  tion_offset..dec
-00000f90: 696d 6174 696f 6e5f 6465 6c61 79da 1564  imation_delay..d
-00000fa0: 6563 696d 6174 696f 6e5f 636f 7272 6563  ecimation_correc
-00000fb0: 7469 6f6e 2906 da05 6c6f 7765 7272 0700  tion)...lowerr..
-00000fc0: 0000 7210 0000 0072 0b00 0000 720e 0000  ..r....r....r...
-00000fd0: 0072 0c00 0000 2905 723c 0000 00da 0d73  .r....).r<.....s
-00000fe0: 616d 706c 696e 675f 7261 7465 724a 0000  ampling_raterJ..
-00000ff0: 005a 1270 7269 6f72 5f6f 7574 7075 745f  .Z.prior_output_
-00001000: 756e 6974 73da 0575 6e69 7473 7217 0000  units..unitsr...
-00001010: 0072 1700 0000 721f 0000 00da 0874 6f5f  .r....r......to_
-00001020: 6f62 7370 796e 0000 0073 2a00 0000 0005  obspyn...s*.....
-00001030: 0401 0801 1401 0401 0201 0201 0201 0201  ................
-00001040: 0201 0201 0201 0201 0201 0401 0401 0201  ................
-00001050: 0401 0401 0801 08f1 7a12 4649 5246 696c  ........z.FIRFil
-00001060: 7465 722e 746f 5f6f 6273 7079 4e63 0300  ter.to_obspyNc..
-00001070: 0000 0000 0000 0000 0000 0800 0000 0800  ................
-00001080: 0000 4300 0000 73b0 0000 0074 006a 0164  ..C...s....t.j.d
-00001090: 0164 0164 0264 038d 035c 027d 035c 025c  .d.d.d...\.}.\.\
-000010a0: 027d 047d 055c 027d 067d 0774 027c 047c  .}.}.\.}.}.t.|.|
-000010b0: 006a 0364 0464 047c 006a 041b 0083 0401  .j.d.d.|.j......
-000010c0: 0074 057c 067c 006a 0364 0464 047c 006a  .t.|.|.j.d.d.|.j
-000010d0: 041b 007c 006a 0683 0501 0074 077c 057c  ...|.j.....t.|.|
-000010e0: 006a 0364 047c 006a 0664 058d 0401 0074  .j.d.|.j.d.....t
-000010f0: 087c 077c 006a 0364 047c 006a 0664 058d  .|.|.j.d.|.j.d..
-00001100: 0401 007c 036a 0964 0664 0764 0864 0964  ...|.j.d.d.d.d.d
-00001110: 0a64 0b64 0c8d 0601 007c 0172 9a74 00a0  .d.d.....|.r.t..
-00001120: 0aa1 0001 007c 0264 0d75 0172 ac74 00a0  .....|.d.u.r.t..
-00001130: 0b7c 02a1 0101 007c 0353 0029 0e7a 2850  .|.....|.S.).z(P
-00001140: 6c6f 7420 4649 5220 6669 6c74 6572 2061  lot FIR filter a
-00001150: 6e64 2069 6d70 6f72 7461 6e74 2070 6172  nd important par
-00001160: 616d 6574 6572 7372 0800 0000 2902 e908  ametersr....)...
-00001170: 0000 0072 1400 0000 2901 da07 6669 6773  ...r....)...figs
-00001180: 697a 6572 0d00 0000 2901 da05 6465 6c61  izer....)...dela
-00001190: 7967 9a99 9999 9999 d93f 679a 9999 9999  yg.......?g.....
-000011a0: 99c9 3f67 ec51 b81e 85eb b13f 67ae 47e1  ..?g.Q.....?g.G.
-000011b0: 7a14 aeef 3f67 9a99 9999 9999 b93f 6766  z...?g.......?gf
-000011c0: 6666 6666 66ee 3f29 06da 0668 7370 6163  fffff.?)...hspac
-000011d0: 65da 0677 7370 6163 65da 046c 6566 74da  e..wspace..left.
-000011e0: 0572 6967 6874 da06 626f 7474 6f6d da03  .right..bottom..
-000011f0: 746f 704e 290c da03 706c 74da 0873 7562  topN)...plt..sub
-00001200: 706c 6f74 73da 0a70 6c6f 745f 6672 6571  plots..plot_freq
-00001210: 7a72 0b00 0000 720e 0000 00da 0b70 6c6f  zr....r......plo
-00001220: 745f 7068 6173 657a 720c 0000 00da 0970  t_phasezr......p
-00001230: 6c6f 745f 696d 707a da0a 706c 6f74 5f73  lot_impz..plot_s
-00001240: 7465 707a da0f 7375 6270 6c6f 7473 5f61  tepz..subplots_a
-00001250: 646a 7573 74da 0473 686f 77da 0773 6176  djust..show..sav
-00001260: 6566 6967 2908 723c 0000 0072 6c00 0000  efig).r<...rl...
-00001270: 726d 0000 00da 0366 6967 da03 6178 31da  rm.....fig..ax1.
-00001280: 0361 7832 da03 6178 33da 0361 7834 7217  .ax2..ax3..ax4r.
-00001290: 0000 0072 1700 0000 721f 0000 00da 0470  ...r....r......p
-000012a0: 6c6f 7489 0000 0073 1a00 0000 0002 2002  lot....s...... .
-000012b0: 1601 1a01 1401 1402 0401 0cff 0603 0401  ................
-000012c0: 0801 0801 0a02 7a0e 4649 5246 696c 7465  ......z.FIRFilte
-000012d0: 722e 706c 6f74 2901 5429 0272 0100 0000  r.plot).T).r....
-000012e0: 4629 0246 4e29 13da 085f 5f6e 616d 655f  F).FN)...__name_
-000012f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00001300: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00001310: 6f63 5f5f da04 6c69 7374 da0f 5f5f 616e  oc__..list..__an
-00001320: 6e6f 7461 7469 6f6e 735f 5f72 0c00 0000  notations__r....
-00001330: 722c 0000 0072 0e00 0000 7210 0000 0072  r,...r....r....r
-00001340: 2a00 0000 da0b 636c 6173 736d 6574 686f  *.....classmetho
-00001350: 6472 3700 0000 723d 0000 0072 3e00 0000  dr7...r=...r>...
-00001360: 7204 0000 0072 4800 0000 725b 0000 0072  r....rH...r[...r
-00001370: 7300 0000 7217 0000 0072 1700 0000 7217  s...r....r....r.
-00001380: 0000 0072 1f00 0000 720a 0000 0012 0000  ...r....r.......
-00001390: 0073 1e00 0000 0a02 0402 0801 0c01 0c01  .s..............
-000013a0: 0c02 0201 0c26 0805 080e 080b 080e 0001  .....&..........
-000013b0: 00ff 0a1b 720a 0000 00da 0562 6c61 636b  ....r......black
-000013c0: 720d 0000 0063 0400 0000 0000 0000 0000  r....c..........
-000013d0: 0000 0700 0000 0700 0000 4300 0000 738e  ..........C...s.
-000013e0: 0000 0074 007c 017c 0283 025c 027d 047d  ...t.|.|...\.}.}
-000013f0: 0564 0174 01a0 0274 01a0 037c 05a1 01a1  .d.t...t...|....
-00001400: 0114 007d 067c 006a 047c 0474 016a 051b  ...}.|.j.|.t.j..
-00001410: 007c 0674 0664 028d 0301 007c 0372 507c  .|.t.d.....|.rP|
-00001420: 006a 077c 0364 0364 0464 0564 0664 078d  .j.|.d.d.d.d.d..
-00001430: 0501 007c 006a 0867 0064 08a2 0164 0964  ...|.j.g.d...d.d
-00001440: 0a64 0564 0664 078d 0501 007c 00a0 0964  .d.d.d.....|...d
-00001450: 0364 0b67 02a1 0101 007c 00a0 0a64 0ca1  .d.g.....|...d..
-00001460: 0101 007c 00a0 0b64 0da1 0101 0064 0053  ...|...d.....d.S
-00001470: 0029 0e4e e914 0000 00a9 01da 0563 6f6c  .).N.........col
-00001480: 6f72 e938 ffff ffe9 c800 0000 e700 0000  or.8............
-00001490: 0000 00e0 3ffa 022d 2da9 02da 026c 77da  ....?..--....lw.
-000014a0: 096c 696e 6573 7479 6c65 2905 7201 0000  .linestyle).r...
-000014b0: 0067 14ae 47e1 7a14 48c0 6785 eb51 b81e  .g..G.z.H.g..Q..
-000014c0: 1558 c067 0000 0000 0010 62c0 6766 6666  .X.g......b.gfff
-000014d0: 6666 1668 c0e7 0000 0000 0000 0000 e700  ff.h............
-000014e0: 0000 0000 00f0 3fe9 0a00 0000 7a0e 4d61  ......?.....z.Ma
-000014f0: 676e 6974 7564 6520 2864 6229 7a12 4672  gnitude (db)z.Fr
-00001500: 6571 7565 6e63 7920 7265 7370 6f6e 7365  equency response
-00001510: 290c 7205 0000 0072 3100 0000 da05 6c6f  ).r....r1.....lo
-00001520: 6731 3072 3000 0000 7273 0000 00da 0270  g10r0...rs.....p
-00001530: 69da 0543 4f4c 4f52 da06 766c 696e 6573  i..COLOR..vlines
-00001540: da06 686c 696e 6573 da08 7365 745f 796c  ..hlines..set_yl
-00001550: 696d da0a 7365 745f 796c 6162 656c da09  im..set_ylabel..
-00001560: 7365 745f 7469 746c 6529 07da 0261 78da  set_title)...ax.
-00001570: 0162 da01 61da 0f64 6573 6972 6564 5f6e  .b..a..desired_n
-00001580: 7971 7569 7374 da01 77da 0168 5a04 685f  yquist..w..hZ.h_
-00001590: 6442 7217 0000 0072 1700 0000 721f 0000  dBr....r....r...
-000015a0: 0072 6700 0000 a400 0000 7316 0000 0000  .rg.......s.....
-000015b0: 010e 0114 0216 0204 0114 0104 010e ff06  ................
-000015c0: 040e 020a 0172 6700 0000 6305 0000 0000  .....rg...c.....
-000015d0: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
-000015e0: 0000 0073 de00 0000 7400 7c01 7c02 8302  ...s....t.|.|...
-000015f0: 5c02 7d05 7d06 7401 a002 7401 a003 7c06  \.}.}.t...t...|.
-00001600: 6a04 7c06 6a05 a102 a101 7d07 7c07 7c05  j.|.j.....}.|.|.
-00001610: 7c04 1400 1700 7401 6a06 6401 1b00 1700  |.....t.j.d.....
-00001620: 7401 6a06 1600 7401 6a06 6401 1b00 1800  t.j...t.j.d.....
-00001630: 7d07 7c00 6a07 7c05 7401 6a06 1b00 7c07  }.|.j.|.t.j...|.
-00001640: 7408 6402 8d03 0100 7c00 a009 740a 740a  t.d.....|...t.t.
-00001650: 7c07 8301 7401 6a06 0b00 8302 740b 740b  |...t.j.....t.t.
-00001660: 7c07 8301 7401 6a06 8302 6702 a101 0100  |...t.j...g.....
-00001670: 7c03 72b2 7c00 a00c a100 7d08 7c00 6a0d  |.r.|.....}.|.j.
-00001680: 7c03 6403 6404 6405 6406 6407 8d05 0100  |.d.d.d.d.d.....
-00001690: 7c00 6a09 7c08 8e00 0100 7c00 6a0e 6408  |.j.|.....|.j.d.
-000016a0: 6409 640a 6405 6406 6407 8d05 0100 7c00  d.d.d.d.d.....|.
-000016b0: a00f 640b a101 0100 7c00 a010 640c a101  ..d.....|...d...
-000016c0: 0100 6400 5300 290d 4e72 0800 0000 727d  ..d.S.).Nr....r}
-000016d0: 0000 0072 7f00 0000 7280 0000 0072 8100  ...r....r....r..
-000016e0: 0000 7282 0000 0072 8300 0000 7201 0000  ..r....r....r...
-000016f0: 0072 8700 0000 7286 0000 007a 0f50 6861  .r....r....z.Pha
-00001700: 7365 2028 7261 6469 616e 7329 7a27 4e6f  se (radians)z'No
-00001710: 726d 616c 697a 6564 2046 7265 7175 656e  rmalized Frequen
-00001720: 6379 2028 7824 5c70 6924 7261 642f 7361  cy (x$\pi$rad/sa
-00001730: 6d70 6c65 2929 1172 0500 0000 7231 0000  mple)).r....r1..
-00001740: 00da 0675 6e77 7261 70da 0761 7263 7461  ...unwrap..arcta
-00001750: 6e32 da04 696d 6167 da04 7265 616c 728a  n2..imag..realr.
-00001760: 0000 0072 7300 0000 728b 0000 0072 8e00  ...rs...r....r..
-00001770: 0000 da03 6d69 6eda 036d 6178 da08 6765  ....min..max..ge
-00001780: 745f 796c 696d 728c 0000 0072 8d00 0000  t_ylimr....r....
-00001790: 728f 0000 00da 0a73 6574 5f78 6c61 6265  r......set_xlabe
-000017a0: 6c29 0972 9100 0000 7292 0000 0072 9300  l).r....r....r..
-000017b0: 0000 7294 0000 0072 5e00 0000 7295 0000  ..r....r^...r...
-000017c0: 0072 9600 0000 5a07 685f 7068 6173 65da  .r....Z.h_phase.
-000017d0: 0479 6c69 6d72 1700 0000 7217 0000 0072  .ylimr....r....r
-000017e0: 1f00 0000 7268 0000 00b6 0000 0073 1800  ....rh.......s..
-000017f0: 0000 0001 0e01 1601 2602 1601 2802 0401  ........&...(...
-00001800: 0801 1401 0a01 1402 0a01 7268 0000 0072  ..........rh...r
-00001810: 8600 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00001820: 0009 0000 0008 0000 0043 0000 0073 d000  .........C...s..
-00001830: 0000 7400 7c02 7401 8302 7214 7402 7c01  ..t.|.t...r.t.|.
-00001840: 8301 7d04 6e04 6401 7d04 7403 a004 6402  ..}.n.d.}.t...d.
-00001850: 7c04 a102 7d05 6403 7c05 6404 3c00 7403  |...}.d.|.d.<.t.
-00001860: a005 6404 7c04 7c04 a103 7d06 7406 7c01  ..d.|.|...}.t.|.
-00001870: 7c02 7c05 8303 7d07 7c00 6a07 7c06 7c07  |.|...}.|.j.|.|.
-00001880: 7408 6405 8d03 0100 7c00 6a09 6406 6407  t.d.....|.j.d.d.
-00001890: 6408 7403 a00a 7c07 a101 6409 9b04 640a  d.t...|...d...d.
-000018a0: 7c03 640b 9b04 640c 9d05 640d 7c00 6a0b  |.d...d...d.|.j.
-000018b0: 640e 8d05 0100 7c00 a00c a100 7d08 7c00  d.....|.....}.|.
-000018c0: 6a0d 7c03 640f 1700 6410 6411 640f 6412  j.|.d...d.d.d.d.
-000018d0: 6413 8d05 0100 7c00 6a0e 7c08 8e00 0100  d.....|.j.|.....
-000018e0: 7c00 a00f 6414 a101 0100 7c00 a010 6415  |...d.....|...d.
-000018f0: a101 0100 7c00 a011 6416 a101 0100 6400  ....|...d.....d.
-00001900: 5300 2917 4ee9 6400 0000 7286 0000 0072  S.).N.d...r....r
-00001910: 8700 0000 7201 0000 0072 7d00 0000 67b8  ....r....r}...g.
-00001920: 1e85 eb51 b8ee 3f67 9a99 9999 9999 e93f  ...Q..?g.......?
-00001930: 7a04 7375 6d3d 7a03 2e32 667a 090a 6465  z.sum=z..2fz..de
-00001940: 6c61 7920 3d20 da01 677a 0820 7361 6d70  lay = ..gz. samp
-00001950: 6c65 7372 6200 0000 2902 da13 686f 7269  lesrb...)...hori
-00001960: 7a6f 6e74 616c 616c 6967 6e6d 656e 74da  zontalalignment.
-00001970: 0974 7261 6e73 666f 726d 7281 0000 0072  .transformr....r
-00001980: 4400 0000 7208 0000 0072 8200 0000 7283  D...r....r....r.
-00001990: 0000 00da 0941 6d70 6c69 7475 6465 fa0b  .....Amplitude..
-000019a0: 6e20 2873 616d 706c 6573 297a 1049 6d70  n (samples)z.Imp
-000019b0: 756c 7365 2072 6573 706f 6e73 6529 12da  ulse response)..
-000019c0: 0a69 7369 6e73 7461 6e63 6572 2c00 0000  .isinstancer,...
-000019d0: 722e 0000 0072 3100 0000 da06 7265 7065  r....r1.....repe
-000019e0: 6174 da08 6c69 6e73 7061 6365 7206 0000  at..linspacer...
-000019f0: 0072 7300 0000 728b 0000 00da 0474 6578  .rs...r......tex
-00001a00: 7472 3200 0000 da09 7472 616e 7341 7865  tr2.....transAxe
-00001a10: 7372 9d00 0000 728c 0000 0072 8e00 0000  sr....r....r....
-00001a20: 728f 0000 0072 9e00 0000 7290 0000 0029  r....r....r....)
-00001a30: 0972 9100 0000 7292 0000 0072 9300 0000  .r....r....r....
-00001a40: 725e 0000 00da 026c 62da 0769 6d70 756c  r^.....lb..impul
-00001a50: 7365 721c 0000 00da 0872 6573 706f 6e73  ser......respons
-00001a60: 6572 9f00 0000 7217 0000 0072 1700 0000  er....r....r....
-00001a70: 721f 0000 0072 6900 0000 c800 0000 732a  r....ri.......s*
-00001a80: 0000 0000 020a 010a 0304 020c 0108 010e  ................
-00001a90: 020c 0210 0104 0102 0102 011a 0102 0104  ................
-00001aa0: fb06 0808 0218 010a 030a 010a 0172 6900  .............ri.
-00001ab0: 0000 6304 0000 0000 0000 0000 0000 0009  ..c.............
-00001ac0: 0000 0007 0000 0043 0000 0073 bc00 0000  .......C...s....
-00001ad0: 7400 7c02 7401 8302 7214 7402 7c01 8301  t.|.t...r.t.|...
-00001ae0: 7d04 6e04 6401 7d04 7403 a004 6402 7c04  }.n.d.}.t...d.|.
-00001af0: a102 7d05 6403 7c05 6404 3c00 7403 a005  ..}.d.|.d.<.t...
-00001b00: 6404 7c04 7c04 a103 7d06 7406 7c01 7c02  d.|.|...}.t.|.|.
-00001b10: 7c05 8303 7d07 7403 a007 7c07 a101 7d08  |...}.t...|...}.
-00001b20: 7c00 6a08 7c06 7c08 7409 6405 8d03 0100  |.j.|.|.t.d.....
-00001b30: 7c00 6a0a 7c03 6406 1700 6407 6408 6406  |.j.|.d...d.d.d.
-00001b40: 6409 640a 8d05 0100 7c00 a00b 740c 740c  d.d.....|...t.t.
-00001b50: 7c08 8301 640b 8302 740d 740d 7c08 8301  |...d...t.t.|...
-00001b60: 640c 8302 6702 a101 0100 7c00 a00e 640d  d...g.....|...d.
-00001b70: a101 0100 7c00 a00f 640e a101 0100 7c00  ....|...d.....|.
-00001b80: a010 640f a101 0100 6400 5300 2910 4e72  ..d.....d.S.).Nr
-00001b90: a000 0000 7286 0000 0072 8700 0000 7201  ....r....r....r.
-00001ba0: 0000 0072 7d00 0000 7281 0000 0072 4400  ...r}...r....rD.
-00001bb0: 0000 7208 0000 0072 8200 0000 7283 0000  ..r....r....r...
-00001bc0: 0067 3333 3333 3333 c3bf 6766 6666 6666  .g333333..gfffff
-00001bd0: 66f2 3f72 a400 0000 72a5 0000 007a 0d53  f.?r....r....z.S
-00001be0: 7465 7020 7265 7370 6f6e 7365 2911 72a6  tep response).r.
-00001bf0: 0000 0072 2c00 0000 722e 0000 0072 3100  ...r,...r....r1.
-00001c00: 0000 72a7 0000 0072 a800 0000 7206 0000  ..r....r....r...
-00001c10: 00da 0663 756d 7375 6d72 7300 0000 728b  ...cumsumrs...r.
-00001c20: 0000 0072 8c00 0000 728e 0000 0072 9b00  ...r....r....r..
-00001c30: 0000 729c 0000 0072 8f00 0000 729e 0000  ..r....r....r...
-00001c40: 0072 9000 0000 2909 7291 0000 0072 9200  .r....).r....r..
-00001c50: 0000 7293 0000 0072 5e00 0000 72ab 0000  ..r....r^...r...
-00001c60: 0072 ac00 0000 721c 0000 0072 ad00 0000  .r....r....r....
-00001c70: da04 7374 6570 7217 0000 0072 1700 0000  ..stepr....r....
-00001c80: 721f 0000 0072 6a00 0000 ea00 0000 731c  r....rj.......s.
-00001c90: 0000 0000 020a 010a 0304 020c 0108 010e  ................
-00001ca0: 020c 010a 0210 0218 0122 020a 010a 0172  .........".....r
-00001cb0: 6a00 0000 2902 720d 0000 004e 2903 720d  j...).r....N).r.
-00001cc0: 0000 004e 7201 0000 0029 0272 0d00 0000  ...Nr....).r....
-00001cd0: 7286 0000 0029 0272 0d00 0000 7201 0000  r....).r....r...
-00001ce0: 0029 1972 7700 0000 7224 0000 00da 0770  .).rw...r$.....p
-00001cf0: 6174 686c 6962 7202 0000 00da 0b64 6174  athlibr......dat
-00001d00: 6163 6c61 7373 6573 7203 0000 00da 056e  aclassesr......n
-00001d10: 756d 7079 7231 0000 00da 116d 6174 706c  umpyr1.....matpl
-00001d20: 6f74 6c69 622e 7079 706c 6f74 da06 7079  otlib.pyplot..py
-00001d30: 706c 6f74 7265 0000 00da 0c73 6369 7079  plotre.....scipy
-00001d40: 2e73 6967 6e61 6c72 0400 0000 7205 0000  .signalr....r...
-00001d50: 0072 0600 0000 da1d 6f62 7370 792e 636f  .r......obspy.co
-00001d60: 7265 2e69 6e76 656e 746f 7279 2e72 6573  re.inventory.res
-00001d70: 706f 6e73 6572 0700 0000 da06 6c6f 6767  ponser......logg
-00001d80: 6572 7209 0000 0072 0a00 0000 728b 0000  err....r....r...
-00001d90: 0072 6700 0000 7268 0000 0072 6900 0000  .rg...rh...ri...
-00001da0: 726a 0000 0072 1700 0000 7217 0000 0072  rj...r....r....r
-00001db0: 1700 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
-00001dc0: 6c65 3e02 0000 0073 2200 0000 0402 0801  le>....s".......
-00001dd0: 0c01 0c02 0801 0c01 1401 0c02 0c02 0603  ................
-00001de0: 0201 107f 000d 0405 0a12 0a12 0a22       ............."
+00000dc0: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
+00000dd0: 0000 1100 0000 4300 0000 733a 0000 0074  ......C...s:...t
+00000de0: 007c 0264 0164 0264 0364 0464 0364 0464  .|.d.d.d.d.d.d.d
+00000df0: 057c 006a 017c 006a 027c 017c 006a 037c  .|.j.|.j.|.|.j.|
+00000e00: 006a 047c 006a 047c 011b 007c 006a 047c  .j.|.j.|...|.j.|
+00000e10: 011b 0064 068d 0f53 0029 077a 320a 2020  ...d...S.).z2.  
+00000e20: 2020 2020 2020 5265 7475 726e 2061 6e20        Return an 
+00000e30: 6f62 7370 7920 4649 5252 6573 706f 6e73  obspy FIRRespons
+00000e40: 6553 7461 6765 0a20 2020 2020 2020 2072  eStage.        r
+00000e50: 0d00 0000 7201 0000 00da 0663 6f75 6e74  ....r......count
+00000e60: 737a 0e64 6967 6974 616c 2063 6f75 6e74  sz.digital count
+00000e70: 7372 4200 0000 290f da15 7374 6167 655f  srB...)...stage_
+00000e80: 7365 7175 656e 6365 5f6e 756d 6265 72da  sequence_number.
+00000e90: 0a73 7461 6765 5f67 6169 6eda 1473 7461  .stage_gain..sta
+00000ea0: 6765 5f67 6169 6e5f 6672 6571 7565 6e63  ge_gain_frequenc
+00000eb0: 79da 0b69 6e70 7574 5f75 6e69 7473 da17  y..input_units..
+00000ec0: 696e 7075 745f 756e 6974 735f 6465 7363  input_units_desc
+00000ed0: 7269 7074 696f 6eda 0c6f 7574 7075 745f  ription..output_
+00000ee0: 756e 6974 73da 186f 7574 7075 745f 756e  units..output_un
+00000ef0: 6974 735f 6465 7363 7269 7074 696f 6eda  its_description.
+00000f00: 0873 796d 6d65 7472 7972 1000 0000 da0c  .symmetryr......
+00000f10: 636f 6566 6669 6369 656e 7473 da1c 6465  coefficients..de
+00000f20: 6369 6d61 7469 6f6e 5f69 6e70 7574 5f73  cimation_input_s
+00000f30: 616d 706c 655f 7261 7465 da11 6465 6369  ample_rate..deci
+00000f40: 6d61 7469 6f6e 5f66 6163 746f 72da 1164  mation_factor..d
+00000f50: 6563 696d 6174 696f 6e5f 6f66 6673 6574  ecimation_offset
+00000f60: da10 6465 6369 6d61 7469 6f6e 5f64 656c  ..decimation_del
+00000f70: 6179 da15 6465 6369 6d61 7469 6f6e 5f63  ay..decimation_c
+00000f80: 6f72 7265 6374 696f 6e29 0572 0700 0000  orrection).r....
+00000f90: 7210 0000 0072 0b00 0000 720e 0000 0072  r....r....r....r
+00000fa0: 0c00 0000 2903 723c 0000 00da 0d73 616d  ....).r<.....sam
+00000fb0: 706c 696e 675f 7261 7465 724a 0000 0072  pling_raterJ...r
+00000fc0: 1700 0000 7217 0000 0072 1f00 0000 da08  ....r....r......
+00000fd0: 746f 5f6f 6273 7079 6e00 0000 7322 0000  to_obspyn...s"..
+00000fe0: 0000 0402 0102 0102 0102 0102 0102 0102  ................
+00000ff0: 0102 0102 0104 0104 0102 0104 0104 0108  ................
+00001000: 0108 f17a 1246 4952 4669 6c74 6572 2e74  ...z.FIRFilter.t
+00001010: 6f5f 6f62 7370 7946 4e63 0300 0000 0000  o_obspyFNc......
+00001020: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+00001030: 0000 73b0 0000 0074 006a 0164 0164 0164  ..s....t.j.d.d.d
+00001040: 0264 038d 035c 027d 035c 025c 027d 047d  .d...\.}.\.\.}.}
+00001050: 055c 027d 067d 0774 027c 047c 006a 0364  .\.}.}.t.|.|.j.d
+00001060: 0464 047c 006a 041b 0083 0401 0074 057c  .d.|.j.......t.|
+00001070: 067c 006a 0364 0464 047c 006a 041b 007c  .|.j.d.d.|.j...|
+00001080: 006a 0683 0501 0074 077c 057c 006a 0364  .j.....t.|.|.j.d
+00001090: 047c 006a 0664 058d 0401 0074 087c 077c  .|.j.d.....t.|.|
+000010a0: 006a 0364 047c 006a 0664 058d 0401 007c  .j.d.|.j.d.....|
+000010b0: 036a 0964 0664 0764 0864 0964 0a64 0b64  .j.d.d.d.d.d.d.d
+000010c0: 0c8d 0601 007c 0172 9a74 00a0 0aa1 0001  .....|.r.t......
+000010d0: 007c 0264 0d75 0172 ac74 00a0 0b7c 02a1  .|.d.u.r.t...|..
+000010e0: 0101 007c 0353 0029 0e7a 2850 6c6f 7420  ...|.S.).z(Plot 
+000010f0: 4649 5220 6669 6c74 6572 2061 6e64 2069  FIR filter and i
+00001100: 6d70 6f72 7461 6e74 2070 6172 616d 6574  mportant paramet
+00001110: 6572 7372 0800 0000 2902 e908 0000 0072  ersr....)......r
+00001120: 1400 0000 2901 da07 6669 6773 697a 6572  ....)...figsizer
+00001130: 0d00 0000 2901 da05 6465 6c61 7967 9a99  ....)...delayg..
+00001140: 9999 9999 d93f 679a 9999 9999 99c9 3f67  .....?g.......?g
+00001150: ec51 b81e 85eb b13f 67ae 47e1 7a14 aeef  .Q.....?g.G.z...
+00001160: 3f67 9a99 9999 9999 b93f 6766 6666 6666  ?g.......?gfffff
+00001170: 66ee 3f29 06da 0668 7370 6163 65da 0677  f.?)...hspace..w
+00001180: 7370 6163 65da 046c 6566 74da 0572 6967  space..left..rig
+00001190: 6874 da06 626f 7474 6f6d da03 746f 704e  ht..bottom..topN
+000011a0: 290c da03 706c 74da 0873 7562 706c 6f74  )...plt..subplot
+000011b0: 73da 0a70 6c6f 745f 6672 6571 7a72 0b00  s..plot_freqzr..
+000011c0: 0000 720e 0000 00da 0b70 6c6f 745f 7068  ..r......plot_ph
+000011d0: 6173 657a 720c 0000 00da 0970 6c6f 745f  asezr......plot_
+000011e0: 696d 707a da0a 706c 6f74 5f73 7465 707a  impz..plot_stepz
+000011f0: da0f 7375 6270 6c6f 7473 5f61 646a 7573  ..subplots_adjus
+00001200: 74da 0473 686f 77da 0773 6176 6566 6967  t..show..savefig
+00001210: 2908 723c 0000 0072 6a00 0000 726b 0000  ).r<...rj...rk..
+00001220: 00da 0366 6967 da03 6178 31da 0361 7832  ...fig..ax1..ax2
+00001230: da03 6178 33da 0361 7834 7217 0000 0072  ..ax3..ax4r....r
+00001240: 1700 0000 721f 0000 00da 0470 6c6f 7484  ....r......plot.
+00001250: 0000 0073 1a00 0000 0002 2002 1601 1a01  ...s...... .....
+00001260: 1401 1402 0401 0cff 0603 0401 0801 0801  ................
+00001270: 0a02 7a0e 4649 5246 696c 7465 722e 706c  ..z.FIRFilter.pl
+00001280: 6f74 2901 5429 0172 0100 0000 2902 464e  ot).T).r....).FN
+00001290: 2913 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000012a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000012b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
+000012c0: 046c 6973 74da 0f5f 5f61 6e6e 6f74 6174  .list..__annotat
+000012d0: 696f 6e73 5f5f 720c 0000 0072 2c00 0000  ions__r....r,...
+000012e0: 720e 0000 0072 1000 0000 722a 0000 00da  r....r....r*....
+000012f0: 0b63 6c61 7373 6d65 7468 6f64 7237 0000  .classmethodr7..
+00001300: 0072 3d00 0000 723e 0000 0072 0400 0000  .r=...r>...r....
+00001310: 7248 0000 0072 5900 0000 7271 0000 0072  rH...rY...rq...r
+00001320: 1700 0000 7217 0000 0072 1700 0000 721f  ....r....r....r.
+00001330: 0000 0072 0a00 0000 1200 0000 731a 0000  ...r........s...
+00001340: 000a 0204 0208 010c 010c 010c 0202 010c  ................
+00001350: 2608 0508 0e08 0b08 0e0a 1672 0a00 0000  &..........r....
+00001360: da05 626c 6163 6b72 0d00 0000 6304 0000  ..blackr....c...
+00001370: 0000 0000 0000 0000 0007 0000 0007 0000  ................
+00001380: 0043 0000 0073 8e00 0000 7400 7c01 7c02  .C...s....t.|.|.
+00001390: 8302 5c02 7d04 7d05 6401 7401 a002 7401  ..\.}.}.d.t...t.
+000013a0: a003 7c05 a101 a101 1400 7d06 7c00 6a04  ..|.......}.|.j.
+000013b0: 7c04 7401 6a05 1b00 7c06 7406 6402 8d03  |.t.j...|.t.d...
+000013c0: 0100 7c03 7250 7c00 6a07 7c03 6403 6404  ..|.rP|.j.|.d.d.
+000013d0: 6405 6406 6407 8d05 0100 7c00 6a08 6700  d.d.d.....|.j.g.
+000013e0: 6408 a201 6409 640a 6405 6406 6407 8d05  d...d.d.d.d.d...
+000013f0: 0100 7c00 a009 6403 640b 6702 a101 0100  ..|...d.d.g.....
+00001400: 7c00 a00a 640c a101 0100 7c00 a00b 640d  |...d.....|...d.
+00001410: a101 0100 6400 5300 290e 4ee9 1400 0000  ....d.S.).N.....
+00001420: a901 da05 636f 6c6f 72e9 38ff ffff e9c8  ....color.8.....
+00001430: 0000 00e7 0000 0000 0000 e03f fa02 2d2d  ...........?..--
+00001440: a902 da02 6c77 da09 6c69 6e65 7374 796c  ....lw..linestyl
+00001450: 6529 0572 0100 0000 6714 ae47 e17a 1448  e).r....g..G.z.H
+00001460: c067 85eb 51b8 1e15 58c0 6700 0000 0000  .g..Q...X.g.....
+00001470: 1062 c067 6666 6666 6616 68c0 e700 0000  .b.gfffff.h.....
+00001480: 0000 0000 00e7 0000 0000 0000 f03f e90a  .............?..
+00001490: 0000 007a 0e4d 6167 6e69 7475 6465 2028  ...z.Magnitude (
+000014a0: 6462 297a 1246 7265 7175 656e 6379 2072  db)z.Frequency r
+000014b0: 6573 706f 6e73 6529 0c72 0500 0000 7231  esponse).r....r1
+000014c0: 0000 00da 056c 6f67 3130 7230 0000 0072  .....log10r0...r
+000014d0: 7100 0000 da02 7069 da05 434f 4c4f 52da  q.....pi..COLOR.
+000014e0: 0676 6c69 6e65 73da 0668 6c69 6e65 73da  .vlines..hlines.
+000014f0: 0873 6574 5f79 6c69 6dda 0a73 6574 5f79  .set_ylim..set_y
+00001500: 6c61 6265 6cda 0973 6574 5f74 6974 6c65  label..set_title
+00001510: 2907 da02 6178 da01 62da 0161 da0f 6465  )...ax..b..a..de
+00001520: 7369 7265 645f 6e79 7175 6973 74da 0177  sired_nyquist..w
+00001530: da01 685a 0468 5f64 4272 1700 0000 7217  ..hZ.h_dBr....r.
+00001540: 0000 0072 1f00 0000 7265 0000 009f 0000  ...r....re......
+00001550: 0073 1600 0000 0001 0e01 1402 1602 0401  .s..............
+00001560: 1401 0401 0eff 0604 0e02 0a01 7265 0000  ............re..
+00001570: 0063 0500 0000 0000 0000 0000 0000 0900  .c..............
+00001580: 0000 0700 0000 4300 0000 73de 0000 0074  ......C...s....t
+00001590: 007c 017c 0283 025c 027d 057d 0674 01a0  .|.|...\.}.}.t..
+000015a0: 0274 01a0 037c 066a 047c 066a 05a1 02a1  .t...|.j.|.j....
+000015b0: 017d 077c 077c 057c 0414 0017 0074 016a  .}.|.|.|.....t.j
+000015c0: 0664 011b 0017 0074 016a 0616 0074 016a  .d.....t.j...t.j
+000015d0: 0664 011b 0018 007d 077c 006a 077c 0574  .d.....}.|.j.|.t
+000015e0: 016a 061b 007c 0774 0864 028d 0301 007c  .j...|.t.d.....|
+000015f0: 00a0 0974 0a74 0a7c 0783 0174 016a 060b  ...t.t.|...t.j..
+00001600: 0083 0274 0b74 0b7c 0783 0174 016a 0683  ...t.t.|...t.j..
+00001610: 0267 02a1 0101 007c 0372 b27c 00a0 0ca1  .g.....|.r.|....
+00001620: 007d 087c 006a 0d7c 0364 0364 0464 0564  .}.|.j.|.d.d.d.d
+00001630: 0664 078d 0501 007c 006a 097c 088e 0001  .d.....|.j.|....
+00001640: 007c 006a 0e64 0864 0964 0a64 0564 0664  .|.j.d.d.d.d.d.d
+00001650: 078d 0501 007c 00a0 0f64 0ba1 0101 007c  .....|...d.....|
+00001660: 00a0 1064 0ca1 0101 0064 0053 0029 0d4e  ...d.....d.S.).N
+00001670: 7208 0000 0072 7b00 0000 727d 0000 0072  r....r{...r}...r
+00001680: 7e00 0000 727f 0000 0072 8000 0000 7281  ~...r....r....r.
+00001690: 0000 0072 0100 0000 7285 0000 0072 8400  ...r....r....r..
+000016a0: 0000 7a0f 5068 6173 6520 2872 6164 6961  ..z.Phase (radia
+000016b0: 6e73 297a 274e 6f72 6d61 6c69 7a65 6420  ns)z'Normalized 
+000016c0: 4672 6571 7565 6e63 7920 2878 245c 7069  Frequency (x$\pi
+000016d0: 2472 6164 2f73 616d 706c 6529 2911 7205  $rad/sample)).r.
+000016e0: 0000 0072 3100 0000 da06 756e 7772 6170  ...r1.....unwrap
+000016f0: da07 6172 6374 616e 32da 0469 6d61 67da  ..arctan2..imag.
+00001700: 0472 6561 6c72 8800 0000 7271 0000 0072  .realr....rq...r
+00001710: 8900 0000 728c 0000 00da 036d 696e da03  ....r......min..
+00001720: 6d61 78da 0867 6574 5f79 6c69 6d72 8a00  max..get_ylimr..
+00001730: 0000 728b 0000 0072 8d00 0000 da0a 7365  ..r....r......se
+00001740: 745f 786c 6162 656c 2909 728f 0000 0072  t_xlabel).r....r
+00001750: 9000 0000 7291 0000 0072 9200 0000 725c  ....r....r....r\
+00001760: 0000 0072 9300 0000 7294 0000 005a 0768  ...r....r....Z.h
+00001770: 5f70 6861 7365 da04 796c 696d 7217 0000  _phase..ylimr...
+00001780: 0072 1700 0000 721f 0000 0072 6600 0000  .r....r....rf...
+00001790: b100 0000 7318 0000 0000 010e 0116 0126  ....s..........&
+000017a0: 0216 0128 0204 0108 0114 010a 0114 020a  ...(............
+000017b0: 0172 6600 0000 7284 0000 0063 0400 0000  .rf...r....c....
+000017c0: 0000 0000 0000 0000 0900 0000 0800 0000  ................
+000017d0: 4300 0000 73d0 0000 0074 007c 0274 0183  C...s....t.|.t..
+000017e0: 0272 1474 027c 0183 017d 046e 0464 017d  .r.t.|...}.n.d.}
+000017f0: 0474 03a0 0464 027c 04a1 027d 0564 037c  .t...d.|...}.d.|
+00001800: 0564 043c 0074 03a0 0564 047c 047c 04a1  .d.<.t...d.|.|..
+00001810: 037d 0674 067c 017c 027c 0583 037d 077c  .}.t.|.|.|...}.|
+00001820: 006a 077c 067c 0774 0864 058d 0301 007c  .j.|.|.t.d.....|
+00001830: 006a 0964 0664 0764 0874 03a0 0a7c 07a1  .j.d.d.d.t...|..
+00001840: 0164 099b 0464 0a7c 0364 0b9b 0464 0c9d  .d...d.|.d...d..
+00001850: 0564 0d7c 006a 0b64 0e8d 0501 007c 00a0  .d.|.j.d.....|..
+00001860: 0ca1 007d 087c 006a 0d7c 0364 0f17 0064  ...}.|.j.|.d...d
+00001870: 1064 1164 0f64 1264 138d 0501 007c 006a  .d.d.d.d.....|.j
+00001880: 0e7c 088e 0001 007c 00a0 0f64 14a1 0101  .|.....|...d....
+00001890: 007c 00a0 1064 15a1 0101 007c 00a0 1164  .|...d.....|...d
+000018a0: 16a1 0101 0064 0053 0029 174e e964 0000  .....d.S.).N.d..
+000018b0: 0072 8400 0000 7285 0000 0072 0100 0000  .r....r....r....
+000018c0: 727b 0000 0067 b81e 85eb 51b8 ee3f 679a  r{...g....Q..?g.
+000018d0: 9999 9999 99e9 3f7a 0473 756d 3d7a 032e  ......?z.sum=z..
+000018e0: 3266 7a09 0a64 656c 6179 203d 20da 0167  2fz..delay = ..g
+000018f0: 7a08 2073 616d 706c 6573 7260 0000 0029  z. samplesr`...)
+00001900: 02da 1368 6f72 697a 6f6e 7461 6c61 6c69  ...horizontalali
+00001910: 676e 6d65 6e74 da09 7472 616e 7366 6f72  gnment..transfor
+00001920: 6d72 7f00 0000 7244 0000 0072 0800 0000  mr....rD...r....
+00001930: 7280 0000 0072 8100 0000 da09 416d 706c  r....r......Ampl
+00001940: 6974 7564 65fa 0b6e 2028 7361 6d70 6c65  itude..n (sample
+00001950: 7329 7a10 496d 7075 6c73 6520 7265 7370  s)z.Impulse resp
+00001960: 6f6e 7365 2912 da0a 6973 696e 7374 616e  onse)...isinstan
+00001970: 6365 722c 0000 0072 2e00 0000 7231 0000  cer,...r....r1..
+00001980: 00da 0672 6570 6561 74da 086c 696e 7370  ...repeat..linsp
+00001990: 6163 6572 0600 0000 7271 0000 0072 8900  acer....rq...r..
+000019a0: 0000 da04 7465 7874 7232 0000 00da 0974  ....textr2.....t
+000019b0: 7261 6e73 4178 6573 729b 0000 0072 8a00  ransAxesr....r..
+000019c0: 0000 728c 0000 0072 8d00 0000 729c 0000  ..r....r....r...
+000019d0: 0072 8e00 0000 2909 728f 0000 0072 9000  .r....).r....r..
+000019e0: 0000 7291 0000 0072 5c00 0000 da02 6c62  ..r....r\.....lb
+000019f0: da07 696d 7075 6c73 6572 1c00 0000 da08  ..impulser......
+00001a00: 7265 7370 6f6e 7365 729d 0000 0072 1700  responser....r..
+00001a10: 0000 7217 0000 0072 1f00 0000 7267 0000  ..r....r....rg..
+00001a20: 00c3 0000 0073 2a00 0000 0002 0a01 0a03  .....s*.........
+00001a30: 0402 0c01 0801 0e02 0c02 1001 0401 0201  ................
+00001a40: 0201 1a01 0201 04fb 0608 0802 1801 0a03  ................
+00001a50: 0a01 0a01 7267 0000 0063 0400 0000 0000  ....rg...c......
+00001a60: 0000 0000 0000 0900 0000 0700 0000 4300  ..............C.
+00001a70: 0000 73bc 0000 0074 007c 0274 0183 0272  ..s....t.|.t...r
+00001a80: 1474 027c 0183 017d 046e 0464 017d 0474  .t.|...}.n.d.}.t
+00001a90: 03a0 0464 027c 04a1 027d 0564 037c 0564  ...d.|...}.d.|.d
+00001aa0: 043c 0074 03a0 0564 047c 047c 04a1 037d  .<.t...d.|.|...}
+00001ab0: 0674 067c 017c 027c 0583 037d 0774 03a0  .t.|.|.|...}.t..
+00001ac0: 077c 07a1 017d 087c 006a 087c 067c 0874  .|...}.|.j.|.|.t
+00001ad0: 0964 058d 0301 007c 006a 0a7c 0364 0617  .d.....|.j.|.d..
+00001ae0: 0064 0764 0864 0664 0964 0a8d 0501 007c  .d.d.d.d.d.....|
+00001af0: 00a0 0b74 0c74 0c7c 0883 0164 0b83 0274  ...t.t.|...d...t
+00001b00: 0d74 0d7c 0883 0164 0c83 0267 02a1 0101  .t.|...d...g....
+00001b10: 007c 00a0 0e64 0da1 0101 007c 00a0 0f64  .|...d.....|...d
+00001b20: 0ea1 0101 007c 00a0 1064 0fa1 0101 0064  .....|...d.....d
+00001b30: 0053 0029 104e 729e 0000 0072 8400 0000  .S.).Nr....r....
+00001b40: 7285 0000 0072 0100 0000 727b 0000 0072  r....r....r{...r
+00001b50: 7f00 0000 7244 0000 0072 0800 0000 7280  ....rD...r....r.
+00001b60: 0000 0072 8100 0000 6733 3333 3333 33c3  ...r....g333333.
+00001b70: bf67 6666 6666 6666 f23f 72a2 0000 0072  .gffffff.?r....r
+00001b80: a300 0000 7a0d 5374 6570 2072 6573 706f  ....z.Step respo
+00001b90: 6e73 6529 1172 a400 0000 722c 0000 0072  nse).r....r,...r
+00001ba0: 2e00 0000 7231 0000 0072 a500 0000 72a6  ....r1...r....r.
+00001bb0: 0000 0072 0600 0000 da06 6375 6d73 756d  ...r......cumsum
+00001bc0: 7271 0000 0072 8900 0000 728a 0000 0072  rq...r....r....r
+00001bd0: 8c00 0000 7299 0000 0072 9a00 0000 728d  ....r....r....r.
+00001be0: 0000 0072 9c00 0000 728e 0000 0029 0972  ...r....r....).r
+00001bf0: 8f00 0000 7290 0000 0072 9100 0000 725c  ....r....r....r\
+00001c00: 0000 0072 a900 0000 72aa 0000 0072 1c00  ...r....r....r..
+00001c10: 0000 72ab 0000 00da 0473 7465 7072 1700  ..r......stepr..
+00001c20: 0000 7217 0000 0072 1f00 0000 7268 0000  ..r....r....rh..
+00001c30: 00e5 0000 0073 1c00 0000 0002 0a01 0a03  .....s..........
+00001c40: 0402 0c01 0801 0e02 0c01 0a02 1002 1801  ................
+00001c50: 2202 0a01 0a01 7268 0000 0029 0272 0d00  ".....rh...).r..
+00001c60: 0000 4e29 0372 0d00 0000 4e72 0100 0000  ..N).r....Nr....
+00001c70: 2902 720d 0000 0072 8400 0000 2902 720d  ).r....r....).r.
+00001c80: 0000 0072 0100 0000 2919 7275 0000 0072  ...r....).ru...r
+00001c90: 2400 0000 da07 7061 7468 6c69 6272 0200  $.....pathlibr..
+00001ca0: 0000 da0b 6461 7461 636c 6173 7365 7372  ....dataclassesr
+00001cb0: 0300 0000 da05 6e75 6d70 7972 3100 0000  ......numpyr1...
+00001cc0: da11 6d61 7470 6c6f 746c 6962 2e70 7970  ..matplotlib.pyp
+00001cd0: 6c6f 74da 0670 7970 6c6f 7472 6300 0000  lot..pyplotrc...
+00001ce0: da0c 7363 6970 792e 7369 676e 616c 7204  ..scipy.signalr.
+00001cf0: 0000 0072 0500 0000 7206 0000 00da 1d6f  ...r....r......o
+00001d00: 6273 7079 2e63 6f72 652e 696e 7665 6e74  bspy.core.invent
+00001d10: 6f72 792e 7265 7370 6f6e 7365 7207 0000  ory.responser...
+00001d20: 00da 066c 6f67 6765 7272 0900 0000 720a  ...loggerr....r.
+00001d30: 0000 0072 8900 0000 7265 0000 0072 6600  ...r....re...rf.
+00001d40: 0000 7267 0000 0072 6800 0000 7217 0000  ..rg...rh...r...
+00001d50: 0072 1700 0000 7217 0000 0072 1f00 0000  .r....r....r....
+00001d60: da08 3c6d 6f64 756c 653e 0200 0000 7322  ..<module>....s"
+00001d70: 0000 0004 0208 010c 010c 0208 010c 0114  ................
+00001d80: 010c 020c 0206 0302 0110 7f00 0804 050a  ................
+00001d90: 120a 120a 22                             ...."
```

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc` & `tiskitpy-0.5rc1/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/decimator.py` & `tiskitpy-0.5rc1/tiskitpy/decimate/decimator.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 #       instruments' response information
 #       scipy doesn't seem to have a minimum phase FIR method: could use
 #       Scherbaum method to convert zero phase to minimum phase
 
 # import obspy
 # from obspy.clients.filesystem import sds
 import time
-# from copy import deepcopy
 from dataclasses import dataclass
 from inspect import getfile, currentframe
 from pathlib import Path
 import warnings
 import fnmatch
-# import logging
 
 from numpy import prod
 from obspy.core.stream import Stream, Trace
 from obspy.core.trace import Stats
 from obspy.core.inventory import (FIRResponseStage,
                                   CoefficientsTypeResponseStage)
 
@@ -47,20 +45,14 @@
         decimates (list): list of decimation factorst to use (integers between
                         2 and 7, will be applied in order)
         verbose (bool): Be chatty
     """
     decimates: list
     verbose: bool = False
 
-    # def __post_init__(self):
-    #     if self.verbose is True:
-    #         logger.setLevel(logging.INFO)
-    #     else:
-    #         logger.setLevel(logging.WARN)
-
     @property
     def decimation_factor(self):
         """Total decimation (product of `decimates`)"""
         return prod(self.decimates)
 
     def decimate(self, data, keep_dtype=True):
         """
@@ -76,31 +68,27 @@
             return self._run_stream(data)
         if isinstance(data, Trace):
             return self._run_trace(data)
         else:
             raise TypeError("data is not a Stream or Trace")
 
     def update_inventory(
-        self, inv, st=None, normalize_firs=False, quiet=False,
-        inv_force_overwrite=False
+        self, inv, st=None, normalize_firs=False, quiet=False
     ):
         """
         Update inventory for channels found in stream
 
         Args:
             inv (:class:`obspy.core.events.inventory.Inventory`): inventory
             st (:class:`obspy.core.stream.Stream`): data stream (used to
                 determine net/sta/chan/loc codes).  If None, will update
                 every channel
             normalize_firs (bool): normalize FIR channels that aren't already
-            inv_force_overwrite (bool): If the target channel seed_id already
-                exists (and it's not the source channel seed_id), overwrite it
 
-        Returns:
-            obspy inventory with new channels
+        : returns: obspy inventory with new channels
         """
         inv = inv.copy()  # Don't overwrite input inventory
         if st is not None:
             stats_list = [tr.stats for tr in st]
         else:
             stats_list = [
                 Stats(
@@ -120,50 +108,22 @@
             new_cha = self._duplicate_channel(
                 inv,
                 network=stats.network,
                 station=stats.station,
                 location=stats.location,
                 channel=stats.channel,
                 normalize_firs=normalize_firs,
-                insert_in_inv=False 
             )
             if not new_cha.sample_rate == stats.sampling_rate:
                 raise ValueError(
-                    "data and metadata sampling rates are different!")
+                    "data and metadata sampling rates are " "different!"
+                )
             self._modify_chan(
                 new_cha, net=stats.network, sta=stats.station, quiet=quiet
             )
-            seed_id = f'{stats.network}.{stats.station}.{stats.location}{new_cha.code}'
-            if new_cha.code == stats.channel:
-                # Do not overwrite mother channel
-                logger.error('New channel has same code as source channel '
-                             f'({seed_id}), rejected!')
-                continue
-            elif len(inv.select(network=stats.network, station=stats.station,
-                                location=stats.location, channel=new_cha.code)) > 0:
-                boilerplate = 'New channel has same seed_id as an existing channel'
-                if inv_force_overwrite is True:
-                    logger.warning(f'{boilerplate} ({seed_id}), overwriting!')
-                    inv = inv.remove(network=stats.network, station=stats.station,
-                                     location=stats.location, channel=new_cha.code)
-                else:
-                    logger.warning(f'{boilerplate} ({seed_id}), rejected!')
-                    continue
-            # Append new channel to inv
-            appended = False
-            for net in inv:
-                if not net.code == stats.network:
-                    continue
-                for sta in net:
-                    if sta.code == stats.station:
-                        sta.channels.append(new_cha)
-                        appended = True
-                        break
-            if appended is not True:
-                raise ValueError(f'Did not find a home for {seed_id}')        
         return inv
 
     def update_inventory_from_nslc(self, inv, network="*", station="*",
                                    channel="*", location="*", quiet=False,
                                    normalize_firs=False):
         """
         Update inventory based on network, station, channel and location codes
@@ -283,24 +243,24 @@
         Args:
             cha (:class:`obspy.core.inventory.channel`): original channel
             net (str): network code (just for clearer progress printout)
             sta (str): station code (just for clearer progress printout)
             normalize_firs (bool): normalizes any FIR channel that isn't
                 already
         """
-        old_seed_id = ".".join([net, sta, cha.location_code, cha.code])
-        # old_cha = cha.copy()
+        logger.info("channel modified from {} ({} sps)".format(
+              ".".join([net, sta, cha.location_code, cha.code]),
+              cha.sample_rate))
         input_sample_rate = cha.sample_rate
         self._add_instrument_response(cha, input_sample_rate)
         self._change_chan_loc(cha, input_sample_rate)
         cha.sample_rate /= self.decimation_factor
-        seed_id = ".".join([net, sta, cha.location_code, cha.code])
-        logger.info("channel modified from "
-                    f"{old_seed_id} ({input_sample_rate:g} sps) "
-                    f"to {seed_id} ({cha.sample_rate:g} sps) ")
+        logger.info("to {} ({:g} sps)".format(
+                    ".".join([net, sta, cha.location_code, cha.code]),
+                    cha.sample_rate))
 
     @staticmethod
     def _normalize_firs(cha):
         """
         Verifies &, if needed, normalizes channel's FIR or Coefficients coeffs
 
         Args:
@@ -318,15 +278,15 @@
                     )
                 else:
                     raise ValueError(
                         f"Unknown FIR coefficient symmetry: {stg.symmetry}"
                     )
                 if abs(coeff_sum - 1) > 0.01:
                     logger.info(f"DECIMATOR: Sum of FIR coeffs = "
-                                f"{coeff_sum}, normalizing")
+                                 f"{coeff_sum}, normalizing")
                     stg.coefficients = [x / coeff_sum
                                         for x in stg.coefficients]
             elif isinstance(stg, CoefficientsTypeResponseStage):
                 if sum(stg.denominator) == 0:
                     coeff_sum = sum(stg.numerator)
                     if coeff_sum == 0:
                         continue
@@ -390,25 +350,22 @@
                     new_loc_code = f"{int(new_loc_code) + 1:02d}"
                     continue
             break
         return new_cha_code, new_loc_code
 
     def _add_instrument_response(self, cha, input_sample_rate):
         """
-        Append  decimation object's instrument response to an existing
-        channel's response
+        Append  decimation object's instrument response to an existing channel's response
         """
         stage_number = cha.response.response_stages[-1].stage_sequence_number
         for d in self.decimates:
             fir_filter = FIRFilter.from_SAC(d)
             stage_number += 1
             cha.response.response_stages.append(
-                fir_filter.to_obspy(
-                    input_sample_rate, stage_number,
-                    cha.response.response_stages[-1].output_units)
+                fir_filter.to_obspy(input_sample_rate, stage_number)
             )
             input_sample_rate /= d
         try:
             cha.response.recalculate_overall_sensitivity()
         except Exception:
             i_u = cha.response.instrument_sensitivity.input_units
             if i_u.upper() == 'PA':
@@ -424,15 +381,15 @@
             raise ValueError("input stream is not an obspy Stream!")
         st = stream.copy()
         newtr = []
         for tr in st.traces:
             newtr.append(self._run_trace(tr))
         st.traces = newtr
         logger.info("New data has {} samples".format([tr.data.size
-                                                      for tr in st]))
+                                                for tr in st]))
         st.verify()
         return st
 
     def _run_trace(self, trace):
         """
         Decimate obspy Trace
         """
@@ -484,16 +441,15 @@
         delay = len(coeffs) - 1
         coeffs = coeffs[-1:0:-1] + coeffs
         return FIRFilter(coeffs, delay, 1, "")
 
     # The following is a combo of obspy's inventory, Network and Station select
     # methods, but which returns the chosen station and channel, not a copy
     def _duplicate_channel(
-        self, inv, network, station, location, channel, normalize_firs=False,
-        insert_in_inv=True
+        self, inv, network, station, location, channel, normalize_firs=False
     ):
         """
         Return Station & Channel matching network, station, location, channel
 
         Arguments:
             network (str): network code
             station (str): station code
@@ -532,10 +488,9 @@
                 "{:d} station-channels matched {}.{}.{}.{}".format(
                     len(stations), network, station, location, channel
                 )
             )
         if normalize_firs is True:
             self._normalize_firs(channels[0])
         new_cha = channels[0].copy()
-        if insert_in_inv is True:
-            stations[0].channels.append(new_cha)
+        stations[0].channels.append(new_cha)
         return new_cha
```

### Comparing `tiskitpy-0.5/tiskitpy/decimate/fir_filter.py` & `tiskitpy-0.5rc1/tiskitpy/decimate/fir_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,30 +103,25 @@
             self.coeffs = self.coeffs + self.coeffs[-2::-1]
         elif symmetry_code == "EVEN":
             self.coeffs = self.coeffs + self.coeffs[-1::-1]
         else:
             raise NameError(f"FIR symmetry = {symmetry_code} not implemented")
         return
 
-    def to_obspy(self, sampling_rate, stage_sequence_number=0,
-                 prior_output_units=False):
+    def to_obspy(self, sampling_rate, stage_sequence_number=0):
         """
         Return an obspy FIRResponseStage
         """
-        units = 'count'     # StationXML recommendation
-        if prior_output_units is not False:
-            if prior_output_units[:5].lower() == 'count':
-                units = prior_output_units
         return FIRResponseStage(
             stage_sequence_number=stage_sequence_number,
             stage_gain=1,
             stage_gain_frequency=0,
-            input_units=units,
+            input_units="counts",
             input_units_description="digital counts",
-            output_units=units,
+            output_units="counts",
             output_units_description="digital counts",
             symmetry="NONE",
             name=self.name,
             coefficients=self.coeffs,
             decimation_input_sample_rate=sampling_rate,
             decimation_factor=self.decim,
             decimation_offset=self.offset,
```

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec2` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec2`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec3` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec3`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec4` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec4`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec5` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec5`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec6` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec6`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/decimate/sac_fir/dec7` & `tiskitpy-0.5rc1/tiskitpy/decimate/sac_fir/dec7`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/fir_corr/fir2caus.py` & `tiskitpy-0.5rc1/tiskitpy/fir_corr/fir2caus.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/logger.py` & `tiskitpy-0.5rc1/tiskitpy/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -74,15 +74,16 @@
                              
     # File Handler
     fileHandler = RotatingFileHandler(logfile, maxBytes=200*1024, backupCount=3)
     fileHandler.setFormatter(logging.Formatter(
         fmt='{asctime} {levelname:<8s} {module}.{funcName}(): {message}',
         style='{', datefmt='%Y-%m-%d %H:%M:%S'))
     fileHandler.setLevel(file_level.upper())
-
+    
+    
     # Console Handler
     console_log_output = console_log_output.lower()
     if (console_log_output == "stdout"):
         console_log_output = sys.stdout
     elif (console_log_output == "stderr"):
         console_log_output = sys.stderr
     else:
@@ -95,44 +96,7 @@
         color=True, style='{'))
     consoleHandler.setLevel(console_level.upper())
     
     logger.addHandler(fileHandler)
     logger.addHandler(consoleHandler)
 
     return logger
-    
-def change_level(logger, htype, level):
-    """
-    Change a handler's logging level
-    
-    Args:
-        htype (str): handler type: 'console' or 'file'
-        level (str): 'DEBUG', 'INFO', 'WARNING', 'ERROR', or 'CRITICAL'
-    """
-    assert htype.upper() in ['CONSOLE', 'FILE']
-    assert level.upper() in ['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
-
-    if htype.upper() == 'CONSOLE':
-        handler_type = logging.StreamHandler
-    else:
-        handler_type = logging.RotatingFileHandler
-    for handler in logger.handlers:
-        if isinstance(handler, handler_type):
-            handler.setLevel(level)
-
-def change_console_level(logger, level):
-    """
-    Change consoleHandlers logging level
-    
-    Args:
-        level (str): 'DEBUG', 'INFO', 'WARNING', 'ERROR', or 'CRITICAL'
-    """
-    change_level(logger, 'console', level)
-
-def change_file_level(logger, level):
-    """
-    Change fileHandler's logging level
-    
-    Args:
-        level (str): 'DEBUG', 'INFO', 'WARNING', 'ERROR', or 'CRITICAL'
-    """
-    change_level(logger, 'file', level)
```

### Comparing `tiskitpy-0.5/tiskitpy/read_mseed.py` & `tiskitpy-0.5rc1/tiskitpy/read_mseed.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/response_functions/response_functions.py` & `tiskitpy-0.5rc1/tiskitpy/response_functions/response_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,25 +270,22 @@
         ir = self._ds["instrument_response"].sel(output=oc).values
         return np.squeeze(ir)
 
     def to_norm_compliance(self, water_depth):
         """
         Change rfs from m/s^2 / Pa to 1 / Pa by multiplying by k / omega^2
         """
-        print(self)
-        print(f'{self.input_units=}')
-        print(f'{self.output_units=}')
         if not self.input_units.upper() == 'PA':
-            logger.error(f'{self.input_units=}, not "PA"')
+            raise ValueError(f'{self.input_units=}, not "PA"')
         om = np.pi * self.freqs
         k = _gravd(om, water_depth)
         rf_multiplier = k / (om**2)
         for oc in self.output_channel_ids:
             if not self.output_units(oc).upper() == 'M/S^2':
-                logger.error(f'{self.output_units(oc)=}, not "M/2^2"')
+                raise ValueError('{self.output_units(oc)=}, not "M/2^2"')
             # 'value' is in physical units, have to change instrument_response
             # so that value w.r.t. counts remains constant
             self._ds["value"].loc[dict(output=oc)] = self.value(oc) * rf_multiplier
             self._ds["instrument_response"].loc[dict(output=oc)] = (
                 self.instrument_response(oc) / rf_multiplier)
             self._ds.coords["out_units"].loc[dict(output=oc)] = '1'
```

### Comparing `tiskitpy-0.5/tiskitpy/rptransient/dirac_comb.py` & `tiskitpy-0.5rc1/tiskitpy/rptransient/dirac_comb.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/rptransient/periodic_transient.py` & `tiskitpy-0.5rc1/tiskitpy/rptransient/periodic_transient.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/rptransient/transients.py` & `tiskitpy-0.5rc1/tiskitpy/rptransient/transients.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/rptransient/utils.py` & `tiskitpy-0.5rc1/tiskitpy/rptransient/utils.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/spectral_density/Peterson_noise_model.py` & `tiskitpy-0.5rc1/tiskitpy/spectral_density/Peterson_noise_model.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/spectral_density/spectral_density.py` & `tiskitpy-0.5rc1/tiskitpy/spectral_density/spectral_density.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .utils import _prol1pi, _prol4pi, coherence_significance_level
 from obspy.core.stream import Stream
 from obspy.core import UTCDateTime
 from scipy import signal, stats
 
 from .Peterson_noise_model import Peterson_noise_model
 from ..time_spans import TimeSpans
-from ..logger import init_logger, change_level
+from ..logger import init_logger
 from ..cleaned_stream import CleanedStream
 from ..utils import match_one_str, CleanSequence as CS
 
 logger = init_logger()
 np.seterr(all="ignore")
 
 
@@ -122,24 +122,28 @@
 
     def __eq__(self, other):
         return self._ds == other._ds
 
     @property
     def ids(self):
         """
-        List of Channel ids: seed_ids + any cleaning information
+        Channel ids
+
         ** Previously called _channel_names **
+
+        Returns:
+            (list of str):
         """
-        outp = list(self._ds.coords["input"].values)
-        assert outp == list(self._ds.coords["output"].values)
-        return outp
+        assert list(self._ds.coords["input"].values) == list(
+            self._ds.coords["output"].values
+        )
+        return list(self._ds.coords["input"].values)
 
     @property
     def seed_ids(self):
-        """list of seed_ids"""
         return list(self._ds.coords["seed_ids"].values)
 
     @property
     def clean_sequences(self):
         """
         Returns:
             (list of list):
@@ -227,16 +231,15 @@
             (int):
         """
         return self._ds.n_windows
 
     @classmethod
     def from_stream(cls, stream, window_s=1000, windowtype="prol1pi",
                     inv=None, data_cleaner=None, starttimes=None,
-                    time_spans=None, avoid_spans=None, z_threshold=3,
-                    quiet=False):
+                    time_spans=None, avoid_spans=None, z_threshold=3):
         """
         Calculate spectral density functions from the provided stream
 
         Should add a window selection algorithm, for now just steps by
         the window length
 
         Args:
@@ -255,18 +258,15 @@
                 time spans.  Incompatible with `starttimes`
             avoid_spans (:class:`TimeSpans`): Do NOT use data from the provided
                 time spans.  Incompatible with `starttimes` and "time_spans"
             subtract_rf_suffix (str): suffix to add to channel names if rf
                 is subtracted
             z_threshold (float or None): reject windows with z-score greater
                 than this value.  None: no rejection
-            quiet (bool): only output errors and beyond to console
         """
-        if quiet is True:
-            change_level(logger, 'console','ERROR')
         if not isinstance(stream, Stream):
             raise ValueError(f"stream is a {type(stream)}, not obspy Stream")
         stream = stream.copy()  # avoid modifying original stream
 
         if time_spans is not None:
             stream = CleanedStream(stream).tag('SPANS')
         if avoid_spans is not None:
@@ -716,85 +716,72 @@
         Returns:
             (float):
         """
         return coherence_significance_level(self.n_windows, prob)
 
     @staticmethod
     def plots(sds,
-              channel=None,
-              line_kws=None,
-              labels=None,
               x=None,
               overlay=True,
               plot_peterson=True,
               show=True,
               outfile=None,
               title=None,
               **fig_kw):
         """
         Plot overlaid autospectra of multiple SpectralDensity objects
 
         Args:
             sds (list): SpectralDensity functions to plot
-            channel (str): Limit to the given channel
-            line_kws(list of dict): Line keywords for each SpectralDensity function
-            labels(list of dict): labels for each sd
         Other Properties:
             **kwargs: any arguments used in plot_autospectra, except
                 overlay (always true)
-        Returns:
-            figinfo (list):
-                fig
-                axa (): amplitude axis
         """
         # Validate inputs
         if overlay is not True:
             logger.warning('You requested overlay=False, ignored!')
-        line_kws, labels = _validate_plots_args(sds, line_kws, labels)
+        if not isinstance(sds, list):
+            raise ValueError('sds is not a list')
+        for sd in sds:
+            if not isinstance(sd, SpectralDensity):
+                raise ValueError('sds element is not a SpectralDensity object')
 
         rows, cols = 1, 1
+        ax_array = np.ndarray((rows, cols), dtype=tuple)
         fig, axs = plt.subplots(rows, cols, sharex=True, **fig_kw)
         if title is None:
             title = "Auto-spectra, multiple SpectralDensities"
         fig.suptitle(title)
         axa, axp = None, None
         first_time = True
-        for sd, l_kw, label in zip(sds, line_kws, labels):
-            assert isinstance(l_kw, dict)
+        for sd in sds:
             new_x = sd._get_validate_ids(x)
             for key, i in zip(new_x, range(len(new_x))):
-                if channel is not None:
-                    if not key.split('.')[-1] == channel:
-                        continue
                 axa, axp = sd.plot_one_spectra(
                     key,
                     key,
                     fig,
                     (1, 1),
                     (0, 0),
-                    show_ylabel=True,   # Would be better to do only LAST time
-                    show_xlabel=True,   # Would be better to do only LAST time
+                    show_ylabel=first_time,
+                    show_xlabel=first_time,
                     ax_a=axa,
                     ax_p=axp,
                     show_phase=False,
                     plot_peterson=plot_peterson,
-                    annotate=False,
-                    label=label,
-                    **fig_kw,
-                    **l_kw
+                    annotate=False
                 )
                 first_time = False
-        if channel is not None and first_time is True:
-            logger.error(f'No channel matching {channel} found, nothing plotted')
-        plt.legend(fontsize='x-small')
+        ax_array[0, 0] = (axa, axp)
+        plt.legend(fontsize='small')
         if outfile:
             plt.savefig(outfile)
         if show:
             plt.show()
-        return fig, axa
+        return ax_array
 
     def plot(self, **kwargs):
         """Shortcut for `plot_autospectra()`"""
         self.plot_autospectra(**kwargs)
 
     def plot_autospectra(
         self,
@@ -949,44 +936,42 @@
         ylabel=None,
         label=None,
         title=None,
         show_coherence=False,
         show_phase=True,
         plot_peterson=True,
         outfile=None,
-        annotate=True,
-        **plot_kws
+        annotate=True
     ):
         """
         Plot one spectral density
 
         Args:
             key (str): input (driving) channel
             subkey (str): output (response) channel
             fig (:class:`matplotlib.figure.Figure`): figure to plot on, if
                 None this method will plot on the current figure or create
                 a new figure.
             fig_grid (tuple): this plot sits in a grid of this many
                               (rows, columns)
-            subplot_spot (tuple): put this plot at this (row, column) of
+            subplot_spot (tuple): put this plot at this (row,column) of
                                   the figure grid
             show_xlabel (bool): put an xlabel on this subplot
             show_ylabel (bool): put a ylabel on this subplot
             ylabel (str): label to put on y axis (if show_label).  If not
                 speficied, will use 'dB ref UNITS/Hz'
             label (str): 'units': print units without channel name in legend
             ax_a (Axis): use an existing axis for the amplitude plot
             ax_p (Axis): use this existing axis for the phase plot
             title (str): title to put on this subplot
             show_coherence (bool): draw coherence on the same plot
             show_phase (bool): show phase as well as amplitude
             plot_peterson(bool): plot Peterson Noise model if channel has
                 units of :math:`(m/s^2)^2/Hz`
             outfile (str): save figure to this filename
-            **plot_kws (dict): keywords to pass on to plot command
 
         Returns:
             (tuple): tuple containing
                 - :class:`matplotlib.axes.axis`: amplitude plot axis
                 - :class:`matplotlib.axes.axis`: phase plot axis
         """
         psd = self.crossspect(key, subkey)
@@ -1035,15 +1020,15 @@
         psd[psd == 0] = None
 
         # Plot amplitude
         if label is None:
             label = f"{subkey} ({PSD_units})"
         elif label == "units":
             label = f"{PSD_units}"
-        ax_a.semilogx(f, 10 * np.log10(np.abs(psd)), label=label, **plot_kws)
+        ax_a.semilogx(f, 10 * np.log10(np.abs(psd)), label=label)
         ax_a.set_xlim(f[1], f[-1])
         if plot_peterson is True and PSD_units.lower() == "(m/s^2)^2":
             lownoise, highnoise = Peterson_noise_model(f, True)
             ax_a.semilogx(f, lownoise, "k--")
             ax_a.semilogx(f, highnoise, "k--")
 
         if label is not None and annotate is True:
@@ -1061,15 +1046,15 @@
         # Plot phase
         if show_phase:
             if ax_p is None:
                 ax_p = plt.subplot2grid(
                     (3 * fig_grid[0], 1 * fig_grid[1]),
                     (3 * plot_spot[0] + 2, plot_spot[1] + 0),
                 )
-            ax_p.semilogx(f, np.degrees(np.angle(psd), **plot_kws))
+            ax_p.semilogx(f, np.degrees(np.angle(psd)))
             ax_p.set_ylim(-180, 180)
             ax_p.set_xlim(f[1], f[-1])
             ax_p.set_yticks((-180, 0, 180))
             if show_ylabel:
                 # ax_p.set_ylabel('Phase')
                 pass
             else:
@@ -1106,128 +1091,16 @@
         if inp_type == 'chan':
             return self._seedid_chan
         elif inp_type == 'loc-chan':
             return self._seedid_loc_chan
         else:
             return self._seedid_full
 
-    @staticmethod
-    def plots_coherences(sds,
-              sds_names=None,
-              line_kws=None,
-              labels=None,
-              x=None,
-              y=None,
-              display='sparse',
-              overlay=False,
-              show=True,
-              label_by="chan",
-              sort_by="chan",
-              outfile=None,
-              title=None,
-              **fig_kw):
-        """
-        Plot overlaid coherences of multiple SpectralDensity objects
-
-        Args:
-            sds (list): SpectralDensity functions to plot.  Each must have
-                same seed_ids
-            sds_names (list): Names to give to each sd in the plot legend
-            line_kws(list of dict): Line keywords for each SpectralDensity function
-            labels(list of dict): Labels for each SpectralDensity function
-        Other Properties:
-            **kwargs: any arguments used in plot_coherences, except
-                overlay (always true)
-        Returns:
-            figinfo (list):
-                fig
-                axa (): amplitude axis
-        """
-        # Validate inputs
-        if overlay is True:
-            logger.error("Can't overlay multiple coherences")
-            overlay=False
-        assert display=='sparse'
-        line_kws, labels = _validate_plots_args(sds, line_kws, labels)
-        if sds_names is None:
-            sds_names = [max(x.clean_sequences, key=len) for x in sds]
-        else:
-            assert len(sds_names) == len(sds)
-
-        x_inp, y_inp = x, y
-        strfun = sds[0]._seedid_strfun(sort_by)
-        x = sorted(sds[0]._get_validate_ids(x_inp), key=strfun)
-        y = sorted(sds[0]._get_validate_ids(y_inp), key=strfun)
-        # Copied from plot_coherences "sparse" option, there's got
-        # to be a way not to repeat code
-        rows, cols = len(x), len(y)
-        reduce_display = False
-        if x[0] == y[0]:
-            reduce_display = True   # Can get rid of one row and column
-            rows -= 1
-            cols -= 1
-        ax_array = np.ndarray((rows, cols), dtype=tuple)
-        ax_array.fill((None, None))
-        fig, axs = plt.subplots(rows, cols, sharex=True, **fig_kw)
-        net_sta = '.'.join(sds[0].seed_ids[0].split('.')[:2])
-        fig.suptitle(f"{net_sta} Coherences, multiple SpectralDensitys")
-        first_time = True
-        for sd, l_kw in zip(sds, line_kws):
-            sort_strfun = sd._seedid_strfun(sort_by)
-            x = sorted(sd._get_validate_ids(x_inp), key=sort_strfun)
-            y = sorted(sd._get_validate_ids(y_inp), key=sort_strfun)
-            label_strfun = sd._seedid_strfun(label_by)
-            assert isinstance(l_kw, dict)
-            # new_x = sd._get_validate_ids(x)
-            plotted = []
-            for in_chan, i in zip(x, range(len(x))):
-                new_row = True
-                for out_chan, jbase in zip(y, range(len(y))):
-                    j = jbase
-                    if reduce_display==True:
-                        j -= 1
-                    if in_chan == out_chan or (out_chan, in_chan) in plotted:
-                        if i < rows and j >= 0:
-                            axs[i, j].axis('off')
-                        continue
-                    plotted.append((in_chan, out_chan))
-                    in_chan_label = label_strfun(in_chan)
-                    out_chan_label = label_strfun(out_chan)
-                    title = out_chan_label if i == 0 else None
-                    axa, axp = sd.plot_one_coherence(
-                        in_chan,
-                        out_chan,
-                        fig,
-                        (rows, cols),
-                        (i, j),
-                        ax_a=ax_array[i,j][0],
-                        ax_p=ax_array[i,j][1],
-                        show_ylabel=new_row & first_time,
-                        show_xlabel=(i == j)  & first_time,
-                        ylabel=in_chan_label,
-                        title=title,
-                        **l_kw
-                    )
-                    new_row = False
-                    ax_array[i, j] = (axa, axp)
-        i, j = rows-1, 0
-        axs[i,j].axis('on')
-        for sds_name, l_kw, label in zip(sds_names, line_kws, labels):
-            if label is None:
-                label = sds_name
-            axs[i,j].plot([1,1],[1,1], label=label, **l_kw)
-        axs[i,j].legend(fontsize='x-small')
-        if outfile:
-            plt.savefig(outfile)
-        if show:
-            plt.show()
-        return fig, axa
-
     def plot_coherences(self, x=None, y=None, display='full', show=True,
-                        outfile=None, label_by="full", sort_by="full",
+                        outfile=None, labels="full", sort_by="full",
                         overlay=False, **fig_kw):
         """
         Plot coherences
 
         Args:
             x (list of str or None): limit to the listed input channels
             y (list of str or None): limit to the listed output channels
@@ -1237,15 +1110,15 @@
                 - "sparse": Only plot the upper diagonal
                 - "minimal": Plot upper diagonal elements in the least
                   number of cells possible
                 - "overlay": One plot with all upper diagonal elemetns overlain
             overlay (bool): [GRANDFATHERED]: same as display="overlay"
             show (bool): show on desktop
             outfile (str): save to the named file
-            label_by (str): labels to put on x and y axes ('full', 'chan' or
+            labels (str): labels to put on x and y axes ('full', 'chan' or
                 'loc-chan')
             sort_by (str): how to sort x and y axes ('full', 'chan' or
                 'loc-chan')
             fig_kw (dict): all additional keyword arguments (such as `figsize`
                 and `dpi`) are passed to the `pyplot.figure` call
 
         Returns:
@@ -1262,15 +1135,15 @@
             if display == 'full':
                 display = 'overlay'
         if display == 'full':
             rows, cols = len(x), len(y)
             ax_array = np.ndarray((rows, cols), dtype=tuple)
             fig, axs = plt.subplots(rows, cols, sharex=True, **fig_kw)
             fig.suptitle("Coherences")
-            strfun = self._seedid_strfun(label_by)
+            strfun = self._seedid_strfun(labels)
             for in_chan, i in zip(x, range(rows)):
                 for out_chan, j in zip(y, range(cols)):
                     in_chan_label = strfun(in_chan)
                     out_chan_label = strfun(out_chan)
                     title = out_chan_label if i == 0 else None
                     axa, axp = self.plot_one_coherence(
                         in_chan, out_chan,
@@ -1287,15 +1160,15 @@
             if x[0] == y[0]:
                 reduce_display = True   # Can get rid of one row and column
                 rows -= 1
                 cols -= 1
             ax_array = np.ndarray((rows, cols), dtype=tuple)
             fig, axs = plt.subplots(rows, cols, sharex=True, **fig_kw)
             fig.suptitle("Coherences")
-            strfun = self._seedid_strfun(label_by)
+            strfun = self._seedid_strfun(labels)
             plotted = []
             for in_chan, i in zip(x, range(len(x))):
                 new_row = True
                 for out_chan, jbase in zip(y, range(len(y))):
                     j = jbase
                     if reduce_display==True:
                         j -= 1
@@ -1329,15 +1202,15 @@
             if rows == 0:
                 rows = 1
             cols = int(np.ceil(len(combis)/rows))
             ax_array = np.ndarray((rows, cols), dtype=tuple)
             fig, axs = plt.subplots(rows, cols, sharex=True, sharey=True,
                                     **fig_kw)
             fig.suptitle("Coherencies")
-            strfun = self._seedid_strfun(label_by)
+            strfun = self._seedid_strfun(labels)
             i, j = 0, 0
             for combi in combis:
                 in_chan = combi[0]
                 out_chan = combi[1]
                 in_chan_label = strfun(in_chan)
                 out_chan_label = strfun(out_chan)
                 title = out_chan_label if i == 0 else None
@@ -1392,21 +1265,30 @@
         if outfile:
             plt.savefig(outfile)
         if show:
             plt.show()
         return ax_array
 
     def plot_one_coherence(
-        self, in_chan, out_chan,
-        fig=None, fig_grid=(1, 1), plot_spot=(0, 0),
-        show_xlabel=True, show_ylabel=True,
-        ax_a=None, ax_p=None,
-        ylabel=None, label=None, title=None,
+        self,
+        in_chan,
+        out_chan,
+        fig=None,
+        fig_grid=(1, 1),
+        plot_spot=(0, 0),
+        show_xlabel=True,
+        show_ylabel=True,
+        ax_a=None,
+        ax_p=None,
+        ylabel=None,
+        label=None,
+        title=None,
         show_phase=True,
-        outfile=None, show=False, **kwargs):
+        **kwargs
+    ):
         """
         Plot one coherence
 
         Args:
             in_chan (str): input (driving) channel
             out_chan (str): output (response) channel
             fig (:class:`matplotlib.figure.Figure`): figure to plot on, if
@@ -1421,16 +1303,14 @@
             ylabel (str): label to put on y axis (if show_label).  If not
                 speficied, will use 'dB ref UNITS/Hz'
             label (str): text to put in legend
             ax_a (Axis): use an existing axis for the amplitude plot
             ax_p (Axis): use this existing axis for the phase plot
             title (str): title to put on this subplot
             show_phase (bool): show phase as well as amplitude
-            outfile (str): plot to the named file
-            show (bool): show on the screen (False by default: parent function shows)
             kwargs (dict): values to pass on to plotting routines
 
         Returns:
             (tuple): tuple containing:
                 - (:class:`matplotlib.axes.axis`): amplitude plot axis
                 - (:class:`matplotlib.axes.axis`): phase plot axis
         """
@@ -1505,35 +1385,29 @@
             fig.add_subplot(rows, cols, row * cols + col + 1, frameon=False)
             if ylabel is None:
                 ylabel = "Coherence"
             plt.tick_params(labelcolor='none', which='both', top=False,
                             bottom=False, left=False, right=False)
             plt.ylabel(ylabel, fontsize='small')
 
-        if outfile:
-            plt.savefig(outfile)
-        if show:
-            plt.show()
         return ax_a, ax_p
 
     def _get_validate_ids(self, x):
         """
         If x is None, return list of all channel ids
         If x is a list, validate each id
 
         Args:
             x (list or None): channel ids to validate
         """
         if x is None:
             x = list(self._ds.coords["input"].values)
-            x = self.ids
         else:
             for key in x:
-                # if key not in list(self._ds.coords["input"].values):
-                if key not in self.ids:
+                if key not in list(self._ds.coords["input"].values):
                     ValueError('key "{key}" not in id list')
         return x
 
     @staticmethod
     def _windowed_rfft(trace, ws, ss=None, win_taper="hanning",
                        starttimes=None, time_spans=None):
         """
@@ -1858,44 +1732,14 @@
         return id
     if "-" not in comps[2]:
         return id
     comps[2] = comps[2].partition("-")[0]
     return ".".join(comps)
 
 
-def _validate_plots_args(sds, line_kws, labels):
-    """ validate arguments passed to plots() and to plots_coherences()"""
-    if not isinstance(sds, (list, tuple)):
-        raise ValueError('sds is not a list or tuple')
-    for i, sd in zip(range(len(sds)), sds):
-        if not isinstance(sd, SpectralDensity):
-            raise ValueError(f'sds[{i}] is not a SpectralDensity object')
-        if i == 0:
-            seed_ids = sorted(sds[0].seed_ids)
-        else:
-            if not (seed_ids == sorted(sd.seed_ids)):
-                raise ValueError(f"sds[{i}].seed_ids={sd.seed_ids}"
-                                 f" does not match {sds[0].seed_ids=}")
-    if line_kws is not None:
-        if not isinstance(line_kws, (list, tuple)):
-            raise ValueError('line_kws is not a list or tuple')
-        if not len(line_kws) == len(sds):
-            raise ValueError(f'{len(line_kws)=} != {len(sds)=}')
-    else:
-        line_kws = [{} for x in sds]
-    if labels is not None:
-        if not isinstance(labels, (list, tuple)):
-            raise ValueError('labels is not a list or tuple')
-        if not len(labels) == len(sds):
-            raise ValueError(f'{len(labels)=} != {len(sds)=}')
-    else:
-        labels = [None for x in sds]
-    return line_kws, labels
-
-
 def _remove_subtracted_chan(id):
     """
     Remove chan code characters including and after first "-"
     """
     comps = id.split(".")
     if not len(comps) == 4:
         return id
```

### Comparing `tiskitpy-0.5/tiskitpy/spectral_density/utils.py` & `tiskitpy-0.5rc1/tiskitpy/spectral_density/utils.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/time_spans.py` & `tiskitpy-0.5rc1/tiskitpy/time_spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,17 @@
         Generate timespans to avoid because of earthquakes
 
         Will read earthquakes from the USGS online catalog the first time,
         saving the information to a file that can be subsequently used
 
         Args:
             starttime (:class:`UTCDateTime` or str): earliest data that will be
-                presented.  If a str, must by ISO8601 compatible.  Forced
-                to the beginning of the day
+                presented.  If a str, must by ISO8601 compatible
             endtime (:class:`UTCDateTime` or str): latest data that will be presented.
-                If a str, must by ISO8601 compatible.  Forced to the
-                end of the day
+                If a str, must by ISO8601 compatible
             minmag (float): EQ Magnitude above which to cut out times
             days_per_magnitude (float): days to cut per magnitude above
                 min_magnitude
             eq_file (str): the eq filename (otherwise, generates it)
             save_eq_file (bool): save the catalog file for future use
         Returns:
             eq_spans (:class:`TimeSpans`): time spans covering EQ signal
@@ -106,39 +104,31 @@
             except Exception:
                 raise ValueError(f"UTCDateTime() could not read {starttime=}")
         if isinstance(endtime, str):
             try:
                 endtime = UTCDateTime(endtime)
             except Exception:
                 raise ValueError(f"UTCDateTime() could not read {endtime=}")
-        starttime = starttime.replace(hour=0, minute=0, second=0, microsecond=0)
-        endtime = endtime.replace(hour=23, minute=59, second=59, microsecond=999999)
         if eq_file is None:
             eq_file = _eq_filename(starttime, endtime, minmag)
         if Path(eq_file).is_file():
             cat = read_events(eq_file, format="quakeml")
         else:
-            logger.info(f"Didn't find local EQ file '{eq_file}', reading from USGS online catalog...")
-            try:
-                cat = Client("USGS").get_events(
-                    starttime=starttime
-                    - _calc_eq_cut(9, minmag, days_per_magnitude),
-                    endtime=endtime,
-                    minmagnitude=minmag,
-                    orderby="time-asc",
-                )
-                logger.info("Done")
-                logger.info(f'writing catalog to "{eq_file}"')
-                if save_eq_file:
-                    cat.write(eq_file, format="quakeml")
-            except Exception as e:  # except FDSNNoServiceException as e:
-                logger.warning(e)
-                logger.warning('!!!Continuing without removing EQs!!!')
-                return cls([])
-            
+            logger.info("Reading EQs from USGS online catalog...")
+            cat = Client("USGS").get_events(
+                starttime=starttime
+                - _calc_eq_cut(9, minmag, days_per_magnitude),
+                endtime=endtime,
+                minmagnitude=minmag,
+                orderby="time-asc",
+            )
+            logger.info("Done")
+            logger.info(f'writing catalog to "{eq_file}"')
+            if save_eq_file:
+                cat.write(eq_file, format="quakeml")
 
         new_cat = Catalog(
             events=[x for x in cat if x.preferred_magnitude().mag >= minmag]
         )
         spans = [[x.preferred_origin().time,
                   x.preferred_origin().time
                   + _calc_eq_cut(x.preferred_magnitude().mag,
@@ -533,13 +523,13 @@
     Create earthquake file filename
 
     Args:
         starttime (UTCDateTime): start time
         endtime (UTCDateTime): end time
         min_magmitude (float): minimum magnitude saved
     Returns:
-        filename (string): includes startday to endday information
+        filename (string):
     """
-    tfmt = "%Y%m%d"
+    tfmt = "%Y%m%dT%H%M%S"
     return "{}-{}_MM{:g}_eqcat.qml".format(
         starttime.strftime(tfmt), endtime.strftime(tfmt), minmag
     )
```

### Comparing `tiskitpy-0.5/tiskitpy/utils/clean_sequence.py` & `tiskitpy-0.5rc1/tiskitpy/utils/clean_sequence.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.5/tiskitpy/utils/functions.py` & `tiskitpy-0.5rc1/tiskitpy/utils/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 """
 Copyright 2023 Wayne Crawford
 """
 import fnmatch  # Allows Unix filename pattern matching
-
-import numpy as np
-from ..logger import init_logger
-
-logger = init_logger()
-
-def stream_unmask(stream):
-    """
-    Check if a stream is masked and, if so, unmask it
-    Interpolates data in gaps
-        """
-    if np.any([np.ma.count_masked(tr.data) for tr in stream]):
-        logger.warning('Unmasking masked data (usually a gap or overlap)')
-        return stream.split().merge(fill_value='interpolate')
-    return stream
+# from ..logger import init_logger
+# 
+# logger = init_logger()
 
 def get_full_id(match_str, stream):
     """
     Return stream trace's channel seed_id matching match_str
     
     Args:
         match_str (str): string to match (may have \* and \? wildcards)
```

### Comparing `tiskitpy-0.5/tiskitpy/utils/seis_rotate.py` & `tiskitpy-0.5rc1/tiskitpy/utils/seis_rotate.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,42 +10,39 @@
 import numpy as np
 import scipy as sp
 import matplotlib.pyplot as plt
 from obspy.signal.rotate import rotate2zne
 from obspy.core.stream import Stream  # , Trace
 
 from ..logger import init_logger
-from .stream_synchronize import stream_synchronize
 
 logger = init_logger()
 
 
 class SeisRotate:
     """
     Class to clean tilt noise from OBS vertical channel through
     non-deforming rotation
     """
 
-    def __init__(self, stream, uselogvar=False, max_reject_sync=0.01):
+    def __init__(self, stream, uselogvar=False):
         """
         Create a seisRotate object from a 3-component obsPy Stream
 
         Arguments:
             stream (Stream): 3+ component data stream
             uselogvar(bool): use logarithmic variance when searching for
                              best angles
-            max_reject_sync(): max_reject value for stream_synchronize()
 
         Channel names must end in Z, N and E or Z, 1, and 2
         Z is up, 1 and 2 are horizontal orthogonal with 2 90° clockwise
         of "1"  (in other words, "1" corresponds to "N" and "2" to "E",
         except that they are not necessarily aligned with geographic
         cardinals)
         """
-        stream = stream_synchronize(stream, max_reject_sync)
         self.uselogvar = uselogvar
         self.Z, self.N, self.E = SeisRotate._get_seis_traces(stream)
         self.fs = self.Z.stats.sampling_rate
         # Verify that all channels have same length
         if not len(self.Z.data) == len(self.N.data):
             raise ValueError("Z and N vectors have different lengths")
         if not len(self.Z.data) == len(self.E.data):
@@ -117,30 +114,27 @@
             self.E.data = E
 
     def calc_zrotate_opt(
         self,
         lowcut=0.001,
         hicut=0.005,
         ignore_spans=None,
-        uselogvar=None
+        uselogvar=None,
+        verbose=False,
     ):
         """
         Calculate the Z channel rotation angle that minimizes tilt noise
 
         Arguments:
-            lowcut (float): low passband frequency in which to evaluate
-                            variance reduction
+            lowcut (float): low passband frequency in which to lood for energy
+                             reduction
             hicut (float): high passpand frequency "" "" ""
             ignore_spans (:class:`TimeSpans``): time spans to ignore
             uselogvar(bool): use logarithmic variance estimate
-
-        Returns: (tuple)
-            angle (float): tilt angle (degrees, 0 means no tilt correction)
-            azimuth (float): tilt azimuth (degrees)
-            var_red (float): obtained reduction in variance (0 to 1)
+            verbose (bool): output information about the angles tested?
 
         The default (lowcut, hicut) values of (0.001, 0.005) correspond to the
         band where removing tilt noise generally has the greatest effect on
         the Z signal (at the low frequency end of the noise notch)
 
         You can input the returned angles to rotateSeis.zrotate() to get
         the properly rotated data
@@ -154,34 +148,37 @@
         filt.E.filter("bandpass", freqmin=lowcut, freqmax=hicut, corners=5)
         if ignore_spans is not None:
             filt.Z = ignore_spans.zero(filt.Z)
             filt.N = ignore_spans.zero(filt.N)
             filt.E = ignore_spans.zero(filt.E)
 
         # Quick estimate of angles using Z/E and Z/N ratios. DOESN'T HELP: SKIP
+        # (startAngle,startAzimuth)=filt._estimateAngles(verbose)
         startAngle, startAzi = (0, 0)
 
         # Search for the best angles
-        angle, azimuth, var_red = filt._searchBestAngles(startAngle, startAzi)
-        return angle, azimuth, var_red
+        angle, azimuth = filt._searchBestAngles(startAngle, startAzi, verbose)
+        return angle, azimuth
 
-    def _estimateAngles(self):
+    def _estimateAngles(self, verbose=False):
         """
         Estimate how far and in which direction Z is tilted from vertical
         by comparing with N and E
 
         azimuth is 0 towards N, 90 towards E
         dip is w.r.t. vertical
 
         Assumes data has already been filtered into the relevant band
 
         Doesn't seem to work AT ALL! I think there is too much other stuff
         (transients, etc) for this to work.  Also doesn't account for any time
         lags: might work better if ratios calculated from cross-corellation
 
+        Arguments:
+            verbose (bool): display extra information?
         """
         logger.debug("Estimating preliminary angle based on signal ratios")
         ZoverN = np.divide(self.Z.data, self.N.data)
         ZoverE = np.divide(self.Z.data, self.E.data)
         # Throw out not-a-numbers
         ZoverN = ZoverN[~np.isnan(ZoverN)]
         ZoverE = ZoverE[~np.isnan(ZoverE)]
@@ -209,60 +206,64 @@
         # return ZN & ZE angles??
         dip_N = angle * M.cos(np.deg2rad(azimuth))
         dip_E = angle * M.sin(np.deg2rad(azimuth))
         logger.info(f"{dip_N=}, {dip_E=}")
 
         return angle, azimuth
 
-    def _searchBestAngles(self, startAngle=0, startAzimuth=0):
+    def _searchBestAngles(self, startAngle=0, startAzimuth=0, verbose=False):
         """
         Find best Z rotation angles
 
         Arguments:
             startAngle (float): starting guess for the angle (degrees)
             startAzimuth (float): starting guess for the azimuth (degrees)
+            verbose (bool): display extra information?
 
         Returns:
             (tuple): 2-tuple containing:
-                angle (float): best angle (degrees, 0 to 90)
-                azimuth (float): best azimuth (degrees, 0 to 360)
-                var_red (float): variance reduction (0 to 1)
+                angle (float): best angle (degrees)
+                azimuth (float): best azimuth (degrees)
 
         Searches for minimum Z energy as function of angle
         """
         logger.debug("Calculating best angle based on variance minimization")
         start_var = self._rotZ_variance([startAngle, startAzimuth])
         logger.debug(f"Starting variance = {start_var}")
 
         xopt, fopt, iter, funcalls, warnflag, allvecs = sp.optimize.fmin(
             func=self._rotZ_variance,
             x0=[startAngle, startAzimuth],
-            disp=False, full_output=True, retall=True)
-        bestAngle, bestAzimuth = xopt
-        if bestAngle < 0:
-            bestAngle = -bestAngle
-            bestAzimuth += 180
-        bestAzimuth %= 360.
-        if bestAngle > 90:
-            logger.warning(f'bestAngle > 90! ({bestAngle})')
-
-        logger.debug(f"{xopt=}, {fopt=}, {iter=}, {funcalls=}, {warnflag=}")
+            disp=False,
+            full_output=True,
+            retall=True,
+        )
+        bestAngles = xopt
 
+        if verbose is True:
+            logger.info(f"{fopt=}, {iter=}, {funcalls=}")
+            logger.debug(f"{xopt=}, {warnflag=}")
+        else:
+            logger.debug(f"{xopt=}, {fopt=}, {iter=}, {funcalls=}, {warnflag=}")
+        
         if self.uselogvar is False:
-            var_red = 1 - fopt / start_var
-            logger.debug("    variance reduced from {:.2e} to {:.2e} ({:.1f}% lower)"
-                        .format(start_var, fopt, 100 * var_red))
+            logger.info(
+                "    variance reduced from "
+                "{:.2e} to {:.2e} ({:.1f}% lower)".format(
+                    start_var, fopt,
+                    100 * (1 - fopt / start_var)))
         else:
-            var_red = 1 - 10 ** (fopt - start_var)
-            logger.debug("    log variance reduced from {:.1f} to {:.1f} ({:.1f}% lower)"
-                        .format(start_var, fopt, 100 * var_red))
+            logger.info("    log variance reduced from "
+                  "{:.1f} to {:.1f} ({:.1f}% lower)".format(
+                      start_var, fopt,
+                      100 * (1 - 10 ** (fopt - start_var))))
         if warnflag:
-            logger.debug(f"optimization warning flag: {allvecs=}")
+            logger.info(f"{allvecs=}")
 
-        return (bestAngle, bestAzimuth, var_red)
+        return (bestAngles[0], bestAngles[1])
 
     def _rotZ_variance(self, angles):
         """
         Calculate the variance for a given rotation
 
         Arguments:
             angles (list): angle, azimuth (in degrees)
```

### Comparing `tiskitpy-0.5/tiskitpy.egg-info/PKG-INFO` & `tiskitpy-0.5rc1/tiskitpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiskitpy
-Version: 0.5
+Version: 0.5rc1
 Summary: TIme Series toolKIT
 Home-page: https://github.com/WayneCrawford/tiskitpy
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `tiskitpy-0.5/tiskitpy.egg-info/SOURCES.txt` & `tiskitpy-0.5rc1/tiskitpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 tiskitpy.egg-info/top_level.txt
 tiskitpy/data_cleaner/__init__.py
 tiskitpy/data_cleaner/data_cleaner_tf.py
 tiskitpy/data_cleaner/rf_list.py
 tiskitpy/decimate/.DS_Store
 tiskitpy/decimate/ToDo.md
 tiskitpy/decimate/__init__.py
+tiskitpy/decimate/decimate_SDS.py
 tiskitpy/decimate/decimator.py
 tiskitpy/decimate/fir_filter.py
 tiskitpy/decimate/version.py
 tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc
 tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc
 tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
 tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc
@@ -58,9 +59,8 @@
 tiskitpy/spectral_density/__init__.py
 tiskitpy/spectral_density/spectral_density.py
 tiskitpy/spectral_density/utils.py
 tiskitpy/spectral_density/version.py
 tiskitpy/utils/__init__.py
 tiskitpy/utils/clean_sequence.py
 tiskitpy/utils/functions.py
-tiskitpy/utils/seis_rotate.py
-tiskitpy/utils/stream_synchronize.py
+tiskitpy/utils/seis_rotate.py
```

