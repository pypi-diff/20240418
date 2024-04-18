# Comparing `tmp/trajectopy_core-2.6.1.tar.gz` & `tmp/trajectopy_core-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy_core-2.6.1.tar", max compression
+gzip compressed data, was "trajectopy_core-2.7.0.tar", max compression
```

## Comparing `trajectopy_core-2.6.1.tar` & `trajectopy_core-2.7.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-2.6.1/LICENSE
--rw-r--r--   0        0        0     1049 2024-02-02 14:22:54.938873 trajectopy_core-2.6.1/pyproject.toml
--rw-r--r--   0        0        0    33078 2024-01-25 13:51:00.895558 trajectopy_core-2.6.1/README.md
--rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-2.6.1/trajectopy_core/__init__.py
--rw-r--r--   0        0        0       49 2023-11-08 14:24:59.343660 trajectopy_core-2.6.1/trajectopy_core/alignment/__init__.py
--rw-r--r--   0        0        0    10066 2024-01-30 09:06:48.053542 trajectopy_core-2.6.1/trajectopy_core/alignment/actions.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.344660 trajectopy_core-2.6.1/trajectopy_core/alignment/direct/__init__.py
--rw-r--r--   0        0        0     2435 2023-11-29 11:29:09.869840 trajectopy_core-2.6.1/trajectopy_core/alignment/direct/helmert_transformation.py
--rw-r--r--   0        0        0     5318 2023-11-08 14:24:59.345660 trajectopy_core-2.6.1/trajectopy_core/alignment/direct/leverarm.py
--rw-r--r--   0        0        0     2163 2023-11-08 14:24:59.345660 trajectopy_core-2.6.1/trajectopy_core/alignment/direct/timeshift.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.345660 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/__init__.py
--rw-r--r--   0        0        0    19410 2024-01-30 09:00:58.078515 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/data.py
--rw-r--r--   0        0        0    36142 2024-01-30 09:07:15.373939 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/estimation.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.347660 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/functional_model/__init__.py
--rw-r--r--   0        0        0    16133 2023-11-08 14:24:59.347660 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/functional_model/equations.py
--rw-r--r--   0        0        0     8549 2023-11-08 14:24:59.347660 trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/functional_model/interface.py
--rw-r--r--   0        0        0    23827 2023-11-29 11:29:09.870840 trajectopy_core-2.6.1/trajectopy_core/alignment/parameters.py
--rw-r--r--   0        0        0     2833 2023-11-08 14:24:59.349660 trajectopy_core-2.6.1/trajectopy_core/alignment/result.py
--rw-r--r--   0        0        0     1021 2023-11-29 11:29:09.871841 trajectopy_core-2.6.1/trajectopy_core/alignment/rotation_alignment.py
--rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-2.6.1/trajectopy_core/alignment/utils.py
--rw-r--r--   0        0        0        0 2023-11-29 11:29:09.871841 trajectopy_core-2.6.1/trajectopy_core/approximation/__init__.py
--rw-r--r--   0        0        0     9308 2023-11-29 11:29:09.871841 trajectopy_core-2.6.1/trajectopy_core/approximation/cubic_approximation.py
--rw-r--r--   0        0        0     6608 2023-11-29 11:29:09.872840 trajectopy_core-2.6.1/trajectopy_core/approximation/math_utils.py
--rw-r--r--   0        0        0     3880 2023-11-29 11:29:09.872840 trajectopy_core-2.6.1/trajectopy_core/approximation/mls_approximation.py
--rw-r--r--   0        0        0     2151 2023-11-29 11:29:09.873840 trajectopy_core-2.6.1/trajectopy_core/approximation/rot_approximation.py
--rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-2.6.1/trajectopy_core/approximation/voxelizer.py
--rw-r--r--   0        0        0     1999 2023-11-08 14:24:59.350662 trajectopy_core-2.6.1/trajectopy_core/definitions.py
--rw-r--r--   0        0        0      112 2023-11-08 14:24:59.350662 trajectopy_core-2.6.1/trajectopy_core/evaluation/__init__.py
--rw-r--r--   0        0        0    15142 2023-12-04 13:28:15.723893 trajectopy_core-2.6.1/trajectopy_core/evaluation/ate_result.py
--rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-2.6.1/trajectopy_core/evaluation/comparison.py
--rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-2.6.1/trajectopy_core/evaluation/deviations.py
--rw-r--r--   0        0        0     9981 2023-12-04 09:19:20.545163 trajectopy_core-2.6.1/trajectopy_core/evaluation/rpe_result.py
--rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-2.6.1/trajectopy_core/evaluation/utils.py
--rw-r--r--   0        0        0        0 2023-10-09 11:26:32.327576 trajectopy_core-2.6.1/trajectopy_core/io/__init__.py
--rw-r--r--   0        0        0     5273 2023-11-29 11:29:09.876841 trajectopy_core-2.6.1/trajectopy_core/io/header.py
--rw-r--r--   0        0        0     3021 2023-11-29 11:29:09.877841 trajectopy_core-2.6.1/trajectopy_core/io/rosbag.py
--rw-r--r--   0        0        0     1197 2023-10-09 11:26:32.328577 trajectopy_core-2.6.1/trajectopy_core/io/rosmsg.py
--rw-r--r--   0        0        0    11291 2023-11-29 11:29:09.877841 trajectopy_core-2.6.1/trajectopy_core/io/trajectory_io.py
--rw-r--r--   0        0        0     1118 2023-11-29 11:29:09.878841 trajectopy_core-2.6.1/trajectopy_core/io/utils.py
--rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-2.6.1/trajectopy_core/kml.py
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-2.6.1/trajectopy_core/LICENSE
--rw-r--r--   0        0        0     9574 2024-01-30 08:26:02.456799 trajectopy_core-2.6.1/trajectopy_core/matching.py
--rw-r--r--   0        0        0     6433 2024-01-30 08:20:56.341344 trajectopy_core-2.6.1/trajectopy_core/pipelines.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-2.6.1/trajectopy_core/plotting/__init__.py
--rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-2.6.1/trajectopy_core/plotting/bar_plots.py
--rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-2.6.1/trajectopy_core/plotting/heatmaps.py
--rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-2.6.1/trajectopy_core/plotting/histograms.py
--rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-2.6.1/trajectopy_core/plotting/line_plots.py
--rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-2.6.1/trajectopy_core/plotting/multi_line_plots.py
--rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-2.6.1/trajectopy_core/plotting/scatter_plots.py
--rw-r--r--   0        0        0     1626 2023-11-29 11:29:09.880840 trajectopy_core-2.6.1/trajectopy_core/plotting/tables.py
--rw-r--r--   0        0        0     1727 2023-12-04 13:28:15.725896 trajectopy_core-2.6.1/trajectopy_core/plotting/utils.py
--rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-2.6.1/trajectopy_core/report/__init__.py
--rw-r--r--   0        0        0     2441 2024-01-25 13:23:14.390650 trajectopy_core-2.6.1/trajectopy_core/report/alignment.py
--rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-2.6.1/trajectopy_core/report/assets/icon.png
--rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-2.6.1/trajectopy_core/report/assets/style.css
--rw-r--r--   0        0        0     6220 2024-01-25 13:43:59.293453 trajectopy_core-2.6.1/trajectopy_core/report/data.py
--rw-r--r--   0        0        0     3640 2024-01-25 13:36:22.539255 trajectopy_core-2.6.1/trajectopy_core/report/multi.py
--rw-r--r--   0        0        0     5286 2024-01-25 13:28:15.283518 trajectopy_core-2.6.1/trajectopy_core/report/single.py
--rw-r--r--   0        0        0     4660 2024-02-02 14:21:04.343956 trajectopy_core-2.6.1/trajectopy_core/report/templates/generic.html
--rw-r--r--   0        0        0     5616 2024-02-02 14:20:15.519891 trajectopy_core-2.6.1/trajectopy_core/report/templates/multi_template.html
--rw-r--r--   0        0        0     7282 2024-02-02 14:19:19.420695 trajectopy_core-2.6.1/trajectopy_core/report/templates/single_template.html
--rw-r--r--   0        0        0     1999 2024-01-22 14:08:45.548680 trajectopy_core-2.6.1/trajectopy_core/report/trajectory.py
--rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-2.6.1/trajectopy_core/report/utils.py
--rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-2.6.1/trajectopy_core/rotationset.py
--rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-2.6.1/trajectopy_core/settings/__init__.py
--rw-r--r--   0        0        0     8838 2023-11-29 11:29:09.884840 trajectopy_core-2.6.1/trajectopy_core/settings/alignment.py
--rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-2.6.1/trajectopy_core/settings/approximation.py
--rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-2.6.1/trajectopy_core/settings/base.py
--rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-2.6.1/trajectopy_core/settings/comparison.py
--rw-r--r--   0        0        0     1212 2023-11-29 11:29:09.885840 trajectopy_core-2.6.1/trajectopy_core/settings/matching.py
--rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-2.6.1/trajectopy_core/settings/processing.py
--rw-r--r--   0        0        0     6091 2024-01-30 08:35:08.718229 trajectopy_core-2.6.1/trajectopy_core/settings/report.py
--rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-2.6.1/trajectopy_core/settings/sorting.py
--rw-r--r--   0        0        0    10908 2023-12-04 09:19:20.551570 trajectopy_core-2.6.1/trajectopy_core/spatialsorter.py
--rw-r--r--   0        0        0    22734 2024-01-30 08:26:33.931539 trajectopy_core-2.6.1/trajectopy_core/trajectory.py
--rw-r--r--   0        0        0     6322 2023-11-29 11:29:09.888841 trajectopy_core-2.6.1/trajectopy_core/utils.py
--rw-r--r--   0        0        0    33953 1970-01-01 00:00:00.000000 trajectopy_core-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1049 2024-04-18 14:05:54.819712 trajectopy_core-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    33078 2024-02-02 14:24:47.281805 trajectopy_core-2.7.0/README.md
+-rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-2.7.0/trajectopy_core/__init__.py
+-rw-r--r--   0        0        0       49 2023-11-08 14:24:59.343660 trajectopy_core-2.7.0/trajectopy_core/alignment/__init__.py
+-rw-r--r--   0        0        0    10137 2024-04-18 14:05:54.820715 trajectopy_core-2.7.0/trajectopy_core/alignment/actions.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.344660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/__init__.py
+-rw-r--r--   0        0        0     2435 2023-11-29 11:29:09.869840 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/helmert_transformation.py
+-rw-r--r--   0        0        0     5318 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/leverarm.py
+-rw-r--r--   0        0        0     2163 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/timeshift.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/__init__.py
+-rw-r--r--   0        0        0    19496 2024-04-18 14:05:54.821747 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/data.py
+-rw-r--r--   0        0        0    36416 2024-04-18 14:05:54.821747 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/estimation.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/__init__.py
+-rw-r--r--   0        0        0    16133 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/equations.py
+-rw-r--r--   0        0        0     8549 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/interface.py
+-rw-r--r--   0        0        0    23827 2023-11-29 11:29:09.870840 trajectopy_core-2.7.0/trajectopy_core/alignment/parameters.py
+-rw-r--r--   0        0        0     2833 2023-11-08 14:24:59.349660 trajectopy_core-2.7.0/trajectopy_core/alignment/result.py
+-rw-r--r--   0        0        0     1021 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/alignment/rotation_alignment.py
+-rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-2.7.0/trajectopy_core/alignment/utils.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/approximation/__init__.py
+-rw-r--r--   0        0        0     9308 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/approximation/cubic_approximation.py
+-rw-r--r--   0        0        0     6608 2023-11-29 11:29:09.872840 trajectopy_core-2.7.0/trajectopy_core/approximation/math_utils.py
+-rw-r--r--   0        0        0     3880 2023-11-29 11:29:09.872840 trajectopy_core-2.7.0/trajectopy_core/approximation/mls_approximation.py
+-rw-r--r--   0        0        0     2151 2023-11-29 11:29:09.873840 trajectopy_core-2.7.0/trajectopy_core/approximation/rot_approximation.py
+-rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-2.7.0/trajectopy_core/approximation/voxelizer.py
+-rw-r--r--   0        0        0     2001 2024-04-18 14:05:54.822747 trajectopy_core-2.7.0/trajectopy_core/definitions.py
+-rw-r--r--   0        0        0      112 2023-11-08 14:24:59.350662 trajectopy_core-2.7.0/trajectopy_core/evaluation/__init__.py
+-rw-r--r--   0        0        0    15142 2023-12-04 13:28:15.723893 trajectopy_core-2.7.0/trajectopy_core/evaluation/ate_result.py
+-rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-2.7.0/trajectopy_core/evaluation/comparison.py
+-rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-2.7.0/trajectopy_core/evaluation/deviations.py
+-rw-r--r--   0        0        0     9981 2023-12-04 09:19:20.545163 trajectopy_core-2.7.0/trajectopy_core/evaluation/rpe_result.py
+-rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-2.7.0/trajectopy_core/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2023-10-09 11:26:32.327576 trajectopy_core-2.7.0/trajectopy_core/io/__init__.py
+-rw-r--r--   0        0        0     5273 2023-11-29 11:29:09.876841 trajectopy_core-2.7.0/trajectopy_core/io/header.py
+-rw-r--r--   0        0        0     3021 2023-11-29 11:29:09.877841 trajectopy_core-2.7.0/trajectopy_core/io/rosbag.py
+-rw-r--r--   0        0        0     1197 2023-10-09 11:26:32.328577 trajectopy_core-2.7.0/trajectopy_core/io/rosmsg.py
+-rw-r--r--   0        0        0    11291 2023-11-29 11:29:09.877841 trajectopy_core-2.7.0/trajectopy_core/io/trajectory_io.py
+-rw-r--r--   0        0        0     1118 2023-11-29 11:29:09.878841 trajectopy_core-2.7.0/trajectopy_core/io/utils.py
+-rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-2.7.0/trajectopy_core/kml.py
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-2.7.0/trajectopy_core/LICENSE
+-rw-r--r--   0        0        0     9635 2024-04-18 14:05:54.822747 trajectopy_core-2.7.0/trajectopy_core/matching.py
+-rw-r--r--   0        0        0     6433 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/pipelines.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-2.7.0/trajectopy_core/plotting/__init__.py
+-rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-2.7.0/trajectopy_core/plotting/bar_plots.py
+-rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-2.7.0/trajectopy_core/plotting/heatmaps.py
+-rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-2.7.0/trajectopy_core/plotting/histograms.py
+-rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-2.7.0/trajectopy_core/plotting/line_plots.py
+-rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-2.7.0/trajectopy_core/plotting/multi_line_plots.py
+-rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-2.7.0/trajectopy_core/plotting/scatter_plots.py
+-rw-r--r--   0        0        0     1626 2023-11-29 11:29:09.880840 trajectopy_core-2.7.0/trajectopy_core/plotting/tables.py
+-rw-r--r--   0        0        0     1727 2023-12-04 13:28:15.725896 trajectopy_core-2.7.0/trajectopy_core/plotting/utils.py
+-rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-2.7.0/trajectopy_core/report/__init__.py
+-rw-r--r--   0        0        0     2441 2024-02-02 14:24:47.286809 trajectopy_core-2.7.0/trajectopy_core/report/alignment.py
+-rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-2.7.0/trajectopy_core/report/assets/icon.png
+-rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-2.7.0/trajectopy_core/report/assets/style.css
+-rw-r--r--   0        0        0     6220 2024-02-02 14:24:47.287810 trajectopy_core-2.7.0/trajectopy_core/report/data.py
+-rw-r--r--   0        0        0     3640 2024-02-02 14:24:47.287810 trajectopy_core-2.7.0/trajectopy_core/report/multi.py
+-rw-r--r--   0        0        0     5286 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/single.py
+-rw-r--r--   0        0        0     4660 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/templates/generic.html
+-rw-r--r--   0        0        0     5616 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/templates/multi_template.html
+-rw-r--r--   0        0        0     7282 2024-02-02 14:24:47.289808 trajectopy_core-2.7.0/trajectopy_core/report/templates/single_template.html
+-rw-r--r--   0        0        0     1999 2024-01-22 14:08:45.548680 trajectopy_core-2.7.0/trajectopy_core/report/trajectory.py
+-rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-2.7.0/trajectopy_core/report/utils.py
+-rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-2.7.0/trajectopy_core/rotationset.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-2.7.0/trajectopy_core/settings/__init__.py
+-rw-r--r--   0        0        0     8889 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/settings/alignment.py
+-rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-2.7.0/trajectopy_core/settings/approximation.py
+-rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-2.7.0/trajectopy_core/settings/base.py
+-rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-2.7.0/trajectopy_core/settings/comparison.py
+-rw-r--r--   0        0        0     1164 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/settings/matching.py
+-rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-2.7.0/trajectopy_core/settings/processing.py
+-rw-r--r--   0        0        0     6091 2024-02-02 14:24:47.289808 trajectopy_core-2.7.0/trajectopy_core/settings/report.py
+-rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-2.7.0/trajectopy_core/settings/sorting.py
+-rw-r--r--   0        0        0    10908 2023-12-04 09:19:20.551570 trajectopy_core-2.7.0/trajectopy_core/spatialsorter.py
+-rw-r--r--   0        0        0    22734 2024-02-02 14:24:47.290806 trajectopy_core-2.7.0/trajectopy_core/trajectory.py
+-rw-r--r--   0        0        0     6322 2023-11-29 11:29:09.888841 trajectopy_core-2.7.0/trajectopy_core/utils.py
+-rw-r--r--   0        0        0    33953 1970-01-01 00:00:00.000000 trajectopy_core-2.7.0/PKG-INFO
```

### Comparing `trajectopy_core-2.6.1/LICENSE` & `trajectopy_core-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/pyproject.toml` & `trajectopy_core-2.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy-core"
-version = "2.6.1"
+version = "2.7.0"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 maintainers = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "MIT"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy-core"
```

### Comparing `trajectopy_core-2.6.1/README.md` & `trajectopy_core-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/actions.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from typing import Tuple
 
 import numpy as np
 
 from trajectopy_core.alignment.ghm.data import AlignmentData
 from trajectopy_core.alignment.ghm.estimation import Alignment
@@ -165,25 +166,24 @@
     estimation depending on the configuration.
     After this, the estimated parameters are applied
     to the 'traj_from' trajectory.
 
     Args:
         traj_from (Trajectory)
         traj_to (Trajectory)
-        alignment_config (AlignmentConfig): Configuration holding all
-                                            relevant settings for aligning
-                                            the trajectories.
+        alignment_settings (AlignmentSettings, optional): Settings for the alignment process. Defaults to AlignmentSettings().
+        matching_settings (MatchingSettings, optional): Settings for the matching process. Defaults to MatchingSettings().
 
     Returns:
-        Tuple[Trajectory, Trajectory]: Aligned trajectories
+        AlignmentResult: Result of the alignment process
     """
     # one of the trajectories is in an unknown datum
     if (
         None in [traj_to.pos.local_transformer, traj_to.pos.local_transformer]
-        and not alignment_settings.estimation_of.helmert_enabled
+        and not alignment_settings.estimation_settings.helmert_enabled
     ):
         print(
             "\n ____________________________________________________\n"
             "| --------------------- WARNING --------------------- |\n"
             f"| {'One of the trajectories is in an unknown datum.':<51} |\n"
             f"| {'However, according to the configuration, no Helmert':<51} |\n"
             f"| {'transformation should be performed.':<51} |\n"
@@ -206,46 +206,46 @@
         _set_group_variances(alignment_data)
 
     ghm_alignment, estimated_parameters = updated_estimation_process(alignment_settings, alignment_data)
 
     if (
         alignment_data.traj_from.rot is not None
         and alignment_data.traj_to.rot is not None
-        and alignment_settings.estimation_of.sensor_rotation
+        and alignment_settings.estimation_settings.sensor_rotation
     ):
         alignment_data.traj_from.apply_transformation(estimated_parameters.sim3_matrix)
         logger.info("Aligning rotations ...")
         sensor_rot_params = align_rotations(rot_from=alignment_data.traj_from.rot, rot_to=alignment_data.traj_to.rot)
         print(sensor_rot_params)
     else:
         sensor_rot_params = SensorRotationParameters(enabled=False)
 
     return AlignmentResult(
         name=f"{alignment_data.traj_from.name} to {alignment_data.traj_to.name}",
         position_parameters=estimated_parameters,
         rotation_parameters=sensor_rot_params,
-        estimation_of=ghm_alignment.settings.estimation_of,
+        estimation_of=ghm_alignment.settings.estimation_settings,
         converged=ghm_alignment.has_results,
     )
 
 
 def updated_estimation_process(alignment_settings: AlignmentSettings, alignment_data: AlignmentData):
     estimation_settings_changed = True
     while estimation_settings_changed:
         ghm_alignment = Alignment(alignment_data=alignment_data)
         estimated_parameters = ghm_alignment.estimate()
 
-        if alignment_settings.estimation_of.auto_update:
+        if alignment_settings.estimation_settings.auto_update:
             estimation_settings = ghm_alignment.update_estimation_settings()
         else:
             estimation_settings = None
 
         if estimation_settings is not None:
             estimation_settings_changed = True
-            alignment_data.alignment_settings.estimation_of = estimation_settings
+            alignment_data.alignment_settings.estimation_settings = estimation_settings
             alignment_data.setup()
         else:
             estimation_settings_changed = False
     return ghm_alignment, estimated_parameters
 
 
 def _set_group_variances(alignment_data: AlignmentData) -> None:
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/direct/helmert_transformation.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/direct/helmert_transformation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/direct/leverarm.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/direct/leverarm.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/direct/timeshift.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/direct/timeshift.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/data.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import copy
 import logging
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import spdiags
 
 from trajectopy_core.alignment.utils import gradient_3d
 from trajectopy_core.matching import match_trajectories
 from trajectopy_core.rotationset import RotationSet
-from trajectopy_core.settings.alignment import AlignmentEstimationSettings, AlignmentSettings
+from trajectopy_core.settings.alignment import AlignmentSettings
 from trajectopy_core.settings.matching import MatchingSettings
 from trajectopy_core.trajectory import Trajectory
 
 logger = logging.getLogger("root")
 
 
 POSITION_VARIANCE_GROUPS: List[str] = ["XY_FROM", "Z_FROM", "XY_TO", "Z_TO"]
@@ -67,16 +68,16 @@
             self.traj_to.crop(time_span[0], time_span[1])
             self.traj_from.crop(time_span[0], time_span[1])
 
         if len(self.traj_from) == 0 or len(self.traj_to) == 0:
             raise ValueError("At least one trajectory is empty after preprocessing!")
 
         match_trajectories(
-            traj_test=self.traj_from,
-            traj_ref=self.traj_to,
+            traj_from=self.traj_from,
+            traj_to=self.traj_to,
             settings=self.matching_settings,
         )
 
         logger.info(
             "Using timespan of %.3f seconds between %.3f and %.3f.",
             self.traj_from.tstamps[-1] - self.traj_from.tstamps[0],
             self.traj_from.tstamps[0],
@@ -99,44 +100,44 @@
     @cached_property
     def observation_groups(
         self,
     ) -> Dict[str, Tuple[Union[int, None], Union[int, None]]]:
         """Returns the observation groups depending on the settings"""
         speed_indices: Tuple[Union[int, None], Union[int, None]] = (None, None)
 
-        if not self.alignment_settings.estimation_of.time_shift_enabled:
+        if not self.alignment_settings.estimation_settings.time_shift_enabled:
             speed_indices = (None, None)
-        elif self.alignment_settings.estimation_of.leverarm_enabled:
+        elif self.alignment_settings.estimation_settings.leverarm_enabled:
             speed_indices = (9, 12)
         else:
             speed_indices = (6, 9)
 
         return {
             "XY_FROM": (0, 2),
             "Z_FROM": (2, 3),
             "XYZ_FROM": (0, 3),
             "XY_TO": (3, 5),
             "Z_TO": (5, 6),
             "XYZ_TO": (3, 6),
             "POSITIONS": (0, 6),
-            "ROLL_PITCH": (6, 8) if self.alignment_settings.estimation_of.leverarm_enabled else (None, None),
-            "YAW": (8, 9) if self.alignment_settings.estimation_of.leverarm_enabled else (None, None),
-            "RPY": (6, 9) if self.alignment_settings.estimation_of.leverarm_enabled else (None, None),
+            "ROLL_PITCH": (6, 8) if self.alignment_settings.estimation_settings.leverarm_enabled else (None, None),
+            "YAW": (8, 9) if self.alignment_settings.estimation_settings.leverarm_enabled else (None, None),
+            "RPY": (6, 9) if self.alignment_settings.estimation_settings.leverarm_enabled else (None, None),
             "SPEED": speed_indices,
         }
 
     @cached_property
     def variance_groups(self) -> List[str]:
         """Returns the variance groups depending on the settings"""
         variance_groups = copy.deepcopy(POSITION_VARIANCE_GROUPS)
 
-        if self.alignment_settings.estimation_of.leverarm_enabled:
+        if self.alignment_settings.estimation_settings.leverarm_enabled:
             variance_groups.extend(ORIENTATION_VARIANCE_GROUPS)
 
-        if self.alignment_settings.estimation_of.time_shift_enabled:
+        if self.alignment_settings.estimation_settings.time_shift_enabled:
             variance_groups.extend(SPEED_VARIANCE_GROUP)
 
         return variance_groups
 
     @property
     def obs_vector(self) -> np.ndarray:
         return self._obs_vector
@@ -197,18 +198,18 @@
     def num_obs_per_epoch(self) -> int:
         """
         Returns the number of observations per epoch depending on the
         enabled estimation modes.
         """
         obs_count = 6
 
-        if self.alignment_settings.estimation_of.leverarm_enabled:
+        if self.alignment_settings.estimation_settings.leverarm_enabled:
             obs_count += 3
 
-        if self.alignment_settings.estimation_of.time_shift_enabled:
+        if self.alignment_settings.estimation_settings.time_shift_enabled:
             obs_count += 3
 
         return obs_count
 
     def build_obs_vector(
         self,
         xyz_from: np.ndarray,
@@ -228,31 +229,31 @@
                                    inertial coordinate system.
 
         Returns:
             np.ndarray: The observation vector required for the alignment adjustment.
         """
         obs_init: np.ndarray = np.c_[xyz_from, xyz_to]
 
-        if self.alignment_settings.estimation_of.leverarm_enabled and rot_from is not None:
+        if self.alignment_settings.estimation_settings.leverarm_enabled and rot_from is not None:
             obs_init = np.c_[obs_init, rot_from.as_euler(seq="xyz")]
-        elif self.alignment_settings.estimation_of.leverarm_enabled:
+        elif self.alignment_settings.estimation_settings.leverarm_enabled:
             raise ValueError(
                 "Failed to create observation vector: Please provide platform orientations for leverarm alignment!"
             )
 
-        if self.alignment_settings.estimation_of.time_shift_enabled:
+        if self.alignment_settings.estimation_settings.time_shift_enabled:
             if speed is None and self.tstamps is not None:
                 speed = speed or gradient_3d(xyz_from, tstamps=self.tstamps)
 
             if speed is None:
                 raise ValueError(
                     "Failed to create observation vector: Please provide platform speed for time shift alignment!"
                 )
 
-            speed[:, not self.alignment_settings.estimation_of.time_shift_filter] = 0
+            speed[:, not self.alignment_settings.estimation_settings.time_shift_filter] = 0
             obs_init = np.c_[obs_init, speed]
 
         return np.reshape(obs_init, (obs_init.size,))
 
     def build_var_vector(self) -> np.ndarray:
         """Sets up the variance vector
 
@@ -280,18 +281,18 @@
         variances_rpy_body[:, 2] = np.ones((self.number_of_epochs,)) * self.alignment_settings.stochastics.var_yaw
 
         variances_speed_to = np.ones((self.number_of_epochs, 3)) * self.alignment_settings.stochastics.var_speed_to
 
         self._set_vector_components(vector=variances, values=variances_xyz_from, key="XYZ_FROM")
         self._set_vector_components(vector=variances, values=variances_xyz_to, key="XYZ_TO")
 
-        if self.alignment_settings.estimation_of.leverarm_enabled:
+        if self.alignment_settings.estimation_settings.leverarm_enabled:
             self._set_vector_components(vector=variances, values=variances_rpy_body, key="RPY")
 
-        if self.alignment_settings.estimation_of.time_shift_enabled:
+        if self.alignment_settings.estimation_settings.time_shift_enabled:
             self._set_vector_components(vector=variances, values=variances_speed_to, key="SPEED")
         return variances
 
     def build_res_vector(self) -> np.ndarray:
         return np.zeros_like(self._obs_vector)
 
     def get_obs_group(self, key: str) -> Tuple[np.ndarray, ...]:
@@ -346,22 +347,22 @@
 
     @property
     def xyz_to(self) -> np.ndarray:
         return np.c_[self.get_obs_group("XYZ_TO")]
 
     @property
     def rpy_from(self) -> np.ndarray:
-        if not self.alignment_settings.estimation_of.leverarm_enabled:
+        if not self.alignment_settings.estimation_settings.leverarm_enabled:
             return np.zeros((self.number_of_epochs, 3))
 
         return np.c_[self.get_obs_group("RPY")]
 
     @property
     def speed(self) -> np.ndarray:
-        if not self.alignment_settings.estimation_of.time_shift_enabled:
+        if not self.alignment_settings.estimation_settings.time_shift_enabled:
             return np.zeros((self.number_of_epochs, 3))
 
         return np.c_[self.get_obs_group("SPEED")]
 
     @property
     def x_from(self) -> np.ndarray:
         return self.xyz_from[:, 0]
@@ -416,22 +417,22 @@
 
     @property
     def est_xyz_to(self) -> np.ndarray:
         return np.c_[self.get_est_obs_group("XYZ_TO")]
 
     @property
     def est_rpy_from(self) -> np.ndarray:
-        if not self.alignment_settings.estimation_of.leverarm_enabled:
+        if not self.alignment_settings.estimation_settings.leverarm_enabled:
             return np.zeros((self.number_of_epochs, 3))
 
         return np.c_[self.get_est_obs_group("RPY")]
 
     @property
     def est_speed(self) -> np.ndarray:
-        if not self.alignment_settings.estimation_of.time_shift_enabled:
+        if not self.alignment_settings.estimation_settings.time_shift_enabled:
             return np.zeros((self.number_of_epochs, 3))
 
         return np.c_[self.get_est_obs_group("SPEED")]
 
     @property
     def est_x_from(self) -> np.ndarray:
         return self.est_xyz_from[:, 0]
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/estimation.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/estimation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from typing import Dict, Union
 
 import numpy as np
 from numpy import matlib
 from scipy.sparse import csc_matrix, spdiags
 from scipy.sparse.linalg import spsolve
@@ -114,19 +115,19 @@
     def estimate(self) -> AlignmentParameters:
         """Handles the estimation of the parameters
 
         Calls either robust reweighting or variance
         estimation methods.
         """
         logger.info("Performing alignment...")
-        if self.settings.estimation_of.all_lq_disabled:
+        if self.settings.estimation_settings.all_lq_disabled:
             logger.warning("Nothing to estimate since all parameters are disabled")
             return AlignmentParameters()
 
-        max_recomputations = 10
+        max_recomputations = 5
         cnt = 0
         while self._reestimation_required:
             if cnt > max_recomputations:
                 logger.warning("Maximum number of recomputations reached. Aborting.")
                 break
 
             self._reestimation_required = False
@@ -182,33 +183,36 @@
         using methods that do not require inital
         parameters.
 
         Returns:
             AlignmentParameters: Hold the estimates parameters.
                                  14 = 7 (helmert+scale) 3 (leverarm) 1 (time) 3 (orientation)
         """
-        if self.settings.estimation_of.helmert_enabled:
+        if self.settings.estimation_settings.helmert_enabled:
             helmert_init = direct_helmert_transformation(xyz_from=self.data.xyz_from, xyz_to=self.data.xyz_to)
             xyz_init = helmert_init.apply_to(self.data.xyz_from)
         else:
             helmert_init = HelmertTransformation()
             xyz_init = self.data.xyz_from
 
         logger.debug("Initial Helmert: %s \n", str(helmert_init))
 
-        if self.settings.estimation_of.time_shift_enabled and not self.settings.estimation_of.leverarm_enabled:
+        if (
+            self.settings.estimation_settings.time_shift_enabled
+            and not self.settings.estimation_settings.leverarm_enabled
+        ):
             time_shift_init, _ = direct_timeshift(xyz_from=xyz_init, xyz_to=self.data.xyz_to, speed=self.data.speed)
         else:
             time_shift_init = Parameter(value=0.0, name="Time shift", unit=Unit.SECOND)
 
         logger.debug("Initial time shift: %.3f", time_shift_init.value)
 
-        if self.settings.estimation_of.leverarm_enabled:
+        if self.settings.estimation_settings.leverarm_enabled:
             leverarm_init, time_shift_init, _ = direct_leverarm(
-                speed=self.data.speed if self.settings.estimation_of.time_shift_enabled else None,
+                speed=self.data.speed if self.settings.estimation_settings.time_shift_enabled else None,
                 xyz_from=xyz_init,
                 xyz_to=self.data.xyz_to,
                 rpy_body=self.data.rpy_from,
             )
         else:
             leverarm_init = Leverarm()
 
@@ -224,16 +228,16 @@
             sim_scale=helmert_init.scale,
             time_shift=time_shift_init,
             lever_x=leverarm_init.x,
             lever_y=leverarm_init.y,
             lever_z=leverarm_init.z,
         )
 
-        alignparams.apply_settings(self.settings.estimation_of)
-        logger.debug("Applied settings: %s \n", str(self.settings.estimation_of))
+        alignparams.apply_settings(self.settings.estimation_settings)
+        logger.debug("Applied settings: %s \n", str(self.settings.estimation_settings))
         return alignparams
 
     @property
     def variance_factor(self) -> float:
         return (
             self.data.res_vector.T @ spsolve(csc_matrix(self.data.sigma_ll), self.data.res_vector)
         ) / self.redundancy
@@ -314,14 +318,17 @@
     def variance_estimation(self) -> None:
         """
         Tests the consistency of the functional and stochastic model and
         adjusts the variance vector if necessary.
         """
         self._global_test(variance_factor=self.variance_factor, redundancy=self.redundancy)
 
+        if not self.data.alignment_settings.stochastics.variance_estimation:
+            return
+
         logger.info("Adjusting variance vector by factor %.3f", self.variance_factor)
 
         if np.allclose(self.variance_factor, 0):
             logger.warning("Variance factor is 0. Aborting.")
             return
 
         if abs(self.variance_factor - 1) > 0.1:
@@ -357,30 +364,30 @@
         # preparation for iterative adjustment
         delta_params = np.ones((len(self._est_params),)) * np.Inf
         self.data.res_vector = np.zeros_like(self.data.obs_vector)
 
         contradiction_w = self._auto_functional_relationship()
 
         it_counter = 0
-        max_iterations = 10
+        max_iterations = 15
         self._converged = True
         while any(abs(value) > threshold for value, threshold in zip(delta_params, self.data.thresholds)):
             if it_counter > max_iterations:
                 logger.error(
                     "Adjustment did not converge after %i iterations. Maximum parameter update: %.3e",
                     it_counter,
                     np.max(np.abs(delta_params)),
                 )
                 self._converged = False
                 break
 
             a_design = self.auto_design_matrix()
 
             # filter design matrix
-            a_design = a_design[:, self.settings.estimation_of.lq_parameter_filter]
+            a_design = a_design[:, self.settings.estimation_settings.lq_parameter_filter]
             b_cond = self._condition_matrix()
 
             bbt = b_cond @ self.data.sigma_ll @ b_cond.T
 
             # solve normal equations
             delta_params = self._compute_parameter_deltas(contradiction_w, a_design, bbt)
             correlates_k = -spsolve(bbt, a_design @ delta_params + contradiction_w)
@@ -679,55 +686,57 @@
             parameters (AlignmentParameters): (current) estimated parameters
 
         Returns:
             np.ndarray: condition matrix data
         """
         xyz_from_component = self._auto_condition_xyz_from()
 
-        rpy_body_component = self._auto_condition_rpy_body() if self.settings.estimation_of.leverarm_enabled else None
+        rpy_body_component = (
+            self._auto_condition_rpy_body() if self.settings.estimation_settings.leverarm_enabled else None
+        )
 
         speed_to_component = (
-            self._auto_condition_speed_to() if self.settings.estimation_of.time_shift_enabled else None
+            self._auto_condition_speed_to() if self.settings.estimation_settings.time_shift_enabled else None
         )
 
         if (
-            self.settings.estimation_of.leverarm_enabled
-            and not self.settings.estimation_of.time_shift_enabled
+            self.settings.estimation_settings.leverarm_enabled
+            and not self.settings.estimation_settings.time_shift_enabled
             and rpy_body_component is not None
         ):
             return np.column_stack(
                 [
                     np.c_[
                         xyz_from_component[i],
                         self._condition_xyz_to[i],
                         rpy_body_component[i],
                     ]
                     for i in range(3)
                 ]
             )
 
         if (
-            self.settings.estimation_of.time_shift_enabled
-            and not self.settings.estimation_of.leverarm_enabled
+            self.settings.estimation_settings.time_shift_enabled
+            and not self.settings.estimation_settings.leverarm_enabled
             and speed_to_component is not None
         ):
             return np.column_stack(
                 [
                     np.c_[
                         xyz_from_component[i],
                         self._condition_xyz_to[i],
                         speed_to_component[i],
                     ]
                     for i in range(3)
                 ]
             )
 
         if (
-            self.settings.estimation_of.leverarm_enabled
-            and self.settings.estimation_of.time_shift_enabled
+            self.settings.estimation_settings.leverarm_enabled
+            and self.settings.estimation_settings.time_shift_enabled
             and rpy_body_component is not None
             and speed_to_component is not None
         ):
             return np.column_stack(
                 [
                     np.c_[
                         xyz_from_component[i],
@@ -920,11 +929,11 @@
     logger.info(alignment.est_params)
 
 
 def settings_str(alignment: Alignment) -> str:
     return (
         f"\n _____________________________________________________________________\n"
         f"| ---------------------------- Alignment ---------------------------- |\n"
-        f"| Estimation of:           {alignment.settings.estimation_of.short_mode_str:<42} |\n"
+        f"| Estimation of:           {alignment.settings.estimation_settings.short_mode_str:<42} |\n"
         f"| Error probability [%]:   {alignment.settings.stochastics.error_probability*100:<42} |\n"
         f"|_____________________________________________________________________|\n"
     )
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/functional_model/equations.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/ghm/functional_model/interface.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/interface.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/parameters.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/parameters.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/result.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/rotation_alignment.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/rotation_alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/alignment/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/approximation/cubic_approximation.py` & `trajectopy_core-2.7.0/trajectopy_core/approximation/cubic_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/approximation/math_utils.py` & `trajectopy_core-2.7.0/trajectopy_core/approximation/math_utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/approximation/mls_approximation.py` & `trajectopy_core-2.7.0/trajectopy_core/approximation/mls_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/approximation/rot_approximation.py` & `trajectopy_core-2.7.0/trajectopy_core/approximation/rot_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/approximation/voxelizer.py` & `trajectopy_core-2.7.0/trajectopy_core/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/definitions.py` & `trajectopy_core-2.7.0/trajectopy_core/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import datetime
 from enum import Enum, auto
 from typing import Dict, Tuple
 
 import numpy as np
 
 
@@ -48,20 +49,20 @@
             return cls.NONE
 
         raise ValueError(f"Unknown unit string {unit_str}")
 
 
 # [multiply with , unit string, number of decimals]
 UNIT_FORMAT_RULES: Dict[Unit, Dict[str, Tuple[float, str, int]]] = {
-    Unit.METER: {"normal": (1, "m", 4), "precise": (1000, "mm", 1)},
-    Unit.RADIAN: {"normal": (180 / np.pi, "°", 4)},
-    Unit.DEGREE: {"normal": (1, "°", 4)},
+    Unit.METER: {"normal": (1, "m", 3), "precise": (1000, "mm", 1)},
+    Unit.RADIAN: {"normal": (180 / np.pi, "°", 3)},
+    Unit.DEGREE: {"normal": (1, "°", 3)},
     Unit.SECOND: {"normal": (1000, "ms", 1), "precise": (1000, "ms", 1)},
-    Unit.SCALE: {"normal": (1, "-", 4), "precise": (1e6, "ppm", 1)},
-    Unit.NONE: {"normal": (1, "-", 4)},
+    Unit.SCALE: {"normal": (1, "-", 3), "precise": (1e6, "ppm", 1)},
+    Unit.NONE: {"normal": (1, "-", 3)},
 }
 
 
 GPS_LEAP_SECONDS = 18
 GPS_WEEK_ZERO = datetime.datetime(1980, 1, 6, 0, 0, 0)
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/evaluation/ate_result.py` & `trajectopy_core-2.7.0/trajectopy_core/evaluation/ate_result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/evaluation/comparison.py` & `trajectopy_core-2.7.0/trajectopy_core/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/evaluation/deviations.py` & `trajectopy_core-2.7.0/trajectopy_core/evaluation/deviations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/evaluation/rpe_result.py` & `trajectopy_core-2.7.0/trajectopy_core/evaluation/rpe_result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/evaluation/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/io/header.py` & `trajectopy_core-2.7.0/trajectopy_core/io/header.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/io/rosbag.py` & `trajectopy_core-2.7.0/trajectopy_core/io/rosbag.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/io/rosmsg.py` & `trajectopy_core-2.7.0/trajectopy_core/io/rosmsg.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/io/trajectory_io.py` & `trajectopy_core-2.7.0/trajectopy_core/io/trajectory_io.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/io/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/io/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/kml.py` & `trajectopy_core-2.7.0/trajectopy_core/kml.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/LICENSE` & `trajectopy_core-2.7.0/trajectopy_core/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/matching.py` & `trajectopy_core-2.7.0/trajectopy_core/matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import copy
 import logging
 from typing import Tuple
 
 import numpy as np
 from pointset import PointSet
 from scipy.spatial import KDTree
@@ -16,47 +17,48 @@
 from trajectopy_core.trajectory import Trajectory
 from trajectopy_core.utils import Line3D
 
 logger = logging.getLogger("root")
 
 
 def match_trajectories(
-    traj_test: Trajectory,
-    traj_ref: Trajectory,
+    traj_from: Trajectory,
+    traj_to: Trajectory,
     settings: MatchingSettings = MatchingSettings(),
     inplace: bool = True,
 ) -> Tuple[Trajectory, Trajectory]:
     """
     Matches two trajectories using the specified method
+    The test trajectory is matched onto the reference trajectory.
 
     Supported methods:
         - MatchingMethod.INTERPOLATION
         - MatchingMethod.NEAREST_TEMPORAL
         - MatchingMethod.NEAREST_SPATIAL
         - MatchingMethod.NEAREST_SPATIAL_INTERPOLATED
 
     """
-    traj_test = traj_test if inplace else traj_test.copy()
-    traj_ref = traj_ref if inplace else traj_ref.copy()
+    traj_from = traj_from if inplace else traj_from.copy()
+    traj_to = traj_to if inplace else traj_to.copy()
 
     logger.info("Matching trajectories using method %s", settings.method.name)
 
     if settings.method == MatchingMethod.INTERPOLATION:
-        return match_trajectories_interpolation(traj_test=traj_test, traj_ref=traj_ref)
+        return match_trajectories_interpolation(traj_test=traj_from, traj_ref=traj_to)
 
     if settings.method == MatchingMethod.NEAREST_TEMPORAL:
-        return match_trajectories_temporal(traj_test=traj_test, traj_ref=traj_ref, max_distance=settings.max_time_diff)
+        return match_trajectories_temporal(traj_test=traj_from, traj_ref=traj_to, max_distance=settings.max_time_diff)
 
     if settings.method == MatchingMethod.NEAREST_SPATIAL:
-        return match_trajectories_spatial(traj_test=traj_test, traj_ref=traj_ref, max_distance=settings.max_distance)
+        return match_trajectories_spatial(traj_test=traj_from, traj_ref=traj_to, max_distance=settings.max_distance)
 
     if settings.method == MatchingMethod.NEAREST_SPATIAL_INTERPOLATED:
         return match_trajectories_spatial_interpolation(
-            traj_test=traj_test,
-            traj_ref=traj_ref,
+            traj_test=traj_from,
+            traj_ref=traj_to,
             max_distance=settings.max_distance,
             k_nearest=settings.k_nearest,
         )
 
     raise ValueError(f"Matching method {settings.method} not supported!")
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/pipelines.py` & `trajectopy_core-2.7.0/trajectopy_core/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Trajectopy - Trajectory Evaluation in Python
 
 High-level API for trajectory evaluation in Python.
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from typing import List, Tuple, Union
 
 import numpy as np
 from pointset import PointSet
 
 from trajectopy_core.alignment import align_trajectories, apply_alignment
@@ -44,15 +45,15 @@
         trajectory_est (Trajectory): Estimated trajectory.
         settings (ProcessingSettings, optional): Processing settings.
 
     Returns:
         ATEResult: Result of the ATE computation.
 
     """
-    match_trajectories(traj_test=trajectory_est, traj_ref=trajectory_gt, settings=settings.matching)
+    match_trajectories(traj_from=trajectory_est, traj_to=trajectory_gt, settings=settings.matching)
     alignment = align_trajectories(
         traj_from=trajectory_est,
         traj_to=trajectory_gt,
         alignment_settings=settings.alignment,
         matching_settings=settings.matching,
     )
     trajectory_est_aligned = apply_alignment(trajectory=trajectory_est, alignment_result=alignment, inplace=False)
@@ -65,15 +66,15 @@
         else compare_trajectories_absolute(traj_ref=trajectory_gt, traj_test=trajectory_est_aligned)
     )
 
 
 def rpe(
     trajectory_gt: Trajectory, trajectory_est: Trajectory, settings: ProcessingSettings = ProcessingSettings()
 ) -> RPEResult:
-    match_trajectories(traj_test=trajectory_est, traj_ref=trajectory_gt, settings=settings.matching)
+    match_trajectories(traj_from=trajectory_est, traj_to=trajectory_gt, settings=settings.matching)
     return compare_trajectories_relative(
         traj_ref=trajectory_gt, traj_test=trajectory_est, settings=settings.relative_comparison
     )
 
 
 def sort_spatially(
     trajectory: Trajectory, sorting_settings: SortingSettings = SortingSettings(), inplace: bool = True
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/bar_plots.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/bar_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/heatmaps.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/heatmaps.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/histograms.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/line_plots.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/multi_line_plots.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/multi_line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/scatter_plots.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/scatter_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/tables.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/tables.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/plotting/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/alignment.py` & `trajectopy_core-2.7.0/trajectopy_core/report/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/assets/icon.png` & `trajectopy_core-2.7.0/trajectopy_core/report/assets/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/assets/style.css` & `trajectopy_core-2.7.0/trajectopy_core/report/assets/style.css`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/data.py` & `trajectopy_core-2.7.0/trajectopy_core/report/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/multi.py` & `trajectopy_core-2.7.0/trajectopy_core/report/multi.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/single.py` & `trajectopy_core-2.7.0/trajectopy_core/report/single.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/templates/generic.html` & `trajectopy_core-2.7.0/trajectopy_core/report/templates/generic.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/templates/multi_template.html` & `trajectopy_core-2.7.0/trajectopy_core/report/templates/multi_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/templates/single_template.html` & `trajectopy_core-2.7.0/trajectopy_core/report/templates/single_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/trajectory.py` & `trajectopy_core-2.7.0/trajectopy_core/report/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/report/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/report/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/rotationset.py` & `trajectopy_core-2.7.0/trajectopy_core/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/alignment.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     std_z_from: float = 1.0
     std_xy_to: float = 1.0
     std_z_to: float = 1.0
     std_roll_pitch: float = float(np.deg2rad(1.0))
     std_yaw: float = float(np.deg2rad(1.0))
     std_speed: float = 1.0
     error_probability: float = 0.05
+    variance_estimation: bool = False
     variance_component_estimation: bool = False
     variance_component_estimation_subset_size: int = 200
 
     @property
     def var_xy_from(self) -> float:
         return self.std_xy_from**2
 
@@ -278,21 +279,21 @@
             - z_to
             - roll_pitch (platform orientations)
             - yaw
 
     """
 
     preprocessing: AlignmentPreprocessing = field(default_factory=AlignmentPreprocessing)
-    estimation_of: AlignmentEstimationSettings = field(default_factory=AlignmentEstimationSettings)
+    estimation_settings: AlignmentEstimationSettings = field(default_factory=AlignmentEstimationSettings)
     stochastics: AlignmentStochastics = field(default_factory=AlignmentStochastics)
     metric_threshold: float = METRIC_THRESHOLD
     time_threshold: float = TIME_THRESHOLD
 
     def __str__(self) -> str:
-        return str(self.preprocessing) + str(self.estimation_of) + str(self.stochastics)
+        return str(self.preprocessing) + str(self.estimation_settings) + str(self.stochastics)
 
 
 if __name__ == "__main__":
     settings = AlignmentSettings()
     settings.to_file("alignment_settings.json")
     imported_settings = AlignmentSettings.from_file("alignment_settings.json")
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/base.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/base.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/comparison.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/matching.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/matching.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Any
 
 from trajectopy_core.settings.base import Settings
 
 
@@ -24,23 +25,19 @@
     method: MatchingMethod = MatchingMethod.INTERPOLATION
     max_time_diff: float = 0.01
     max_distance: float = 0.00
     k_nearest: int = 10
 
     @staticmethod
     def encoder(name: str, value: Any) -> Any:
-        if name == "method":
-            return value.value
-        return value
+        return value.value if name == "method" else value
 
     @staticmethod
     def decoder(name: str, value: Any) -> Any:
-        if name == "method":
-            return MatchingMethod(value)
-        return value
+        return MatchingMethod(value) if name == "method" else value
 
 
 if __name__ == "__main__":
     settings = MatchingSettings()
     settings.to_file("matching_settings.json")
     imported_settings = MatchingSettings.from_file("matching_settings.json")
```

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/processing.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/processing.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/settings/report.py` & `trajectopy_core-2.7.0/trajectopy_core/settings/report.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/spatialsorter.py` & `trajectopy_core-2.7.0/trajectopy_core/spatialsorter.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/trajectory.py` & `trajectopy_core-2.7.0/trajectopy_core/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/trajectopy_core/utils.py` & `trajectopy_core-2.7.0/trajectopy_core/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.6.1/PKG-INFO` & `trajectopy_core-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy-core
-Version: 2.6.1
+Version: 2.7.0
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 Maintainer: Gereon Tombrink
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trajectopy-core Version: 2.6.1 Summary: Trajectory
+Metadata-Version: 2.1 Name: trajectopy-core Version: 2.7.0 Summary: Trajectory
 Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT Keywords:
 trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Author:
 Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de Maintainer: Gereon
 Tombrink Maintainer-email: tombrink@igg.uni-bonn.de Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

