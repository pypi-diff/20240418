# Comparing `tmp/hidrokit-0.5.1.tar.gz` & `tmp/hidrokit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidrokit-0.5.1.tar", last modified: Wed Apr 17 14:54:39 2024, max compression
+gzip compressed data, was "hidrokit-0.5.2.tar", last modified: Thu Apr 18 00:48:57 2024, max compression
```

## Comparing `hidrokit-0.5.1.tar` & `hidrokit-0.5.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.541784 hidrokit-0.5.1/
--rw-rw-rw-   0        0        0     6060 2024-04-14 07:31:59.000000 hidrokit-0.5.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    15622 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CHANGELOG_gen.md
--rw-rw-rw-   0        0        0     6464 2024-04-14 07:31:59.000000 hidrokit-0.5.1/CHANGELOG_old.md
--rw-rw-rw-   0        0        0     3369 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      128 2024-04-11 05:03:58.000000 hidrokit-0.5.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1109 2024-04-14 07:31:59.000000 hidrokit-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2024-04-11 05:03:58.000000 hidrokit-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5956 2024-04-17 14:54:39.541784 hidrokit-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4626 2024-04-16 06:22:26.000000 hidrokit-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.466771 hidrokit-0.5.1/hidrokit/
--rw-rw-rw-   0        0        0      299 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-17 14:53:46.000000 hidrokit-0.5.1/hidrokit/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.480399 hidrokit-0.5.1/hidrokit/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.481393 hidrokit-0.5.1/hidrokit/contrib/
--rw-rw-rw-   0        0        0       46 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.520721 hidrokit-0.5.1/hidrokit/contrib/taruma/
--rw-rw-rw-   0        0        0     2436 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/__init__.py
--rw-rw-rw-   0        0        0      549 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/anfrek.py
--rw-rw-rw-   0        0        0     9158 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/bmkg_utils.py
--rw-rw-rw-   0        0        0    11049 2024-04-17 14:41:16.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/chi_square.py
--rw-rw-rw-   0        0        0     4218 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/dataframe_to_tensor.py
--rw-rw-rw-   0        0        0     4657 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/dependable_flow.py
--rw-rw-rw-   0        0        0    20229 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/evapotranspiration.py
--rw-rw-rw-   0        0        0     6927 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/fjmock_model.py
--rw-rw-rw-   0        0        0    18688 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/gumbel.py
--rw-rw-rw-   0        0        0     8396 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_excel_parser.py
--rw-rw-rw-   0        0        0     6021 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py
--rw-rw-rw-   0        0        0     9264 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/kolmogorov_smirnov.py
--rw-rw-rw-   0        0        0     7815 2024-04-17 14:41:16.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/lognormal.py
--rw-rw-rw-   0        0        0    24565 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/logpearson3.py
--rw-rw-rw-   0        0        0     3293 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/model_calibration.py
--rw-rw-rw-   0        0        0     8668 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/normal.py
--rw-rw-rw-   0        0        0     8127 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/nreca_model.py
--rw-rw-rw-   0        0        0     6436 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/outlier_hydrology.py
--rw-rw-rw-   0        0        0    11543 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py
--rw-rw-rw-   0        0        0     3827 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/statistic_summary.py
--rw-rw-rw-   0        0        0     4156 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/statistical_coefficients.py
--rw-rw-rw-   0        0        0     5752 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/summary_hourly.py
--rw-rw-rw-   0        0        0     2484 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/thiessen.py
--rw-rw-rw-   0        0        0      411 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/ujidist.py
--rw-rw-rw-   0        0        0     3469 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/upsampling.py
--rw-rw-rw-   0        0        0     1667 2024-04-16 04:13:00.000000 hidrokit-0.5.1/hidrokit/contrib/taruma/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.526234 hidrokit-0.5.1/hidrokit/prep/
--rw-rw-rw-   0        0        0       86 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/__init__.py
--rw-rw-rw-   0        0        0     3931 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/excel.py
--rw-rw-rw-   0        0        0     2217 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/read.py
--rw-rw-rw-   0        0        0     4217 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/prep/timeseries.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.531237 hidrokit-0.5.1/hidrokit/viz/
--rw-rw-rw-   0        0        0       62 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/graph.py
--rw-rw-rw-   0        0        0     1253 2024-04-11 05:03:58.000000 hidrokit-0.5.1/hidrokit/viz/table.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.478355 hidrokit-0.5.1/hidrokit.egg-info/
--rw-rw-rw-   0        0        0     5956 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1778 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 14:54:39.000000 hidrokit-0.5.1/hidrokit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2024-04-17 14:54:39.544407 hidrokit-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3134 2024-04-14 07:33:33.000000 hidrokit-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:54:39.538789 hidrokit-0.5.1/tests/
--rw-rw-rw-   0        0        0     1797 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_excel.py
--rw-rw-rw-   0        0        0      844 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_read.py
--rw-rw-rw-   0        0        0     5086 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_prep_timeseries.py
--rw-rw-rw-   0        0        0      477 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_viz_graph.py
--rw-rw-rw-   0        0        0     1632 2024-04-11 05:03:58.000000 hidrokit-0.5.1/tests/test_viz_table.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.083980 hidrokit-0.5.2/
+-rw-rw-rw-   0        0        0     6060 2024-04-14 07:31:59.000000 hidrokit-0.5.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    15622 2024-04-11 05:03:58.000000 hidrokit-0.5.2/CHANGELOG_gen.md
+-rw-rw-rw-   0        0        0     6464 2024-04-14 07:31:59.000000 hidrokit-0.5.2/CHANGELOG_old.md
+-rw-rw-rw-   0        0        0     3369 2024-04-11 05:03:58.000000 hidrokit-0.5.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      128 2024-04-11 05:03:58.000000 hidrokit-0.5.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1109 2024-04-14 07:31:59.000000 hidrokit-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2024-04-11 05:03:58.000000 hidrokit-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5956 2024-04-18 00:48:57.082979 hidrokit-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4626 2024-04-16 06:22:26.000000 hidrokit-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:56.999878 hidrokit-0.5.2/hidrokit/
+-rw-rw-rw-   0        0        0      299 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-18 00:40:29.000000 hidrokit-0.5.2/hidrokit/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.013972 hidrokit-0.5.2/hidrokit/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.015514 hidrokit-0.5.2/hidrokit/contrib/
+-rw-rw-rw-   0        0        0       46 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.059604 hidrokit-0.5.2/hidrokit/contrib/taruma/
+-rw-rw-rw-   0        0        0     2428 2024-04-18 00:34:33.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/__init__.py
+-rw-rw-rw-   0        0        0      549 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/anfrek.py
+-rw-rw-rw-   0        0        0     9158 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/bmkg_utils.py
+-rw-rw-rw-   0        0        0    11049 2024-04-17 14:41:16.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/chi_square.py
+-rw-rw-rw-   0        0        0     4218 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/dataframe_to_tensor.py
+-rw-rw-rw-   0        0        0     4657 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/dependable_flow.py
+-rw-rw-rw-   0        0        0    20229 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/evapotranspiration.py
+-rw-rw-rw-   0        0        0     6927 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/fjmock_model.py
+-rw-rw-rw-   0        0        0    18688 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/gumbel.py
+-rw-rw-rw-   0        0        0     8396 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/hidrokit_excel_parser.py
+-rw-rw-rw-   0        0        0     6021 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py
+-rw-rw-rw-   0        0        0     9264 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/kolmogorov_smirnov.py
+-rw-rw-rw-   0        0        0     7815 2024-04-17 14:41:16.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/lognormal.py
+-rw-rw-rw-   0        0        0    24565 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/logpearson3.py
+-rw-rw-rw-   0        0        0     3293 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/model_calibration.py
+-rw-rw-rw-   0        0        0     8668 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/normal.py
+-rw-rw-rw-   0        0        0     8127 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/nreca_model.py
+-rw-rw-rw-   0        0        0     6436 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/outlier_hydrology.py
+-rw-rw-rw-   0        0        0    11543 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py
+-rw-rw-rw-   0        0        0     3827 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/statistic_summary.py
+-rw-rw-rw-   0        0        0     4156 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/statistical_coefficients.py
+-rw-rw-rw-   0        0        0     5752 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/summary_hourly.py
+-rw-rw-rw-   0        0        0     2484 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/thiessen.py
+-rw-rw-rw-   0        0        0      411 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/ujidist.py
+-rw-rw-rw-   0        0        0     3469 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/upsampling.py
+-rw-rw-rw-   0        0        0     1667 2024-04-16 04:13:00.000000 hidrokit-0.5.2/hidrokit/contrib/taruma/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.066679 hidrokit-0.5.2/hidrokit/prep/
+-rw-rw-rw-   0        0        0       86 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/prep/__init__.py
+-rw-rw-rw-   0        0        0     3931 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/prep/excel.py
+-rw-rw-rw-   0        0        0     2217 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/prep/read.py
+-rw-rw-rw-   0        0        0     4217 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/prep/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.071773 hidrokit-0.5.2/hidrokit/viz/
+-rw-rw-rw-   0        0        0       62 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/viz/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/viz/graph.py
+-rw-rw-rw-   0        0        0     1253 2024-04-11 05:03:58.000000 hidrokit-0.5.2/hidrokit/viz/table.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.012937 hidrokit-0.5.2/hidrokit.egg-info/
+-rw-rw-rw-   0        0        0     5956 2024-04-18 00:48:56.000000 hidrokit-0.5.2/hidrokit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2024-04-18 00:48:56.000000 hidrokit-0.5.2/hidrokit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 00:48:56.000000 hidrokit-0.5.2/hidrokit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-18 00:48:56.000000 hidrokit-0.5.2/hidrokit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 00:48:56.000000 hidrokit-0.5.2/hidrokit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-04-18 00:48:57.087379 hidrokit-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     3134 2024-04-14 07:33:33.000000 hidrokit-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 00:48:57.080981 hidrokit-0.5.2/tests/
+-rw-rw-rw-   0        0        0     1797 2024-04-11 05:03:58.000000 hidrokit-0.5.2/tests/test_prep_excel.py
+-rw-rw-rw-   0        0        0      844 2024-04-11 05:03:58.000000 hidrokit-0.5.2/tests/test_prep_read.py
+-rw-rw-rw-   0        0        0     5086 2024-04-11 05:03:58.000000 hidrokit-0.5.2/tests/test_prep_timeseries.py
+-rw-rw-rw-   0        0        0      477 2024-04-11 05:03:58.000000 hidrokit-0.5.2/tests/test_viz_graph.py
+-rw-rw-rw-   0        0        0     1632 2024-04-11 05:03:58.000000 hidrokit-0.5.2/tests/test_viz_table.py
```

### Comparing `hidrokit-0.5.1/CHANGELOG.md` & `hidrokit-0.5.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/CHANGELOG_gen.md` & `hidrokit-0.5.2/CHANGELOG_gen.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/CHANGELOG_old.md` & `hidrokit-0.5.2/CHANGELOG_old.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/CODE_OF_CONDUCT.md` & `hidrokit-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/LICENSE.txt` & `hidrokit-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/PKG-INFO` & `hidrokit-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.5.1
+Version: 0.5.2
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.5.1 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.2 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
```

### Comparing `hidrokit-0.5.1/README.md` & `hidrokit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/__init__.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     "hk84": "summary_hourly",
     "hk87": "dependable_flow",
     "hk88": "hidrokit_excel_parser",
     "hk89": "nreca_model",
     "hk90": "model_calibration",
     "hk96": "fjmock_model",
     "hk98": "statistic_summary",
-    "hk99": "thiessen_polygon",
+    "hk99": "thiessen",
     "hk102": "upsampling",
     "hk106": "evapotranspiration",
     "hk124": "lognormal",
     "hk126": "logpearson3",
     "hk127": "gumbel",
     "hk140": "kolmogorov_smirnov",
     "hk141": "chi_square",
```

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/anfrek.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/anfrek.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/bmkg_utils.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/bmkg_utils.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/chi_square.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/chi_square.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/dataframe_to_tensor.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/dataframe_to_tensor.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/dependable_flow.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/dependable_flow.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/evapotranspiration.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/fjmock_model.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/fjmock_model.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/gumbel.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/gumbel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_excel_parser.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/hidrokit_excel_parser.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/kolmogorov_smirnov.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/kolmogorov_smirnov.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/lognormal.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/lognormal.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/logpearson3.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/logpearson3.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/model_calibration.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/model_calibration.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/normal.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/normal.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/nreca_model.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/nreca_model.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/outlier_hydrology.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/outlier_hydrology.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/statistic_summary.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/statistic_summary.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/statistical_coefficients.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/statistical_coefficients.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/summary_hourly.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/summary_hourly.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/thiessen.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/thiessen.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/upsampling.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/upsampling.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/contrib/taruma/utils.py` & `hidrokit-0.5.2/hidrokit/contrib/taruma/utils.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/prep/excel.py` & `hidrokit-0.5.2/hidrokit/prep/excel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/prep/read.py` & `hidrokit-0.5.2/hidrokit/prep/read.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/prep/timeseries.py` & `hidrokit-0.5.2/hidrokit/prep/timeseries.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/viz/graph.py` & `hidrokit-0.5.2/hidrokit/viz/graph.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit/viz/table.py` & `hidrokit-0.5.2/hidrokit/viz/table.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/hidrokit.egg-info/PKG-INFO` & `hidrokit-0.5.2/hidrokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.5.1
+Version: 0.5.2
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.5.1 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.2 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
```

### Comparing `hidrokit-0.5.1/hidrokit.egg-info/SOURCES.txt` & `hidrokit-0.5.2/hidrokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/setup.py` & `hidrokit-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/tests/test_prep_excel.py` & `hidrokit-0.5.2/tests/test_prep_excel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/tests/test_prep_read.py` & `hidrokit-0.5.2/tests/test_prep_read.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/tests/test_prep_timeseries.py` & `hidrokit-0.5.2/tests/test_prep_timeseries.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.5.1/tests/test_viz_table.py` & `hidrokit-0.5.2/tests/test_viz_table.py`

 * *Files identical despite different names*

