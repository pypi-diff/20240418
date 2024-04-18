# Comparing `tmp/fpsim-0.22.0.tar.gz` & `tmp/fpsim-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpsim-0.22.0.tar", last modified: Fri Jan 27 20:28:44 2023, max compression
+gzip compressed data, was "fpsim-0.28.1.tar", last modified: Thu Apr 18 07:51:05 2024, max compression
```

## Comparing `fpsim-0.22.0.tar` & `fpsim-0.28.1.tar`

### file list

```diff
@@ -1,90 +1,577 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19034 2023-01-27 20:23:17.000000 fpsim-0.22.0/CHANGELOG.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3474 2022-10-27 01:56:19.000000 fpsim-0.22.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1093 2022-10-27 01:56:19.000000 fpsim-0.22.0/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      226 2022-10-27 01:56:19.000000 fpsim-0.22.0/MANIFEST.in
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9480 2023-01-27 20:28:44.676897 fpsim-0.22.0/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8675 2022-10-28 16:55:59.000000 fpsim-0.22.0/README.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.672897 fpsim-0.22.0/docs/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.analyzers.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.base.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.calibration.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.defaults.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.experiment.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.interventions.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.locations.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      157 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.locations.senegal.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.parameters.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.scenarios.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.settings.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      115 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.sim.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.utils.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/fpsim.version.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      381 2022-10-28 16:14:33.000000 fpsim-0.22.0/docs/index.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      451 2022-10-28 16:48:36.000000 fpsim-0.22.0/docs/modules.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       93 2022-10-27 01:56:19.000000 fpsim-0.22.0/docs/overview.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2022-10-28 16:14:49.000000 fpsim-0.22.0/docs/requirements.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.672897 fpsim-0.22.0/docs/tutorials/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      343 2022-10-28 16:55:59.000000 fpsim-0.22.0/docs/tutorials/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2022-10-28 16:14:33.000000 fpsim-0.22.0/docs/tutorials.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-10-27 01:56:19.000000 fpsim-0.22.0/docs/whatsnew.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      295 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17018 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/analyzers.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20417 2022-10-28 16:14:33.000000 fpsim-0.22.0/fpsim/base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14641 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/calibration.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2852 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/defaults.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    51476 2022-10-28 16:14:33.000000 fpsim-0.22.0/fpsim/experiment.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18012 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/interventions.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim/locations/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       41 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/__init__.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim/locations/data_processing/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3129 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/data_processing/mcpr_by_parity.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      801 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/data_processing/process_matrices.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      964 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/data_processing/sexual_debut_age_probs.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim/locations/kenya/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13647 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/calibrate_manual.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2409 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/explore_plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4577 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_asfr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      479 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_basic_dhs.yaml
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       65 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_bf_stats.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      563 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_cpr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      876 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_popsize.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3224 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_skyscrapers.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      675 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/kenya_tfr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14672 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/matrices_kenya_dhs_2014.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14188 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/matrices_kenya_pma_2019_20.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      495 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/mix_kenya.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2468 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/kenya/mortality_prob_kenya.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      939 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/locations/kenya/mortality_trend_kenya.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      166 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya/use_kenya.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    43999 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/kenya.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim/locations/senegal/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    97222 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/BirthSpacing.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7594 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/Method_v312.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    29123 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/SNIR80FL.obj
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    34632 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/Skyscrapers-All-DHS.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4518 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/senegal/plot_birth_spacing.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/senegal-asfr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      482 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/senegal-basic-dhs.yaml
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       83 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/senegal-mcpr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      871 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/senegal-popsize.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2022-10-28 16:17:08.000000 fpsim-0.22.0/fpsim/locations/senegal/senegal-tfr.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    36510 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/locations/senegal.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20462 2022-12-01 19:28:09.000000 fpsim-0.22.0/fpsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19830 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/scenarios.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19756 2022-10-27 01:56:19.000000 fpsim-0.22.0/fpsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   109620 2022-10-28 16:14:33.000000 fpsim-0.22.0/fpsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7916 2022-10-28 16:14:33.000000 fpsim-0.22.0/fpsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      134 2023-01-27 20:23:17.000000 fpsim-0.22.0/fpsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/fpsim.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9480 2023-01-27 20:28:44.000000 fpsim-0.22.0/fpsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2275 2023-01-27 20:28:44.000000 fpsim-0.22.0/fpsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-01-27 20:28:44.000000 fpsim-0.22.0/fpsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2023-01-27 20:28:44.000000 fpsim-0.22.0/fpsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        6 2023-01-27 20:28:44.000000 fpsim-0.22.0/fpsim.egg-info/top_level.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-01-27 20:28:44.676897 fpsim-0.22.0/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1555 2022-10-28 16:14:33.000000 fpsim-0.22.0/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-01-27 20:28:44.676897 fpsim-0.22.0/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      847 2022-10-27 01:56:19.000000 fpsim-0.22.0/tests/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       30 2022-10-28 16:17:08.000000 fpsim-0.22.0/tests/requirements_test.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.407053 fpsim-0.28.1/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24181 2024-04-17 12:40:46.000000 fpsim-0.28.1/CHANGELOG.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3474 2022-10-27 01:56:19.000000 fpsim-0.28.1/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1093 2023-04-05 04:38:50.000000 fpsim-0.28.1/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      226 2022-10-27 01:56:19.000000 fpsim-0.28.1/MANIFEST.in
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9480 2024-04-18 07:51:05.407053 fpsim-0.28.1/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8675 2023-04-05 04:38:50.000000 fpsim-0.28.1/README.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.355057 fpsim-0.28.1/docs/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.355057 fpsim-0.28.1/docs/_templates/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      512 2024-02-09 17:24:14.000000 fpsim-0.28.1/docs/_templates/custom-class-template.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2024-02-09 17:24:14.000000 fpsim-0.28.1/docs/_templates/custom-function-template.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1294 2024-02-09 17:24:14.000000 fpsim-0.28.1/docs/_templates/custom-module-template.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.355057 fpsim-0.28.1/docs/api/
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.387055 fpsim-0.28.1/docs/api/_autosummary/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.Analyzer.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      230 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.age_pyramids.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      248 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.education_recorder.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      254 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.empowerment_recorder.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      346 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.analyzers.snapshot.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      509 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.base.BasePeople.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      320 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.base.BaseSim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      208 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.base.ParsObj.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      275 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.base.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      227 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.calibration.Calibration.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      269 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.calibration.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.defaults.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      223 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.experiment.Experiment.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      202 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.experiment.Fit.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.experiment.compute_gof.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.experiment.diff_summaries.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      451 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.experiment.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      232 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.interventions.Intervention.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      228 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.interventions.change_par.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      314 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.interventions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      240 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.interventions.update_methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      157 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.calibration_scripts.calibrate_auto.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      163 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.calibration_scripts.calibrate_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      484 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.calibration_scripts.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      112 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.barriers.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      135 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.debut_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      129 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      115 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.lactational_amenorrhea.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      168 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      115 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      895 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      112 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.sexual_activity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      135 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.sexual_activity_pp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      158 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      155 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      149 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      135 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      167 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      161 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      188 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      135 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      816 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      178 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      167 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.addis_ababa.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      131 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      137 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      137 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      160 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      154 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      117 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      181 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      146 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      146 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      793 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      171 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      160 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      120 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.afar.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      183 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      799 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.amhara.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      161 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      155 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      167 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      194 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      834 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      184 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.benishangul_gumuz.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      153 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      165 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      186 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      151 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      116 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      151 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      810 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      176 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      165 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.dire_dawa.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      189 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.ethiopia_regions_multisim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      134 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      151 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      131 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      163 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      157 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      120 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      143 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      184 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      149 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      131 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      149 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      802 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      128 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      174 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      163 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      143 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.gambela.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      183 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      799 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.harari.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      183 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      799 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.oromia.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      801 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      149 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      143 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      129 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      161 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      155 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      182 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      120 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      129 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      112 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      796 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      172 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      161 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      141 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.snnpr.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      183 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      799 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.somali.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.barriers_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.debut_age_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      119 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      183 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.lactational_amenorrhea_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      113 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      125 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.region_proportions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      799 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      173 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.sexual_activity_pp_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      162 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.sexual_activity_region.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      122 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.ethiopia_regions.tigray.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      115 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.age_partnership.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       98 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.barriers.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.debut_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.education_attainment.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.education_distributions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      147 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.education_dropout_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.education_objective.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_decision_health.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      156 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_decision_wages.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      151 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_distributions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_paid_employment.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_regression_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.empowerment_sexual_autonomy.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      112 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      138 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      101 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.lactational_amenorrhea.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      112 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      107 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1055 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.sexual_activity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.sexual_activity_pp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.kenya.urban_proportion.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      374 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      117 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.age_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.age_pyramid.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      100 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.barriers.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      134 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.birth_spacing_pref.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.data2interp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.debut_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.exposure_age.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.exposure_parity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      146 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.fecundity_ratio_nullip.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      140 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.female_age_fecundity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      103 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.filenames.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      126 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.infant_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      144 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.lactational_amenorrhea.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      105 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.make_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      132 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.maternal_mortality.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      114 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.method_probs.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.methods.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      109 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.miscarriage.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      702 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      111 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.scalar_pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      123 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.sexual_activity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      134 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.sexual_activity_pp.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.locations.senegal.stillbirth.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      205 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.parameters.Pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       81 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.parameters.pars.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      407 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.parameters.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      216 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.scenarios.Scenario.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      219 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.scenarios.Scenarios.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       97 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.scenarios.make_scen.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      429 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.scenarios.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      110 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.settings.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      210 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.sim.MultiSim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      460 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.sim.People.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      295 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.sim.Sim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       86 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.sim.parallel.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      417 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.sim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       70 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.bc.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       70 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.bt.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.match_ages.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       70 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.mt.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       73 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.rbt.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      320 2024-04-16 07:34:57.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       82 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.sample.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2024-04-16 07:34:58.000000 fpsim-0.28.1/docs/api/_autosummary/fpsim.utils.set_seed.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      477 2024-04-17 05:45:09.000000 fpsim-0.28.1/docs/api/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      387 2024-02-09 17:24:14.000000 fpsim-0.28.1/docs/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       90 2024-02-09 17:24:14.000000 fpsim-0.28.1/docs/overview.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      250 2024-04-17 05:45:09.000000 fpsim-0.28.1/docs/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.387055 fpsim-0.28.1/docs/tutorials/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      343 2023-04-05 04:38:50.000000 fpsim-0.28.1/docs/tutorials/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      175 2023-04-05 04:38:50.000000 fpsim-0.28.1/docs/tutorials.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2023-04-05 04:38:50.000000 fpsim-0.28.1/docs/whatsnew.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.391054 fpsim-0.28.1/fpsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      345 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20628 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/analyzers.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23393 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14638 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/calibration.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7903 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/defaults.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12848 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/empowerment.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    48697 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/experiment.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18012 2023-09-12 23:55:06.000000 fpsim-0.28.1/fpsim/interventions.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.391054 fpsim-0.28.1/fpsim/locations/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      515 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/__init__.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.391054 fpsim-0.28.1/fpsim/locations/data_processing/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9070 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/data_processing/UN_data_scraping.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6799 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/data_processing/WorldBank_data_scraping.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    39298 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/data_processing/countries.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16186 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/data_processing/country_codes.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3129 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/data_processing/mcpr_by_parity.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      801 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/data_processing/process_matrices.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      964 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/data_processing/sexual_debut_age_probs.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.395054 fpsim-0.28.1/fpsim/locations/ethiopia/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       25 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/ethiopia/afb.median.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    92129 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/ethiopia/afb.table.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4875 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/locations/ethiopia/ageparity.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4757 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/asfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      469 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/basic_dhs.yaml
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8287 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/ethiopia/birth_spacing_dhs.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      822 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/cpr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14089 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/ethiopia/matrices_ethiopia_dhs_2008_11.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      335 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/locations/ethiopia/mix.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2508 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/mortality_prob.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      962 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/mortality_trend.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      892 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/popsize.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      319 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/pyramid.csv
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.395054 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12619 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/asfr_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1530 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/barriers_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      723 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/bf_stats_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    81423 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/birth_spacing_dhs_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1299 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/counseling_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2576 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/lam_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    69671 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/mix_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4372 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/pyramid_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      353 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5473 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/sexual_activity_pp_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2336 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/sexual_activity_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5569 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/sexual_debut_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4227 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/tfr_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19787 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia/subnational_data/use_region.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      666 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/tfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       35 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/locations/ethiopia/urban.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      157 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/ethiopia/use.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    49958 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.399054 fpsim-0.28.1/fpsim/locations/ethiopia_regions/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       21 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23334 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/addis_ababa.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23318 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/afar.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23178 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/amhara.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23426 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/benishangul_gumuz.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23263 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/dire_dawa.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      705 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/ethiopia_regions_multisim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23216 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/gambela.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23191 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/harari.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23271 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/oromia.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23238 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/snnpr.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23175 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/somali.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23245 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/ethiopia_regions/tigray.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.403053 fpsim-0.28.1/fpsim/locations/kenya/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       26 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/afb.median.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   470740 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/afb.table.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      963 2023-09-12 23:01:00.000000 fpsim-0.28.1/fpsim/locations/kenya/age_partnership.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3224 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/locations/kenya/ageparity.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4211 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/asfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      479 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/basic_dhs.yaml
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       65 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/bf_stats.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9932 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/birth_spacing_dhs.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      789 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/cpr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2781 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/edu_initialization.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1304 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/edu_objective.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1333 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/edu_stop.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5421 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/empowerment.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2409 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/explore_plotting.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      675 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/kenya_tfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16018 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/kenya/matrices_kenya_dhs_2014.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16699 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/kenya/matrices_kenya_pma_2019_20_21.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      469 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/mix.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2468 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/mortality_prob.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      939 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/mortality_trend.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5832 2023-04-05 04:38:50.000000 fpsim-0.28.1/fpsim/locations/kenya/optimize-space-prefs-kenya.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      876 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/popsize.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       55 2023-09-12 23:01:00.000000 fpsim-0.28.1/fpsim/locations/kenya/urban.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      166 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/kenya/use.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    57327 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/kenya.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.407053 fpsim-0.28.1/fpsim/locations/senegal/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    34632 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/locations/senegal/Age-parity-All-DHS.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    97222 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/BirthSpacing.obj
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7594 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/Method_v312.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    29123 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/SNIR80FL.obj
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       26 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/afb.median.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   131637 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/afb.table.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    27913 2024-03-15 03:45:39.000000 fpsim-0.28.1/fpsim/locations/senegal/ageparity.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4716 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/asfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      482 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/basic_dhs.yaml
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7602 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/birth_spacing_dhs.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      589 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/cpr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14384 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/matrices_senegal_dhs_2017_18.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      362 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/mix.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5502 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/optimize-space-prefs.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4518 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/plot_birth_spacing.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      842 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/popsize.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       92 2023-08-07 23:03:23.000000 fpsim-0.28.1/fpsim/locations/senegal/senegal-asfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       74 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/senegal-mcpr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      129 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/senegal-tfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      843 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/tfr.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       54 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/locations/senegal/urban.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      159 2024-02-09 17:24:14.000000 fpsim-0.28.1/fpsim/locations/senegal/use.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    33062 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/locations/senegal.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    26361 2024-04-18 07:50:39.000000 fpsim-0.28.1/fpsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    47440 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19830 2023-09-12 23:55:06.000000 fpsim-0.28.1/fpsim/scenarios.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19756 2023-09-12 23:55:06.000000 fpsim-0.28.1/fpsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67697 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3900 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/subnational.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12859 2024-04-17 05:45:09.000000 fpsim-0.28.1/fpsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      136 2024-04-17 12:40:46.000000 fpsim-0.28.1/fpsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.391054 fpsim-0.28.1/fpsim.egg-info/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9480 2024-04-18 07:51:05.000000 fpsim-0.28.1/fpsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    36451 2024-04-18 07:51:05.000000 fpsim-0.28.1/fpsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-18 07:51:05.000000 fpsim-0.28.1/fpsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      106 2024-04-18 07:51:05.000000 fpsim-0.28.1/fpsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        6 2024-04-18 07:51:05.000000 fpsim-0.28.1/fpsim.egg-info/top_level.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-18 07:51:05.407053 fpsim-0.28.1/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1555 2023-04-05 04:38:50.000000 fpsim-0.28.1/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 07:51:05.407053 fpsim-0.28.1/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      847 2022-10-27 01:56:19.000000 fpsim-0.28.1/tests/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       30 2023-04-05 04:38:50.000000 fpsim-0.28.1/tests/requirements_test.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2227 2024-02-09 17:24:14.000000 fpsim-0.28.1/tests/test_analyzers.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4804 2024-04-17 05:45:09.000000 fpsim-0.28.1/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      751 2023-04-05 04:38:50.000000 fpsim-0.28.1/tests/test_experiment.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4095 2023-04-05 04:38:50.000000 fpsim-0.28.1/tests/test_interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1101 2022-10-27 01:56:19.000000 fpsim-0.28.1/tests/test_multisim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4704 2023-04-05 04:38:50.000000 fpsim-0.28.1/tests/test_other.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6959 2024-04-17 05:45:09.000000 fpsim-0.28.1/tests/test_parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15195 2023-04-05 04:38:50.000000 fpsim-0.28.1/tests/test_scenarios.py
```

### Comparing `fpsim-0.22.0/CHANGELOG.rst` & `fpsim-0.28.1/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,128 @@
 
 All notable changes to the codebase are documented in this file. Changes that may result in differences in model output, or are required in order to run an old parameter set with the current version, are flagged with the term "Regression information".
 
 .. contents:: **Contents**
    :local:
    :depth: 1
 
+Version 0.28.1 (2024-04-11)
+---------------------------
+- Updates regional parameters to calibrate subnationally in Ethiopia
+- Revises subnational calibration script to run for all regions and includes a new multisim script for subnational comparisons 
+- *GitHub info*: PR `https://github.com/fpsim/fpsim/pull/319>`_
+
+Version 0.27.0 (2024-02-09)
+---------------------------
+- Builds out new regional attribute and parameters for subnational dynamics in Ethiopia
+- Creates new subnational calibration script and subfolder for regional datasets and figures 
+- *GitHub info*: PR `https://github.com/fpsim/fpsim/pull/241>`_
+
+Version 0.26.8 (2024-02-08)
+---------------------------
+- Removed unused ``timeseries_recorder`` and ``verbose_sim`` analyzers.
+- *GitHub info*: PR `257 <https://github.com/fpsim/fpsim/pull/257>`_
+
+Version 0.26.7 (2023-10-24)
+---------------------------
+- Created two scripts in data_processing dir to scrape UN and World Bank country calibration data
+- Updated location_template.txt with logic to pull this scraped data for future contexts
+- *GitHub info*: PR `213 <https://github.com/fpsim/fpsim/pull/213>`_
+
+Version 0.26.6 (2023-9-27)
+--------------------------
+- Renamed the country data filenames to be standardized across contexts
+- Updated references to these updated country data files
+- *GitHub info*: PR `196 <https://github.com/fpsim/fpsim/pull/196>`_
+
+Version 0.26.5 (2023-9-27)
+--------------------------
+- Adds Tutorial for manual calibration to docs/tutorials/ directory
+- *GitHub info*: PR `166 <https://github.com/fpsim/fpsim/pull/166>`_
+
+Version 0.26.4 (2023-9-27)
+--------------------------
+- Refactoring of Experiment class to run with the latest country data formats
+- Country files have updated references to these updated country data files
+- Senegal country data files updated to latest standard format (based on Kenya)
+- *GitHub info*: PR `193 <https://github.com/fpsim/fpsim/pull/193>`_
+
+Version 0.26.3 (2023-9-27)
+--------------------------
+- Updates Senegal files in locations/senegal to be in the same format as Kenya for standardization purposes
+- Minor updates to calibrate_manual.py to be able to run with Senegal data (in addition to Kenya and other contexts)
+- *GitHub info*: PR `165 <https://github.com/fpsim/fpsim/pull/165>`_
+
+Version 0.26.2 (2023-7-25)
+--------------------------
+- Updates code for manual calibration
+- Adds folder to create figures for manual calibration runs
+- *GitHub info*: PR `164 <https://github.com/fpsim/fpsim/pull/164>`_
+
+Version 0.26.1 (2023-6-29)
+--------------------------
+- Updates code for contraceptive matrices
+- Adds contraceptive matrices for Ethiopia to run manual calibration
+- *GitHub info*: PR `161 <https://github.com/fpsim/fpsim/pull/161>`_
+
+Version 0.26.0 (2023-5-31)
+--------------------------
+- Builds out new parameters file for Ethiopia
+- Adds camparison data for Ethiopia calibration
+- *GitHub info*: PR `156 <https://github.com/fpsim/fpsim/pull/156>`_
+
+Version 0.25.0 (2023-5-13)
+--------------------------
+- Adds to sim.py to track sexual inactivity in agents
+- Restricts method use to only those women sexually active over the last 12 months and debuted
+- *GitHub info*: PR `157 <https://github.com/fpsim/fpsim/pull/157>`_
+
+Version 0.24.1 (2023-4-14)
+--------------------------
+- Fixes example_calib.py and example_exp.py to run with fpsim library
+- Updates manual_calibration.py to be flexible to take any location with identically structured data as Kenya
+- *GitHub info*: PR `133 <https://github.com/fpsim/fpsim/pull/133>`_
+
+Version 0.24.0 (2023-3-17)
+--------------------------
+- Finish a manual calibration script for plotting model outcomes vs data for Kenya
+- Goal is to make this script more flexible for other locations, still needs some tweaks for data import
+- Compares ASFR, TFR, age/parity mix, contraceptive use and mix, CPR, pop growth rate, age at first birth, and birth spacing bins
+- *GitHub info*: PR `133 <https://github.com/fpsim/fpsim/pull/133>`_
+
+Version 0.23.2 (2023-3-6)
+--------------------------
+- Add duration of a short birth interval between live births (short_int) to senegal.py
+- Track number of short interval births an agent has had over their life and number are happening at each time step in sim.py 
+- Add age limit parameters (age_low, age_high) to senegal.py to track age-specific short interval births.
+- Create a time series plot of all short births interval during a sim as well as the age-specific time series.
+- *GitHub info*: PR `107 <https://github.com/fpsim/fpsim/pull/107>`_
+
+Version 0.23.1 (2023-2-28)
+--------------------------
+- Add location folder for Ethiopia calibration
+- Add comparison data to Ethiopia folder
+- *GitHub info*: PR `118 <https://github.com/fpsim/fpsim/pull/118>`_
+
+Version 0.23.0 (2023-2-10)
+--------------------------
+- Add optimize-space-prefs.py using Calibration class to algorithmically find best birth space params
+- *GitHub info*: PR `119 <https://github.com/fpsim/fpsim/pull/119>`_
+
+Version 0.22.1 (2023-2-03)
+--------------------------
+- Update contraceptive matrices to be weighted
+- *GitHub info*: PR `113 <https://github.com/fpsim/fpsim/pull/113>`_
+
+
 Version 0.22.0 (2023-1-24)
 --------------------------
 - Add calibrate_manual.py to compare sim runs to data with new data structures
 - Add plot_birth_spacing.py under senegal location to fine tune this calibration
-- *GitHub info*: PR `https://github.com/fpsim/fpsim/pull/109>`_
+- *GitHub info*: PR `109 <https://github.com/fpsim/fpsim/pull/109>`_
 
 Version 0.21.2 (2022-12-16)
 ---------------------------
 - Updates Kenya, 2nd pass, completed 1st draft
 - Starts calibrate_manual.py for Kenya with ASFR plot
 - *GitHub info*: PR `76 <https://github.com/fpsim/fpsim/pull/76>`_
```

### Comparing `fpsim-0.22.0/CODE_OF_CONDUCT.rst` & `fpsim-0.28.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/LICENSE` & `fpsim-0.28.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/PKG-INFO` & `fpsim-0.28.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpsim
-Version: 0.22.0
+Version: 0.28.1
 Summary: FPsim: Family Planning Simulator
 Home-page: http://fpsim.org
 Author: Michelle O'Brien, Annie Valente, Cliff Kerr, Sam Buxton, Daniel Klein, Marita Zimmermann
 Author-email: info@fpsim.org
 Keywords: family planning,women's health,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `fpsim-0.22.0/README.rst` & `fpsim-0.28.1/README.rst`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/base.py` & `fpsim-0.28.1/fpsim/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 '''
 Base classes for loading parameters and for running simulations with FP model
 '''
-
 import numpy as np
 import pandas as pd
 import sciris as sc
 import pylab as pl
 from . import utils as fpu
 from . import defaults as fpd
 
 obj_get = object.__getattribute__ # Alias the default getattribute method
 obj_set = object.__setattr__
 
 
 __all__ = ['ParsObj', 'BasePeople', 'BaseSim']
+__all__ += ['ndict']
+
 
 
 class FlexPretty(sc.prettyobj):
     '''
     A class that supports multiple different display options: namely obj.brief()
     for a one-line description and obj.disp() for a full description.
     '''
@@ -205,18 +206,15 @@
                 newpeople[key] = np.concatenate([npval, p2val], axis=0)
             elif isinstance(npval, list):
                 newpeople[key] += p2val
             else:
                 errormsg = f'Not sure what to do with object of type {type(npval)}'
                 raise TypeError(errormsg)
 
-        # Validate
-        for key in keys:
-            assert len(newpeople[key]) == len(newpeople)
-        newpeople.uid[n_orig:] = max_uid + np.arange(n_new) # Reassign UIDs so they're unique
+        newpeople.uid[n_orig:] = max_uid + np.arange(n_new)  # Reassign UIDs so they're unique
 
         return newpeople
 
 
     def __radd__(self, people2):
         ''' Allows sum() to work correctly '''
         if not people2: return self
@@ -307,36 +305,37 @@
 
 
     def filter(self, criteria=None, inds=None):
         '''
         Store indices to allow for easy filtering of the People object.
 
         Args:
-            criteria (array): a boolean array for the filtering critria
+            criteria (bool array): a boolean array for the filtering critria
             inds (array): alternatively, explicitly filter by these indices
 
         Returns:
             A filtered People object, which works just like a normal People object
             except only operates on a subset of indices.
         '''
 
         # Create a new People object with the same properties as the original
         filtered = object.__new__(self.__class__) # Create a new People instance
         BasePeople.__init__(filtered) # Perform essential initialization
-        filtered.__dict__ = {k:v for k,v in self.__dict__.items()} # Copy pointers to the arrays in People
+        filtered.__dict__ = sc.cp(self.__dict__) # Copy pointers to the arrays in People
 
         # Perform the filtering
         if criteria is None: # No filtering: reset
             filtered._inds = None
             if inds is not None: # Unless indices are supplied directly, in which case use them
                 filtered._inds = inds
         else: # Main use case: perform filtering
-            if len(criteria) == len(self): # Main use case: a new filter applied on an already filtered object, e.g. filtered.filter(filtered.age > 5)
+            len_criteria = len(criteria)
+            if len_criteria == self.len_inds: # Main use case: a new filter applied on an already filtered object, e.g. filtered.filter(filtered.age > 5)
                 new_inds = criteria.nonzero()[0] # Criteria is already filtered, just get the indices
-            elif len(criteria) == self.len_people: # Alternative: a filter on the underlying People object is applied to the filtered object, e.g. filtered.filter(people.age > 5)
+            elif len_criteria == self.len_people: # Alternative: a filter on the underlying People object is applied to the filtered object, e.g. filtered.filter(people.age > 5)
                 new_inds = criteria[filtered.inds].nonzero()[0] # Apply filtering before getting the new indices
             else:
                 errormsg = f'"criteria" must be boolean array matching either current filter length ({self.len_inds}) or else the total number of people ({self.len_people}), not {len(criteria)}'
                 raise ValueError(errormsg)
             if filtered.inds is None: # Not yet filtered: use the indices directly
                 filtered._inds = new_inds
             else: # Already filtered: map them back onto the original People indices
@@ -550,7 +549,100 @@
 
     def get_analyzer(self, label=None, partial=False, first=False, die=True):
         '''
         Same as get_intervention(), but for analyzers.
         '''
         return self._get_ia('analyzers', label=label, partial=partial, first=first, die=die, as_inds=False, as_list=False)
 
+
+class ndict(sc.objdict):
+    """
+    A dictionary-like class that provides additional functionalities for handling named items.
+
+    Args:
+        name (str): The items' attribute to use as keys.
+        type (type): The expected type of items.
+        strict (bool): If True, only items with the specified attribute will be accepted.
+        duplicates (bool): If True, it accepts duplicated keys an renames the using enumeration. Default: False.
+
+    **Examples**::
+
+        networks = ss.ndict(ss.mf(), ss.maternal())
+        networks = ss.ndict([ss.mf(), ss.maternal()])
+        networks = ss.ndict({'mf':ss.mf(), 'maternal':ss.maternal()})
+
+    """
+
+    def __init__(self, *args, name='name', type=None, strict=True, **kwargs):
+        self.setattribute('_name', name)  # Since otherwise treated as keys
+        self.setattribute('_type', type)
+        self.setattribute('_strict', strict)
+
+        self._initialize(*args, **kwargs)
+        return
+
+    def append(self, arg, key=None):
+        valid = False
+        if arg is None:
+            return  # Nothing to do
+        elif hasattr(arg, self._name):
+            key = key or getattr(arg, self._name)
+            valid = True
+        elif isinstance(arg, dict):
+            if self._name in arg:
+                key = key or arg[self._name]
+                valid = True
+            else:
+                for k, v in arg.items():
+                    self.append(v, key=k)
+                valid = None  # Skip final processing
+        elif not self._strict:
+            key = key or f'item{len(self) + 1}'
+            valid = True
+        else:
+            valid = False
+
+        if valid is True:
+            self._check_type(arg)
+            # Check if this key already exists
+            if key in self:
+                raise fpu.DuplicateNameException(self[key])
+            self[key] = arg
+        elif valid is None:
+            pass  # Nothing to do
+        else:
+            errormsg = f'Could not interpret argument {arg}: does not have expected attribute "{self._name}"'
+            raise ValueError(errormsg)
+
+        return
+
+    def _check_type(self, arg):
+        """ Check types """
+        if self._type is not None:
+            if not isinstance(arg, self._type):
+                errormsg = f'The following item does not have the expected type {self._type}:\n{arg}'
+                raise TypeError(errormsg)
+        return
+
+    def _initialize(self, *args, **kwargs):
+        args = sc.mergelists(*args)
+        for arg in args:
+            self.append(arg)
+        for key, arg in kwargs.items():
+            self.append(arg, key=key)
+        return
+
+    def copy(self):
+        new = self.__class__.__new__(name=self._name, type=self._type, strict=self._strict)
+        new.update(self)
+        return new
+
+    def __add__(self, dict2):
+        """ Allow c = a + b """
+        new = self.copy()
+        new.append(dict2)
+        return new
+
+    def __iadd__(self, dict2):
+        """ Allow a += b """
+        self.append(dict2)
+        return self
```

### Comparing `fpsim-0.22.0/fpsim/calibration.py` & `fpsim-0.28.1/fpsim/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             return exp.fit.mismatch
 
 
     def run_trial(self, trial):
         ''' Define the objective for Optuna '''
         pars = {}
         for key, (best,low,high) in self.calib_pars.items():
-            pars[key] = trial.suggest_uniform(key, low, high) # Sample from beta values within this range
+            pars[key] = trial.suggest_float(key, low, high) # Sample from beta values within this range
         mismatch = self.run_exp(pars)
         return mismatch
 
 
     def worker(self):
         ''' Run a single worker '''
         study = op.load_study(storage=self.g.storage, study_name=self.g.name)
@@ -175,15 +175,14 @@
 
 
     def run_workers(self):
         ''' Run multiple workers in parallel '''
         output = sc.parallelize(self.worker, self.g.n_workers)
         return output
 
-
     def remove_db(self):
         '''
         Remove the database file if keep_db is false and the path exists.
         '''
         if os.path.exists(self.g.db_name):
             os.remove(self.g.db_name)
             if self.verbose:
```

### Comparing `fpsim-0.22.0/fpsim/experiment.py` & `fpsim-0.28.1/fpsim/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,23 @@
 
 __all__ = ['Experiment', 'Fit', 'compute_gof', 'diff_summaries']
 
 # ...more settings
 min_age = 15
 max_age = 50
 bin_size = 5
-year_str = '2017'
-mpy = 12 # Months per year
+first_birth_age = 25  # age to start assessing first birth age in model
+mpy = 12  # Months per year
 
 # Flags for what to run
 default_flags = sc.objdict(
     popsize       = 1, # Population size and growth over time on whole years, adjusted for n number of agents; 'pop_size'
-    skyscrapers   = 1, # Population distribution of agents in each age/parity bin (skyscraper plot); 'skyscrapers'
+    ageparity   = 1, # Population distribution of agents in each age/parity bin (age-parity plot); 'ageparity'
     first_birth   = 1, # Age at first birth mean with standard deviation; 'age_first_birth'
     birth_space   = 1, # Birth spacing both in bins and mean with standard deviation; 'spacing'
-    age_pregnancy = 1, # Summary stats (mean, std, 25, 50, 75%) ages of those currently pregnant; 'age_pregnant_stats',
     mcpr          = 1, # Modern contraceptive prevalence; 'mcpr'
     methods       = 1, # Overall percentage of method use and method use among users; 'methods'
     mmr           = 1, # Maternal mortality ratio at end of sim in model vs data; 'maternal_mortality_ratio'
     infant_m      = 1, # Infant mortality rate at end of sim in model vs data; 'infant_mortality_rate'
     cdr           = 1, # Crude death rate at end of sim in model vs data; 'crude_death_rate'
     cbr           = 1, # Crude birth rate (per 1000 inhabitants); 'crude_birth_rate'
     tfr           = 1, # Total fertility rate
@@ -86,34 +85,35 @@
     def extract_data(self):
         ''' Load data '''
 
         json = self.load_data('basic_dhs')
 
         self.data.update(json)
 
-        self.data['pregnancy_parity'] = self.load_data('pregnancy_parity')
+        #self.data['pregnancy_parity'] = self.load_data('pregnancy_parity')
 
         # Extract population size over time
         if self.pars:
             n = self.pars['n_agents']
         else:
             n = 1000 # Use default if not available
             print(f'Warning: parameters not defined, using default of n={n}')
         pop_size = self.load_data('popsize')
         self.data['pop_years'] = pop_size.year.to_numpy()
-        self.data['pop_size']  = pop_size.popsize.to_numpy() / (pop_size.popsize[0] / n)  # Corrected for # of agents, needs manual adjustment for # agents
+        self.data['pop_size']  = pop_size.population.to_numpy() / (pop_size.population[0] / n)  # Corrected for # of agents, needs manual adjustment for # agents
 
         # Extract population growth rate
         data_growth_rate = self.pop_growth_rate(self.data['pop_years'], self.data['pop_size'])
         self.data['pop_growth_rate'] = data_growth_rate
 
         # Extract mcpr over time
         mcpr = self.load_data('mcpr')
         self.data['mcpr_years'] = mcpr.iloc[:,0].to_numpy()
-        self.data['mcpr'] = mcpr.iloc[:,1].to_numpy()
+        #self.data['cpr'] = mcpr.iloc[:,1].to_numpy()
+        self.data['mcpr'] = mcpr.iloc[:,2].to_numpy()
 
         self.initialized = True
 
         return
 
 
     def pop_growth_rate(self, years, population):
@@ -143,18 +143,14 @@
         return
 
 
     def post_process_sim(self):
         self.people = self.sim.people  # Extract people objects from sim
         self.model_results = self.sim.results  # Stores dictionary of results
 
-        # Store dataframe of agent's age, pregnancy status, and parity
-        model_pregnancy_parity = self.sim.store_postpartum()
-        model_pregnancy_parity = model_pregnancy_parity.drop(['PP0to5', 'PP6to11', 'PP12to23', 'NonPP'], axis=1)
-        self.model['pregnancy_parity'] = model_pregnancy_parity
         self.method_keys = list(self.sim['methods']['map'].keys())
         return
 
 
     def extract_model(self):
         if self.flags.popsize:  self.model_pop_size()
         if self.flags.mcpr:     self.model_mcpr()
@@ -242,16 +238,20 @@
         return
 
 
     def model_data_asfr(self, ind=-1):
 
         # Extract ASFR for different age bins
         asfr = self.load_data('asfr')  # From DHS
-        self.data['asfr_bins'] = list(asfr.iloc[:, 0])
-        self.data['asfr']      = asfr.iloc[:, 1].to_numpy()
+        age_bins = list(asfr.columns)
+        age_bins.remove('year')
+        self.data['asfr_bins'] = age_bins
+
+        year_data = asfr[asfr['year'] == self.pars['end_year']]
+        self.data['asfr'] = year_data.drop(['year'], axis=1).values.tolist()[0]
 
         # Model extraction
         age_bins = list(fpd.age_bin_map.keys())
         self.model['asfr_bins'] = age_bins
         self.model['asfr'] = []
         for ab in age_bins:
             val = self.model_results['asfr'][ab][ind] # Only use one index (default: last) CK: TODO: match year automatically
@@ -259,171 +259,174 @@
 
         # Check
         assert self.data['asfr_bins'] == self.model['asfr_bins'], f'ASFR data age bins do not match sim: {sc.strjoin(age_bins)}'
 
         return
 
 
-    def extract_skyscrapers(self):
+    def extract_ageparity(self):
 
         # Set up
-        min_age = 15 # CK: TODO: remove hardcoding
-        max_age = 50
-        bin_size = 5
+        age_keys = list(fpd.age_bin_map.keys())[1:]
         age_bins = pl.arange(min_age, max_age, bin_size)
-        parity_bins = pl.arange(0, 7)
+        parity_bins = pl.arange(0, 7)  # Plot up to parity 6
         n_age = len(age_bins)
         n_parity = len(parity_bins)
-        x_age = pl.arange(n_age)
 
-        # Load data
-        data_parity_bins = pl.arange(0, 18) # CK: TODO: refactor
-        sky_raw_data = self.load_data('skyscrapers')
-        sky_raw_data = sky_raw_data[sky_raw_data.year == year_str]
+        # Load data TO NOTE: By default, the dataset that is used for comparison with the model is the last dataset (
+        # typically the most recent) in the ageparity file
+        sky_raw_data = self.load_data('ageparity')
+        dataset = sky_raw_data.iloc[-1]['dataset']
+        sky_raw_data = sky_raw_data[sky_raw_data.dataset == dataset]
         # sky_parity = sky_raw_data[2].to_numpy() # Not used currently
-        sky_props = sky_raw_data.percentage.to_numpy()
+        sky_parity = sky_raw_data['parity'].to_numpy()
+        sky_props = sky_raw_data['percentage'].to_numpy()
         sky_arr = sc.odict()
 
-        sky_arr['Data'] = pl.zeros((len(age_bins), len(parity_bins)))
-        count = -1
-        for age_bin in x_age:
-            for dpb in data_parity_bins:
-                count += 1
-                parity_bin = min(n_parity - 1, dpb)
-                sky_arr['Data'][age_bin, parity_bin] += sky_props[count]
-        assert count == len(sky_props) - 1  # Ensure they're the right length
+        sky_arr['Data'] = pl.zeros((len(age_keys), len(parity_bins)))
+
+        for age, row in sky_raw_data.iterrows():
+            if row.age in age_keys and row.parity < n_parity:
+                age_ind = age_keys.index(row.age)
+                sky_arr['Data'][age_ind, row.parity] = row.percentage
 
         # Extract from model
         sky_arr['Model'] = pl.zeros((len(age_bins), len(parity_bins)))
         ppl = self.people
         for i in range(len(ppl)):
             if ppl.alive[i] and not ppl.sex[i] and ppl.age[i] >= min_age and ppl.age[i] < max_age:
                 age_bin = sc.findinds(age_bins <= ppl.age[i])[-1]
                 parity_bin = sc.findinds(parity_bins <= ppl.parity[i])[-1]
                 sky_arr['Model'][age_bin, parity_bin] += 1
 
         # Normalize
         for key in ['Data', 'Model']:
             sky_arr[key] /= sky_arr[key].sum() / 100
 
-        self.data['skyscrapers'] = sky_arr['Data']
-        self.model['skyscrapers'] = sky_arr['Model']
+        self.data['ageparity'] = sky_arr['Data']
+        self.model['ageparity'] = sky_arr['Model']
         self.age_bins = age_bins
         self.parity_bins = parity_bins
 
         return
 
-
     def extract_birth_spacing(self):
 
+        # Set up
+        data_afb = self.load_data('afb')
+        data_afb = data_afb.sort_values(by='afb')
+        data_spaces = self.load_data('spacing')
+        data_spaces = data_spaces.sort_values(by='space_mo')
         spacing_bins = sc.odict({'0-12': 0, '12-24': 1, '24-48': 2, '>48': 4})  # Spacing bins in years
-
-        # From data
-        data = self.load_data('spacing')
-        spacing, first = data['spacing'], data['first']
-        data_spacing_counts = sc.odict().make(keys=spacing_bins.keys(), vals=0.0)
-
-        # Spacing bins from data
-        spacing_bins_array = sc.cat(spacing_bins[:], np.inf)
-        for i in range(len(spacing_bins_array)-1):
-            lower = spacing_bins_array[i]
-            upper = spacing_bins_array[i+1]
-            matches = np.intersect1d(sc.findinds(spacing >= lower), sc.findinds(spacing < upper))
-            data_spacing_counts[i] += len(matches)
-
-        data_spacing_counts[:] /= data_spacing_counts[:].sum()
-        data_spacing_counts[:] *= 100
-        data_spacing_stats = np.array([pl.percentile(spacing, 25),
-                                        pl.percentile(spacing, 50),
-                                        pl.percentile(spacing, 75)])
-        data_age_first_stats = np.array([pl.percentile(first, 25),
-                                          pl.percentile(first, 50),
-                                          pl.percentile(first, 75)])
-
-        # Save to dictionary
-        self.data['spacing_bins'] = np.array(data_spacing_counts.values())
-        self.data['spacing_stats'] = data_spacing_stats
-        self.data['age_first_stats'] = data_age_first_stats
-
-        # From model
         model_age_first = []
         model_spacing = []
         model_spacing_counts = sc.odict().make(keys=spacing_bins.keys(), vals=0.0)
+        data_spacing_counts = sc.odict().make(keys=spacing_bins.keys(), vals=0.0)
         ppl = self.people
-        for i in  range(len(ppl)):
-            if ppl.alive[i] and not ppl.sex[i] and ppl.age[i] >= min_age and ppl.age[i] < max_age:
+
+        # Extract age at first birth and birth spaces from model
+        for i in range(len(ppl)):
+            if ppl.alive[i] and not ppl.sex[i] and min_age <= ppl.age[i] < max_age:
                 if len(ppl.dobs[i]):
                     model_age_first.append(ppl.dobs[i][0])
                 if len(ppl.dobs[i]) > 1:
                     for d in range(len(ppl.dobs[i]) - 1):
                         space = ppl.dobs[i][d + 1] - ppl.dobs[i][d]
                         ind = sc.findinds(space > spacing_bins[:])[-1]
                         model_spacing_counts[ind] += 1
-
                         model_spacing.append(space)
 
+        # Normalize model birth space bin counts to percentages
         model_spacing_counts[:] /= model_spacing_counts[:].sum()
         model_spacing_counts[:] *= 100
+
+        # Extract birth spaces and age at first birth from data
+        for i, j in data_spaces.iterrows():
+            space = j['space_mo'] / mpy
+            ind = sc.findinds(space > spacing_bins[:])[-1]
+            data_spacing_counts[ind] += j['Freq']
+
+        # Normalize dat birth space bin counts to percentages
+        data_spacing_counts[:] /= data_spacing_counts[:].sum()
+        data_spacing_counts[:] *= 100
+
+        # Extract afb and respective weights data
+        afb_values = data_afb["afb"].values.tolist()
+        afb_weights = data_afb["wt"].values.tolist()
+
+        # Calculate the cumulative weights and total weight of the afb data
+        afb_cum_weights = np.cumsum(afb_weights)
+        afb_total_weight = afb_cum_weights[-1]
+
+        # Extract birth spacing and respective frequency data
+        birth_spacing_values = data_spaces["space_mo"].values.tolist()
+        birth_spacing_weights = data_spaces["Freq"].values.tolist()
+
+        # Calculate the cumulative weights and total weight of the birth spacing data
+        birth_spacing_cum_weights = np.cumsum(birth_spacing_weights)
+        birth_spacing_total_weight = birth_spacing_cum_weights[-1]
+
+        data_spacing_stats = np.array([np.interp((.25 * afb_total_weight), afb_cum_weights, afb_values),
+                                       np.interp((.50 * afb_total_weight), afb_cum_weights, afb_values),
+                                       np.interp((.75 * afb_total_weight), afb_cum_weights, afb_values)])
+
+        data_age_first_stats = np.array([np.interp((.25 * birth_spacing_total_weight), birth_spacing_cum_weights, birth_spacing_values),
+                                       np.interp((.50 * birth_spacing_total_weight), birth_spacing_cum_weights, birth_spacing_values),
+                                       np.interp((.75 * birth_spacing_total_weight), birth_spacing_cum_weights, birth_spacing_values)])
+
+        # Save to dictionary
+        self.data['spacing_bins'] = np.array(data_spacing_counts.values())
+        self.data['spacing_stats'] = data_spacing_stats
+        self.data['age_first_stats'] = data_age_first_stats
+
         try:
             model_spacing_stats = np.array([np.percentile(model_spacing, 25),
                                             np.percentile(model_spacing, 50),
                                             np.percentile(model_spacing, 75)])
             model_age_first_stats = np.array([np.percentile(model_age_first, 25),
-                                            np.percentile(model_age_first, 50),
-                                            np.percentile(model_age_first, 75)])
-        except Exception as E: # pragma: nocover
+                                              np.percentile(model_age_first, 50),
+                                              np.percentile(model_age_first, 75)])
+        except Exception as E:  # pragma: nocover
             print(f'Could not calculate birth spacing, returning zeros: {E}')
-            model_spacing_counts = {k:0 for k in spacing_bins.keys()}
+            model_spacing_counts = {k: 0 for k in spacing_bins.keys()}
             model_spacing_stats = np.zeros(data_spacing_stats.shape)
             model_age_first_stats = np.zeros(data_age_first_stats.shape)
 
         # Save arrays to dictionary
         self.model['spacing_bins'] = np.array(model_spacing_counts.values())
         self.model['spacing_stats'] = model_spacing_stats
         self.model['age_first_stats'] = model_age_first_stats
 
         return
 
     def extract_methods(self):
-
-        min_age = 15
-        max_age = 50
-
         data_method_counts = sc.odict().make(self.method_keys, vals=0.0)
         model_method_counts = sc.dcp(data_method_counts)
 
-        # Load data from DHS -- from dropbox/Method_v312.csv
-
-        data = [
-            ['Other modern', 'emergency contraception', 0.015216411570543636, 2017.698615635373],
-            ['Condoms', 'female condom', 0.005239036180154552, 2017.698615635373],
-            ['BTL', 'female sterilization', 0.24609377594176307, 2017.698615635373],
-            ['Implants', 'implants/norplant', 5.881839602070953, 2017.698615635373],
-            ['Injectables', 'injections', 7.101718239287355, 2017.698615635373],
-            ['IUDs', 'iud', 1.4865067612487317, 2017.698615635373],
-            ['Other modern', 'lactational amenorrhea (lam)', 0.04745447091361792, 2017.698615635373],
-            ['Condoms', 'male condom', 1.0697377418682412, 2017.698615635373],
-            ['None', 'not using', 80.10054235699272, 2017.698615635373],
-            ['Other modern', 'other modern method', 0.007832257135437748, 2017.698615635373],
-            ['Other traditional', 'other traditional', 0.5127850142889963, 2017.698615635373],
-            ['Other traditional', 'periodic abstinence', 0.393946698444533, 2017.698615635373],
-            ['Pill', 'pill', 2.945874450486654, 2017.698615635373],
-            ['Other modern', 'standard days method (sdm)', 0.06132534128612159, 2017.698615635373],
-            ['Withdrawal', 'withdrawal', 0.12388784228417069, 2017.698615635373],
-        ]
-
-        for entry in data:
-            data_method_counts[entry[0]] += entry[2]
-        data_method_counts[:] /= data_method_counts[:].sum()
+        # Extract from data
+        data_methods = self.load_data('methods')
+        for index, row in data_methods.iterrows():
+            data_method_counts[row['method']] = row['perc']
+
+        # Update data method mix using non-user percentage from 'use' file
+        data_use = self.load_data('use')
+        data_method_counts['None'] = data_use.loc[0, 'perc']
+        use_freq = (data_use.loc[1, 'perc'])/100
+        for key, value in data_method_counts.items():
+            value /= 100
+            if key != 'None':
+                value *= use_freq
+            data_method_counts.update({key: value})
 
-        # From model
+        # Extract from model
         ppl = self.people
         for i in range(len(ppl)):
             if ppl.alive[i] and not ppl.sex[i] and ppl.age[i] >= min_age and ppl.age[i] < max_age:
                 model_method_counts[ppl.method[i]] += 1
+
         model_method_counts[:] /= model_method_counts[:].sum()
 
         # Make labels
         data_labels = data_method_counts.keys()
         for d in range(len(data_labels)):
             if data_method_counts[d] > 0.01:
                 data_labels[d] = f'{data_labels[d]}: {data_method_counts[d] * 100:0.1f}%'
@@ -437,80 +440,41 @@
                 model_labels[d] = ''
 
         self.data['method_counts'] = np.array(data_method_counts.values())
         self.model['method_counts'] = np.array(model_method_counts.values())
 
         return
 
-    def extract_age_pregnancy(self):
-
-        index = [0, 1, 2, 3, 7] #indices of count, min, and max to drop from descriptive stats
-        # Keep mean [1], 25% [4], 50%[5], 75% [6]
-
-        data = self.data['pregnancy_parity'] # Copy DataFrame for mainupation
-        preg = data[data['Pregnant'] == 1]
-        stat = preg['Age'].describe()
-        data_stats_all = stat.to_numpy()
-        data_stats = np.delete(data_stats_all, index)
-
-        self.data['age_pregnant_stats'] = data_stats  # Array of mean, std, 25%, 50%, 75% of ages of agents currently pregnant
-
-        model = self.model['pregnancy_parity']  # Copy DataFrame for manipulation
-        pregnant = model[model['Pregnant'] == 1]
-        stats = pregnant['Age'].describe()
-        model_stats_all = stats.to_numpy()
-        model_stats = np.delete(model_stats_all, index)
-
-        self.model['age_pregnant_stats'] = model_stats
-
-        parity_data = data.groupby('Parity')['Age'].describe()
-        parity_data = parity_data.head(11) # Include only parities 0-10 to exclude outliers
-        parity_data = parity_data.drop(['count', 'mean', 'std', 'min', 'max'], axis = 1)
-        parity_data.fillna(0)
-        parity_data_stats = parity_data.to_numpy()
-
-        self.data['age_parity_stats'] = parity_data_stats
-
-        parity_model = model.groupby('Parity')['Age'].describe()
-        parity_model = parity_model.head(11)
-        parity_model = parity_model.drop(['count', 'mean', 'std', 'min', 'max'], axis = 1)
-        parity_model.fillna(0)
-        parity_model_stats = parity_model.to_numpy()
-
-        self.model['age_parity_stats'] = parity_model_stats
-
-
     def compute_fit(self, *args, **kwargs):
         ''' Compute how good the fit is '''
         data = sc.dcp(self.data)
-        sim = sc.dcp(self.model)
+        try:
+            sim = sc.dcp(self.model, die=False) # Sometimes fails with a dict_keys copy error (!)
+        except:
+            sim = {k:self.model[k] for k in data.keys()}
         for k in data.keys():
             data[k] = sc.promotetoarray(data[k])
             data[k] = data[k].flatten()
             sim[k] = sc.promotetoarray(sim[k])
             sim[k] = sim[k].flatten()
         self.fit = Fit(data, sim, *args, **kwargs)
         pass
 
 
     def post_process_results(self, keep_people=False, compute_fit=True, **kwargs):
         ''' Compare the model and the data '''
         self.extract_model()
-        if self.flags.skyscrapers:   self.extract_skyscrapers()
+        if self.flags.ageparity:   self.extract_ageparity()
         if self.flags.birth_space:   self.extract_birth_spacing()
         if self.flags.methods:       self.extract_methods()
-        if self.flags.age_pregnancy: self.extract_age_pregnancy()
 
         # Remove people, they're large!
         if not keep_people:
             del self.people
 
-        # Remove raw dataframes of pregnancy / parity data from dictionary
-        del self.data['pregnancy_parity']
-        del self.model['pregnancy_parity']
 
         # Compute comparison
         self.df = self.compare()
 
         # Compute fit
         if compute_fit:
             self.compute_fit(**kwargs)
@@ -633,15 +597,15 @@
                      'crude_death_rate',
                      'crude_birth_rate']
         non_calibrated_keys = ['pop_years', 'mcpr_years', 'tfr_years', 'asfr_bins']
         for key in rate_keys + non_calibrated_keys:
             if key in keys:
                 keys.remove(key)
         nkeys = len(keys)
-        expected = 13
+        expected = 11
         if nkeys != expected:
             errormsg = f'Number of keys changed -- expected {expected}, actually {nkeys} -- did you use run_model() instead of run()?'
             raise ValueError(errormsg)
 
         with fpo.with_style():
 
             fig, axs = pl.subplots(nrows=4, ncols=3)
@@ -688,25 +652,25 @@
             ax.plot(data.mcpr_years, data.mcpr, 'o', label='Data')
             ax.plot(sim.mcpr_years,  sim.mcpr,  '-', label='Sim')
             ax.set_title('MCPR')
             ax.set_xlabel('Year')
             ax.set_ylabel('Modern contraceptive prevalence rate')
             ax.legend()
 
-            # Data skyscraper
+            # Data age-parity
             ax = axs[0,1]
-            ax.pcolormesh(self.age_bins, self.parity_bins, data.skyscrapers.transpose(), shading='nearest', cmap='turbo')
+            ax.pcolormesh(self.age_bins, self.parity_bins, data.ageparity.transpose(), shading='nearest', cmap='turbo')
             ax.set_aspect(1./ax.get_data_ratio()) # Make square
             ax.set_title('Age-parity plot: data')
             ax.set_xlabel('Age')
             ax.set_ylabel('Parity')
 
-            # Sim skyscraper
+            # Sim age-parity
             ax = axs[1,1]
-            ax.pcolormesh(self.age_bins, self.parity_bins, sim.skyscrapers.transpose(), shading='nearest', cmap='turbo')
+            ax.pcolormesh(self.age_bins, self.parity_bins, sim.ageparity.transpose(), shading='nearest', cmap='turbo')
             ax.set_aspect(1./ax.get_data_ratio())
             ax.set_title('Age-parity plot: sim')
             ax.set_xlabel('Age')
             ax.set_ylabel('Parity')
 
             # Spacing bins
             ax = axs[2, 1]
@@ -738,43 +702,14 @@
             ax.barh(y=y-height/2, width=sim.age_first_stats,  height=height, align='center', label='Sim')
             ax.set_title('Age at first birth')
             ax.set_xlabel('Age')
             ax.set_yticks(range(n_quartiles))
             ax.set_yticklabels(quartile_keys)
             ax.legend()
 
-            # Age pregnant stats
-            ax = axs[0,2]
-            height = 0.4
-            y = np.arange(len(data.age_pregnant_stats))
-            ax.barh(y=y+height/2, width=data.age_pregnant_stats, height=height, align='center', label='Data')
-            ax.barh(y=y-height/2, width=sim.age_pregnant_stats,  height=height, align='center', label='Sim')
-            ax.set_title('Age of women currently pregnant')
-            ax.set_xlabel('Age')
-            ax.set_yticks(range(n_quartiles))
-            ax.set_yticklabels(quartile_keys)
-            ax.legend()
-
-            # Age parity stats
-            ax = axs[1,2]
-            cols = sc.gridcolors(3)
-            for i,yvals in enumerate([data.age_parity_stats, sim.age_parity_stats]):
-                for j in range(3):
-                    vals = yvals[:,j]
-                    if i==0:
-                        marker = 'o'
-                        label = 'Data'
-                    else:
-                        marker = '-'
-                        label = 'Sim'
-                    ax.plot(vals, marker, c=cols[j], label=label)
-            ax.set_title('Age parity stats - quartiles')
-            ax.set_xlabel('Parity')
-            ax.set_ylabel('Age')
-            ax.legend()
 
             # Method counts
             ax = axs[2,2]
 
             height = 0.4
             y = np.arange(len(data.method_counts))
             y1 = y + height/2
@@ -1192,22 +1127,22 @@
     sim1 = sim1['model']
     sim2 = sim2['model']
 
     # Compare keys
     keymatchmsg = ''
     sim1_keys = set(sim1.keys())
     sim2_keys = set(sim2.keys())
-    if sim1_keys != sim2_keys and not skip_key_diffs: # pragma: no cover
-        keymatchmsg = "Keys don't match!\n"
-        missing = list(sim1_keys - sim2_keys)
-        extra   = list(sim2_keys - sim1_keys)
-        if missing:
-            keymatchmsg += f'  Missing sim1 keys: {missing}\n'
-        if extra:
-            keymatchmsg += f'  Extra sim2 keys: {extra}\n'
+    #if sim1_keys !=    _keys and not skip_key_diffs: # pragma: no cover
+        #keymatchmsg = "Keys don't match!\n"
+       # missing = list(sim1_keys - sim2_keys)
+        #extra   = list(sim2_keys - sim1_keys)
+        #if missing:
+            #keymatchmsg += f'  Missing sim1 keys: {missing}\n'
+        #if extra:
+            #keymatchmsg += f'  Extra sim2 keys: {extra}\n'
 
     # Compare values
     valmatchmsg = ''
     mismatches = {}
     for key in sim2.keys(): # To ensure order
         if key in sim1_keys: # If a key is missing, don't count it as a mismatch
             sim1_val = sim1[key] if key in sim1 else 'not present'
@@ -1226,15 +1161,15 @@
         for mdict in mismatches.values():
             old = mdict['sim1']
             new = mdict['sim2']
             numeric = sc.isnumber(sim1_val) and sc.isnumber(sim2_val)
             if numeric and old>0:
                 this_diff  = new - old
                 this_ratio = new/old
-                abs_ratio  = max(this_ratio, 1.0/this_ratio)
+                abs_ratio  = max(this_ratio, sc.safedivide(1.0, this_ratio, np.inf))
 
                 # Set the character to use
                 if abs_ratio<small_change:
                     change_char = '≈'
                 elif new > old:
                     change_char = '↑'
                 elif new < old:
@@ -1277,8 +1212,8 @@
         elif output:
             return mismatchmsg
         else:
             print(mismatchmsg)
     else:
         if not output:
             print('Sims match')
-    return
+    return
```

### Comparing `fpsim-0.22.0/fpsim/interventions.py` & `fpsim-0.28.1/fpsim/interventions.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/data_processing/mcpr_by_parity.py` & `fpsim-0.28.1/fpsim/locations/data_processing/mcpr_by_parity.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/data_processing/process_matrices.py` & `fpsim-0.28.1/fpsim/locations/data_processing/process_matrices.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/data_processing/sexual_debut_age_probs.py` & `fpsim-0.28.1/fpsim/locations/data_processing/sexual_debut_age_probs.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/explore_plotting.py` & `fpsim-0.28.1/fpsim/locations/kenya/explore_plotting.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/kenya_asfr.csv` & `fpsim-0.28.1/fpsim/locations/kenya/asfr.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-year,10-14,15-19,20-24,25-29,30-34,35-39,40-44,45-49,50-54
-1950,16.63,162.77,307.78,302.12,284.71,207.54,128.72,53.22,4.06
-1951,16.77,163.53,308.39,303.88,285.33,208.38,130.33,53.77,4.01
-1952,16.69,164.30,310.75,305.03,285.91,209.17,130.82,53.96,3.96
-1953,17.25,166.95,311.02,305.70,285.63,209.89,131.44,55.47,4.05
-1954,17.18,167.73,312.86,307.39,287.06,211.26,132.12,56.04,4.05
-1955,17.29,169.73,313.01,307.67,287.65,211.18,132.12,57.08,4.11
-1956,17.26,170.83,317.76,307.65,288.81,212.37,133.17,57.87,4.19
-1957,17.60,173.11,321.67,308.52,289.56,213.57,134.30,58.96,4.37
-1958,17.86,174.91,324.43,308.56,288.71,212.76,134.76,59.22,4.52
-1959,17.33,173.78,326.12,308.99,289.82,212.89,134.77,60.19,4.71
-1960,17.59,173.67,326.86,309.26,289.74,212.93,135.67,60.60,4.76
-1961,18.57,176.00,331.21,312.80,290.58,213.73,137.21,61.84,4.85
-1962,18.28,174.61,337.06,318.54,292.16,215.35,139.28,63.05,4.97
-1963,18.00,172.11,340.85,322.13,294.95,218.92,140.11,63.29,5.01
-1964,16.76,168.27,344.62,325.14,299.58,222.06,141.30,63.13,4.95
-1965,16.45,169.28,346.64,328.43,302.74,229.71,144.92,63.99,4.92
-1966,16.30,171.87,344.70,330.55,301.82,232.99,146.74,63.30,4.78
-1967,16.65,174.44,345.09,328.90,298.94,233.04,147.24,61.98,4.67
-1968,16.55,174.25,343.89,330.29,296.37,233.86,147.84,60.91,4.61
-1969,16.30,172.67,343.48,331.11,294.99,235.04,148.20,59.30,4.45
-1970,15.48,168.03,337.86,332.81,295.15,240.55,150.93,58.46,4.28
-1971,16.83,175.02,337.11,326.84,288.96,241.93,153.21,55.91,3.92
-1972,16.27,173.44,337.24,325.47,288.11,239.84,153.37,55.99,3.92
-1973,14.69,167.73,338.87,326.71,286.88,237.07,153.57,56.42,3.95
-1974,13.37,163.08,339.13,328.54,286.41,236.34,152.00,56.62,3.95
-1975,13.21,162.86,337.04,328.99,285.74,234.40,150.61,56.75,3.94
-1976,13.55,164.76,336.37,326.28,283.77,235.98,148.18,54.05,3.68
-1977,13.34,163.31,337.84,324.78,282.41,234.01,146.07,52.71,3.63
-1978,12.84,160.69,339.27,323.23,281.02,231.56,143.53,50.74,3.53
-1979,12.58,158.88,337.59,321.90,283.01,227.89,139.65,48.40,3.39
-1980,12.00,155.95,331.90,321.83,280.25,226.66,138.40,47.29,3.29
-1981,12.40,157.43,329.56,315.31,279.03,224.22,134.54,45.20,3.10
-1982,11.11,149.25,331.04,316.11,275.12,218.76,129.47,44.75,3.14
-1983,10.09,142.41,329.26,312.17,273.14,213.11,124.01,43.69,3.12
-1984,10.46,144.14,320.18,311.75,269.66,205.24,117.32,42.03,3.01
-1985,9.93,140.37,317.24,307.44,264.43,199.47,114.01,39.30,2.77
-1986,8.81,135.72,317.82,307.70,256.99,192.61,110.23,37.43,2.62
-1987,9.02,136.98,313.46,302.62,245.85,185.78,104.92,35.78,2.48
-1988,8.60,133.80,305.19,297.67,236.98,178.69,101.17,37.27,2.64
-1989,8.27,130.06,296.75,289.73,230.59,174.55,95.97,37.85,2.74
-1990,8.17,127.24,284.51,281.13,221.45,169.67,91.31,41.47,3.11
-1991,7.86,123.76,274.26,268.97,217.74,165.07,86.30,41.72,3.16
-1992,7.37,120.74,268.04,264.35,210.73,153.87,82.59,40.21,3.02
-1993,6.85,117.43,265.55,260.75,203.06,143.18,78.70,38.33,2.87
-1994,6.88,115.83,262.40,254.80,198.01,139.49,75.43,35.99,2.69
-1995,6.97,114.68,260.67,250.14,195.31,137.25,73.78,34.24,2.60
-1996,7.45,116.48,252.94,244.40,194.31,138.74,72.60,33.59,2.59
-1997,7.50,114.78,250.20,240.97,193.17,138.91,72.25,33.45,2.60
-1998,7.94,116.52,248.34,241.35,189.84,138.20,71.73,34.29,2.70
-1999,8.00,115.99,244.23,238.15,188.12,136.11,69.99,34.84,2.79
-2000,8.01,114.96,241.01,237.42,187.75,134.63,68.98,34.04,2.64
-2001,8.68,117.28,237.82,235.50,185.37,132.53,68.30,32.39,2.41
-2002,8.36,114.05,232.90,230.99,184.20,133.62,67.17,31.56,2.38
-2003,8.02,112.34,228.90,227.80,181.07,128.62,64.00,30.50,2.38
-2004,8.04,112.52,225.81,224.15,179.11,124.93,61.80,29.77,2.41
-2005,7.50,109.26,225.63,221.94,178.30,124.14,60.91,29.46,2.44
-2006,7.18,107.55,224.60,219.05,178.67,123.29,60.05,29.61,2.48
-2007,7.28,108.00,220.86,216.93,178.01,123.12,60.22,29.87,2.50
-2008,7.24,106.59,217.27,215.08,173.59,121.47,57.94,30.31,2.56
-2009,7.01,103.53,211.74,211.20,167.51,117.53,54.64,29.85,2.53
-2010,6.92,101.77,203.48,206.23,160.52,113.97,51.36,28.95,2.44
-2011,6.51,97.34,199.67,199.90,154.21,109.73,48.25,27.93,2.37
-2012,6.21,93.70,197.08,193.14,148.20,106.26,45.39,27.00,2.32
-2013,6.02,90.86,194.32,185.96,143.26,100.73,42.44,26.03,2.27
-2014,5.77,86.96,192.22,183.32,139.81,94.11,40.21,25.26,2.23
-2015,5.37,81.43,194.38,184.79,139.27,90.07,38.73,24.73,2.22
-2016,5.20,76.81,191.88,189.11,134.18,85.86,36.80,23.57,2.12
-2017,5.08,72.35,183.34,189.58,135.67,84.34,35.72,21.37,1.90
-2018,4.82,71.30,175.75,181.48,138.07,85.42,37.87,20.13,1.72
-2019,3.64,69.58,174.28,176.43,135.88,80.84,36.62,15.75,1.27
-2020,3.03,64.94,172.26,174.12,136.10,80.51,34.88,13.12,1.03
-2021,3.03,64.19,169.02,172.34,133.42,78.52,33.75,12.34,0.96
+year,10-14,15-19,20-24,25-29,30-34,35-39,40-44,45-49
+1950,16.63,162.77,307.78,302.12,284.71,207.54,128.72,53.22
+1951,16.77,163.53,308.39,303.88,285.33,208.38,130.33,53.77
+1952,16.69,164.30,310.75,305.03,285.91,209.17,130.82,53.96
+1953,17.25,166.95,311.02,305.70,285.63,209.89,131.44,55.47
+1954,17.18,167.73,312.86,307.39,287.06,211.26,132.12,56.04
+1955,17.29,169.73,313.01,307.67,287.65,211.18,132.12,57.08
+1956,17.26,170.83,317.76,307.65,288.81,212.37,133.17,57.87
+1957,17.60,173.11,321.67,308.52,289.56,213.57,134.30,58.96
+1958,17.86,174.91,324.43,308.56,288.71,212.76,134.76,59.22
+1959,17.33,173.78,326.12,308.99,289.82,212.89,134.77,60.19
+1960,17.59,173.67,326.86,309.26,289.74,212.93,135.67,60.60
+1961,18.57,176.00,331.21,312.80,290.58,213.73,137.21,61.84
+1962,18.28,174.61,337.06,318.54,292.16,215.35,139.28,63.05
+1963,18.00,172.11,340.85,322.13,294.95,218.92,140.11,63.29
+1964,16.76,168.27,344.62,325.14,299.58,222.06,141.30,63.13
+1965,16.45,169.28,346.64,328.43,302.74,229.71,144.92,63.99
+1966,16.30,171.87,344.70,330.55,301.82,232.99,146.74,63.30
+1967,16.65,174.44,345.09,328.90,298.94,233.04,147.24,61.98
+1968,16.55,174.25,343.89,330.29,296.37,233.86,147.84,60.91
+1969,16.30,172.67,343.48,331.11,294.99,235.04,148.20,59.30
+1970,15.48,168.03,337.86,332.81,295.15,240.55,150.93,58.46
+1971,16.83,175.02,337.11,326.84,288.96,241.93,153.21,55.91
+1972,16.27,173.44,337.24,325.47,288.11,239.84,153.37,55.99
+1973,14.69,167.73,338.87,326.71,286.88,237.07,153.57,56.42
+1974,13.37,163.08,339.13,328.54,286.41,236.34,152.00,56.62
+1975,13.21,162.86,337.04,328.99,285.74,234.40,150.61,56.75
+1976,13.55,164.76,336.37,326.28,283.77,235.98,148.18,54.05
+1977,13.34,163.31,337.84,324.78,282.41,234.01,146.07,52.71
+1978,12.84,160.69,339.27,323.23,281.02,231.56,143.53,50.74
+1979,12.58,158.88,337.59,321.90,283.01,227.89,139.65,48.40
+1980,12.00,155.95,331.90,321.83,280.25,226.66,138.40,47.29
+1981,12.40,157.43,329.56,315.31,279.03,224.22,134.54,45.20
+1982,11.11,149.25,331.04,316.11,275.12,218.76,129.47,44.75
+1983,10.09,142.41,329.26,312.17,273.14,213.11,124.01,43.69
+1984,10.46,144.14,320.18,311.75,269.66,205.24,117.32,42.03
+1985,9.93,140.37,317.24,307.44,264.43,199.47,114.01,39.30
+1986,8.81,135.72,317.82,307.70,256.99,192.61,110.23,37.43
+1987,9.02,136.98,313.46,302.62,245.85,185.78,104.92,35.78
+1988,8.60,133.80,305.19,297.67,236.98,178.69,101.17,37.27
+1989,8.27,130.06,296.75,289.73,230.59,174.55,95.97,37.85
+1990,8.17,127.24,284.51,281.13,221.45,169.67,91.31,41.47
+1991,7.86,123.76,274.26,268.97,217.74,165.07,86.30,41.72
+1992,7.37,120.74,268.04,264.35,210.73,153.87,82.59,40.21
+1993,6.85,117.43,265.55,260.75,203.06,143.18,78.70,38.33
+1994,6.88,115.83,262.40,254.80,198.01,139.49,75.43,35.99
+1995,6.97,114.68,260.67,250.14,195.31,137.25,73.78,34.24
+1996,7.45,116.48,252.94,244.40,194.31,138.74,72.60,33.59
+1997,7.50,114.78,250.20,240.97,193.17,138.91,72.25,33.45
+1998,7.94,116.52,248.34,241.35,189.84,138.20,71.73,34.29
+1999,8.00,115.99,244.23,238.15,188.12,136.11,69.99,34.84
+2000,8.01,114.96,241.01,237.42,187.75,134.63,68.98,34.04
+2001,8.68,117.28,237.82,235.50,185.37,132.53,68.30,32.39
+2002,8.36,114.05,232.90,230.99,184.20,133.62,67.17,31.56
+2003,8.02,112.34,228.90,227.80,181.07,128.62,64.00,30.50
+2004,8.04,112.52,225.81,224.15,179.11,124.93,61.80,29.77
+2005,7.50,109.26,225.63,221.94,178.30,124.14,60.91,29.46
+2006,7.18,107.55,224.60,219.05,178.67,123.29,60.05,29.61
+2007,7.28,108.00,220.86,216.93,178.01,123.12,60.22,29.87
+2008,7.24,106.59,217.27,215.08,173.59,121.47,57.94,30.31
+2009,7.01,103.53,211.74,211.20,167.51,117.53,54.64,29.85
+2010,6.92,101.77,203.48,206.23,160.52,113.97,51.36,28.95
+2011,6.51,97.34,199.67,199.90,154.21,109.73,48.25,27.93
+2012,6.21,93.70,197.08,193.14,148.20,106.26,45.39,27.00
+2013,6.02,90.86,194.32,185.96,143.26,100.73,42.44,26.03
+2014,5.77,86.96,192.22,183.32,139.81,94.11,40.21,25.26
+2015,5.37,81.43,194.38,184.79,139.27,90.07,38.73,24.73
+2016,5.20,76.81,191.88,189.11,134.18,85.86,36.80,23.57
+2017,5.08,72.35,183.34,189.58,135.67,84.34,35.72,21.37
+2018,4.82,71.30,175.75,181.48,138.07,85.42,37.87,20.13
+2019,3.64,69.58,174.28,176.43,135.88,80.84,36.62,15.75
+2020,3.03,64.94,172.26,174.12,136.10,80.51,34.88,13.12
+2021,3.03,64.19,169.02,172.34,133.42,78.52,33.75,12.34
```

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/kenya_popsize.csv` & `fpsim-0.28.1/fpsim/locations/kenya/popsize.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/kenya_skyscrapers.csv` & `fpsim-0.28.1/fpsim/locations/kenya/ageparity.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/kenya_tfr.csv` & `fpsim-0.28.1/fpsim/locations/kenya/kenya_tfr.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/matrices_kenya_dhs_2014.csv` & `fpsim-0.28.1/fpsim/locations/kenya/matrices_kenya_pma_2019_20_21.csv`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-postpartum,age_grp,From,n,None,Withdrawal,Other.trad,Condom,Pill,Injectable,Implant,IUD,F.sterilization,Other.mod
-1,<18,Birth,1365,0.923809523809524,0.00146520146520147,0.0124542124542125,0.00293040293040293,0.0102564102564103,0.0417582417582418,0.00512820512820513,0.0021978021978022,0,0
-1,18-20,Birth,1213,0.905193734542457,0.000824402308326463,0.00824402308326463,0.00329760923330585,0.0189612530915087,0.0494641384995878,0.00989282769991756,0.00329760923330585,0.000824402308326463,0
-1,20-25,Birth,3419,0.895583503948523,0.00175489909330214,0.00877449546651068,0.00321731500438725,0.0233986545773618,0.0532319391634981,0.0090669786487277,0.00438724773325534,0.000584966364434045,0
-1,25-35,Birth,4008,0.896457085828343,0.00249500998003992,0.0124750499001996,0.00548902195608782,0.0207085828343313,0.0394211576846307,0.0094810379241517,0.00274451097804391,0.0107285429141717,0
-1,>35,Birth,969,0.909184726522188,0.00103199174406605,0.0175438596491228,0.00412796697626419,0.0175438596491228,0.0175438596491228,0.00928792569659443,0.00309597523219814,0.0185758513931889,0.00206398348813209
-6,<18,None,945,0.766137566137566,0.00740740740740741,0.019047619047619,0.00740740740740741,0.0253968253968254,0.15026455026455,0.0232804232804233,0.00105820105820106,0,0
-6,<18,Withdrawal,1,0,1,0,0,0,0,0,0,0,0
-6,<18,Other.trad,14,0,0,1,0,0,0,0,0,0,0
-6,<18,Condom,4,0,0,0,1,0,0,0,0,0,0
-6,<18,Pill,9,0.111111111111111,0,0,0,0.888888888888889,0,0,0,0,0
-6,<18,Injectable,37,0.027027027027027,0,0,0,0,0.972972972972973,0,0,0,0
-6,<18,Implant,6,0.166666666666667,0,0,0,0,0,0.833333333333333,0,0,0
-6,<18,IUD,1,0,0,0,0,0,0,0,1,0,0
-6,<18,F.sterilization,0,0,0,0,0,0,0,0,0,1,0
-6,<18,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,18-20,None,916,0.7117903930131,0.00982532751091703,0.0185589519650655,0.00655021834061135,0.0414847161572052,0.181222707423581,0.027292576419214,0.00327510917030568,0,0
-6,18-20,Withdrawal,0,0,1,0,0,0,0,0,0,0,0
-6,18-20,Other.trad,9,0,0,1,0,0,0,0,0,0,0
-6,18-20,Condom,4,0,0,0,1,0,0,0,0,0,0
-6,18-20,Pill,22,0.0909090909090909,0,0.0454545454545455,0.0454545454545455,0.545454545454545,0.272727272727273,0,0,0,0
-6,18-20,Injectable,57,0.105263157894737,0,0,0,0,0.824561403508772,0.0701754385964912,0,0,0
-6,18-20,Implant,8,0,0,0,0,0,0,1,0,0,0
-6,18-20,IUD,6,0,0,0,0,0,0,0,1,0,0
-6,18-20,F.sterilization,1,0,0,0,0,0,0,0,0,1,0
-6,18-20,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,20-25,None,2799,0.714898177920686,0.00357270453733476,0.0117899249732047,0.00893176134333691,0.0371561271882815,0.18399428367274,0.0314397999285459,0.00714540907466953,0.000714540907466952,0.000357270453733476
-6,20-25,Withdrawal,7,0,1,0,0,0,0,0,0,0,0
-6,20-25,Other.trad,28,0,0,0.892857142857143,0,0,0.107142857142857,0,0,0,0
-6,20-25,Condom,11,0,0,0,1,0,0,0,0,0,0
-6,20-25,Pill,67,0,0,0,0,0.835820895522388,0.104477611940299,0.0149253731343284,0.0447761194029851,0,0
-6,20-25,Injectable,162,0.037037037037037,0,0.00617283950617284,0,0.0185185185185185,0.925925925925926,0.0123456790123457,0,0,0
-6,20-25,Implant,28,0,0,0,0,0,0,1,0,0,0
-6,20-25,IUD,10,0,0,0,0,0,0,0,1,0,0
-6,20-25,F.sterilization,1,0,0,0,0,0,0,0,0,1,0
-6,20-25,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,25-35,None,3377,0.707136511696772,0.00829138288421676,0.0189517323067812,0.0106603494225644,0.0547823511992893,0.14569144210838,0.0390879478827362,0.0109564702398579,0.00384957062481492,0.000592241634586911
-6,25-35,Withdrawal,9,0,0.888888888888889,0,0,0,0,0,0.111111111111111,0,0
-6,25-35,Other.trad,54,0.0185185185185185,0,0.981481481481482,0,0,0,0,0,0,0
-6,25-35,Condom,20,0,0,0,0.9,0,0.05,0,0.05,0,0
-6,25-35,Pill,88,0,0,0.0113636363636364,0,0.840909090909091,0.0909090909090909,0.0454545454545455,0.0113636363636364,0,0
-6,25-35,Injectable,146,0.0136986301369863,0,0.0136986301369863,0,0.0136986301369863,0.910958904109589,0.0342465753424658,0.00684931506849315,0.00684931506849315,0
-6,25-35,Implant,33,0,0,0,0,0,0,1,0,0,0
-6,25-35,IUD,10,0,0,0,0,0,0,0,1,0,0
-6,25-35,F.sterilization,39,0,0,0,0,0,0,0,0,1,0
-6,25-35,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,>35,None,888,0.79954954954955,0.0045045045045045,0.0349099099099099,0.00788288288288288,0.0337837837837838,0.0844594594594595,0.0191441441441441,0.00788288288288288,0.00788288288288288,0
-6,>35,Withdrawal,2,0,1,0,0,0,0,0,0,0,0
-6,>35,Other.trad,16,0,0,1,0,0,0,0,0,0,0
-6,>35,Condom,3,0,0,0,1,0,0,0,0,0,0
-6,>35,Pill,18,0,0,0,0,0.944444444444444,0.0555555555555556,0,0,0,0
-6,>35,Injectable,22,0.0909090909090909,0,0.0454545454545455,0,0,0.818181818181818,0,0,0.0454545454545455,0
-6,>35,Implant,8,0,0,0,0,0,0,1,0,0,0
-6,>35,IUD,3,0,0,0,0,0,0,0,1,0,0
-6,>35,F.sterilization,18,0,0,0,0,0,0,0,0,1,0
-6,>35,Other.mod,2,0,0,0,0,0,0,0,0,0,1
-No,<18,None,237754,0.983167997417528,0.000269704532781845,0.00219588142347683,0.00732483463022711,0.00123406276426527,0.0047083293008299,0.000931396522130923,4.09935961326419E-05,0,0.000126799812626875
-No,<18,Withdrawal,202,0.128619523797137,0.740270649650873,0.000352787454580801,0.0419845833284028,0.00126012513184655,0.0868567954678762,0.000645081145967725,2.57792673806121E-06,0,7.87609657752264E-06
-No,<18,Other.trad,1464,0.140725741376562,1.97714492021109E-05,0.827151316966351,0.0186467086636593,0.000381062645268218,0.0129171425156841,0.000146337496578488,2.93815352780141E-06,0,8.98073316735388E-06
-No,<18,Condom,2579,0.361360885405694,0.000148309930562771,0.00403905153632114,0.617824773617483,0.0150116451640759,0.00141024404545202,0.000172576148146993,8.01139753380635E-06,0,2.45027547305372E-05
-No,<18,Pill,919,0.30476553132456,0.00907895758403943,0.0195018517967511,0.0182456633081901,0.603226145069645,0.0447030081594752,0.000451727054812624,6.68180960049182E-06,0,2.04338929252878E-05
-No,<18,Injectable,4424,0.294961865275357,0.000122463120356027,0.00257893855817359,0.00133410403786254,0.0127793723721014,0.677289056938594,0.0109080625687796,6.44087656409345E-06,0,1.96962522114454E-05
-No,<18,Implant,611,0.0950295742715199,1.30055848542794E-05,0.000121548846203993,0.000354559734470109,0.000187043176988366,0.0158206324211559,0.88846563367042,1.97274658527491E-06,0,6.02954780218085E-06
-No,<18,IUD,27,0.0567164506155361,1.52086781736986E-05,0.00047536072369924,0.000164084518593796,0.00268121307917711,0.302016759879978,0.00213582265940975,0.635792708661309,0,2.39118412265649E-06
-No,<18,F.sterilization,19,0,0,0,0,0,0,0,0,1,0
-No,<18,Other.mod,32,0.31403294428427,4.37002845516526E-05,0.000350743065731089,0.00123157193093161,0.000201568570633661,0.000776848033224583,0.00014616647124336,6.87424361210802E-06,0,0.683209583115801
-No,18-20,None,37490,0.924014292715044,0.00142272161955317,0.00686296389359832,0.0202388055032033,0.00748326137723802,0.0323112309109126,0.00627620668446556,0.00084834505891807,0,0.000542172237067623
-No,18-20,Withdrawal,280,0.155837576825681,0.805669570061443,0.000760552981633373,0.0330799488187737,0.00101542672197904,0.00276585832362435,0.000604753869505039,6.75991629477856E-05,0,0.000198713234412646
-No,18-20,Other.trad,1275,0.114418799599628,8.86607650327862E-05,0.851736979266323,0.0153965765060784,0.00780105957943438,0.00981015447605147,0.000595505170187891,4.90959132466574E-05,0,0.000103168724017966
-No,18-20,Condom,1666,0.312225408954197,0.00024364025738353,0.0120150422345258,0.629959220793054,0.0202359181139609,0.0130204725435137,0.00667085144517286,0.000142094444600796,0,0.00548735121359143
-No,18-20,Pill,1660,0.256886872858917,0.000260225513745498,0.00128201168583735,0.00300285230425745,0.630781447225996,0.0797525559139742,0.0278314829127787,0.00011553069138467,0,8.70208931093129E-05
-No,18-20,Injectable,6732,0.240141519953577,0.00156009839377689,0.00520171022066481,0.00519166184168821,0.0184072621220338,0.714501006416573,0.01479702129726,0.000107240898345767,0,9.24788560809445E-05
-No,18-20,Implant,988,0.153405910537145,0.000128066190674322,0.0107218883776362,0.00177637310914126,0.0185393914909844,0.0222097726852918,0.793101256868845,6.67215821538588E-05,0,5.06191581284581E-05
-No,18-20,IUD,193,0.0655894778350033,4.64338784597512E-05,0.053207341839599,0.00110398787855218,0.0467358480313435,0.0036293922012576,0.00101855743352575,0.828647130844033,0,2.18300582251742E-05
-No,18-20,F.sterilization,26,0.360298429776954,0.000277255413187521,0.0013145454613241,0.00412060738165313,0.00147316351393046,0.00642756151666791,0.00120188940745104,0.00016568534127212,0.624597049580065,0.000123812607494156
-No,18-20,Other.mod,28,0.475630231890482,0.000603865982957435,0.00406222525302138,0.166554739504248,0.00742475941213766,0.182603362165281,0.00448935639990643,0.000246952913174793,0,0.15838450647879
-No,20-25,None,74293,0.888470204367373,0.000896937224615902,0.00852734890047238,0.0130007865948817,0.0138129404577825,0.0581341247701729,0.0137068811457251,0.00209705464704744,0.000305463951994961,0.00104825793993569
-No,20-25,Withdrawal,507,0.164206293981972,0.69761024844322,0.0379379772940376,0.0183380061722311,0.00226767554846173,0.0584302301403546,0.0207198841018761,0.000318069565212345,2.57154604031727E-05,0.000145899292230391
-No,20-25,Other.trad,4351,0.113515506836863,0.000113468610013429,0.828460112891267,0.00726492243290152,0.00559781755713748,0.0388464771025007,0.00359284359612355,0.00250480668997635,1.7409793909093E-05,8.66344893072612E-05
-No,20-25,Condom,3716,0.215103403282448,0.00476995152890225,0.021274701459507,0.692252432929992,0.0183167112837676,0.034010979945572,0.00979037200235295,0.000354404642878264,3.42339860124666E-05,0.00409280893856856
-No,20-25,Pill,8343,0.215673234989278,0.00121645555040334,0.0111597700007989,0.00780710063891919,0.674514964691283,0.0624110669917697,0.0214066706554171,0.00475925261105653,3.43905986127921E-05,0.00101709327246115
-No,20-25,Injectable,30840,0.210466363408434,0.00184714629921266,0.00487688476248015,0.00364229798216897,0.0216648184674059,0.737489373836106,0.0173578216687055,0.00247645917928219,3.34412522658886E-05,0.000145393143938492
-No,20-25,Implant,5986,0.0905187483007751,0.00166990835668341,0.0022870429799604,0.0038901458910466,0.0102995325305137,0.0130776933801098,0.876305483909897,0.00187038947965078,1.38390626956911E-05,6.72161086681377E-05
-No,20-25,IUD,1371,0.0908721460695641,9.56637654992702E-05,0.00799753663657294,0.0008118235342506,0.0278711591243578,0.0248471654597242,0.0162854503900506,0.831136007332146,1.37702746729028E-05,6.92774131616465E-05
-No,20-25,F.sterilization,104,0,0,0,0,0,0,0,0,1,0
-No,20-25,Other.mod,191,0.326341098599224,0.000374592193556289,0.00286641968668841,0.0413974015100676,0.116862146791297,0.0160278356751358,0.00418814486927579,0.000731924386661187,5.43337886783323E-05,0.491156102499416
-No,25-35,None,95715,0.894080718407184,0.000883181811910486,0.00601961503599188,0.00853302412817273,0.0157769145787106,0.0540722065866882,0.0151420558749794,0.00398994612239138,0.00137122655418148,0.000131110899790006
-No,25-35,Withdrawal,1409,0.162678756446363,0.799795893912488,0.000589545510474252,0.00077193039693676,0.00819401581586791,0.0186669740488869,0.00873538420918753,0.000421456096162432,0.000129057546614688,1.69860170184715E-05
-No,25-35,Other.trad,8280,0.0797640820288775,4.41896481647301E-05,0.859623614995325,0.00290900766380898,0.00476978833558283,0.0372940451513555,0.00866302489343654,0.00412742518695211,0.0027894269585092,1.53951379875673E-05
-No,25-35,Condom,5257,0.133104493496756,0.00195650103059691,0.00438939343102778,0.82487177418117,0.00845854899564184,0.0118098841488569,0.013051671199223,0.000360190680507957,0.000109500283086668,0.00188804255313315
-No,25-35,Pill,18367,0.165283311062495,0.00109435908997734,0.0106146112948337,0.00246755954525638,0.709868537521129,0.0755128553255422,0.0210730776986197,0.0116940489725734,0.00186413918195162,0.000527500307621865
-No,25-35,Injectable,56382,0.160849709602166,0.000102603346048332,0.00458183286566962,0.00457224612259547,0.0286118049742516,0.776702044983717,0.0177120169539154,0.00519842355528056,0.00147044935841079,0.000198868237946173
-No,25-35,Implant,13675,0.0767191077213785,0.000792636826001015,0.00343239787975005,0.00189818189797192,0.0129293567400633,0.0160528242588684,0.884711767691817,0.0026312118337615,7.76940300764835E-05,0.000754821120310778
-No,25-35,IUD,5413,0.0724207660807627,4.58844768748395E-05,0.000349949095786767,0.000358411946218748,0.0169565691150318,0.0121087838059928,0.00875796241179762,0.888916408142792,7.15867830220883E-05,1.36781417206554E-05
-No,25-35,F.sterilization,4243,0,0,0,0,0,0,0,0,1,0
-No,25-35,Other.mod,101,0.109698754010189,5.06927616543415E-05,0.000552498465494666,0.000691889060915951,0.002439371962606,0.0975838326625219,0.0017207868537868,0.000478102690868267,0.000145495636660946,0.786638575895302
-No,>35,None,90718,0.954648484395293,0.000387744682823539,0.00411013462891569,0.00353234576473293,0.00735261243593772,0.0194197605578421,0.00677627065642389,0.00139267452346594,0.00237188697000037,8.08538456480851E-06
-No,>35,Withdrawal,733,0.0771237556458427,0.891248499922701,0.000224027150148571,0.0147420187447626,0.000447228445962413,0.000873781836787433,0.0151251984382047,0.000127766403704502,8.74655895699181E-05,2.57822315437213E-07
-No,>35,Other.trad,8955,0.0527697605205442,0.00124256293061289,0.923906251170436,0.00379105844822052,0.00267922109004845,0.00891611394221807,0.00397639606398111,0.00134706815132522,0.00136828099429596,3.28668831793339E-06
-No,>35,Condom,3481,0.0992864106706795,3.17078634223757E-05,0.00961036556448798,0.873781200622683,0.00634906803801654,0.00712825627576685,0.00352874299320003,0.00014231351645102,0.000137175367539039,4.75908775401547E-06
-No,>35,Pill,10756,0.0970687566340639,0.00101579644436729,0.00439343150408718,0.00896530458717011,0.809487654982681,0.0503973274479088,0.0123868420005513,0.0120777525120395,0.00323924071270901,0.000967893174422244
-No,>35,Injectable,24626,0.104776146332597,0.00131000453997036,0.00808170860742794,0.00747943289883663,0.0220751105971402,0.831967150751299,0.0155090466560617,0.0055125595761822,0.00285440278819253,0.000434437252292689
-No,>35,Implant,6525,0.0515896689858522,2.58851754701557E-05,0.000226207470723457,0.00187193399596326,0.0163196126865887,0.0122839077992346,0.907143056885022,0.0104165565420737,0.000112023996902632,1.11464621681645E-05
-No,>35,IUD,4923,0.0312725565693595,1.93150959334073E-05,0.00697107767820452,0.00235717188219389,0.00669715693550896,0.00922179053789332,0.00249181850573598,0.938534791656249,0.00242886439789527,5.45674102678592E-06
-No,>35,F.sterilization,12037,0.000975238354069019,1.78789917889534E-07,1.89954402875655E-06,1.64412477340373E-06,3.46144082124028E-06,9.19941642181012E-06,3.13750814279025E-06,6.24145011185116E-07,0.999004614374283,2.30253042683543E-09
-No,>35,Other.mod,193,0.0604538195514679,4.84171902601811E-05,0.000344166378525395,0.000313355676912525,0.00085473407245106,0.0545071295471378,0.000632153390136902,0.000192941017031593,0.000144727566124995,0.882508555609952
+"postpartum","age_grp","From","n","None","Withdrawal","Other.trad","Condom","Pill","Injectable","Implant","IUD","F.sterilization","Other.mod"
+"1","<18","Birth",283.68367743979,0.800980213188989,0,0.00518965691047249,0.00993134367231809,0.00885221762049127,0.0507767737819975,0.124269794825731,0,0,0
+"1","18-20","Birth",355.347481764245,0.784855903041144,0,0.00655199210382721,0.0133572534177736,0.00815669975212254,0.0792981835593429,0.100700514113139,0.00380458257522344,0,0.00327487143742732
+"1","20-25","Birth",989.904901852143,0.72524512427127,0.00304586157391163,0.0104067449679841,0.0150901051192661,0.0107611807944115,0.124166960320661,0.106812961172305,0.00154821672283032,0,0.00292284505735989
+"1","25-35","Birth",1371.59463768787,0.770562389401038,0.00404161796426906,0.0109623990560826,0.0120752344767374,0.0141902335908799,0.0834628361238019,0.0829045018901436,0.00953334039185173,0.00916471375786734,0.00310273334732841
+"1",">35","Birth",363.051614490445,0.80128064049253,0,0.00369788521981218,0.00929684833196331,0.00587541723784746,0.0594360859143558,0.0621895663865769,0.00753259528768073,0.0406015272802031,0.0100894338490301
+"6","<18","None",137.312655063215,0.700495446740929,0,0.00544492146622592,0.0259977281431988,0.0171503751743176,0.109563622830394,0.141347905644935,0,0,0
+"6","<18","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6","<18","Other.trad",0.747656623138173,0,0,1,0,0,0,0,0,0,0
+"6","<18","Condom",0.819625518197536,0,0,0,1,0,0,0,0,0,0
+"6","<18","Pill",2.51122964807827,0,0,0,0,0.615392405479464,0.384607594520536,0,0,0,0
+"6","<18","Injectable",7.58755272070508,0.0912878292990385,0,0,0,0,0.785767269858482,0.122944900842479,0,0,0
+"6","<18","Implant",18.5727217682504,0,0,0,0,0,0,1,0,0,0
+"6","<18","IUD",0,0,0,0,0,0,0,0,1,0,0
+"6","<18","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","<18","Other.mod",0,0,0,0,0,0,0,0,0,0,1
+"6","18-20","None",162.474778583151,0.565003766923843,0,0,0.00784326669401571,0.0146250243295906,0.220494689286598,0.192033252765953,0,0,0
+"6","18-20","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6","18-20","Other.trad",2.32823389463422,0,0,0.678828570407984,0,0,0.321171429592016,0,0,0,0
+"6","18-20","Condom",2.62108810202434,0,0,0,0.397016954504767,0,0.602983045495233,0,0,0,0
+"6","18-20","Pill",1.3078808590428,0,0,0,0,1,0,0,0,0,0
+"6","18-20","Injectable",12.222035227592,0,0,0,0,0,0.923674666329041,0.0763253336709587,0,0,0
+"6","18-20","Implant",30.5818860582454,0,0,0,0,0,0,1,0,0,0
+"6","18-20","IUD",0.798547449846652,0,0,0,0,0,0,0,1,0,0
+"6","18-20","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","18-20","Other.mod",0,0,0,0,0,0,0,0,0,0,1
+"6","20-25","None",485.962563566959,0.481420326560037,0.00620219059303444,0.00852213777681671,0.0191390726565953,0.0364036180129003,0.254073750624959,0.171209245697735,0.020484460390643,0,0.00254519768727808
+"6","20-25","Withdrawal",2.6484057481282,0,1,0,0,0,0,0,0,0,0
+"6","20-25","Other.trad",5.0463812003124,0,0,0.654939618066431,0,0,0.345060381933569,0,0,0,0
+"6","20-25","Condom",10.3644475166669,0,0,0,0.507513097529206,0,0.450976807428222,0.0415100950425716,0,0,0
+"6","20-25","Pill",8.18764324244072,0,0,0,0,0.608739551924415,0.319971809571134,0.0712886385044507,0,0,0
+"6","20-25","Injectable",92.21545650029,0.0329268333904569,0,0,0,0,0.855814378812374,0.10142343364878,0.00983535414838899,0,0
+"6","20-25","Implant",65.5673007859264,0,0,0,0,0,0,1,0,0,0
+"6","20-25","IUD",0.911051172384307,0,0,0,0,0,0,0,1,0,0
+"6","20-25","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","20-25","Other.mod",2.89333864963487,0,0,0,0,0,0.330330026633235,0,0,0,0.669669973366765
+"6","25-35","None",727.912472926319,0.530903691604947,0,0.0128337446945971,0.0118913325474501,0.035538242445889,0.201235252129493,0.193178882834386,0.0144188537432382,0,0
+"6","25-35","Withdrawal",4.63241035499009,0,0.809412867941609,0,0,0,0.190587132058391,0,0,0,0
+"6","25-35","Other.trad",10.9137790384541,0,0,0.921420003187245,0,0,0.0785799968127553,0,0,0,0
+"6","25-35","Condom",13.5840473803958,0.0959625512013908,0,0,0.805194977175019,0,0.0703587529127866,0,0,0,0.0284837187108035
+"6","25-35","Pill",16.3723514510013,0,0,0,0,0.736106778654333,0.156850695887571,0.107042525458096,0,0,0
+"6","25-35","Injectable",80.7219039619132,0.0444698832786082,0,0,0,0,0.90780286960703,0.0350363089835146,0,0.0126909381308477,0
+"6","25-35","Implant",92.7722328235806,0.0062514649504057,0,0,0,0.0051821364192482,0.0140092274079869,0.974557171222359,0,0,0
+"6","25-35","IUD",11.1940510092495,0,0,0,0,0,0,0,1,0,0
+"6","25-35","F.sterilization",9.90340974029157,0.231834467334251,0,0,0,0,0,0,0,0.768165532665749,0
+"6","25-35","Other.mod",2.65716933754801,0,0,0,0,0,0,0,0,0,1
+"6",">35","None",213.146437632304,0.657172449379868,0,0.0115073903259851,0.0183995813113972,0.0638817736714209,0.131838336065334,0.106807204141625,0.00314269353219168,0.00473114200623824,0.0025194295659408
+"6",">35","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6",">35","Other.trad",0.781135738471966,0,0,1,0,0,0,0,0,0,0
+"6",">35","Condom",1.65598880012649,0.439083012639911,0,0,0.560916987360089,0,0,0,0,0,0
+"6",">35","Pill",2.13307971400551,0,0,0,0,1,0,0,0,0,0
+"6",">35","Injectable",14.9440506400651,0,0,0,0,0,1,0,0,0,0
+"6",">35","Implant",19.5658539868174,0.0391984307145107,0,0,0,0,0,0.960801569285489,0,0,0
+"6",">35","IUD",2.7347208804956,0,0,0,0,0,0,0,1,0,0
+"6",">35","F.sterilization",12.5301273369373,0,0,0,0,0,0,0,0,1,0
+"6",">35","Other.mod",2.10076884142422,0,0,0,0,0,0,0,0,0,1
+"No","<18","None",15671.7307564081,0.845670873311465,0.00123769903717076,0.00880861874307843,0.0880777681883083,0.00954723172237253,0.0192186435608037,0.0150487378326992,0.000126943454259614,0.000890714754508683,0.0113727693953336
+"No","<18","Withdrawal",20.3600092591495,0.527601959232508,0.0184099216713499,0.00334994135486646,0.107415041461223,0.258262790370327,0.0357404902285142,0.00639699406367662,4.85370405257829e-05,0.000330775626679378,0.0424435489503284
+"No","<18","Other.trad",339.053891205812,0.10315032786601,0.000142573647961109,0.822194416695302,0.051094770656644,0.0177069146786476,0.00245585443451039,0.000799323817976862,6.63865534864607e-06,4.47053828072174e-05,0.00240447416479104
+"No","<18","Condom",1552.09311029974,0.563763618356945,0.00113959893130304,0.00311287105653161,0.369945561428445,0.0110023854570715,0.0193496790002979,0.00570457411521483,4.51579378663831e-05,0.000306191541545282,0.0256303621747793
+"No","<18","Pill",363.679050237616,0.159554781751362,0.000174682974195164,0.000762621258512119,0.0233080848406279,0.706609474079037,0.092368694499852,0.00422129580127747,1.0847907253662e-05,7.31760381853933e-05,0.0129163408496947
+"No","<18","Injectable",860.840053217009,0.149070477361402,0.000154326853393258,0.00121471131048668,0.00850927899329415,0.018728726629907,0.765142527237161,0.0557309739010786,1.05119736991497e-05,7.100735443931e-05,0.0013674583851394
+"No","<18","Implant",864.384143527019,0.107328801607824,0.000110227608967904,0.0165776564205782,0.00638475091022766,0.00105458724417238,0.034918014184494,0.832715310729956,7.44825684178289e-06,5.02881755822184e-05,0.000852914861356881
+"No","<18","IUD",11.523352152721,0.172642787452722,0.000178845477635593,0.000839648301897382,0.00965949121919685,0.00087334797011001,0.00179032093739183,0.00141782121362647,0.811146547877882,8.24174569314135e-05,0.00136877209260658
+"No","<18","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"No","<18","Other.mod",171.514963750379,0.675897124563814,0.000976408392107953,0.00433956239150007,0.173169518222607,0.0302191154194791,0.0377612559178373,0.00855158334119949,6.28210645359513e-05,0.000428216667915955,0.0685943940190022
+"No","18-20","None",9384.16956412937,0.756251899758387,0.00137393760210801,0.0212160147371649,0.106141232552276,0.021151438459898,0.050196840476118,0.0290548129891307,0.000522662466976434,0.000200497945856946,0.0138906630120848
+"No","18-20","Withdrawal",40.8064126487296,0.270966706580725,0.514489074875432,0.00540730869258327,0.180416776767134,0.00747921989707645,0.0111839932606178,0.00679528721507195,8.1147460418025e-05,3.15439431150281e-05,0.00314894130782522
+"No","18-20","Other.trad",566.742641427673,0.175133086401395,0.0106209479316344,0.691571509578737,0.07364169730561,0.00442479455295892,0.016532054286779,0.00465943600942513,4.99509627921149e-05,1.94269645841766e-05,0.0233470960060868
+"No","18-20","Condom",1522.75088708302,0.395191660961917,0.000485123640169979,0.0191921976125517,0.48756078909219,0.0326565309469285,0.0335773881975805,0.0246092090247707,0.000130220907779219,5.05702466554076e-05,0.00654630936945674
+"No","18-20","Pill",463.125038054846,0.23667793655215,0.000372085189096927,0.0042331699613484,0.0398354740421781,0.577838933012888,0.100164363730582,0.0277166608662277,7.19264101769685e-05,2.79547962418563e-05,0.0130614954391104
+"No","18-20","Injectable",2026.81532174855,0.227995736629899,0.000224597300847759,0.00594934033870168,0.0191904626898201,0.0206468869177924,0.621891501887936,0.100587460387368,7.07918128300304e-05,2.75073253401618e-05,0.00341571470946585
+"No","18-20","Implant",2471.61173894888,0.121972933194884,0.000115963159769582,0.00165334277349112,0.00893443864362633,0.0271920254625177,0.0385222720076318,0.798906868968101,3.5661838719218e-05,1.38651856592346e-05,0.00265262876560157
+"No","18-20","IUD",10.9690624427155,0,0,0,0,0,0,0,1,0,0
+"No","18-20","F.sterilization",32.3635906570766,0.0581365257371342,4.55698153151478e-05,0.000713715239782193,0.00393841103636463,0.000708167710509365,0.00173924881606954,0.000921982409987286,1.70330820497043e-05,0.93319016868272,0.000589177470068292
+"No","18-20","Other.mod",206.973126872919,0.525294535035695,0.0110349321870358,0.0564780534139418,0.143090492767935,0.0346882022120799,0.0245406487232783,0.0265193474926035,0.00019379612657594,7.51706439462165e-05,0.178084821396908
+"No","20-25","None",19015.7852760673,0.72360665294974,0.00676095695747552,0.018916493511973,0.0601617937228666,0.018025673229627,0.0974197502580399,0.047584218047213,0.0032989858956334,0.000314930708707582,0.0239105447187227
+"No","20-25","Withdrawal",263.956063822005,0.431936402939062,0.173432342319776,0.149250875446886,0.0317277335713091,0.00986451559783598,0.0813419530863565,0.0978385460452252,0.00110017005734251,0.000102723867997907,0.0234047370682084
+"No","20-25","Other.trad",1592.79064294115,0.16344824981549,0.0129047974592782,0.613007824415146,0.0707676761779801,0.015531138315745,0.067118860172711,0.0307381283004002,0.000477781986060997,2.96675242404609e-05,0.0259758758329481
+"No","20-25","Condom",2632.14586430144,0.309847722655611,0.0116558898558182,0.0236564204463502,0.516083770985818,0.0159391649429329,0.0668713794343056,0.0357728623151257,0.00202737205939511,6.34688748135765e-05,0.0180819484298291
+"No","20-25","Pill",1765.2911782453,0.207695348572531,0.00720802570557336,0.0117652307366112,0.0201989687487019,0.576417129884584,0.105284800093417,0.0478889416532992,0.0119370037679399,4.07425646055796e-05,0.0115638082727357
+"No","20-25","Injectable",10910.0702401699,0.188168962277219,0.0021145659210545,0.00673242563426482,0.0111162817541672,0.0273065806478553,0.690660351695775,0.0671743063734154,0.00059960313991531,3.69007861072389e-05,0.00609002177022625
+"No","20-25","Implant",11740.8673355639,0.133826560479366,0.00143756833654887,0.00313039973685786,0.0095302185393062,0.0113465166495669,0.0507812550555207,0.785659669775228,0.000720373231477977,2.55762074550673e-05,0.00354186198867125
+"No","20-25","IUD",480.886376535157,0.11522251027926,0.000582541017593221,0.00130712913399642,0.00453824970142224,0.00158311443690905,0.0220233238221396,0.0223772021017662,0.830037804803736,2.20638109647877e-05,0.00230606089221218
+"No","20-25","F.sterilization",52.915087212352,0.17160992633294,0.000847402970670225,0.00189409096091399,0.00675336531207497,0.0018598209437865,0.0103213165384137,0.00479919309449372,0.000339482926348726,0.798152949576641,0.00342245134371779
+"No","20-25","Other.mod",646.57131680175,0.489780508589197,0.00923628900002153,0.081618457557146,0.102343615314798,0.0440543721624115,0.128442583480626,0.0423867395193081,0.00179198910419986,0.000124897171195813,0.100220548101096
+"No","25-35","None",29521.86561342,0.755643273838502,0.00300620841362317,0.0112857120464418,0.0268426234964299,0.0244539760182218,0.0989420932648351,0.0577150454965598,0.00685203075818269,0.00191847320550116,0.0133405634617012
+"No","25-35","Withdrawal",737.111228275479,0.179463410088731,0.534954224441519,0.00887346454026204,0.0415671657500016,0.0418674109801924,0.0833679613385358,0.0968530262564852,0.00117250450096551,0.000267746582408913,0.0116130855209
+"No","25-35","Other.trad",2225.97103570823,0.121419247040154,0.000804823754185128,0.669208520146206,0.0299568613079637,0.037327820854157,0.081467382678572,0.0305750125223983,0.0111278704389881,0.000237784663164129,0.0178746765942125
+"No","25-35","Condom",2134.31090171814,0.351252635349114,0.0178701183499532,0.018430946400004,0.483351100445704,0.0289481369334892,0.0476126785764525,0.0178179007927509,0.00320602509621242,0.000597099530316546,0.030913358526004
+"No","25-35","Pill",5631.88034215276,0.164976692533637,0.00254881823061393,0.00842446182922279,0.0104355601902473,0.654374915070565,0.0899181594699373,0.0540396773764926,0.00788632766826678,0.000226892381127831,0.00716849524989105
+"No","25-35","Injectable",25400.8726047037,0.165581265494938,0.00231601571934937,0.00847671528711541,0.00919300637342482,0.0266280199629119,0.724259593225598,0.057520728137369,0.00218574719366814,0.000466671502081583,0.00337223710354482
+"No","25-35","Implant",25548.5090763888,0.0980771440395839,0.00196337620730793,0.00265683107378695,0.00227064135454978,0.00774390126436411,0.0401080862742778,0.841878004615104,0.00269754061983674,0.000118489546362036,0.00248598500482751
+"No","25-35","IUD",2407.26274345809,0.0851899166168138,0.00353844233923986,0.00609246268481678,0.00170254076192522,0.0145070817340051,0.0106150957698388,0.0234898482619807,0.853840127296298,9.15697079460038e-05,0.00093291482713515
+"No","25-35","F.sterilization",1153.99661299145,0.0321082963234437,5.89726736854192e-05,0.000311782309601544,0.000991597668558395,0.000478233935321105,0.00224316819441864,0.00115565878877994,0.000122193750126534,0.957994758346631,0.00453533800943184
+"No","25-35","Other.mod",832.042437568435,0.370282763355865,0.00267155213960756,0.0282287124230453,0.105834100579182,0.0159624159332114,0.125772051895407,0.0504015249083013,0.00216387450852499,0.00637479540126377,0.292308208855592
+"No",">35","None",32484.9808843115,0.879203507189883,0.00173093437282742,0.00341253902355678,0.0264750692517297,0.0154040322419185,0.0456320189526981,0.0181338159373109,0.000929582670852122,0.00273936291682605,0.0063391374423975
+"No",">35","Withdrawal",307.311641634925,0.11762204624925,0.775377561413157,0.000519386155780914,0.0295954846208784,0.00180028081829289,0.0424668330011139,0.0313977220742166,0.000184852750161059,0.000217901035982738,0.000817931881167088
+"No",">35","Other.trad",2761.38393736168,0.0326827210917257,0.00262729824692334,0.928395080602176,0.00507631856506267,0.00565506757127658,0.0206255177900886,0.00119495012295645,0.00111343173005955,6.13068163410625e-05,0.00256830746339049
+"No",">35","Condom",2421.10463293159,0.210664870835499,0.010594049587957,0.000672624691448069,0.72225271799297,0.00688151056504813,0.00869835459243923,0.0235239221082242,0.000142379403094853,0.000317308628885573,0.016252261594435
+"No",">35","Pill",3850.11729788996,0.142262687557663,0.000267270977684691,0.0144079245259171,0.00428693710666189,0.7126080258434,0.0685100995773661,0.0508209592143597,0.0057775709300593,0.000292643437297556,0.00076588082959044
+"No",">35","Injectable",15243.3866253205,0.11948558037833,0.00139229768608682,0.0116923345873979,0.00528545144551024,0.0231589866068133,0.776822631469909,0.0521451944673566,0.00463609477460432,0.00182079284902942,0.00356063573496302
+"No",">35","Implant",13750.5840052907,0.0701463999411593,0.00233172504945429,0.00461243221102044,0.00326335433378071,0.0156353636872242,0.038543887415533,0.858697987935352,0.00205007517464738,0.00130931190846945,0.00340946234336123
+"No",">35","IUD",2457.75409571225,0.060684114684616,6.94184254276601e-05,0.00138859598979283,0.00093664156684831,0.000742386405172348,0.0132530483431076,0.00662645699155946,0.912642812333284,9.69972173005017e-05,0.00355952804289037
+"No",">35","F.sterilization",4518.57491685354,0.00657555266060744,9.16511311530206e-06,1.72383554155571e-05,9.48762215033815e-05,7.59941302574115e-05,0.000211961789907303,0.00303303838534049,5.85135052685485e-06,0.989948843629762,2.74783635614008e-05
+"No",">35","Other.mod",777.674863824774,0.208564766186913,0.000505048259462453,0.0202026107612663,0.0250352218149925,0.0274716808044319,0.0731300784345896,0.0706011584517703,0.00044865683862316,0.000414011506503807,0.573626766941447
```

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/matrices_kenya_pma_2019_20.csv` & `fpsim-0.28.1/fpsim/locations/ethiopia/matrices_ethiopia_dhs_2008_11.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-postpartum,age_grp,From,n,None,Withdrawal,Other.trad,Condom,Pill,Injectable,Implant,IUD,F.sterilization,Other.mod
-1,<18,Birth,282,0.75531914893617,0,0.00354609929078014,0.0177304964539007,0.0106382978723404,0.0638297872340425,0.148936170212766,0,0,0
-1,18-20,Birth,420,0.764285714285714,0,0.00714285714285714,0.00714285714285714,0.0166666666666667,0.0904761904761905,0.104761904761905,0.00714285714285714,0,0.00238095238095238
-1,20-25,Birth,1083,0.734995383194829,0.00369344413665743,0.0110803324099723,0.00923361034164358,0.0193905817174515,0.112650046168052,0.0987996306555863,0.00184672206832872,0,0.00831024930747922
-1,25-35,Birth,1456,0.752747252747253,0.00343406593406593,0.0144230769230769,0.0144230769230769,0.0212912087912088,0.0899725274725275,0.0782967032967033,0.00824175824175824,0.00824175824175824,0.00892857142857143
-1,>35,Birth,372,0.793010752688172,0,0.00806451612903226,0.00537634408602151,0.00806451612903226,0.0403225806451613,0.0806451612903226,0.00537634408602151,0.0483870967741935,0.010752688172043
-6,<18,None,140,0.714285714285714,0,0,0.0142857142857143,0.0214285714285714,0.128571428571429,0.121428571428571,0,0,0
-6,<18,Withdrawal,0,0,1,0,0,0,0,0,0,0,0
-6,<18,Other.trad,0,0,0,1,0,0,0,0,0,0,0
-6,<18,Condom,1,0,0,0,1,0,0,0,0,0,0
-6,<18,Pill,3,0,0,0,0,0.666666666666667,0.333333333333333,0,0,0,0
-6,<18,Injectable,12,0.0833333333333333,0,0,0,0.0833333333333333,0.75,0.0833333333333333,0,0,0
-6,<18,Implant,29,0,0,0,0,0,0,1,0,0,0
-6,<18,IUD,0,0,0,0,0,0,0,0,1,0,0
-6,<18,F.sterilization,0,0,0,0,0,0,0,0,0,1,0
-6,<18,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,18-20,None,222,0.558558558558559,0,0.0045045045045045,0.0045045045045045,0.0225225225225225,0.211711711711712,0.198198198198198,0,0,0
-6,18-20,Withdrawal,0,0,1,0,0,0,0,0,0,0,0
-6,18-20,Other.trad,3,0,0,0.666666666666667,0,0,0.333333333333333,0,0,0,0
-6,18-20,Condom,3,0,0,0,0.333333333333333,0,0.333333333333333,0.333333333333333,0,0,0
-6,18-20,Pill,6,0,0,0,0,0.5,0.166666666666667,0.333333333333333,0,0,0
-6,18-20,Injectable,29,0,0,0,0,0,0.896551724137931,0.103448275862069,0,0,0
-6,18-20,Implant,39,0,0,0,0,0,0,1,0,0,0
-6,18-20,IUD,1,0,0,0,0,0,0,0,1,0,0
-6,18-20,F.sterilization,0,0,0,0,0,0,0,0,0,1,0
-6,18-20,Other.mod,0,0,0,0,0,0,0,0,0,0,1
-6,20-25,None,636,0.482704402515723,0.00157232704402516,0.00628930817610063,0.0188679245283019,0.0408805031446541,0.257861635220126,0.177672955974843,0.0110062893081761,0,0.00314465408805031
-6,20-25,Withdrawal,3,0,1,0,0,0,0,0,0,0,0
-6,20-25,Other.trad,8,0,0,0.75,0,0,0.125,0,0,0.125,0
-6,20-25,Condom,7,0,0,0,0.285714285714286,0,0.571428571428571,0.142857142857143,0,0,0
-6,20-25,Pill,20,0,0,0,0,0.6,0.25,0.15,0,0,0
-6,20-25,Injectable,102,0.0588235294117647,0,0,0,0,0.833333333333333,0.0980392156862745,0.00980392156862745,0,0
-6,20-25,Implant,84,0,0,0,0,0,0,1,0,0,0
-6,20-25,IUD,1,0,0,0,0,0,0,0,1,0,0
-6,20-25,F.sterilization,0,0,0,0,0,0,0,0,0,1,0
-6,20-25,Other.mod,9,0,0,0,0,0.111111111111111,0.111111111111111,0.111111111111111,0,0,0.666666666666667
-6,25-35,None,889,0.548931383577053,0.00337457817772778,0.00899887514060742,0.015748031496063,0.0382452193475816,0.184476940382452,0.175478065241845,0.0213723284589426,0.00112485939257593,0.00224971878515186
-6,25-35,Withdrawal,4,0,0.75,0,0,0,0.25,0,0,0,0
-6,25-35,Other.trad,18,0,0,0.944444444444444,0,0,0.0555555555555556,0,0,0,0
-6,25-35,Condom,18,0.111111111111111,0,0,0.666666666666667,0,0.0555555555555556,0.111111111111111,0,0,0.0555555555555556
-6,25-35,Pill,29,0,0,0,0,0.724137931034483,0.137931034482759,0.103448275862069,0.0344827586206897,0,0
-6,25-35,Injectable,103,0.029126213592233,0,0,0,0,0.932038834951456,0.029126213592233,0.00970873786407767,0,0
-6,25-35,Implant,105,0,0,0,0.00952380952380952,0.00952380952380952,0.00952380952380952,0.971428571428571,0,0,0
-6,25-35,IUD,10,0,0,0,0,0,0,0,1,0,0
-6,25-35,F.sterilization,12,0,0,0,0,0,0,0,0,1,0
-6,25-35,Other.mod,11,0,0,0,0,0,0,0,0,0,1
-6,>35,None,252,0.595238095238095,0.00396825396825397,0.0317460317460317,0.0119047619047619,0.0436507936507936,0.166666666666667,0.115079365079365,0.00793650793650794,0.0119047619047619,0.0119047619047619
-6,>35,Withdrawal,0,0,1,0,0,0,0,0,0,0,0
-6,>35,Other.trad,3,0,0,1,0,0,0,0,0,0,0
-6,>35,Condom,1,0,0,0,1,0,0,0,0,0,0
-6,>35,Pill,3,0,0,0,0,1,0,0,0,0,0
-6,>35,Injectable,13,0,0,0,0,0,1,0,0,0,0
-6,>35,Implant,28,0.0357142857142857,0,0,0,0,0,0.964285714285714,0,0,0
-6,>35,IUD,2,0,0,0,0,0,0,0,1,0,0
-6,>35,F.sterilization,16,0,0,0,0,0,0,0,0,1,0
-6,>35,Other.mod,3,0,0,0,0,0,0,0,0,0,1
-No,<18,None,43352,0.944751819613194,0.00122102282740034,0.00262635200009514,0.0305869282272007,0.00204933896706218,0.00628583889635198,0.00788297631834313,0.000268679332897911,0,0.00432704381745283
-No,<18,Withdrawal,122,0.416466492198195,0.232246605886468,0.0474733320717631,0.104465784420973,0.0899112210503367,0.0560902184147357,0.00663175910237017,5.74476789180559E-05,0,0.0466571391762405
-No,<18,Other.trad,285,0.228393944323099,0.00016900345113238,0.681602417287721,0.067404018621041,0.000837562825983891,0.00223886701304411,0.00155495427242589,2.86390597886129E-05,0,0.0177705931457649
-No,<18,Condom,1429,0.657275099010727,0.000639657569619765,0.00581061736653172,0.296267569950679,0.00152152353657139,0.0165019339639325,0.0044905856413356,0.000102370123564115,0,0.0173906428370372
-No,<18,Pill,269,0.248670124311603,0.000360213502276671,0.00106984783667353,0.0282560227109057,0.665630388991342,0.0352736362418882,0.00310632755506405,3.27132697717351E-05,0,0.017600725580475
-No,<18,Injectable,825,0.109877288802577,0.00724712839073313,0.000903819874133284,0.00294580973125761,0.000880677634909256,0.80351524990281,0.073798061128468,1.42491331921407E-05,0,0.000817715401919574
-No,<18,Implant,1060,0.124278205837112,0.000139041369299758,0.00900680880357786,0.00266852036627108,0.000132920266140062,0.00990382193894422,0.85340597380613,1.63080761346421E-05,0,0.00044839953639011
-No,<18,IUD,16,0,0,0,0,0,0,0,1,0,0
-No,<18,F.sterilization,0,0,0,0,0,0,0,0,0,1,0
-No,<18,Other.mod,195,0.663444055768006,0.000754987868423489,0.0246795686384671,0.0866152272177022,0.023514246324951,0.0301493779022767,0.0309123117456213,0.000108727113454532,0,0.139821497421097
-No,18-20,None,14295,0.848999483638825,0.00186920276727978,0.0134199181226119,0.0596707566357376,0.0111296432234131,0.0349147665271017,0.0198000747101015,0.000774332776963767,0,0.00942182159796515
-No,18-20,Withdrawal,90,0.40069405783565,0.213003631635669,0.00908670650204958,0.262598307470078,0.0591860537505937,0.0161513911493858,0.00707090814674655,0.000173906164455449,0,0.0320350373453717
-No,18-20,Other.trad,478,0.154373382846478,0.000712034050738575,0.740124926761863,0.0556930151293048,0.00273023218763028,0.0219590207682703,0.00318658721630485,5.95960983113159E-05,0,0.0211612049410992
-No,18-20,Condom,1179,0.42226899112632,0.0114940818664706,0.0166885392584121,0.501740741025295,0.00998312589946163,0.0216716796527446,0.00586448544601764,0.000187974522040911,0,0.0101003812032377
-No,18-20,Pill,455,0.275436192287349,0.000658529762322907,0.0032597517344035,0.0407268467366386,0.570759427429189,0.0731663921738998,0.0247443738082529,0.000115711008034851,0,0.0111327750599102
-No,18-20,Injectable,2442,0.241111413887013,0.000273917018059337,0.0054409524355137,0.00955185856847591,0.0178575584887726,0.648187884138841,0.073791702585513,0.000101639314170206,0,0.00368307356364133
-No,18-20,Implant,2669,0.160757796342874,0.000177400139675328,0.00139853864786162,0.0062979580664277,0.0169485134037884,0.0461098251406565,0.765198490699856,6.52571070876125E-05,0,0.00304622045177308
-No,18-20,IUD,26,0,0,0,0,0,0,0,1,0,0
-No,18-20,F.sterilization,10,0,0,0,0,0,0,0,0,1,0
-No,18-20,Other.mod,198,0.554915285847907,0.00209946517824254,0.0542595732439473,0.12096146807157,0.0467074626757721,0.0409771869717167,0.0339715854840049,0.00028278587096782,0,0.145825186655871
-No,20-25,None,23495,0.783635972725049,0.0049410429456991,0.0128715915055542,0.0428646014975542,0.016597027076478,0.074479516358645,0.0432657105024226,0.00176560296160391,0.00071446661386953,0.018864467813125
-No,20-25,Withdrawal,208,0.4657348789915,0.319171953269567,0.0619195775677326,0.0178609395264682,0.00721924914909223,0.0569150179580557,0.0487778409508441,0.000579604077489053,0.000232674860632807,0.0215882636486179
-No,20-25,Other.trad,1228,0.163364055452572,0.0105135994249956,0.642800538841422,0.0348045255658771,0.0221215505105008,0.0522046367892553,0.0509946329662246,0.000337308209001859,6.80900177036426E-05,0.0227910622224465
-No,20-25,Condom,2086,0.385057385000765,0.00643616693426798,0.0243539712354377,0.46209610303594,0.0117665213875847,0.0488955083464433,0.0386131420245445,0.00049967485524634,0.00018231946864701,0.0220992077111238
-No,20-25,Pill,1746,0.187642588943073,0.00402462732168628,0.00252959995914693,0.0136776995520298,0.611636456803162,0.109215853776241,0.0535974709349754,0.00999946570859738,8.21219595783548E-05,0.00759411504150853
-No,20-25,Injectable,11883,0.221339466794206,0.00137912452512778,0.00804593783533227,0.01080745996736,0.024512460663478,0.660982509615237,0.0660788746987946,0.00114513420265456,9.93989869780945E-05,0.00560963271083076
-No,20-25,Implant,11816,0.132415465404315,0.000500213722131383,0.00272551636133508,0.00703063303382132,0.0121420570328198,0.0485419107389333,0.792703512704341,0.00102962346090215,5.71777536555084E-05,0.00285388978774601
-No,20-25,IUD,372,0.134836049561925,0.000503012147195806,0.00110694066934834,0.00387089288876838,0.0246652204713083,0.0316412475556217,0.0305537360806658,0.770686851644578,5.85876254971759E-05,0.0020774613550914
-No,20-25,F.sterilization,47,0.224148819241767,0.00142018408623454,0.00420902153742034,0.145736427618026,0.00303027943068566,0.0132509617476543,0.00857676142441939,0.000224450888430318,0.593534994573248,0.00586809945211595
-No,20-25,Other.mod,632,0.558006845607444,0.007388074091845,0.0457274969446646,0.0826077707638457,0.0222300290493651,0.107938721378894,0.0544232408612828,0.000919468984654157,0.00031236574405868,0.120445986573946
-No,25-35,None,35445,0.777421734340582,0.00366483846063637,0.0110767806207633,0.026416998988199,0.0183854636909432,0.0883434313120514,0.0562245961015398,0.00481703513992939,0.00181781104032358,0.0118313103050318
-No,25-35,Withdrawal,768,0.185038289711006,0.57213646436089,0.0120677789691766,0.0207059731109349,0.0238577500258163,0.0941406309902215,0.0884637175420889,0.000895760110137007,0.000231198261734901,0.0024624369179946
-No,25-35,Other.trad,2256,0.121968109808041,0.000609327156053473,0.679646671549691,0.0266267643338399,0.0429536074067543,0.0782897499530666,0.0175150133216568,0.00499938656537001,0.000149107486694107,0.027242262418833
-No,25-35,Condom,2059,0.373005976807267,0.0104459749848621,0.010498824560804,0.466630841123867,0.0255924190794495,0.0501143610953016,0.0354375666065661,0.00152532587232386,0.000426001325980434,0.0263227085435783
-No,25-35,Pill,5545,0.194756257177956,0.00200578172435779,0.00485474988646576,0.0102630556511861,0.631643640887236,0.0795089826414506,0.0593545827128321,0.0104228556730403,0.000234123187624422,0.00695597045784957
-No,25-35,Injectable,26225,0.188402651927822,0.00261850681586334,0.00826105321480307,0.00876705683223637,0.0258898196340459,0.690191419976688,0.067740835225041,0.00323378727753114,0.000953937566684152,0.00394093152928438
-No,25-35,Implant,25084,0.10807021529984,0.00165520052579459,0.00458724909049132,0.00280447902486396,0.00888156189283402,0.0350710238602752,0.8334834500222,0.00202000013970297,0.000120811599385029,0.00330600854461318
-No,25-35,IUD,2429,0.113177074652731,0.00383216136746232,0.00464512114941786,0.00528331241208242,0.0162556637216964,0.0146416949111476,0.00874228879379087,0.832194601675122,0.000116760147026016,0.0011113211695229
-No,25-35,F.sterilization,793,0.0264790885573275,5.58044002060641E-05,0.000165031875904082,0.000426902212656041,0.000271621955636944,0.00134219465290622,0.000808526917578336,6.93669721756595E-05,0.970177563622226,0.000203898833384028
-No,25-35,Other.mod,912,0.390884498735252,0.00192421417944214,0.029281522909488,0.080481912392549,0.02718311148013,0.116756193184901,0.0628292134875542,0.00871333936435447,0.000503887762987872,0.281442106503341
-No,>35,None,41518,0.909156850156284,0.0013169412332621,0.00432401236111489,0.0204171554647055,0.0101662763958686,0.0280613977450053,0.0174563367450248,0.00119580171529524,0.00223572574680547,0.00566950243663507
-No,>35,Withdrawal,412,0.153695082560043,0.744851818527927,0.000855401486954817,0.001999972845726,0.00188902602258758,0.0685704398347065,0.026859689198612,0.000289245719135218,0.000257812803639607,0.00073151100066926
-No,>35,Other.trad,2605,0.0837592655261902,0.00386193782236669,0.854640045351431,0.0117030287006889,0.00792396512665075,0.0241197972835271,0.00594181223179346,0.00418953931106027,0.000115947561672827,0.00374466108461991
-No,>35,Condom,2198,0.273099599714091,0.00416526671245326,0.00524950265360483,0.659186138711022,0.00202583805123524,0.0130259155329282,0.024578748856353,0.000238223169095938,0.000346585344100359,0.0180841812551157
-No,>35,Pill,3180,0.187064686461951,0.000302163890010023,0.0156249125791457,0.00513051308493786,0.660326640224361,0.073851284122297,0.047126461284983,0.00924320254528776,0.000324796703461079,0.00100533910356524
-No,>35,Injectable,13195,0.16315277044098,0.00225100354132111,0.0111114908741715,0.00794449652755781,0.0238627933728423,0.727175386569284,0.0537075248656814,0.00405250886513167,0.00179841274319337,0.00494361219983617
-No,>35,Implant,12391,0.0946536950440962,0.00169069100402517,0.00803978522231729,0.00499692727632759,0.00774525157774653,0.037333158522861,0.834858899502407,0.00355031559028364,0.00190780176618931,0.00522347449374573
-No,>35,IUD,1990,0.0841215669842402,9.06492206584361E-05,0.00565541292170896,0.0011052866608347,0.000763536422334483,0.0162296382892036,0.0066709387954417,0.880567811910768,0.000111097877258846,0.00468406091755186
-No,>35,F.sterilization,3258,0.0139883299388557,9.18941022102323E-06,2.91514904397442E-05,0.000149732549780276,7.33019030987491E-05,0.000200300854442527,0.000118762782920662,7.94938777040452E-06,0.985381343966367,4.19377161039727E-05
-No,>35,Other.mod,739,0.243209801092358,0.000432257139120107,0.0245747531497352,0.033851003182345,0.0227243738365575,0.0390005948187704,0.0844670758010167,0.000571174602461358,0.000401051615619272,0.550767914762016
+"postpartum","age_grp","From","n","None","Withdrawal","Other.trad","Condom","Pill","Injectable","Implant","IUD","F.sterilization","Other.mod"
+"1","<18","Birth",1209.310123,0.949998166020479,0,0,0,0.00314523787377574,0.038275124072537,0.00730921939036807,0.00127225264284007,0,0
+"1","18-20","Birth",1134.407523,0.938179646574858,0,0,0,0.00153091368382965,0.0466064962793798,0.0118061576007373,0.00187678586119532,0,0
+"1","20-25","Birth",3608.427083,0.958265461782646,0.000596515032863143,0,0,0.000296626750487118,0.0342821944727101,0.00528032839842201,0.00125736252822599,0,2.15110346460062e-05
+"1","25-35","Birth",4861.624184,0.969266948380805,0,0.000507785856447846,0,0.00319684356745416,0.0195150567812792,0.00444460414507433,0.00252688968440429,0.000529800927121602,1.20706574138599e-05
+"1",">35","Birth",1223.020567,0.955597068875784,0,0,0,0.000936277795236783,0.0297832620177024,0.00284792430641111,0.00480787172240579,0.00602759528245938,0
+"6","<18","None",838.58196,0.831641275707863,0,0.00462189646912986,0,0.00692560569750391,0.137569086270351,0.0180165800370902,0.0012255558180622,0,0
+"6","<18","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6","<18","Other.trad",0,0,0,1,0,0,0,0,0,0,0
+"6","<18","Condom",0,0,0,0,1,0,0,0,0,0,0
+"6","<18","Pill",3.803568,0.013459993353609,0,0,0,0.186122083264976,0.800417923381414,0,0,0,0
+"6","<18","Injectable",37.647729,0.00364176017097871,0,0,0,0,0.996358239829021,0,0,0,0
+"6","<18","Implant",6.352089,0,0,0,0,0,0,1,0,0,0
+"6","<18","IUD",0,0,0,0,0,0,0,0,1,0,0
+"6","<18","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","<18","Other.mod",0,0,0,0,0,0,0,0,0,0,1
+"6","18-20","None",895.341791,0.797071488423352,0,0.00268660306508579,0,0.00457809301565373,0.153363638758151,0.0383253360280153,0.00397484070974187,0,0
+"6","18-20","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6","18-20","Other.trad",0,0,0,1,0,0,0,0,0,0,0
+"6","18-20","Condom",0,0,0,0,1,0,0,0,0,0,0
+"6","18-20","Pill",0,0,0,0,0,1,0,0,0,0,0
+"6","18-20","Injectable",49.28511,0.21506020783965,0,0,0,0.0337022480014755,0.701637999793447,0.049599544365428,0,0,0
+"6","18-20","Implant",8.593817,0,0,0,0,0,0,1,0,0,0
+"6","18-20","IUD",2.709903,0,0,0,0,0,0,0,1,0,0
+"6","18-20","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","18-20","Other.mod",0,0,0,0,0,0,0,0,0,0,1
+"6","20-25","None",2948.672404,0.806995748246573,0.000538650545867828,0.00109138437882569,0.00110542256087123,0.0187220719823307,0.133825315916647,0.0306546128614971,0.00666758368048267,0,0.000399209826904868
+"6","20-25","Withdrawal",2.152481,0,1,0,0,0,0,0,0,0,0
+"6","20-25","Other.trad",0,0,0,1,0,0,0,0,0,0,0
+"6","20-25","Condom",0,0,0,0,1,0,0,0,0,0,0
+"6","20-25","Pill",2.807036,0,0,0,0,0.381311817874798,0.618688182125202,0,0,0,0
+"6","20-25","Injectable",105.830483,0.0722173969479096,0,0,0,0,0.92778260305209,0,0,0,0
+"6","20-25","Implant",19.082669,0,0,0,0,0,0,1,0,0,0
+"6","20-25","IUD",4.487141,0,0,0,0,0,0,0,1,0,0
+"6","20-25","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"6","20-25","Other.mod",0.077621,0,0,0,0,0,0,0,0,0,1
+"6","25-35","None",4361.482223,0.858240242333323,0.000721462300913751,0.00187885507288929,9.26643694358582e-05,0.0117661953840778,0.108270890228503,0.0151386241245721,0.00389106618628536,0,0
+"6","25-35","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6","25-35","Other.trad",2.468664,0,0,1,0,0,0,0,0,0,0
+"6","25-35","Condom",0,0,0,0,1,0,0,0,0,0,0
+"6","25-35","Pill",13.340493,0.295444028942559,0,0,0,0.621396225761672,0,0,0.0831597452957698,0,0
+"6","25-35","Injectable",81.053036,0,0,0,0,0,0.989029578114754,0,0.00665688821329284,0.00431353367195277,0
+"6","25-35","Implant",20.632007,0,0,0,0,0,0,1,0,0,0
+"6","25-35","IUD",11.834989,0,0,0,0,0,0,0,1,0,0
+"6","25-35","F.sterilization",2.575693,0,0,0,0,0,0,0,0,1,0
+"6","25-35","Other.mod",0.058683,0,0,0,0,0,0,0,0,0,1
+"6",">35","None",1148.1786,0.889735299891498,0,0.0035019786991327,0.000439587534552551,0.0012098788463746,0.0732609491241171,0.0194032766330952,0.00992230128657685,0,0.00252672798465326
+"6",">35","Withdrawal",0,0,1,0,0,0,0,0,0,0,0
+"6",">35","Other.trad",0,0,0,1,0,0,0,0,0,0,0
+"6",">35","Condom",0,0,0,0,1,0,0,0,0,0,0
+"6",">35","Pill",1.145087,0,0,0,0,1,0,0,0,0,0
+"6",">35","Injectable",31.26771,0.0567757600412694,0,0,0,0,0.943224239958731,0,0,0,0
+"6",">35","Implant",3.894872,0,0,0,0,0,0,1,0,0,0
+"6",">35","IUD",5.880126,0,0,0,0,0,0,0,1,0,0
+"6",">35","F.sterilization",5.416673,0,0,0,0,0,0,0,0,1,0
+"6",">35","Other.mod",0,0,0,0,0,0,0,0,0,0,1
+"No","<18","None",76395.327294,0.923560327963726,0.000416905814177658,0.00167613801900936,0.000667366906730844,0.0042046381255809,0.0595524819031303,0.00758277716700051,0.0006019039947123,0,0.00173746010593117
+"No","<18","Withdrawal",5.201384,0,1,0,0,0,0,0,0,0,0
+"No","<18","Other.trad",150.232227,0.13742230610505,2.84952263458264e-05,0.857073026121836,4.71013798231068e-05,0.000342243678651082,0.00437555694012898,0.000531991322718495,4.26545553616279e-05,0,0.000136624670085734
+"No","<18","Condom",75.141319,0.28146161345436,6.0364997492978e-05,0.000253109346994278,0.699510074487722,0.000741333584402521,0.0164195698134462,0.00116319454040213,0.000101822326996119,0,0.000288917448182992
+"No","<18","Pill",379.232466,0.46814198999777,0.00010810477812104,0.000630282335068105,0.00130517847949833,0.302288880510928,0.186892353550558,0.00303197633952981,0.000477085937037741,0,0.0371241480714883
+"No","<18","Injectable",8376.236897,0.326673720898834,7.094668380595e-05,0.0017336609822235,0.000528994993726471,0.00429880559633976,0.654869797554714,0.00897211313422257,0.00234990698628072,0,0.000502053169851324
+"No","<18","Implant",1038.675544,0.193702862916288,4.06551565969422e-05,0.000770688600222662,6.80343398937653e-05,0.000746782577449591,0.00871967960508464,0.795680261380346,6.47165979412501e-05,0,0.000206318826176897
+"No","<18","IUD",62.478632,0.415777153703642,9.26257444022619e-05,0.000377664721804988,0.00015284672038688,0.00110124754962328,0.0141653060646468,0.00172678782677813,0.566165782904194,0,0.000440584764522104
+"No","<18","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"No","<18","Other.mod",138.802284,0.598753667596625,0.000143877889276215,0.000588634774849968,0.024044336208744,0.0185508174554758,0.0257536601174573,0.00269165409631437,0.0002188534375615,0,0.329254498423696
+"No","18-20","None",26090.015382,0.878345317278128,0.000221106440046947,0.00210467347188936,0.00170263440394177,0.0114620919212556,0.0844813456957486,0.0194376061185074,0.00164655710986346,0,0.000598667560617962
+"No","18-20","Withdrawal",74.233496,0.0598918691347912,0.936174394583507,6.64283187725034e-05,7.06684489516102e-05,0.000362547122192084,0.00274421561447276,0.000606195822738613,5.23177969888546e-05,0,3.13631575858434e-05
+"No","18-20","Other.trad",210.336418,0.187364315750264,2.18317696618407e-05,0.800180580735751,0.000225900102441403,0.00116626326745863,0.00882258855393115,0.00195066186254515,0.000168289148541649,0,9.95688094042932e-05
+"No","18-20","Condom",43.479078,0.802276880507005,0.000122772559317502,0.00119427507410027,0.11704604570356,0.00681237411645297,0.0498468488146254,0.0109387642816266,0.008970626193664,0,0.0027914127496481
+"No","18-20","Pill",491.095988,0.232622781699299,2.73572317350085e-05,0.000267735508349481,0.000282616013298587,0.738449605425997,0.0250325701307138,0.00261730415323643,0.00025281081142492,0,0.00044721902594467
+"No","18-20","Injectable",8075.979097,0.278986741780505,3.33191180540873e-05,0.000325967710822879,0.000366280970809544,0.00692426573479144,0.686774112182957,0.021903585215172,0.0045336387961686,0,0.000152088490717996
+"No","18-20","Implant",1684.978423,0.204634787800489,2.3846456509599e-05,0.000233423626131575,0.00179046314080993,0.00583057064658958,0.022416551149686,0.76469853887445,0.000244510108955675,0,0.000127308196378942
+"No","18-20","IUD",172.341053,0.323935131226764,3.94422247760204e-05,0.00038570372153946,0.000404819836698576,0.0372278288829772,0.115106885043956,0.00483050032583294,0.517881340250295,0,0.000188348487160855
+"No","18-20","F.sterilization",0,0,0,0,0,0,0,0,0,1,0
+"No","18-20","Other.mod",16.655668,0.897395508279317,0.000176366599378522,0.00170298465541421,0.00156427684136233,0.00928486976406328,0.0693379833834988,0.0156369552885497,0.00133760255609781,0,0.00356345263231783
+"No","20-25","None",64673.126926,0.870374903162304,0.000773887059676911,0.00262169917728346,0.00111088773031446,0.010640663024617,0.079427564902343,0.0291170704803293,0.00469789089318732,0,0.00123543356994442
+"No","20-25","Withdrawal",174.100255,0.153457122255013,0.835727436733143,0.000211384589175396,9.03072414902368e-05,0.000935291046451771,0.00669290947568474,0.00238544338489938,0.000372120546885301,0,0.000127984727256963
+"No","20-25","Other.trad",629.552563,0.047340650523645,1.67201078367805e-05,0.868120149920786,2.5774542213736e-05,0.0332538495782051,0.0407718307584086,0.00472599318722739,0.000442661731998977,0,0.00530236964968002
+"No","20-25","Condom",324.96586,0.0850739146337553,3.44615942524963e-05,0.000126687488706588,0.888688564952995,0.000643631552248542,0.0236779870275511,0.00142530198529015,0.000255186624172447,0,7.42641410271665e-05
+"No","20-25","Pill",1672.294334,0.35534888647889,0.000158222674143192,0.00268824136210445,0.000230133676933748,0.49164117924982,0.108756439052785,0.0297274259873875,0.0111042686821977,0,0.000345202835740226
+"No","20-25","Injectable",24646.815134,0.250452411472527,0.000106496985500108,0.00139293530562243,0.000243717976988558,0.0118303373440664,0.715115824408026,0.0151638628862614,0.00518093540885227,0,0.000513478212154605
+"No","20-25","Implant",8180.774976,0.141322078110991,5.80662636419562e-05,0.000217059605716466,8.42655310129355e-05,0.00269874638258665,0.0409240395854201,0.812715464058212,0.00185510728089296,0,0.000125173181524653
+"No","20-25","IUD",1584.87254,0.0686699785361641,2.78029971803378e-05,9.2990249304295e-05,3.94407604404205e-05,0.000657443636202499,0.00379481996784393,0.0264987767401459,0.900162457095339,0,5.62900173788915e-05
+"No","20-25","F.sterilization",8.4656,0,0,0,0,0,0,0,0,1,0
+"No","20-25","Other.mod",112.58729,0.704162809818865,0.000369310694565903,0.0254409853280422,0.000526358809948989,0.0213533694123907,0.0609749621873202,0.0144523187159537,0.00240422395971999,0,0.170315661073193
+"No","25-35","None",103568.779642,0.874958629117281,0.000110357023181889,0.00140118685608727,0.000821727224878583,0.00782445183418366,0.0826804144642343,0.0260857245148037,0.00575684715963198,0.00023136438944337,0.000129297416274587
+"No","25-35","Withdrawal",320.397136,0.0663805694123607,0.897380433050853,7.26488448559795e-05,3.02230804748658e-05,0.000461845390209969,0.0341843259122601,0.00118691209583852,0.000283728843041885,1.47088935515004e-05,4.60447655402966e-06
+"No","25-35","Other.trad",1014.679664,0.179478035203436,1.01813038295085e-05,0.802834456168583,8.04573213473281e-05,0.000816712236585592,0.00814004382876749,0.00806874007622079,0.000536839668736907,2.09428809405967e-05,1.3591311553072e-05
+"No","25-35","Condom",444.236323,0.161346945493664,1.52415941543423e-05,0.000163441107812071,0.759365599278711,0.00102884252542928,0.0613262040014841,0.00274228065972956,0.000933201020690027,3.15742470919784e-05,0.0130466700712341
+"No","25-35","Pill",2500.429666,0.34068972603166,3.69151321483752e-05,0.00182650689313036,0.000171181900043351,0.460538958633574,0.145155669095063,0.0462746513194277,0.00519780059650161,7.6613704415605e-05,3.197669403604e-05
+"No","25-35","Injectable",42532.488023,0.205908724582828,0.000205834002728201,0.0015511905919061,0.00018143253920325,0.00943784492649666,0.756058228129015,0.0202952163599845,0.00590480322306855,0.000438845808149127,1.78798366210625e-05
+"No","25-35","Implant",13551.325997,0.109836140725022,7.52963021028836e-06,0.000662605083355975,4.89663235874622e-05,0.0013592176606731,0.017619641414245,0.869198216764302,0.00101668177359701,1.5535310367569e-05,0.0002354653146405
+"No","25-35","IUD",3675.349943,0.0641017592642433,3.53710610559355e-06,0.00133202632685359,2.79940117844355e-05,0.000283559823320665,0.0028186517440381,0.000859760520945531,0.930560962454961,7.27290059685356e-06,4.47584714938164e-06
+"No","25-35","F.sterilization",632.103701,0,0,0,0,0,0,0,0,1,0
+"No","25-35","Other.mod",196.07277,0.360273752222513,2.16229781987671e-05,0.000304902571920141,0.000170464553264769,0.00171973720051745,0.0171629612523005,0.00522391175965884,0.0337531054883014,4.4515243858943e-05,0.581325026729466
+"No",">35","None",76177.170207,0.934203998481473,0.000102462780208174,0.000870788631303866,0.000147976717303352,0.00341730008284315,0.0482428477697264,0.0118080136476036,0.00100453882389978,0,0.00020207306563915
+"No",">35","Withdrawal",196.443841,0,1,0,0,0,0,0,0,0,0
+"No",">35","Other.trad",507.190114,0.0867296870616335,4.20335815185874e-06,0.910433319865122,6.45116113522836e-06,0.000150484665850455,0.00211671954105655,0.000507892353560815,4.26468665254786e-05,0,8.5951269646502e-06
+"No",">35","Condom",461.537219,0.176915505948491,8.89860122253739e-06,7.65340483490708e-05,0.816217271748099,0.000315822147462285,0.00529738841419512,0.00106147214153762,8.92282948346422e-05,0,1.78786558086689e-05
+"No",">35","Pill",1091.82635,0.198485497396797,2.05910969465235e-05,0.0141163235112338,1.70047445794692e-05,0.692147697677606,0.066006394419528,0.00754899807829967,0.0183257608078661,0,0.00333173226714337
+"No",">35","Injectable",20896.94128,0.174741386155267,0.000318440722847711,0.000484282717894568,4.48608536124822e-05,0.0060905178517119,0.805377827652482,0.0117458035609438,0.00116750153775807,0,2.93789474823633e-05
+"No",">35","Implant",5637.840456,0.0997998626701986,9.67953846780301e-06,0.00132169150448449,0.000209931327027561,0.00605788014093088,0.0314617891614677,0.860987184652107,0.000130408619141164,0,2.15723861758351e-05
+"No",">35","IUD",1358.298968,0.129947774955976,6.40046501423701e-06,0.000179528411836477,9.74304506398131e-06,0.0148478013126033,0.00374687541579634,0.000821846474229916,0.850397686732045,0,4.23431874348582e-05
+"No",">35","F.sterilization",1303.752007,0,0,0,0,0,0,0,0,1,0
+"No",">35","Other.mod",174.609688,0.0956570774154595,4.64479834546036e-06,4.05558508465878e-05,7.12804244338494e-06,0.000166271701365226,0.00233879275431871,0.000561193280265228,4.71233566118547e-05,0,0.901177212800344
```

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/mortality_prob_kenya.csv` & `fpsim-0.28.1/fpsim/locations/kenya/mortality_prob.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya/mortality_trend_kenya.csv` & `fpsim-0.28.1/fpsim/locations/kenya/mortality_trend.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/kenya.py` & `fpsim-0.28.1/fpsim/locations/senegal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,279 +1,239 @@
 '''
-Set the parameters for FPsim, specifically for Kenya.
+Set the parameters for FPsim, specifically for Senegal.
 '''
 
 import numpy as np
 import pandas as pd
+
 import sciris as sc
 from scipy import interpolate as si
 from .. import defaults as fpd
 
-# %% Housekeeping
-
-thisdir = sc.path(sc.thisdir())  # For loading CSV files
+thisdir = sc.path(sc.thisdir(__file__))  # For loading CSV files
 
+# %% Housekeeping
 
 def scalar_pars():
     scalar_pars = {
-        # Basic parameters
-        'location': 'kenya',
-        'n_agents': 1_000,  # Number of agents
-        'scaled_pop': None,  # Scaled population / total population size
-        'start_year': 1960,  # Start year of simulation
-        'end_year': 2020,  # End year of simulation
-        'timestep': 1,  # The simulation timestep in months
-        'method_timestep': 1,  # How many simulation timesteps to go for every method update step
-        'seed': 1,  # Random seed
-        'verbose': 1,  # How much detail to print during the simulation
-        'track_switching': 0,  # Whether to track method switching
-        'track_as': 0,  # Whether to track age-specific channels
-
-        # Age limits (in years)
-        'method_age': 15,
-        'age_limit_fecundity': 50,
-        'max_age': 99,
-
-        # Durations (in months)
-        'switch_frequency': 12,  # How frequently to check for changes to contraception
-        'end_first_tri': 3,
-        'preg_dur_low': 9,
-        'preg_dur_high': 9,
-        'postpartum_dur': 23,
-        'breastfeeding_dur_mu': 11.4261936291137,  # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R
-        'breastfeeding_dur_beta': 7.5435309020483, # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R 
-        'max_lam_dur': 5,  # Duration of lactational amenorrhea
-
-        # Pregnancy outcomes
-        'abortion_prob': 0.201,
-        # From https://bmcpregnancychildbirth.biomedcentral.com/articles/10.1186/s12884-015-0621-1, % of all pregnancies calculated
-        'twins_prob': 0.016,  # From https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0025239
-        'LAM_efficacy': 0.98,  # From Cochrane review: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6823189/
-        'maternal_mortality_factor': 1,
-
-        # Fecundity and exposure
-        'fecundity_var_low': 0.7,
-        'fecundity_var_high': 1.1,
-        'high_parity': 4,
-        'high_parity_nonuse': 0.6,
-        'primary_infertility': 0.05,
-        'exposure_factor': 1.0,  # Overall exposure correction factor
-
-        # MCPR
-        'mcpr_growth_rate': 0.02,  # The year-on-year change in MCPR after the end of the data
-        'mcpr_max': 0.90,  # Do not allow MCPR to increase beyond this
-        'mcpr_norm_year': 2020,  # Year to normalize MCPR trend to 1
+        'location': 'senegal',
+        'breastfeeding_dur_mu': 19.66828,
+        # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R
+        'breastfeeding_dur_beta': 7.2585,
+        # Scale parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R
+        'abortion_prob': 0.08,  # From https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4712915/
+        'twins_prob': 0.015,  # From https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0025239
+        'mcpr_norm_year': 2018,  # Year to normalize MCPR trend to 1
     }
     return scalar_pars
 
 
 def data2interp(data, ages, normalize=False):
     ''' Convert unevenly spaced data into an even spline interpolation '''
     model = si.interp1d(data[0], data[1])
     interp = model(ages)
     if normalize:
         interp = np.minimum(1, np.maximum(0, interp))
     return interp
 
 
-# TODO- these need to be changed for Kenya calibration and commented with their data source
 def filenames():
     ''' Data files for use with calibration, etc -- not needed for running a sim '''
     files = {}
-    files['base'] = sc.thisdir(aspath=True) / 'kenya'
-    files['basic_dhs'] = 'kenya_basic_dhs.yaml' # From World Bank https://data.worldbank.org/indicator/SH.STA.MMRT?locations=KE
-    files['popsize'] = 'kenya_popsize.csv' # Downloaded from World Bank: https://data.worldbank.org/indicator/SP.POP.TOTL?locations=KE
-    files['mcpr'] = 'kenya_cpr.csv'  # From UN Population Division Data Portal, married women 1970-1986, all women 1990-2030
-    files['tfr'] = 'kenya_tfr.csv'   # From World Bank https://data.worldbank.org/indicator/SP.DYN.TFRT.IN?locations=KE
-    files['asfr'] = 'kenya_asfr.csv' # From UN World Population Prospects 2022: https://population.un.org/wpp/Download/Standard/Fertility/
-    files['skyscrapers'] = 'kenya_skyscrapers.csv' # Choose from either DHS 2014 or PMA 2022
-    #files['pregnancy_parity'] = 'SNIR80FL.obj'
-    #files['spacing'] = 'BirthSpacing.obj'
-    #files['methods'] = 'Method_v312.csv'
+    files['base'] = sc.thispath(__file__) / 'senegal'
+    files['basic_dhs']        = 'basic_dhs.yaml'
+    files['popsize']          = 'popsize.csv'
+    files['mcpr']             = 'cpr.csv'
+    files['tfr']              = 'tfr.csv'
+    files['asfr']             = 'asfr.csv'
+    files['ageparity']        = 'ageparity.csv'
+    files['spacing']          = 'birth_spacing_dhs.csv'
+    files['methods']          = 'mix.csv'
+    files['afb'] = 'afb.table.csv'
+    files['use'] = 'use.csv'
     return files
 
 
 # %% Demographics and pregnancy outcome
 
 def age_pyramid():
-    '''
-    Starting age bin, male population, female population
-    Data are from World Population Prospects
-    https://population.un.org/wpp/Download/Standard/Population/
-     '''
-    pyramid = np.array([[0, 801895, 800503],  # Kenya 1960
-                        [5, 620524, 625424],
-                        [10, 463547, 464020],
-                        [15, 333241, 331921],
-                        [20, 307544, 309057],
-                        [25, 292141, 287621],
-                        [30, 247826, 236200],
-                        [35, 208416, 190234],
-                        [40, 177914, 162057],
-                        [45, 156771, 138943],
-                        [50, 135912, 123979],
-                        [55, 108653, 111939],
-                        [60, 85407, 94582],
-                        [65, 61664, 71912],
-                        [70, 40797, 49512],
-                        [75, 22023, 29298],
-                        [80, 11025, 17580],
-                        ], dtype=float)
+    ''' Starting age bin, male population, female population '''
+    pyramid = np.array([
+        [0, 318225, 314011],  # Senegal 1962
+        [5, 249054, 244271],
+        [10, 191209, 190998],
+        [15, 157800, 159536],
+        [20, 141480, 141717],
+        [25, 125002, 124293],
+        [30, 109339, 107802],
+        [35, 93359, 92119],
+        [40, 77605, 78231],
+        [45, 63650, 66117],
+        [50, 51038, 54934],
+        [55, 39715, 44202],
+        [60, 29401, 33497],
+        [65, 19522, 23019],
+        [70, 11686, 14167],
+        [75, 5985, 7390],
+        [80, 2875, 3554],
+    ], dtype=float)
 
     return pyramid
 
 
 def age_mortality():
     '''
-    Age-dependent mortality rates taken from UN World Population Prospects 2022.  From probability of dying each year.
-    https://population.un.org/wpp/
-    Used CSV WPP2022_Life_Table_Complete_Medium_Female_1950-2021, Kenya, 2010
-    Used CSV WPP2022_Life_Table_Complete_Medium_Male_1950-2021, Kenya, 2010
-    Mortality rate trend from crude death rate per 1000 people, also from UN Data Portal, 1950-2030:
-    https://population.un.org/dataportal/data/indicators/59/locations/404/start/1950/end/2030/table/pivotbylocation
-    Projections go out until 2030, but the csv file can be manually adjusted to remove any projections and stop at your desired year
-    '''
-    data_year = 2010
-    mortality_data = pd.read_csv(thisdir / 'kenya' / 'mortality_prob_kenya.csv')
-    mortality_trend = pd.read_csv(thisdir / 'kenya' / 'mortality_trend_kenya.csv')
-
+    Age-dependent mortality rates, Senegal specific from 1990-1995 -- see age_dependent_mortality.py in the fp_analyses repository
+    Mortality rate trend from crude mortality rate per 1000 people: https://data.worldbank.org/indicator/SP.DYN.CDRT.IN?locations=SN
+    '''
     mortality = {
-        'ages': mortality_data['age'].to_numpy(),
-        'm': mortality_data['male'].to_numpy(),
-        'f': mortality_data['female'].to_numpy()
+        'bins': np.array([0., 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95]),
+        'm': np.array(
+            [0.03075891, 0.00266326, 0.00164035, 0.00247776, 0.00376541, 0.00377009, 0.00433534, 0.00501743, 0.00656144,
+             0.00862479, 0.01224844, 0.01757291, 0.02655129, 0.0403916, 0.06604032, 0.10924413, 0.17495116, 0.26531436,
+             0.36505174, 0.43979833]),
+        'f': np.array(
+            [0.02768283, 0.00262118, 0.00161414, 0.0023998, 0.00311697, 0.00354105, 0.00376715, 0.00429043, 0.00503436,
+             0.00602394, 0.00840777, 0.01193858, 0.01954465, 0.03220238, 0.05614077, 0.0957751, 0.15973906, 0.24231313,
+             0.33755308, 0.41632442])
     }
 
-    mortality['year'] = mortality_trend['year'].to_numpy()
-    mortality['probs'] = mortality_trend['crude_death_rate'].to_numpy()
-    trend_ind = np.where(mortality['year'] == data_year)
-    trend_val = mortality['probs'][trend_ind]
+    mortality['year'] = np.array(
+        [1950., 1955, 1960, 1965, 1970, 1975, 1980, 1985, 1990, 1995, 2000, 2005, 2010, 2015, 2020, 2025,
+         2030])  # Starting year bin
+    mortality['probs'] = np.array(
+        [28, 27, 26.023, 25.605, 24.687, 20.995, 16.9, 13.531, 11.335, 11.11, 10.752, 9.137, 7.305, 6.141, 5.7, 5.7,
+         5.7])  # First 2 estimated, last 3 are projected
+    mortality['probs'] /= mortality['probs'][8]  # Normalize around 2000 for trending # CK: TODO: shouldn't be hardcoded
 
-    mortality['probs'] /= trend_val  # Normalize around data year for trending
-    m_mortality_spline_model = si.splrep(x=mortality['ages'],
+    m_mortality_spline_model = si.splrep(x=mortality['bins'],
                                          y=mortality['m'])  # Create a spline of mortality along known age bins
-    f_mortality_spline_model = si.splrep(x=mortality['ages'], y=mortality['f'])
+    f_mortality_spline_model = si.splrep(x=mortality['bins'], y=mortality['f'])
     m_mortality_spline = si.splev(fpd.spline_ages,
                                   m_mortality_spline_model)  # Evaluate the spline along the range of ages in the model with resolution
     f_mortality_spline = si.splev(fpd.spline_ages, f_mortality_spline_model)
     m_mortality_spline = np.minimum(1, np.maximum(0, m_mortality_spline))  # Normalize
     f_mortality_spline = np.minimum(1, np.maximum(0, f_mortality_spline))
 
     mortality['m_spline'] = m_mortality_spline
     mortality['f_spline'] = f_mortality_spline
 
     return mortality
 
 
 def maternal_mortality():
     '''
-    From World Bank indicators for maternal mortality ratio (modeled estimate) per 100,000 live births:
-    https://data.worldbank.org/indicator/SH.STA.MMRT?locations=KE
+    Risk of maternal death assessed at each pregnancy. Data from Huchon et al. (2013) prospective study on risk of maternal death in Senegal and Mali.
+    Maternal deaths: The annual number of female deaths from any cause related to or aggravated by pregnancy
+    or its management (excluding accidental or incidental causes) during pregnancy and childbirth or within
+    42 days of termination of pregnancy, irrespective of the duration and site of the pregnancy,
+    expressed per 100,000 live births, for a specified time period.
     '''
 
     data = np.array([
-        [2000, 708],
-        [2001, 702],
-        [2002, 692],
-        [2003, 678],
-        [2004, 653],
-        [2005, 618],
-        [2006, 583],
-        [2007, 545],
-        [2008, 513],
-        [2009, 472],
-        [2010, 432],
-        [2011, 398],
-        [2012, 373],
-        [2013, 364],
-        [2014, 358],
-        [2015, 353],
-        [2016, 346],
-        [2017, 342],
-
+        [1990, 0.00278, 0.00319, 0.00364],
+        [2000, 0.00268, 0.00309, 0.00354],
+        [2001, 0.00263, 0.00304, 0.00350],
+        [2002, 0.00259, 0.00300, 0.00346],
+        [2003, 0.00255, 0.00296, 0.00341],
+        [2004, 0.00252, 0.00293, 0.00338],
+        [2005, 0.00249, 0.00290, 0.00335],
+        [2006, 0.00245, 0.00286, 0.00331],
+        [2007, 0.00242, 0.00283, 0.00329],
+        [2008, 0.00237, 0.00278, 0.00323],
+        [2009, 0.00230, 0.00271, 0.00317],
+        [2010, 0.00220, 0.00261, 0.00306],
+        [2011, 0.00207, 0.00248, 0.00293],
+        [2012, 0.00194, 0.00235, 0.00280],
+        [2013, 0.00182, 0.002228327, 0.00268338],
+        [2014, 0.00172, 0.00213, 0.00258],
+        [2015, 0.00161, 0.00202, 0.00248],
+        [2016, 0.00152, 0.00193, 0.00239],
+        [2017, 0.00143, 0.00184, 0.00230],
+        [2018, 0.00135, 0.00176, 0.00222],
+        [2019, 0.00128, 0.00169, 0.00214]
     ])
 
     maternal_mortality = {}
     maternal_mortality['year'] = data[:, 0]
-    maternal_mortality['probs'] = data[:, 1] / 100000  # ratio per 100,000 live births
-    # maternal_mortality['ages'] = np.array([16, 17,   19, 22,   25, 50])
-    # maternal_mortality['age_probs'] = np.array([2.28, 1.63, 1.3, 1.12, 1.0, 1.0]) #need to be added
+    maternal_mortality['probs'] = data[:, 3]
 
     return maternal_mortality
 
 
 def infant_mortality():
     '''
-    From World Bank indicators for infant mortality (< 1 year) for Kenya, per 1000 live births
+    From World Bank indicators for infant morality (< 1 year) for Senegal, per 1000 live births
     From API_SP.DYN.IMRT.IN_DS2_en_excel_v2_1495452.numbers
     Adolescent increased risk of infant mortality gradient taken
     from Noori et al for Sub-Saharan African from 2014-2018.  Odds ratios with age 23-25 as reference group:
     https://www.medrxiv.org/content/10.1101/2021.06.10.21258227v1
     '''
 
     data = np.array([
-        [1960, 118.1],
-        [1961, 113.7],
-        [1962, 109.8],
-        [1963, 106.5],
-        [1964, 103.8],
-        [1965, 101.6],
-        [1966, 99.8],
-        [1967, 98.0],
-        [1968, 96.3],
-        [1969, 94.5],
-        [1970, 92.6],
-        [1971, 90.8],
-        [1972, 88.8],
-        [1973, 86.7],
-        [1974, 84.5],
-        [1975, 82.2],
-        [1976, 79.8],
-        [1977, 77.4],
-        [1978, 75.0],
-        [1979, 72.7],
-        [1980, 70.5],
-        [1981, 68.5],
-        [1982, 66.7],
-        [1983, 65.1],
-        [1984, 63.8],
-        [1985, 62.9],
-        [1986, 62.4],
-        [1987, 62.4],
-        [1988, 62.8],
-        [1989, 63.7],
-        [1990, 64.8],
-        [1991, 66.1],
-        [1992, 67.2],
-        [1993, 67.9],
-        [1994, 68.0],
-        [1995, 67.6],
-        [1996, 66.5],
-        [1997, 65.1],
-        [1998, 63.5],
-        [1999, 61.7],
-        [2000, 59.7],
-        [2001, 57.6],
-        [2002, 55.4],
-        [2003, 53.1],
-        [2004, 50.7],
-        [2005, 48.1],
-        [2006, 45.8],
-        [2007, 43.8],
-        [2008, 41.4],
-        [2009, 40.3],
-        [2010, 39.4],
-        [2011, 38.6],
-        [2012, 38.2],
-        [2013, 37.5],
-        [2014, 36.5],
-        [2015, 35.3],
-        [2016, 34.5],
-        [2017, 33.9],
-        [2018, 32.8],
-        [2019, 31.9]
+        [1960, 128.3],
+        [1961, 128.2],
+        [1962, 128.3],
+        [1963, 128.6],
+        [1964, 128.8],
+        [1965, 128.9],
+        [1966, 128.6],
+        [1967, 128.2],
+        [1968, 127.7],
+        [1969, 126.7],
+        [1970, 125.4],
+        [1971, 123.6],
+        [1972, 121.4],
+        [1973, 118.7],
+        [1974, 115.6],
+        [1975, 112.2],
+        [1976, 108.4],
+        [1977, 104.6],
+        [1978, 101],
+        [1979, 97.7],
+        [1980, 94.9],
+        [1981, 92.5],
+        [1982, 90.4],
+        [1983, 88.2],
+        [1984, 85.7],
+        [1985, 82.9],
+        [1986, 79.9],
+        [1987, 77],
+        [1988, 74.4],
+        [1989, 72.4],
+        [1990, 71],
+        [1991, 70.3],
+        [1992, 70.1],
+        [1993, 70.3],
+        [1994, 70.6],
+        [1995, 71],
+        [1996, 71.2],
+        [1997, 71.1],
+        [1998, 70.6],
+        [1999, 69.4],
+        [2000, 67.5],
+        [2001, 65.1],
+        [2002, 62.2],
+        [2003, 59.2],
+        [2004, 56.1],
+        [2005, 53.2],
+        [2006, 50.6],
+        [2007, 48.2],
+        [2008, 46.2],
+        [2009, 44.3],
+        [2010, 42.6],
+        [2011, 41.1],
+        [2012, 39.8],
+        [2013, 38.6],
+        [2014, 37.5],
+        [2015, 36.4],
+        [2016, 35.4],
+        [2017, 34.4],
+        [2018, 33.6],
+        [2019, 32.7],
     ])
 
     infant_mortality = {}
     infant_mortality['year'] = data[:, 0]
     infant_mortality['probs'] = data[:, 1] / 1000  # Rate per 1000 live births, used after stillbirth is filtered out
     infant_mortality['ages'] = np.array([16, 17, 19, 22, 25, 50])
     infant_mortality['age_probs'] = np.array([2.28, 1.63, 1.3, 1.12, 1.0, 1.0])
@@ -294,21 +254,21 @@
     return miscarriage_interp
 
 
 def stillbirth():
     '''
     From Report of the UN Inter-agency Group for Child Mortality Estimation, 2020
     https://childmortality.org/wp-content/uploads/2020/10/UN-IGME-2020-Stillbirth-Report.pdf
-
+    
     Age adjustments come from an extension of Noori et al., which were conducted June 2022.
     '''
 
     data = np.array([
-        [2000, 22.5],
-        [2010, 20.6],
+        [2000, 25.3],
+        [2010, 22.6],
         [2019, 19.7],
     ])
 
     stillbirth_rate = {}
     stillbirth_rate['year'] = data[:, 0]
     stillbirth_rate['probs'] = data[:, 1] / 1000  # Rate per 1000 total births
     stillbirth_rate['ages'] = np.array([15, 16, 17, 19, 20, 28, 31, 36, 50])
@@ -319,15 +279,15 @@
 
 # %% Fecundity
 
 def female_age_fecundity():
     '''
     Use fecundity rates from PRESTO study: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5712257/
     Fecundity rate assumed to be approximately linear from onset of fecundity around age 10 (average age of menses 12.5) to first data point at age 20
-    45-50 age bin estimated at 0.10 of fecundity of 25-27 yr olds
+    45-50 age bin estimated at 0.10 of fecundity of 25-27 yr olds, based on fertility rates from Senegal
     '''
     fecundity = {
         'bins': np.array([0., 5, 10, 15, 20, 25, 28, 31, 34, 37, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95, 99]),
         'f': np.array([0., 0, 0, 65, 70.8, 79.3, 77.9, 76.6, 74.8, 67.4, 55.5, 7.9, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])}
     fecundity[
         'f'] /= 100  # Conceptions per hundred to conceptions per woman over 12 menstrual cycles of trying to conceive
 
@@ -352,29 +312,29 @@
 
 
 def lactational_amenorrhea():
     '''
     Returns an array of the percent of breastfeeding women by month postpartum 0-11 months who meet criteria for LAM:
     Exclusively breastfeeding (bf + water alone), menses have not returned.  Extended out 5-11 months to better match data
     as those women continue to be postpartum insusceptible.
-    From DHS Kenya 2014 calendar data
+    From DHS Senegal calendar data
     '''
     data = np.array([
-        [0, 0.9557236],
-        [1, 0.8889493],
-        [2, 0.7040052],
-        [3, 0.5332317],
-        [4, 0.4115276],
-        [5, 0.2668908],
-        [6, 0.1364079],
-        [7, 0.0571638],
-        [8, 0.0025502],
-        [9, 0.0259570],
-        [10, 0.0072750],
-        [11, 0.0046938],
+        [0, 0.903125],
+        [1, 0.868794326],
+        [2, 0.746478873],
+        [3, 0.648854962],
+        [4, 0.563573883],
+        [5, 0.457564576],
+        [6, 0.254966887],
+        [7, 0.2],
+        [8, 0.146341463],
+        [9, 0.10982659],
+        [10, 0.10982659],
+        [11, 0.101796407],
     ])
 
     lactational_amenorrhea = {}
     lactational_amenorrhea['month'] = data[:, 0]
     lactational_amenorrhea['rate'] = data[:, 1]
 
     return lactational_amenorrhea
@@ -391,110 +351,120 @@
     Includes women who have had sex "within the last four weeks"
     Excludes women who answer "never had sex", probabilities are only applied to agents who have sexually debuted
     Data taken from 2018 DHS, no trend over years for now
     Onset of sexual activity probabilities assumed to be linear from age 10 to first data point at age 15
     '''
 
     sexually_active = np.array([[0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50],
-                                [0, 0, 0, 31.4, 55.0, 64.4, 69.6, 65.3, 60.7, 57.4, 57.4]])
+                                [0, 0, 0, 50.4, 55.9, 57.3, 60.8, 66.4, 67.5, 68.2, 68.2]])
 
     sexually_active[1] /= 100  # Convert from percent to rate per woman
     activity_ages = sexually_active[0]
     activity_interp_model = si.interp1d(x=activity_ages, y=sexually_active[1])
     activity_interp = activity_interp_model(fpd.spline_preg_ages)  # Evaluate interpolation along resolution of ages
 
     return activity_interp
 
 
 def sexual_activity_pp():
     '''
     Returns an array of monthly likelihood of having resumed sexual activity within 0-35 months postpartum
-    Uses 2014 Kenya DHS individual recode (postpartum (v222), months since last birth, and sexual activity within 30 days.
-    Data is weighted.
-    Limited to 23 months postpartum (can use any limit you want 0-23 max)
+    Uses DHS Senegal 2018 individual recode (postpartum (v222), months since last birth, and sexual activity within 30 days.
+    Limited to 35 months postpartum (can use any limit you want 0-35 max)
     Postpartum month 0 refers to the first month after delivery
-    TODO-- Add code for processing this for other countries to data_processing
     '''
 
     postpartum_sex = np.array([
-        [0, 0.08453],
-        [1, 0.08870],
-        [2, 0.40634],
-        [3, 0.58030],
-        [4, 0.52688],
-        [5, 0.60641],
-        [6, 0.58103],
-        [7, 0.72973],
-        [8, 0.62647],
-        [9, 0.73497],
-        [10, 0.60254],
-        [11, 0.75723],
-        [12, 0.73159],
-        [13, 0.68409],
-        [14, 0.74925],
-        [15, 0.74059],
-        [16, 0.70051],
-        [17, 0.78479],
-        [18, 0.74965],
-        [19, 0.79351],
-        [20, 0.77338],
-        [21, 0.70340],
-        [22, 0.72395],
-        [23, 0.72202],
+        [0, 0.104166667],
+        [1, 0.300000000],
+        [2, 0.383177570],
+        [3, 0.461538462],
+        [4, 0.476635514],
+        [5, 0.500000000],
+        [6, 0.565217391],
+        [7, 0.541666667],
+        [8, 0.547368421],
+        [9, 0.617391304],
+        [10, 0.578947368],
+        [11, 0.637254902],
+        [12, 0.608247423],
+        [13, 0.582278481],
+        [14, 0.542553191],
+        [15, 0.678260870],
+        [16, 0.600000000],
+        [17, 0.605042017],
+        [18, 0.562500000],
+        [19, 0.529411765],
+        [20, 0.674698795],
+        [21, 0.548780488],
+        [22, 0.616161616],
+        [23, 0.709401709],
+        [24, 0.651376147],
+        [25, 0.780219780],
+        [26, 0.717647059],
+        [27, 0.716417910],
+        [28, 0.683544304],
+        [29, 0.716417910],
+        [30, 0.640625000],
+        [31, 0.650000000],
+        [32, 0.676470588],
+        [33, 0.645161290],
+        [34, 0.606557377],
+        [35, 0.644736842],
     ])
 
-
-
     postpartum_activity = {}
     postpartum_activity['month'] = postpartum_sex[:, 0]
     postpartum_activity['percent_active'] = postpartum_sex[:, 1]
 
     return postpartum_activity
 
 
 def debut_age():
     '''
     Returns an array of weighted probabilities of sexual debut by a certain age 10-45.
     Data taken from DHS variable v531 (imputed age of sexual debut, imputed with data from age at first union)
-    Use sexual_debut_age_probs.py under locations/data_processing to output for other DHS countries
+    Use sexual_debut_age_probs.py under fp_analyses/data to output for other DHS countries
     '''
 
     sexual_debut = np.array([
-        [10.0, 0.008404629256166524],
-        [11.0, 0.006795048697926663],
-        [12.0, 0.026330525753311643],
-        [13.0, 0.04440278185223372],
-        [14.0, 0.08283157906888061],
-        [15.0, 0.14377365580688461],
-        [16.0, 0.13271744734209995],
-        [17.0, 0.11915611658325072],
-        [18.0, 0.13735481818469894],
-        [19.0, 0.0841039265081519],
-        [20.0, 0.07725867074164659],
-        [21.0, 0.03982337306065369],
-        [22.0, 0.031195559243867545],
-        [23.0, 0.020750304422300126],
-        [24.0, 0.014468030815585422],
-        [25.0, 0.010870195645684769],
-        [26.0, 0.007574195696769944],
-        [27.0, 0.0034378402773621282],
-        [28.0, 0.0031344552061394622],
-        [29.0, 0.0018168079578966389],
-        [30.0, 0.001385356426809007],
-        [31.0, 0.0004912818135032509],
-        [32.0, 0.00045904179812542576],
-        [33.0, 0.0005049625590548578],
-        [34.0, 0.000165858204720886],
-        [35.0, 0.00019259487032758347],
-        [36.0, 0.0002126920535675137],
-        [37.0, 8.84428869703282e-05],
-        [38.0, 5.07209448615522e-05],
-        [39.0, 6.555458199225806e-05],
-        [41.0, 0.00013980442816424654],
-        [44.0, 4.372731039149624e-05]])
+        [10, 0.004362494588533180],
+        [11, 0.005887267309386780],
+        [12, 0.016249279181639800],
+        [13, 0.0299019826473517],
+        [14, 0.055785658051997],
+        [15, 0.09813952463469960],
+        [16, 0.112872333807184],
+        [17, 0.11953800217275100],
+        [18, 0.10881048442282400],
+        [19, 0.08688267743864320],
+        [20, 0.0781062086093285],
+        [21, 0.055562127900473800],
+        [22, 0.047649966917757800],
+        [23, 0.03670233295320280],
+        [24, 0.02962171655627400],
+        [25, 0.03071900157389080],
+        [26, 0.020088166028125700],
+        [27, 0.012959307423989900],
+        [28, 0.009789125590573670],
+        [29, 0.010992698492904500],
+        [30, 0.0064009386756690000],
+        [31, 0.00531499008144595],
+        [32, 0.004500210075413140],
+        [33, 0.004643541107103950],
+        [34, 0.0015287248836055500],
+        [35, 0.0012933308143284600],
+        [36, 0.0008169702220519970],
+        [37, 0.0005138447212362420],
+        [38, 0.0030994890039629400],
+        [39, 0.0007583698086919300],
+        [40, 0.0001470674087999730],
+        [42, 0.00018238823303343100],
+        [43, 0.0000620676775406016],
+        [45, 0.0001177109855848480]])
 
     debut_age = {}
     debut_age['ages'] = sexual_debut[:, 0]
     debut_age['probs'] = sexual_debut[:, 1]
 
     return debut_age
 
@@ -599,46 +569,39 @@
         '<18': [0, 18],
         '18-20': [18, 20],
         '21-25': [20, 25],
         '26-35': [25, 35],
         '>35': [35, fpd.max_age + 1],  # +1 since we're using < rather than <=
     }
 
-    # Data on trend in CPR over time in from Kenya, in %.
-    # Taken from UN Population Division Data Portal, married women 1970-1986, all women 1990-2030
-    # https://population.un.org/dataportal/data/indicators/1/locations/404/start/1950/end/2040/table/pivotbylocation
-    # Projections go out until 2030, but the csv file can be manually adjusted to remove any projections and stop at your desired year
-    cpr_data = pd.read_csv(thisdir / 'kenya' / 'kenya_cpr.csv')
-    methods['mcpr_years'] = cpr_data['year'].to_numpy()
-    methods['mcpr_rates'] = cpr_data['cpr'].to_numpy() / 100  # convert from percent to rate
+    # Data on trend in MCPR in Senegal over time, in % # CK: TODO: find source
+    methods['mcpr_years'] = np.array(
+        [1950, 1980, 1986, 1992, 1997, 2005, 2010, 2012, 2014, 2015, 2016, 2017, 2018, 2019, 2020])
+    methods['mcpr_rates'] = np.array(
+        [0.50, 1.0, 2.65, 4.53, 7.01, 7.62, 8.85, 11.3, 14.7, 15.3, 16.5, 18.8, 19, 20, 20.4]) / 100
 
     return methods
 
 
-'''
-For reference
-def method_probs_senegal():
-    
-    It does leave Senegal matrices in place in the Kenya file for now. 
-    We may want to test with these as we work through scenarios and calibration. 
-    
+def method_probs():
+    '''
     Define "raw" (un-normalized, un-trended) matrices to give transitional probabilities
     from 2018 DHS Senegal contraceptive calendar data.
 
     Probabilities in this function are annual probabilities of initiating (top row), discontinuing (first column),
     continuing (diagonal), or switching methods (all other entries).
 
     Probabilities at postpartum month 1 are 1 month transitional probabilities
     for starting a method after delivery.
 
     Probabilities at postpartum month 6 are 5 month transitional probabilities
     for starting or changing methods over the first 6 months postpartum.
 
     Data from Senegal DHS contraceptive calendars, 2017 and 2018 combined
-    
+    '''
 
     raw = {
 
         # Main switching matrix: all non-postpartum women
         'annual': {
             '<18': np.array([
                 [0.9953, 0., 0.0002, 0.0012, 0.0002, 0.0017, 0.0014, 0.0001, 0., 0.],
@@ -762,196 +725,52 @@
             '18-20': np.array([0.9525, 0.0006, 0.0017, 0.0006, 0.0028, 0.0215, 0.0198, 0.0006, 0., 0.]),
             '21-25': np.array([0.9379, 0., 0.0053, 0.0009, 0.0083, 0.0285, 0.0177, 0.0013, 0., 0.]),
             '26-35': np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004, 0.0022, 0.0004]),
             '>35': np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004, 0.0022, 0.0004]),
         }
     }
     return raw
-    '''
-
-def method_probs():
-    '''
-    Define "raw" (un-normalized, un-trended) matrices to give transitional probabilities
-    from PMA Kenya contraceptive calendar data.
-
-    Probabilities in this function are annual probabilities of initiating (top row), discontinuing (first column),
-    continuing (diagonal), or switching methods (all other entries).
-
-    Probabilities at postpartum month 1 are 1 month transitional probabilities
-    for starting a method after delivery.
-
-    Probabilities at postpartum month 6 are 5 month transitional probabilities
-    for starting or changing methods over the first 6 months postpartum.
-
-    Data from Kenya PMA contraceptive calendars, 2019-2020
-    Processed from matrices_kenya_pma_2019_20.csv using process_matrices.py
-    '''
-
-    raw = {
-
-        # Main switching matrix: all non-postpartum women
-        'annual': {
-            '<18': np.array([
-                [0.9448, 0.0012, 0.0026, 0.0306, 0.002, 0.0063, 0.0079, 0.0003, 0., 0.0043],
-                [0.4165, 0.2322, 0.0475, 0.1045, 0.0899, 0.0561, 0.0066, 0.0001, 0., 0.0467],
-                [0.2284, 0.0002, 0.6816, 0.0674, 0.0008, 0.0022, 0.0016, 0., 0., 0.0178],
-                [0.6573, 0.0006, 0.0058, 0.2963, 0.0015, 0.0165, 0.0045, 0.0001, 0., 0.0174],
-                [0.2487, 0.0004, 0.0011, 0.0283, 0.6656, 0.0353, 0.0031, 0., 0., 0.0176],
-                [0.1099, 0.0072, 0.0009, 0.0029, 0.0009, 0.8035, 0.0738, 0., 0., 0.0008],
-                [0.1243, 0.0001, 0.009, 0.0027, 0.0001, 0.0099, 0.8534, 0., 0., 0.0004],
-                [0., 0., 0., 0., 0., 0., 0., 1., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 1., 0.],
-                [0.6634, 0.0008, 0.0247, 0.0866, 0.0235, 0.0301, 0.0309, 0.0001, 0., 0.1398]]),
-            '18-20': np.array([
-                [0.849, 0.0019, 0.0134, 0.0597, 0.0111, 0.0349, 0.0198, 0.0008, 0., 0.0094],
-                [0.4007, 0.213, 0.0091, 0.2626, 0.0592, 0.0162, 0.0071, 0.0002, 0., 0.032],
-                [0.1544, 0.0007, 0.7401, 0.0557, 0.0027, 0.022, 0.0032, 0.0001, 0., 0.0212],
-                [0.4223, 0.0115, 0.0167, 0.5017, 0.01, 0.0217, 0.0059, 0.0002, 0., 0.0101],
-                [0.2754, 0.0007, 0.0033, 0.0407, 0.5708, 0.0732, 0.0247, 0.0001, 0., 0.0111],
-                [0.2411, 0.0003, 0.0054, 0.0096, 0.0179, 0.6482, 0.0738, 0.0001, 0., 0.0037],
-                [0.1608, 0.0002, 0.0014, 0.0063, 0.0169, 0.0461, 0.7652, 0.0001, 0., 0.003],
-                [0., 0., 0., 0., 0., 0., 0., 1.,0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0.,1., 0.],
-                [0.5549, 0.0021, 0.0543, 0.121, 0.0467, 0.041, 0.034, 0.0003, 0., 0.1458]]),
-            '21-25': np.array([
-                [0.7836, 0.0049, 0.0129, 0.0429, 0.0166, 0.0745, 0.0433, 0.0018,0.0007, 0.0189],
-                [0.4657, 0.3192, 0.0619, 0.0179, 0.0072, 0.0569, 0.0488, 0.0006, 0.0002, 0.0216],
-                [0.1634, 0.0105, 0.6428, 0.0348, 0.0221, 0.0522, 0.051, 0.0003, 0.0001, 0.0228],
-                [0.3851, 0.0064, 0.0244, 0.4621, 0.0118, 0.0489, 0.0386, 0.0005, 0.0002, 0.0221],
-                [0.1876, 0.004, 0.0025, 0.0137, 0.6116, 0.1092, 0.0536, 0.01, 0.0001, 0.0076],
-                [0.2213, 0.0014, 0.008, 0.0108, 0.0245, 0.661, 0.0661, 0.0011, 0.0001, 0.0056],
-                [0.1324, 0.0005, 0.0027, 0.007, 0.0121, 0.0485, 0.7927, 0.001, 0.0001, 0.0029],
-                [0.1348, 0.0005, 0.0011, 0.0039, 0.0247, 0.0316, 0.0306, 0.7707, 0.0001, 0.0021],
-                [0.2241, 0.0014, 0.0042, 0.1457, 0.003, 0.0133, 0.0086, 0.0002, 0.5935, 0.0059],
-                [0.558, 0.0074, 0.0457, 0.0826, 0.0222, 0.1079, 0.0544, 0.0009, 0.0003, 0.1204]]),
-            '26-35': np.array([
-                [0.7774, 0.0037, 0.0111, 0.0264, 0.0184, 0.0883, 0.0562, 0.0048, 0.0018, 0.0118],
-                [0.185, 0.5721, 0.0121, 0.0207, 0.0239, 0.0941, 0.0885, 0.0009, 0.0002, 0.0025],
-                [0.122, 0.0006, 0.6796, 0.0266, 0.043, 0.0783, 0.0175, 0.005, 0.0001, 0.0272],
-                [0.373, 0.0104, 0.0105, 0.4666, 0.0256, 0.0501, 0.0354, 0.0015, 0.0004, 0.0263],
-                [0.1948, 0.002, 0.0049, 0.0103, 0.6316, 0.0795, 0.0594, 0.0104, 0.0002, 0.007],
-                [0.1884, 0.0026, 0.0083, 0.0088, 0.0259, 0.6902, 0.0677, 0.0032, 0.001, 0.0039],
-                [0.1081, 0.0017, 0.0046, 0.0028, 0.0089, 0.0351, 0.8335, 0.002, 0.0001, 0.0033],
-                [0.1132, 0.0038, 0.0046, 0.0053, 0.0163, 0.0146, 0.0087, 0.8322, 0.0001, 0.0011],
-                [0.0265, 0.0001, 0.0002, 0.0004, 0.0003, 0.0013, 0.0008, 0.0001, 0.9702, 0.0002],
-                [0.3909, 0.0019, 0.0293, 0.0805, 0.0272, 0.1168, 0.0628, 0.0087, 0.0005, 0.2814]]),
-            '>35': np.array([
-                [0.9092, 0.0013, 0.0043, 0.0204, 0.0102, 0.0281, 0.0175, 0.0012, 0.0022, 0.0057],
-                [0.1537, 0.7449, 0.0009, 0.002, 0.0019, 0.0686, 0.0269, 0.0003, 0.0003, 0.0007],
-                [0.0838, 0.0039, 0.8546, 0.0117, 0.0079, 0.0241, 0.0059, 0.0042, 0.0001, 0.0037],
-                [0.2731, 0.0042, 0.0052, 0.6592, 0.002, 0.013, 0.0246, 0.0002, 0.0003, 0.0181],
-                [0.1871, 0.0003, 0.0156, 0.0051, 0.6603, 0.0739, 0.0471, 0.0092, 0.0003, 0.001],
-                [0.1632, 0.0023, 0.0111, 0.0079, 0.0239, 0.7272, 0.0537, 0.0041, 0.0018, 0.0049],
-                [0.0947, 0.0017, 0.008, 0.005, 0.0077, 0.0373, 0.8349, 0.0036, 0.0019, 0.0052],
-                [0.0841, 0.0001, 0.0057, 0.0011, 0.0008, 0.0162, 0.0067, 0.8806, 0.0001, 0.0047],
-                [0.014, 0., 0., 0.0001, 0.0001, 0.0002, 0.0001, 0., 0.9854, 0.],
-                [0.2432, 0.0004, 0.0246, 0.0339, 0.0227, 0.039, 0.0845, 0.0006, 0.0004, 0.5508]])
-        },
-
-        # Postpartum switching matrix, 1 to 6 months
-        'pp1to6': {
-            '<18': np.array([
-                [0.7143, 0., 0., 0.0143, 0.0214, 0.1286, 0.1214, 0., 0., 0.],
-                [0., 1., 0., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 1., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0., 1., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0., 0., 0.6667, 0.3333, 0., 0.,0., 0.],
-                [0.0833, 0., 0., 0., 0.0833, 0.75, 0.0833, 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 1., 0.,0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 1.,0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0.,1., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0.,0., 1.]]),
-            '18-20': np.array([
-                [0.5586, 0., 0.0045, 0.0045, 0.0225, 0.2117, 0.1982, 0., 0., 0.],
-                [0., 1., 0., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0.6667, 0., 0., 0.3333, 0., 0., 0., 0.],
-                [0., 0., 0., 0.3333, 0., 0.3333, 0.3333, 0., 0., 0.],
-                [0., 0., 0., 0., 0.5, 0.1667, 0.3333, 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0.8966, 0.1034, 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 1., 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 1., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 1., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0.,0., 1.]]),
-            '21-25': np.array([
-                [0.4827, 0.0016, 0.0063, 0.0189, 0.0409, 0.2579, 0.1777, 0.011, 0., 0.0031],
-                [0., 1., 0., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0.75, 0., 0., 0.125, 0., 0., 0.125, 0.],
-                [0., 0., 0., 0.2857, 0., 0.5714, 0.1429, 0., 0., 0.],
-                [0., 0., 0., 0., 0.6, 0.25, 0.15, 0., 0., 0.],
-                [0.0588, 0., 0., 0., 0., 0.8333, 0.098, 0.0098, 0., 0.],
-                [0., 0., 0., 0., 0., 0., 1., 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 1., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 1., 0.],
-                [0., 0., 0., 0., 0.1111, 0.1111, 0.1111, 0., 0., 0.6667]]),
-            '26-35': np.array([
-                [0.5489, 0.0034, 0.009, 0.0157, 0.0382, 0.1845, 0.1755, 0.0214, 0.0011, 0.0022],
-                [0., 0.75, 0., 0., 0., 0.25, 0., 0., 0., 0.],
-                [0., 0., 0.9444, 0., 0., 0.0556, 0., 0., 0., 0.],
-                [0.1111, 0., 0., 0.6667, 0., 0.0556, 0.1111, 0., 0., 0.0556],
-                [0., 0., 0., 0., 0.7241, 0.1379, 0.1034, 0.034, 0., 0.],
-                [0.0291, 0., 0., 0., 0., 0.932, 0.0291, 0.0097, 0., 0.],
-                [0., 0., 0., 0.0095, 0.0095, 0.0095, 0.9714, 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 1., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 1., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.]]),
-            '>35': np.array([
-                [0.5952, 0.004, 0.0317, 0.0119, 0.0437, 0.1667, 0.1151, 0.0079, 0.0119, 0.0119],
-                [0., 1., 0., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 1., 0., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0., 1., 0., 0., 0., 0., 0., 0.],
-                [0., 0., 0., 0., 1., 0., 0., 0., 0., 0.],
-                [0., 0., 0., 0., 0., 1., 0., 0., 0., 0.],
-                [0.0357, 0., 0., 0., 0., 0., 0.9643, 0., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 1., 0., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0., 1., 0.],
-                [0., 0., 0., 0., 0., 0., 0., 0.,0., 1.]])
-        },
-
-        # Postpartum initiation vectors, 0 to 1 month
-        'pp0to1': {
-            '<18': np.array([0.7553, 0., 0.0035, 0.0177, 0.0106, 0.0638, 0.1489, 0., 0., 0.]),
-            '18-20': np.array([0.7643, 0., 0.0071, 0.0071, 0.0167, 0.0905, 0.1048, 0.0071, 0., 0.0024]),
-            '21-25': np.array([0.735, 0.0037, 0.0111, 0.0092, 0.0194, 0.1127, 0.0988, 0.0018, 0., 0.0083]),
-            '26-35': np.array([0.7527, 0.0034, 0.0144, 0.0144, 0.0213, 0.09, 0.0783, 0.0082, 0.0082, 0.0089]),
-            '>35': np.array([0.793, 0., 0.0081, 0.0054, 0.0081, 0.0403, 0.0806, 0.0054, 0.0484, 0.0108]),
-        }
-    }
-
-    return raw
 
 
 def barriers():
-    ''' Reasons for nonuse -- taken from Kenya DHS 2014. '''
+    ''' Reasons for nonuse -- taken from DHS '''
 
     barriers = sc.odict({
-        'No need': 40.3,
-        'Opposition': 22.7,
-        'Knowledge': 3.5,
-        'Access': 13.4,
-        'Health': 32.5,
+        'No need': 54.2,
+        'Opposition': 30.5,
+        'Knowledge': 1.7,
+        'Access': 4.5,
+        'Health': 12.9,
     })
 
     barriers[:] /= barriers[:].sum()  # Ensure it adds to 1
     return barriers
 
 
+def urban_proportion():
+    """Load information about the proportion of people who live in an urban setting"""
+    urban_data = pd.read_csv(thisdir / 'senegal' / 'urban.csv')
+    return urban_data["mean"][0]  # Return this value as a float
+
+
 # %% Make and validate parameters
 
-def make_pars():
-    '''
+def make_pars(use_empowerment=None, use_education=None, use_partnership=None, use_subnational=None, seed=None):
+    """
     Take all parameters and construct into a dictionary
-    '''
+    """
 
     # Scalar parameters and filenames
     pars = scalar_pars()
     pars['filenames'] = filenames()
 
     # Demographics and pregnancy outcome
     pars['age_pyramid'] = age_pyramid()
     pars['age_mortality'] = age_mortality()
+    pars['urban_prop'] = urban_proportion()
     pars['maternal_mortality'] = maternal_mortality()
     pars['infant_mortality'] = infant_mortality()
     pars['miscarriage_rates'] = miscarriage()
     pars['stillbirth_rate'] = stillbirth()
 
     # Fecundity
     pars['age_fecundity'] = female_age_fecundity()
@@ -967,8 +786,16 @@
     pars['spacing_pref'] = birth_spacing_pref()
 
     # Contraceptive methods
     pars['methods'] = methods()
     pars['methods']['raw'] = method_probs()
     pars['barriers'] = barriers()
 
+    # Handle modules that have not been implemented yet
+    kwargs = locals()
+    not_implemented_args = ['use_empowerment', 'use_education', 'use_partnership', 'use_subnational']
+    true_args = [key for key in not_implemented_args if kwargs[key] is True]
+    if true_args:
+        errmsg = f"{true_args} not implemented yet for {pars['location']}"
+        raise NotImplementedError(errmsg)
+
     return pars
```

### Comparing `fpsim-0.22.0/fpsim/locations/senegal/BirthSpacing.obj` & `fpsim-0.28.1/fpsim/locations/senegal/BirthSpacing.obj`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/senegal/Method_v312.csv` & `fpsim-0.28.1/fpsim/locations/senegal/Method_v312.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/senegal/SNIR80FL.obj` & `fpsim-0.28.1/fpsim/locations/senegal/SNIR80FL.obj`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/senegal/Skyscrapers-All-DHS.csv` & `fpsim-0.28.1/fpsim/locations/senegal/Age-parity-All-DHS.csv`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/senegal/plot_birth_spacing.py` & `fpsim-0.28.1/fpsim/locations/senegal/plot_birth_spacing.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/locations/senegal.py` & `fpsim-0.28.1/fpsim/locations/ethiopia.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,31 @@
 '''
-Set the parameters for FPsim, specifically for Senegal.
+Set the parameters for FPsim, specifically for Ethiopia.
 '''
 
 import numpy as np
+import pandas as pd
 import sciris as sc
 from scipy import interpolate as si
 from .. import defaults as fpd
 
-#%% Housekeeping
+# %% Housekeeping
+
+thisdir = sc.thispath(__file__)  # For loading CSV files
+
 
 def scalar_pars():
     scalar_pars = {
-        # Basic parameters
-        'location'               : 'senegal',
-        'n_agents'               : 1_000, # Number of agents
-        'scaled_pop'             : None, # Scaled population / total population size
-        'start_year'             : 1960, # Start year of simulation
-        'end_year'               : 2020, # End year of simulation
-        'timestep'               : 1, # The simulation timestep in months
-        'method_timestep'        : 1, # How many simulation timesteps to go for every method update step
-        'seed'                   : 1, # Random seed
-        'verbose'                : 1, # How much detail to print during the simulation
-        'track_switching'        : 0, # Whether to track method switching
-        'track_as'               : 0, # Whether to track age-specific channels
-
-        # Age limits (in years)
-        'method_age'             : 15,
-        'age_limit_fecundity'    : 50,
-        'max_age'                : 99,
-
-        # Durations (in months)
-        'switch_frequency'       : 12, # How frequently to check for changes to contraception
-        'end_first_tri'          : 3,
-        'preg_dur_low'           : 9,
-        'preg_dur_high'          : 9,
-        'postpartum_dur'         : 35,
-        'breastfeeding_dur_mu'   : 19.66828, # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R 
-        'breastfeeding_dur_beta' : 7.2585, # Scale parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R 
-        'max_lam_dur'            : 5, # Duration of lactational amenorrhea
-
-        # Pregnancy outcomes
-        'abortion_prob'             : 0.08, # From https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4712915/
-        'twins_prob'                : 0.015, # From https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0025239
-        'LAM_efficacy'              : 0.98, # From Cochrane review: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6823189/
-        'maternal_mortality_factor' : 1,
-
-         # Fecundity and exposure
-        'fecundity_var_low'      : 0.7,
-        'fecundity_var_high'     : 1.1,
-        'high_parity'            : 4,
-        'high_parity_nonuse'     : 0.6,
-        'primary_infertility'    : 0.05,
-        'exposure_factor'        : 1.0, # Overall exposure correction factor
-
-        # MCPR
-        'mcpr_growth_rate'       : 0.02, # The year-on-year change in MCPR after the end of the data
-        'mcpr_max'               : 0.90, # Do not allow MCPR to increase beyond this
-        'mcpr_norm_year'         : 2018, # Year to normalize MCPR trend to 1
+        'location':             'ethiopia',
+        'postpartum_dur':       23,
+        'breastfeeding_dur_mu': 9.30485863,     # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R
+        'breastfeeding_dur_beta': 8.20149079,   # Location parameter of gumbel distribution. Requires children's recode DHS file, see data_processing/breastfeedin_stats.R
+        'abortion_prob':        0.176,          # From https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5568682/, % of all pregnancies calculated
+        'twins_prob':           0.011,          # From https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0025239
+        'mcpr_norm_year':       2020,           # Year to normalize MCPR trend to 1
     }
     return scalar_pars
 
 
 def data2interp(data, ages, normalize=False):
     ''' Convert unevenly spaced data into an even spline interpolation '''
     model = si.interp1d(data[0], data[1])
@@ -69,737 +34,1010 @@
         interp = np.minimum(1, np.maximum(0, interp))
     return interp
 
 
 def filenames():
     ''' Data files for use with calibration, etc -- not needed for running a sim '''
     files = {}
-    files['base'] = sc.thisdir(aspath=True) / 'senegal'
-    files['basic_dhs']        = 'senegal-basic-dhs.yaml'
-    files['popsize']          = 'senegal-popsize.csv'
-    files['mcpr']             = 'senegal-mcpr.csv'
-    files['tfr']              = 'senegal-tfr.csv'
-    files['asfr']             = 'senegal-asfr.csv'
-    files['skyscrapers']      = 'Skyscrapers-All-DHS.csv'
-    files['pregnancy_parity'] = 'SNIR80FL.obj'
-    files['spacing']          = 'BirthSpacing.obj'
-    files['methods']          = 'Method_v312.csv'
+    files['base'] = sc.thisdir(aspath=True) / 'ethiopia'
+    files['basic_dhs'] = 'basic_dhs.yaml' # From World Bank https://data.worldbank.org/indicator/SH.STA.MMRT?locations=ET
+    files['popsize'] = 'popsize.csv' # From UN World Population Prospects 2022: https://population.un.org/wpp/Download/Standard/Population/
+    files['mcpr'] = 'cpr.csv'  # From UN Population Division Data Portal, married women 1970-1986, all women 1990-2030
+    files['tfr'] = 'tfr.csv'   # From World Bank https://data.worldbank.org/indicator/SP.DYN.TFRT.IN?locations=ET
+    files['asfr'] = 'asfr.csv' # From UN World Population Prospects 2022: https://population.un.org/wpp/Download/Standard/Fertility/
+    files['ageparity'] = 'ageparity.csv' # Choose from either DHS 2016 or PMA 2022
+    files['spacing'] = 'birth_spacing_dhs.csv'
+    files['methods'] = 'mix.csv'
+    files['afb'] = 'afb.table.csv'
+    files['use'] = 'use.csv'
+    files['urban'] = 'urban.csv'
+    #subnational_data files
+    files['region'] = '/subnational_data/region.csv' ## From DHS 2016
+    files['asfr_region'] = '/subnational_data/asfr_region.csv' ## From DHS 2016
+    files['tfr_region'] = '/subnational_data/tfr_region.csv' ## From DHS 2016
+    files['methods_region'] = '/subnational_data/mix_region.csv' ## From DHS 2016
+    files['use_region'] = '/subnational_data/use_region.csv'  ## From PMA 2019
+    files['barriers_region'] = '/subnational_data/barriers_region.csv' ## From PMA 2019
+    files['lactational_amenorrhea_region'] = '/subnational_data/lam_region.csv' ## From DHS 2016
+    files['sexual_activity_region'] = '/subnational_data/sexual_activity_region.csv' ## From DHS 2016
+    files['sexual_activity_pp_region'] = '/subnational_data/sexual_activity_pp_region.csv' ## From DHS 2016
+    files['debut_age_region'] = '/subnational_data/sexual_debut_region.csv' ## From DHS 2016
     return files
 
 
-#%% Demographics and pregnancy outcome
+# %% Demographics and pregnancy outcome
 
 def age_pyramid():
-    ''' Starting age bin, male population, female population '''
-    pyramid = np.array([
-         [0,  318225,  314011], # Senegal 1962
-         [5,  249054,  244271],
-        [10,  191209,  190998],
-        [15,  157800,  159536],
-        [20,  141480,  141717],
-        [25,  125002,  124293],
-        [30,  109339,  107802],
-        [35,  93359,   92119],
-        [40,  77605,   78231],
-        [45,  63650,   66117],
-        [50,  51038,   54934],
-        [55,  39715,   44202],
-        [60,  29401,   33497],
-        [65,  19522,   23019],
-        [70,  11686,   14167],
-        [75,  5985,    7390],
-        [80,  2875,    3554],
-    ], dtype=float)
+    '''
+    Starting age bin, male population, female population
+    Data are from World Population Prospects
+    https://population.un.org/wpp/Download/Standard/Population/
+     '''
+    pyramid = np.array([[0, 2018504, 1986199],  # Ethiopia 1962
+                        [5, 1508878, 1515088],
+                        [10, 1349237, 1359040],
+                        [15, 1227673, 1215562],
+                        [20, 1021618, 1018324],
+                        [25, 862087, 864220],
+                        [30, 727361, 732051],
+                        [35, 612416, 620469],
+                        [40, 510553, 521148],
+                        [45, 423644, 434699],
+                        [50, 345374, 360522],
+                        [55, 276116, 297462],
+                        [60, 182129, 224203],
+                        [65, 117217, 162750],
+                        [70, 77018, 111877],
+                        [75, 40877,	66069],
+                        [80, 21275,	40506],
+                        ], dtype=float)
 
     return pyramid
 
 
-def age_mortality():
+def region_proportions():
+    '''
+    Defines the proportion of the population in each region to establish the probability of living in a given region.
+    Uses 2016 Ethiopia DHS individual recode (v025) for region and V024 for urban to produce subnational estimates
     '''
-    Age-dependent mortality rates, Senegal specific from 1990-1995 -- see age_dependent_mortality.py in the fp_analyses repository
-    Mortality rate trend from crude mortality rate per 1000 people: https://data.worldbank.org/indicator/SP.DYN.CDRT.IN?locations=SN
+    region_data = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'region.csv')
+
+    region_dict = {}
+    region_dict['region'] = region_data['region'] # Return region names
+    region_dict['mean'] = region_data['mean'] # Return proportion living in each region
+    region_dict['urban'] = region_data['urban'] # Return proportion living in an urban area by region
+
+    return region_dict
+
+
+def age_mortality():
     '''
+    Age-dependent mortality rates taken from UN World Population Prospects 2022.  From probability of dying each year.
+    https://population.un.org/wpp/
+    Used CSV WPP2022_Life_Table_Complete_Medium_Female_1950-2021, Ethiopia, 2020 
+    Used CSV WPP2022_Life_Table_Complete_Medium_Male_1950-2021, Ethiopia, 2020
+    Mortality rate trend from crude death rate per 1000 people, also from UN Data Portal, 1950-2030:
+    https://population.un.org/dataportal/data/indicators/59/locations/231/start/1950/end/2030/table/pivotbylocation
+    Projections go out until 2030, but the csv file can be manually adjusted to remove any projections and stop at your desired year
+    '''
+    data_year = 2020 # NORMED TO 2020 BASED ON ETHIOPIA PROBABILITY DATA
+    mortality_data = pd.read_csv(thisdir / 'ethiopia' / 'mortality_prob.csv')
+    mortality_trend = pd.read_csv(thisdir / 'ethiopia' / 'mortality_trend.csv')
+
     mortality = {
-        'bins': np.array([ 0.,  5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95]),
-        'm': np.array([0.03075891, 0.00266326, 0.00164035, 0.00247776, 0.00376541,0.00377009, 0.00433534, 0.00501743, 0.00656144, 0.00862479, 0.01224844, 0.01757291, 0.02655129, 0.0403916 , 0.06604032,0.10924413, 0.17495116, 0.26531436, 0.36505174, 0.43979833]),
-        'f': np.array([0.02768283, 0.00262118, 0.00161414, 0.0023998 , 0.00311697, 0.00354105, 0.00376715, 0.00429043, 0.00503436, 0.00602394, 0.00840777, 0.01193858, 0.01954465, 0.03220238, 0.05614077, 0.0957751 , 0.15973906, 0.24231313, 0.33755308, 0.41632442])
+        'ages': mortality_data['age'].to_numpy(),
+        'm': mortality_data['male'].to_numpy(),
+        'f': mortality_data['female'].to_numpy()
     }
 
-    mortality['year']  = np.array([1950., 1955, 1960, 1965, 1970, 1975, 1980, 1985, 1990, 1995, 2000, 2005, 2010, 2015, 2020, 2025, 2030]) # Starting year bin
-    mortality['probs'] = np.array([28,    27,    26.023, 25.605, 24.687, 20.995, 16.9, 13.531, 11.335, 11.11, 10.752, 9.137, 7.305, 6.141, 5.7, 5.7, 5.7]) # First 2 estimated, last 3 are projected
-    mortality['probs'] /= mortality['probs'][8]  # Normalize around 2000 for trending # CK: TODO: shouldn't be hardcoded
-
-    m_mortality_spline_model = si.splrep(x=mortality['bins'], y=mortality['m'])  # Create a spline of mortality along known age bins
-    f_mortality_spline_model = si.splrep(x=mortality['bins'], y=mortality['f'])
-    m_mortality_spline = si.splev(fpd.spline_ages, m_mortality_spline_model)  # Evaluate the spline along the range of ages in the model with resolution
+    mortality['year'] = mortality_trend['year'].to_numpy()
+    mortality['probs'] = mortality_trend['crude_death_rate'].to_numpy()
+    trend_ind = np.where(mortality['year'] == data_year)
+    trend_val = mortality['probs'][trend_ind]
+
+    mortality['probs'] /= trend_val  # Normalize around data year for trending
+    m_mortality_spline_model = si.splrep(x=mortality['ages'],
+                                         y=mortality['m'])  # Create a spline of mortality along known age bins
+    f_mortality_spline_model = si.splrep(x=mortality['ages'], y=mortality['f'])
+    m_mortality_spline = si.splev(fpd.spline_ages,
+                                  m_mortality_spline_model)  # Evaluate the spline along the range of ages in the model with resolution
     f_mortality_spline = si.splev(fpd.spline_ages, f_mortality_spline_model)
-    m_mortality_spline = np.minimum(1, np.maximum(0, m_mortality_spline)) # Normalize
+    m_mortality_spline = np.minimum(1, np.maximum(0, m_mortality_spline))  # Normalize
     f_mortality_spline = np.minimum(1, np.maximum(0, f_mortality_spline))
 
     mortality['m_spline'] = m_mortality_spline
     mortality['f_spline'] = f_mortality_spline
 
     return mortality
 
 
 def maternal_mortality():
     '''
-    Risk of maternal death assessed at each pregnancy. Data from Huchon et al. (2013) prospective study on risk of maternal death in Senegal and Mali.
-    Maternal deaths: The annual number of female deaths from any cause related to or aggravated by pregnancy
-    or its management (excluding accidental or incidental causes) during pregnancy and childbirth or within
-    42 days of termination of pregnancy, irrespective of the duration and site of the pregnancy,
-    expressed per 100,000 live births, for a specified time period.
+    From World Bank indicators for maternal mortality ratio (modeled estimate) per 100,000 live births:
+    https://data.worldbank.org/indicator/SH.STA.MMRT?locations=ET
     '''
 
     data = np.array([
-        [1990, 0.00278, 0.00319, 0.00364],
-        [2000, 0.00268, 0.00309, 0.00354],
-        [2001, 0.00263, 0.00304, 0.00350],
-        [2002, 0.00259, 0.00300, 0.00346],
-        [2003, 0.00255, 0.00296, 0.00341],
-        [2004, 0.00252, 0.00293, 0.00338],
-        [2005, 0.00249, 0.00290, 0.00335],
-        [2006, 0.00245, 0.00286, 0.00331],
-        [2007, 0.00242, 0.00283, 0.00329],
-        [2008, 0.00237, 0.00278, 0.00323],
-        [2009, 0.00230, 0.00271, 0.00317],
-        [2010, 0.00220, 0.00261, 0.00306],
-        [2011, 0.00207, 0.00248, 0.00293],
-        [2012, 0.00194, 0.00235, 0.00280],
-        [2013, 0.00182, 0.002228327, 0.00268338],
-        [2014, 0.00172, 0.00213, 0.00258],
-        [2015, 0.00161, 0.00202, 0.00248],
-        [2016, 0.00152, 0.00193, 0.00239],
-        [2017, 0.00143, 0.00184, 0.00230],
-        [2018, 0.00135, 0.00176, 0.00222],
-        [2019, 0.00128, 0.00169, 0.00214]
+        [2000, 953],
+        [2001, 955],
+        [2002, 960],
+        [2003, 906],
+        [2004, 900],
+        [2005, 880],
+        [2006, 814],
+        [2007, 780],
+        [2008, 725],
+        [2009, 684],
+        [2010, 635],
+        [2011, 603],
+        [2012, 543],
+        [2013, 498],
+        [2014, 447],
+        [2015, 399],
+        [2016, 365],
+        [2017, 348],
+        [2018, 312],
+        [2019, 294],
+        [2020, 267],
+
     ])
 
     maternal_mortality = {}
-    maternal_mortality['year'] = data[:,0]
-    maternal_mortality['probs'] = data[:,3]
+    maternal_mortality['year'] = data[:, 0]
+    maternal_mortality['probs'] = data[:, 1] / 100000  # ratio per 100,000 live births
+    # maternal_mortality['ages'] = np.array([16, 17,   19, 22,   25, 50])
+    # maternal_mortality['age_probs'] = np.array([2.28, 1.63, 1.3, 1.12, 1.0, 1.0]) #need to be added
 
     return maternal_mortality
 
 
 def infant_mortality():
     '''
-    From World Bank indicators for infant morality (< 1 year) for Senegal, per 1000 live births
-    From API_SP.DYN.IMRT.IN_DS2_en_excel_v2_1495452.numbers
+    From World Bank indicators for infant mortality (< 1 year) for Ethiopia, per 1000 live births
+    From API_SP.DYN.IMRT.IN_DS2_en_csv_v2_5358355
     Adolescent increased risk of infant mortality gradient taken
     from Noori et al for Sub-Saharan African from 2014-2018.  Odds ratios with age 23-25 as reference group:
     https://www.medrxiv.org/content/10.1101/2021.06.10.21258227v1
     '''
 
     data = np.array([
-        [1960, 128.3],
-        [1961, 128.2],
-        [1962, 128.3],
-        [1963, 128.6],
-        [1964, 128.8],
-        [1965, 128.9],
-        [1966, 128.6],
-        [1967, 128.2],
-        [1968, 127.7],
-        [1969, 126.7],
-        [1970, 125.4],
-        [1971, 123.6],
-        [1972, 121.4],
-        [1973, 118.7],
-        [1974, 115.6],
-        [1975, 112.2],
-        [1976, 108.4],
-        [1977, 104.6],
-        [1978, 101],
-        [1979, 97.7],
-        [1980, 94.9],
-        [1981, 92.5],
-        [1982, 90.4],
-        [1983, 88.2],
-        [1984, 85.7],
-        [1985, 82.9],
-        [1986, 79.9],
-        [1987, 77],
-        [1988, 74.4],
-        [1989, 72.4],
-        [1990, 71],
-        [1991, 70.3],
-        [1992, 70.1],
-        [1993, 70.3],
-        [1994, 70.6],
-        [1995, 71],
-        [1996, 71.2],
-        [1997, 71.1],
-        [1998, 70.6],
-        [1999, 69.4],
-        [2000, 67.5],
-        [2001, 65.1],
-        [2002, 62.2],
-        [2003, 59.2],
-        [2004, 56.1],
-        [2005, 53.2],
-        [2006, 50.6],
-        [2007, 48.2],
-        [2008, 46.2],
-        [2009, 44.3],
-        [2010, 42.6],
-        [2011, 41.1],
-        [2012, 39.8],
-        [2013, 38.6],
-        [2014, 37.5],
-        [2015, 36.4],
-        [2016, 35.4],
-        [2017, 34.4],
-        [2018, 33.6],
-        [2019, 32.7],
+        [1966, 146.6],        
+        [1967, 146.1],
+        [1968, 145.9],
+        [1969, 145.8],
+        [1970, 145.6],
+        [1971, 145.4],
+        [1972, 145.1],
+        [1973, 145],
+        [1974, 144.7],
+        [1975, 144.4],
+        [1976, 144.1],
+        [1977, 143.8],
+        [1978, 143.4],
+        [1979, 142.6],
+        [1980, 141.5],
+        [1981, 139.9],
+        [1982, 138],
+        [1983, 135.8],
+        [1984, 133.4],
+        [1985, 131],
+        [1986, 128.7],
+        [1987, 126.4],
+        [1988, 124.2],
+        [1989, 121.9],
+        [1990, 119.5],
+        [1991, 116.9],
+        [1992, 114],
+        [1993, 110.7],
+        [1994, 107.2],
+        [1995, 103.7],
+        [1996, 100.3],
+        [1997, 96.8],
+        [1998, 93.5],
+        [1999, 90.3],
+        [2000, 87],
+        [2001, 83.7],
+        [2002, 80.2],
+        [2003, 76.7],
+        [2004, 73.1],
+        [2005, 69.5],
+        [2006, 66.1],
+        [2007, 62.8],
+        [2008, 59.8],
+        [2009, 57],
+        [2010, 54.4],
+        [2011, 51.9],
+        [2012, 49.5],
+        [2013, 47.3],
+        [2014, 45.2],
+        [2015, 43.2],
+        [2016, 41.3],
+        [2017, 39.6],
+        [2018, 38],
+        [2019, 36.6],
+        [2020, 35.4],
+        [2021, 34.3]
     ])
 
     infant_mortality = {}
-    infant_mortality['year'] = data[:,0]
-    infant_mortality['probs'] = data[:,1]/1000   # Rate per 1000 live births, used after stillbirth is filtered out
-    infant_mortality['ages'] = np.array([16, 17,   19, 22,   25, 50])
+    infant_mortality['year'] = data[:, 0]
+    infant_mortality['probs'] = data[:, 1] / 1000  # Rate per 1000 live births, used after stillbirth is filtered out
+    infant_mortality['ages'] = np.array([16, 17, 19, 22, 25, 50])
     infant_mortality['age_probs'] = np.array([2.28, 1.63, 1.3, 1.12, 1.0, 1.0])
 
     return infant_mortality
 
 
 def miscarriage():
     '''
     Returns a linear interpolation of the likelihood of a miscarriage
     by age, taken from data from Magnus et al BMJ 2019: https://pubmed.ncbi.nlm.nih.gov/30894356/
     Data to be fed into likelihood of continuing a pregnancy once initialized in model
     Age 0 and 5 set at 100% likelihood.  Age 10 imputed to be symmetrical with probability at age 45 for a parabolic curve
     '''
-    miscarriage_rates = np.array([[0, 5,    10,     15,     20,    25,    30,    35,    40,    45,    50],
-                                  [1, 1, 0.569,  0.167,  0.112, 0.097, 0.108, 0.167, 0.332, 0.569, 0.569]])
+    miscarriage_rates = np.array([[0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50],
+                                  [1, 1, 0.569, 0.167, 0.112, 0.097, 0.108, 0.167, 0.332, 0.569, 0.569]])
     miscarriage_interp = data2interp(miscarriage_rates, fpd.spline_preg_ages)
     return miscarriage_interp
 
 
 def stillbirth():
     '''
     From Report of the UN Inter-agency Group for Child Mortality Estimation, 2020
     https://childmortality.org/wp-content/uploads/2020/10/UN-IGME-2020-Stillbirth-Report.pdf
-    
-    Age adjustments come from an extension of Noori et al., which were conducted June 2022.
+
+    Age adjustments come from an extension of Noori et al., which were conducted June 2022. 
     '''
 
-    data = np.array([
-        [2000, 25.3],
-        [2010, 22.6],
-        [2019, 19.7],
-        ])
+    data = np.array([ 
+        [2000, 35.8],
+        [2010, 31.1],
+        [2019, 24.6],
+    ])
 
     stillbirth_rate = {}
-    stillbirth_rate['year'] = data[:,0]
-    stillbirth_rate['probs'] = data[:,1]/1000    # Rate per 1000 total births
-    stillbirth_rate['ages']      = np.array([15,   16,   17,   19,   20,   28,  31,  36,   50])
-    stillbirth_rate['age_probs'] = np.array([3.27, 1.64, 1.85, 1.39, 0.89, 1.0, 1.5, 1.55, 1.78]) #odds ratios 
+    stillbirth_rate['year'] = data[:, 0]
+    stillbirth_rate['probs'] = data[:, 1] / 1000  # Rate per 1000 total births
+    stillbirth_rate['ages'] = np.array([15, 16, 17, 19, 20, 28, 31, 36, 50])
+    stillbirth_rate['age_probs'] = np.array([3.27, 1.64, 1.85, 1.39, 0.89, 1.0, 1.5, 1.55, 1.78])  # odds ratios
 
     return stillbirth_rate
 
 
-
-#%% Fecundity
+# %% Fecundity
 
 def female_age_fecundity():
     '''
     Use fecundity rates from PRESTO study: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5712257/
     Fecundity rate assumed to be approximately linear from onset of fecundity around age 10 (average age of menses 12.5) to first data point at age 20
-    45-50 age bin estimated at 0.10 of fecundity of 25-27 yr olds, based on fertility rates from Senegal
+    45-50 age bin estimated at 0.10 of fecundity of 25-27 yr olds
     '''
     fecundity = {
-        'bins': np.array([0., 5, 10, 15, 20,     25,   28,  31,   34,   37,  40,   45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95, 99]),
-        'f': np.array([0.,    0,  0, 65, 70.8, 79.3,  77.9, 76.6, 74.8, 67.4, 55.5, 7.9, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])}
-    fecundity['f'] /= 100  # Conceptions per hundred to conceptions per woman over 12 menstrual cycles of trying to conceive
+        'bins': np.array([0., 5, 10, 15, 20, 25, 28, 31, 34, 37, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95, 99]),
+        'f': np.array([0., 0, 0, 65, 70.8, 79.3, 77.9, 76.6, 74.8, 67.4, 55.5, 7.9, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])}
+    fecundity[
+        'f'] /= 100  # Conceptions per hundred to conceptions per woman over 12 menstrual cycles of trying to conceive
 
     fecundity_interp_model = si.interp1d(x=fecundity['bins'], y=fecundity['f'])
     fecundity_interp = fecundity_interp_model(fpd.spline_preg_ages)
-    fecundity_interp = np.minimum(1, np.maximum(0, fecundity_interp)) # Normalize to avoid negative or >1 values
+    fecundity_interp = np.minimum(1, np.maximum(0, fecundity_interp))  # Normalize to avoid negative or >1 values
 
     return fecundity_interp
 
 
-def fecundity_ratio_nullip():
+def fecundity_ratio_nullip(): 
     '''
     Returns an array of fecundity ratios for a nulliparous woman vs a gravid woman
     from PRESTO study: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5712257/
     Approximates primary infertility and its increasing likelihood if a woman has never conceived by age
     '''
-    fecundity_ratio_nullip = np.array([[ 0,  5, 10, 12.5,  15,  18,  20,   25,   30,   34,   37,   40,   45,   50],
-                                        [1,  1,  1,    1,   1,   1,   1, 0.96, 0.95, 0.71, 0.73, 0.42, 0.42, 0.42]])
+    fecundity_ratio_nullip = np.array([[0, 5, 10, 12.5, 15, 18, 20, 25, 30, 34, 37, 40, 45, 50],
+                                       [1, 1, 1, 1, 1, 1, 1, 0.96, 0.95, 0.71, 0.73, 0.42, 0.42, 0.42]])
     fecundity_nullip_interp = data2interp(fecundity_ratio_nullip, fpd.spline_preg_ages)
 
     return fecundity_nullip_interp
 
 
 def lactational_amenorrhea():
     '''
     Returns an array of the percent of breastfeeding women by month postpartum 0-11 months who meet criteria for LAM:
     Exclusively breastfeeding (bf + water alone), menses have not returned.  Extended out 5-11 months to better match data
     as those women continue to be postpartum insusceptible.
-    From DHS Senegal calendar data
+    From DHS Ethiopia 2016 calendar data
     '''
     data = np.array([
-        [0, 0.903125],
-        [1, 0.868794326],
-        [2, 0.746478873],
-        [3, 0.648854962],
-        [4, 0.563573883],
-        [5, 0.457564576],
-        [6, 0.254966887],
-        [7, 0.2],
-        [8, 0.146341463],
-        [9, 0.10982659],
-        [10, 0.10982659],
-        [11, 0.101796407],
+        [0, 0.9892715],
+        [1, 0.8494371],
+        [2, 0.8265375],
+        [3, 0.730395],
+        [4, 0.666934],
+        [5, 0.4947101],
+        [6, 0.3667066],
+        [7, 0.2191162],
+        [8, 0.3135374],
+        [9, 0.1113177],
+        [10, 0.0981782],
+        [11, 0.0847675],
     ])
 
     lactational_amenorrhea = {}
     lactational_amenorrhea['month'] = data[:, 0]
     lactational_amenorrhea['rate'] = data[:, 1]
 
     return lactational_amenorrhea
 
 
+def lactational_amenorrhea_region():
+    '''
+    Returns an array of the percent of breastfeeding women by month postpartum 0-11 months who meet criteria for LAM, stratified by region
+    '''
+    lam_region = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'lam_region.csv')
+    lam_dict = {}
+    lam_dict['region'] = lam_region['region']  # Return region names
+    lam_dict['month'] = lam_region['month']  # Return month postpartum
+    lam_dict['rate'] = lam_region['rate']  # Return percent of breastfeeding women
 
-#%% Pregnancy exposure
+    return lam_dict
+
+
+# %% Pregnancy exposure
 
 def sexual_activity():
     '''
     Returns a linear interpolation of rates of female sexual activity, defined as
     percentage women who have had sex within the last four weeks.
     From STAT Compiler DHS https://www.statcompiler.com/en/
     Using indicator "Timing of sexual intercourse"
     Includes women who have had sex "within the last four weeks"
     Excludes women who answer "never had sex", probabilities are only applied to agents who have sexually debuted
     Data taken from 2018 DHS, no trend over years for now
     Onset of sexual activity probabilities assumed to be linear from age 10 to first data point at age 15
+    Last value duplicated so that it interpolates out to 50 and then stops
     '''
 
-    sexually_active = np.array([[0, 5, 10,    15,   20,   25,   30,   35,   40,   45,   50],
-                                [0, 0,  0,  50.4, 55.9, 57.3, 60.8, 66.4, 67.5, 68.2, 68.2]])
+    sexually_active = np.array([[0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50],
+                                [0, 0, 0, 15, 51.2, 69.4, 69.3, 68.6, 68.1, 59.7, 59.7]])
 
-    sexually_active[1] /= 100 # Convert from percent to rate per woman
+    sexually_active[1] /= 100  # Convert from percent to rate per woman
     activity_ages = sexually_active[0]
     activity_interp_model = si.interp1d(x=activity_ages, y=sexually_active[1])
     activity_interp = activity_interp_model(fpd.spline_preg_ages)  # Evaluate interpolation along resolution of ages
 
     return activity_interp
 
+def sexual_activity_region():
+    '''
+    Returns a linear interpolation of rates of female sexual activity, stratified by region
+    '''
+    sexually_active_region_data = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'sexual_activity_region.csv')
+    sexually_active_region_dict = {}
+    sexually_active_region_dict['region'] = sexually_active_region_data.iloc[:, 0]  # Return region names
+    sexually_active_region_dict['age'] = sexually_active_region_data.iloc[:, 1]   # Return age
+    sexually_active_region_dict['perc'] = sexually_active_region_data.iloc[:, 2] / 100  # Return perc divide by 100 to convert to a rate
+    activity_ages_region = sexually_active_region_dict['age']
+    activity_interp_model_region = si.interp1d(x=activity_ages_region, y=sexually_active_region_dict['perc'])
+    activity_interp_region = activity_interp_model_region(fpd.spline_preg_ages)
+
+    return activity_interp_region
 
 def sexual_activity_pp():
     '''
     Returns an array of monthly likelihood of having resumed sexual activity within 0-35 months postpartum
-    Uses DHS Senegal 2018 individual recode (postpartum (v222), months since last birth, and sexual activity within 30 days.
-    Limited to 35 months postpartum (can use any limit you want 0-35 max)
+    Uses 2016 Ethiopia DHS individual recode (postpartum (v222), months since last birth, and sexual activity within 30 days.
+    Data is weighted.
+    Limited to 23 months postpartum (can use any limit you want 0-23 max)
     Postpartum month 0 refers to the first month after delivery
     '''
 
     postpartum_sex = np.array([
-        [0,  0.104166667],
-        [1,  0.300000000],
-        [2,  0.383177570],
-        [3,  0.461538462],
-        [4,  0.476635514],
-        [5,  0.500000000],
-        [6,  0.565217391],
-        [7,  0.541666667],
-        [8,  0.547368421],
-        [9,  0.617391304],
-        [10, 0.578947368],
-        [11, 0.637254902],
-        [12, 0.608247423],
-        [13, 0.582278481],
-        [14, 0.542553191],
-        [15, 0.678260870],
-        [16, 0.600000000],
-        [17, 0.605042017],
-        [18, 0.562500000],
-        [19, 0.529411765],
-        [20, 0.674698795],
-        [21, 0.548780488],
-        [22, 0.616161616],
-        [23, 0.709401709],
-        [24, 0.651376147],
-        [25, 0.780219780],
-        [26, 0.717647059],
-        [27, 0.716417910],
-        [28, 0.683544304],
-        [29, 0.716417910],
-        [30, 0.640625000],
-        [31, 0.650000000],
-        [32, 0.676470588],
-        [33, 0.645161290],
-        [34, 0.606557377],
-        [35, 0.644736842],
+        [0, 0.19253],
+        [1, 0.31858],
+        [2, 0.49293],
+        [3, 0.64756],
+        [4, 0.78684],
+        [5, 0.67009],
+        [6, 0.75804],
+        [7, 0.79867],
+        [8, 0.84857],
+        [9, 0.80293],
+        [10, 0.89259],
+        [11, 0.8227],
+        [12, 0.85876],
+        [13, 0.83104],
+        [14, 0.77563],
+        [15, 0.79917],
+        [16, 0.79582],
+        [17, 0.84817],
+        [18, 0.77804],
+        [19, 0.80811],
+        [20, 0.82049],
+        [21, 0.77607],
+        [22, 0.79261],
+        [23, 0.8373],
     ])
 
+
+
     postpartum_activity = {}
     postpartum_activity['month'] = postpartum_sex[:, 0]
     postpartum_activity['percent_active'] = postpartum_sex[:, 1]
 
     return postpartum_activity
 
 
+def sexual_activity_pp_region():
+    '''
+     # Returns an additional array of monthly likelihood of having resumed sexual activity by region
+    '''
+    pp_activity_region = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'sexual_activity_pp_region.csv')
+    pp_activity_region_dict = {}
+    pp_activity_region_dict['region'] = pp_activity_region['region'] # Return region names
+    pp_activity_region_dict['month'] = pp_activity_region['month'] # Return month postpartum
+    pp_activity_region_dict['perc'] = pp_activity_region['perc'] # Return likelihood of resumed sexual activity
+
+    return pp_activity_region_dict
+
+
 def debut_age():
     '''
     Returns an array of weighted probabilities of sexual debut by a certain age 10-45.
     Data taken from DHS variable v531 (imputed age of sexual debut, imputed with data from age at first union)
-    Use sexual_debut_age_probs.py under fp_analyses/data to output for other DHS countries
+    Use sexual_debut_age_probs.py under locations/data_processing to output for other DHS countries
     '''
 
     sexual_debut = np.array([
-        [10, 0.004362494588533180],
-        [11, 0.005887267309386780],
-        [12, 0.016249279181639800],
-        [13, 0.0299019826473517],
-        [14, 0.055785658051997],
-        [15, 0.09813952463469960],
-        [16, 0.112872333807184],
-        [17, 0.11953800217275100],
-        [18, 0.10881048442282400],
-        [19, 0.08688267743864320],
-        [20, 0.0781062086093285],
-        [21, 0.055562127900473800],
-        [22, 0.047649966917757800],
-        [23, 0.03670233295320280],
-        [24, 0.02962171655627400],
-        [25, 0.03071900157389080],
-        [26, 0.020088166028125700],
-        [27, 0.012959307423989900],
-        [28, 0.009789125590573670],
-        [29, 0.010992698492904500],
-        [30, 0.0064009386756690000],
-        [31, 0.00531499008144595],
-        [32, 0.004500210075413140],
-        [33, 0.004643541107103950],
-        [34, 0.0015287248836055500],
-        [35, 0.0012933308143284600],
-        [36, 0.0008169702220519970],
-        [37, 0.0005138447212362420],
-        [38, 0.0030994890039629400],
-        [39, 0.0007583698086919300],
-        [40, 0.0001470674087999730],
-        [42, 0.00018238823303343100],
-        [43, 0.0000620676775406016],
-        [45, 0.0001177109855848480]])
+        [10, 0.00671240845335203],
+        [11, 0.00918135820646243],
+        [12, 0.0309770814788788],
+        [13, 0.059400507503726],
+        [14, 0.130291755291],
+        [15, 0.196183864268175],
+        [16, 0.130556610013873],
+        [17, 0.103290455840828],
+        [18, 0.110776245328648],
+        [19, 0.0530816775521274],
+        [20, 0.0588590881799291],
+        [21, 0.026991174849838],
+        [22, 0.0271788262050103],
+        [23, 0.0188626403851833],
+        [24, 0.0112214052863469],
+        [25, 0.0109271507351524],
+        [26, 0.00443999952806908],
+        [27, 0.00359275321149036],
+        [28, 0.00303477463739577],
+        [29, 0.0017573689141809],
+        [30, 0.00121215246872525],
+        [31, 0.000711491329468429],
+        [32, 0.000137332034070925],
+        [33, 0.000279848072025066],
+        [34, 7.17053090713206E-06],
+        [35, 9.65008015799441E-05],
+        [36, 8.46224502635213E-06],
+        [37, 3.97705796721265E-05],
+        [43, 0.00019012606885453]])
 
     debut_age = {}
     debut_age['ages'] = sexual_debut[:, 0]
     debut_age['probs'] = sexual_debut[:, 1]
 
     return debut_age
 
+def debut_age_region():
+    '''
+ #   Returns an additional array of weighted probabilities of sexual debut by region
+    '''
+    sexual_debut_region_data = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'sexual_debut_region.csv')
+    debut_age_region_dict = {}
+    debut_age_region_dict['region'] = sexual_debut_region_data['region'] # Return region names
+    debut_age_region_dict['age'] = sexual_debut_region_data['age'] # Return month postpartum
+    debut_age_region_dict['prob'] = sexual_debut_region_data['prob'] # Return weighted probabilities of sexual debut
+    return debut_age_region_dict
+
 
 def exposure_age():
     '''
     Returns an array of experimental factors to be applied to account for
     residual exposure to either pregnancy or live birth by age.  Exposure to pregnancy will
     increase factor number and residual likelihood of avoiding live birth (mostly abortion,
     also miscarriage), will decrease factor number
     '''
-    exposure_correction_age = np.array([[0, 5, 10, 12.5,  15,  18,  20,  25,  30,  35,  40,  45,  50],
-                                        [1, 1,  1,    1,   1,   1,   1,   1,   1, 1, 1, 1, 1]])
+    exposure_correction_age = np.array([[0, 5, 10, 12.5, 15, 18, 20, 25, 30, 35, 40, 45, 50],
+                                        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]])
     exposure_age_interp = data2interp(exposure_correction_age, fpd.spline_preg_ages)
 
     return exposure_age_interp
 
 
 def exposure_parity():
     '''
     Returns an array of experimental factors to be applied to account for residual exposure to either pregnancy
     or live birth by parity.
     '''
-    exposure_correction_parity = np.array([[0, 1, 2, 3, 4, 5, 6,   7,   8,   9,   10,   11,    12,  20],
-                                           [1, 1, 1, 1, 1, 1, 1, 0.8, 0.5, 0.3, 0.15, 0.10,  0.05, 0.01]])
+    exposure_correction_parity = np.array([[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 20],
+                                           [1, 1, 1, 1, 1, 1, 1, 0.8, 0.5, 0.3, 0.15, 0.10, 0.05, 0.01]])
     exposure_parity_interp = data2interp(exposure_correction_parity, fpd.spline_parities)
 
     return exposure_parity_interp
 
 
 def birth_spacing_pref():
     '''
     Returns an array of birth spacing preferences by closest postpartum month.
     Applied to postpartum pregnancy likelihoods.
 
     NOTE: spacing bins must be uniform!
     '''
     postpartum_spacing = np.array([
-        [0,  0.5],
-        [3,  0.5],
-        [6,  0.5],
-        [9,  0.5],
-        [12, 0.8],
-        [15, 1.2],
-        [18, 5.0],
-        [21, 5.0],
-        [24, 9.0],
-        [27, 9.0],
-        [30, 9.0],
-        [33, 9.0],
-        [36, 5.0],
+        [0, 1],
+        [3, 1],
+        [6, 1],
+        [9, 1],
+        [12, 1],
+        [15, 1],
+        [18, 1],
+        [21, 1],
+        [24, 1],
+        [27, 1],
+        [30, 1],
+        [33, 1],
+        [36, 1],
     ])
 
     # Calculate the intervals and check they're all the same
     intervals = np.diff(postpartum_spacing[:, 0])
     interval = intervals[0]
-    assert np.all(intervals == interval), f'In order to be computed in an array, birth spacing preference bins must be equal width, not {intervals}'
+    assert np.all(
+        intervals == interval), f'In order to be computed in an array, birth spacing preference bins must be equal width, not {intervals}'
     pref_spacing = {}
-    pref_spacing['interval'] = interval # Store the interval (which we've just checked is always the same)
-    pref_spacing['n_bins'] = len(intervals) # Actually n_bins - 1, but we're counting 0 so it's OK
-    pref_spacing['months'] = postpartum_spacing[:,0]
-    pref_spacing['preference'] = postpartum_spacing[:, 1] # Store the actual birth spacing data
+    pref_spacing['interval'] = interval  # Store the interval (which we've just checked is always the same)
+    pref_spacing['n_bins'] = len(intervals)  # Actually n_bins - 1, but we're counting 0 so it's OK
+    pref_spacing['months'] = postpartum_spacing[:, 0]
+    pref_spacing['preference'] = postpartum_spacing[:, 1]  # Store the actual birth spacing data
 
     return pref_spacing
 
 
-
-#%% Contraceptive methods
+# %% Contraceptive methods
 
 def methods():
     '''
     Names, indices, modern/traditional flag, and efficacies of contraceptive methods -- see also parameters.py
     Efficacy from Guttmacher, fp_prerelease/docs/gates_review/contraceptive-failure-rates-in-developing-world_1.pdf
     BTL failure rate from general published data
     Pooled efficacy rates for all women in this study: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4970461/
     '''
 
     # Define method data
-    data = {                # Index, modern, efficacy
-        'None'              : [0, False, 0.000],
-        'Withdrawal'        : [1, False, 0.866],
-        'Other traditional' : [2, False, 0.861], # 1/2 periodic abstinence, 1/2 other traditional approx.  Using rate from periodic abstinence
-        'Condoms'           : [3, True,  0.946],
-        'Pill'              : [4, True,  0.945],
-        'Injectables'       : [5, True,  0.983],
-        'Implants'          : [6, True,  0.994],
-        'IUDs'              : [7, True,  0.986],
-        'BTL'               : [8, True,  0.995],
-        'Other modern'      : [9, True,  0.880], # SDM makes up about 1/2 of this, perfect use is 95% and typical is 88%.  EC also included here, efficacy around 85% https : //www.aafp.org/afp/2004/0815/p707.html
+    data = {  # Index, modern, efficacy
+        'None': [0, False, 0.000],
+        'Withdrawal': [1, False, 0.866],
+        'Other traditional': [2, False, 0.861],
+        # 1/2 periodic abstinence, 1/2 other traditional approx.  Using rate from periodic abstinence
+        'Condoms': [3, True, 0.946],
+        'Pill': [4, True, 0.945],
+        'Injectables': [5, True, 0.983],
+        'Implants': [6, True, 0.994],
+        'IUDs': [7, True, 0.986],
+        'BTL': [8, True, 0.995],
+        'Other modern': [9, True, 0.880],
+        # SDM makes up about 1/2 of this, perfect use is 95% and typical is 88%.  EC also included here, efficacy around 85% https : //www.aafp.org/afp/2004/0815/p707.html
     }
 
     keys = data.keys()
     methods = {}
-    methods['map']    = {k:data[k][0] for k in keys}
-    methods['modern'] = {k:data[k][1] for k in keys}
-    methods['eff']    = {k:data[k][2] for k in keys}
+    methods['map'] = {k: data[k][0] for k in keys}
+    methods['modern'] = {k: data[k][1] for k in keys}
+    methods['eff'] = {k: data[k][2] for k in keys}
 
     # Age bins for different method switching matrices -- duplicated in defaults.py
     methods['age_map'] = {
-        '<18'   : [ 0, 18],
-        '18-20' : [18, 20],
-        '21-25' : [20, 25],
-        '26-35' : [25, 35],
-        '>35'   : [35, fpd.max_age+1], # +1 since we're using < rather than <=
+        '<18': [0, 18],
+        '18-20': [18, 20],
+        '21-25': [20, 25],
+        '26-35': [25, 35],
+        '>35': [35, fpd.max_age + 1],  # +1 since we're using < rather than <=
     }
 
-    # Data on trend in MCPR in Senegal over time, in % # CK: TODO: find source
-    methods['mcpr_years'] = np.array([1950, 1980, 1986, 1992, 1997, 2005, 2010, 2012, 2014, 2015, 2016, 2017, 2018, 2019, 2020])
-    methods['mcpr_rates'] = np.array([0.50,  1.0, 2.65, 4.53, 7.01, 7.62, 8.85, 11.3, 14.7, 15.3, 16.5, 18.8,   19,   20, 20.4])/100
+    # Data on trend in CPR over time in from Ethiopia, in %.
+    # Taken from UN Population Division Data Portal, married women 1970-1986, all women 1990-2030
+    # https://population.un.org/dataportal/data/indicators/1/locations/231/start/1950/end/2040/table/pivotbylocation
+    # Projections go out until 2030, but the csv file can be manually adjusted to remove any projections and stop at your desired year
+    cpr_data = pd.read_csv(thisdir / 'ethiopia' / 'cpr.csv')
+    methods['mcpr_years'] = cpr_data['year'].to_numpy()
+    methods['mcpr_rates'] = cpr_data['cpr'].to_numpy() / 100  # convert from percent to rate
 
     return methods
 
 
-def method_probs():
-    '''
+'''
+For reference
+def method_probs_senegal():
+    
+    It does leave Senegal matrices in place in the Ethiopia file for now. 
+    We may want to test with these as we work through scenarios and calibration. 
+    
     Define "raw" (un-normalized, un-trended) matrices to give transitional probabilities
     from 2018 DHS Senegal contraceptive calendar data.
 
     Probabilities in this function are annual probabilities of initiating (top row), discontinuing (first column),
     continuing (diagonal), or switching methods (all other entries).
 
     Probabilities at postpartum month 1 are 1 month transitional probabilities
     for starting a method after delivery.
 
     Probabilities at postpartum month 6 are 5 month transitional probabilities
     for starting or changing methods over the first 6 months postpartum.
 
     Data from Senegal DHS contraceptive calendars, 2017 and 2018 combined
+    
+
+    raw = {
+
+        # Main switching matrix: all non-postpartum women
+        'annual': {
+            '<18': np.array([
+                [0.9953, 0., 0.0002, 0.0012, 0.0002, 0.0017, 0.0014, 0.0001, 0., 0.],
+                [0., 1.0000, 0., 0., 0., 0., 0., 0., 0., 0.],
+                [0.0525, 0., 0.9475, 0., 0., 0., 0., 0., 0., 0.],
+                [0.307, 0., 0., 0.693, 0., 0., 0., 0., 0., 0.],
+                [0.5358, 0., 0., 0., 0.3957, 0.0685, 0., 0., 0., 0.],
+                [0.3779, 0., 0., 0., 0.0358, 0.5647, 0.0216, 0., 0., 0.],
+                [0.2003, 0., 0., 0., 0., 0., 0.7997, 0., 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 1.0000, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]]),
+            '18-20': np.array([
+                [0.9774, 0., 0.0014, 0.0027, 0.0027, 0.0104, 0.0048, 0.0003, 0., 0.0003],
+                [0., 1.0000, 0., 0., 0., 0., 0., 0., 0., 0.],
+                [0.3216, 0., 0.6784, 0., 0., 0., 0., 0., 0., 0.],
+                [0.182, 0., 0., 0.818, 0., 0., 0., 0., 0., 0.],
+                [0.4549, 0., 0., 0., 0.4754, 0.0463, 0.0234, 0., 0., 0.],
+                [0.4389, 0., 0.0049, 0.0099, 0.0196, 0.5218, 0.0049, 0., 0., 0.],
+                [0.17, 0., 0., 0., 0., 0.0196, 0.8103, 0., 0., 0.],
+                [0.1607, 0., 0., 0., 0., 0., 0., 0.8393, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0.4773, 0., 0., 0.4773, 0., 0., 0., 0., 0., 0.0453]]),
+            '21-25': np.array([
+                [0.9581, 0.0001, 0.0011, 0.0024, 0.0081, 0.0184, 0.0108, 0.0006, 0., 0.0004],
+                [0.4472, 0.5528, 0., 0., 0., 0., 0., 0., 0., 0.],
+                [0.2376, 0., 0.7624, 0., 0., 0., 0., 0., 0., 0.],
+                [0.1896, 0., 0.0094, 0.754, 0.0094, 0., 0.0188, 0., 0., 0.0188],
+                [0.3715, 0.003, 0.003, 0., 0.5703, 0.0435, 0.0088, 0., 0., 0.],
+                [0.3777, 0., 0.0036, 0.0036, 0.0258, 0.5835, 0.0036, 0.0024, 0., 0.],
+                [0.137, 0., 0., 0.003, 0.0045, 0.0045, 0.848, 0.003, 0., 0.],
+                [0.1079, 0., 0., 0., 0.0445, 0., 0.0225, 0.8251, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0.3342, 0., 0., 0.1826, 0., 0., 0., 0., 0., 0.4831]]),
+            '26-35': np.array([
+                [0.9462, 0.0001, 0.0018, 0.0013, 0.0124, 0.0209, 0.0139, 0.003, 0.0001, 0.0002],
+                [0.0939, 0.8581, 0., 0., 0., 0.048, 0., 0., 0., 0.],
+                [0.1061, 0., 0.8762, 0.0051, 0.0025, 0.0025, 0.0051, 0.0025, 0., 0.],
+                [0.1549, 0., 0., 0.8077, 0.0042, 0.0125, 0.0083, 0.0083, 0., 0.0042],
+                [0.3031, 0.0016, 0.0021, 0.0021, 0.6589, 0.0211, 0.0053, 0.0053, 0., 0.0005],
+                [0.2746, 0., 0.0028, 0.002, 0.0173, 0.691, 0.0073, 0.0048, 0., 0.0003],
+                [0.1115, 0.0003, 0.0009, 0.0003, 0.0059, 0.0068, 0.8714, 0.0025, 0.0003, 0.],
+                [0.0775, 0., 0.0015, 0., 0.0058, 0.0044, 0.0044, 0.905, 0., 0.0015],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0.1581, 0., 0.0121, 0., 0., 0., 0., 0., 0., 0.8297]]),
+            '>35': np.array([
+                [0.9462, 0.0001, 0.0018, 0.0013, 0.0124, 0.0209, 0.0139, 0.003, 0.0001, 0.0002],
+                [0.0939, 0.8581, 0., 0., 0., 0.048, 0., 0., 0., 0.],
+                [0.1061, 0., 0.8762, 0.0051, 0.0025, 0.0025, 0.0051, 0.0025, 0., 0.],
+                [0.1549, 0., 0., 0.8077, 0.0042, 0.0125, 0.0083, 0.0083, 0., 0.0042],
+                [0.3031, 0.0016, 0.0021, 0.0021, 0.6589, 0.0211, 0.0053, 0.0053, 0., 0.0005],
+                [0.2746, 0., 0.0028, 0.002, 0.0173, 0.691, 0.0073, 0.0048, 0., 0.0003],
+                [0.1115, 0.0003, 0.0009, 0.0003, 0.0059, 0.0068, 0.8714, 0.0025, 0.0003, 0.],
+                [0.0775, 0., 0.0015, 0., 0.0058, 0.0044, 0.0044, 0.905, 0., 0.0015],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0.1581, 0., 0.0121, 0., 0., 0., 0., 0., 0., 0.8297]])
+        },
+
+        # Postpartum switching matrix, 1 to 6 months
+        'pp1to6': {
+            '<18': np.array([
+                [0.9014, 0., 0.0063, 0.001, 0.0126, 0.051, 0.0272, 0.0005, 0., 0.],
+                [0., 0.5, 0., 0., 0., 0., 0.5, 0., 0., 0.],
+                [0., 0., 1.0000, 0., 0., 0., 0., 0., 0., 0.],
+                [0., 0., 0., 1.0000, 0., 0., 0., 0., 0., 0.],
+                [0.4, 0., 0., 0., 0.6, 0., 0., 0., 0., 0.],
+                [0.0714, 0., 0., 0., 0., 0.9286, 0., 0., 0., 0.],
+                [0., 0., 0., 0., 0., 0., 1.0000, 0., 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 1.0000, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]]),
+            '18-20': np.array([
+                [0.8775, 0.0007, 0.0026, 0.0033, 0.0191, 0.0586, 0.0329, 0.0046, 0., 0.0007],
+                [0., 1.0000, 0., 0., 0., 0., 0., 0., 0., 0.],
+                [0., 0., 1.0000, 0., 0., 0., 0., 0., 0., 0.],
+                [0., 0., 0., 1.0000, 0., 0., 0., 0., 0., 0.],
+                [0., 0., 0., 0., 0.75, 0.25, 0., 0., 0., 0.],
+                [0.0278, 0., 0., 0., 0., 0.9722, 0., 0., 0., 0.],
+                [0.0312, 0., 0., 0., 0., 0., 0.9688, 0., 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 1.0000, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]]),
+            '21-25': np.array([
+                [0.8538, 0.0004, 0.0055, 0.0037, 0.0279, 0.0721, 0.0343, 0.0022, 0., 0.],
+                [0., 1.0000, 0., 0., 0., 0., 0., 0., 0., 0.],
+                [0., 0., 0.9583, 0., 0., 0.0417, 0., 0., 0., 0.],
+                [0., 0., 0., 0.5, 0.25, 0.25, 0., 0., 0., 0.],
+                [0.0244, 0., 0., 0., 0.9512, 0.0244, 0., 0., 0., 0.],
+                [0.0672, 0., 0., 0., 0., 0.9328, 0., 0., 0., 0.],
+                [0.0247, 0., 0., 0., 0., 0.0123, 0.963, 0., 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 1.0000, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]]),
+            '26-35': np.array([
+                [0.8433, 0.0008, 0.0065, 0.004, 0.029, 0.0692, 0.039, 0.0071, 0.0001, 0.001],
+                [0., 0.5, 0., 0., 0., 0., 0.5, 0., 0., 0.],
+                [0.027, 0., 0.9189, 0., 0., 0.027, 0.027, 0., 0., 0.],
+                [0.1667, 0., 0., 0.6667, 0., 0., 0.1667, 0., 0., 0.],
+                [0.0673, 0., 0., 0., 0.8654, 0.0288, 0.0385, 0., 0., 0.],
+                [0.0272, 0., 0.0039, 0., 0.0078, 0.9533, 0.0078, 0., 0., 0.],
+                [0.0109, 0., 0., 0., 0.0036, 0., 0.9855, 0., 0., 0.],
+                [0.0256, 0., 0., 0., 0., 0.0256, 0., 0.9487, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]]),
+            '>35': np.array([
+                [0.8433, 0.0008, 0.0065, 0.004, 0.029, 0.0692, 0.039, 0.0071, 0.0001, 0.001],
+                [0., 0.5, 0., 0., 0., 0., 0.5, 0., 0., 0.],
+                [0.027, 0., 0.9189, 0., 0., 0.027, 0.027, 0., 0., 0.],
+                [0.1667, 0., 0., 0.6667, 0., 0., 0.1667, 0., 0., 0.],
+                [0.0673, 0., 0., 0., 0.8654, 0.0288, 0.0385, 0., 0., 0.],
+                [0.0272, 0., 0.0039, 0., 0.0078, 0.9533, 0.0078, 0., 0., 0.],
+                [0.0109, 0., 0., 0., 0.0036, 0., 0.9855, 0., 0., 0.],
+                [0.0256, 0., 0., 0., 0., 0.0256, 0., 0.9487, 0., 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 1.0000, 0.],
+                [0., 0., 0., 0., 0., 0., 0., 0., 0., 1.0000]])
+        },
+
+        # Postpartum initiation vectors, 0 to 1 month
+        'pp0to1': {
+            '<18': np.array([0.9607, 0.0009, 0.0017, 0.0009, 0.0021, 0.0128, 0.0205, 0.0004, 0., 0.]),
+            '18-20': np.array([0.9525, 0.0006, 0.0017, 0.0006, 0.0028, 0.0215, 0.0198, 0.0006, 0., 0.]),
+            '21-25': np.array([0.9379, 0., 0.0053, 0.0009, 0.0083, 0.0285, 0.0177, 0.0013, 0., 0.]),
+            '26-35': np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004, 0.0022, 0.0004]),
+            '>35': np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004, 0.0022, 0.0004]),
+        }
+    }
+    return raw
+    '''
+
+def method_probs():
+    '''
+    Define "raw" (un-normalized, un-trended) matrices to give transitional probabilities
+    from PMA Ethiopia contraceptive calendar data.
+
+    Probabilities in this function are annual probabilities of initiating (top row), discontinuing (first column),
+    continuing (diagonal), or switching methods (all other entries).
+
+    Probabilities at postpartum month 1 are 1 month transitional probabilities
+    for starting a method after delivery.
+
+    Probabilities at postpartum month 6 are 5 month transitional probabilities
+    for starting or changing methods over the first 6 months postpartum.
+
+    Data from Ethiopia PMA contraceptive calendars, 2019-2020
+    Processed from matrices_ethiopia_pma_2019_20.csv using process_matrices.py
     '''
 
     raw = {
 
-    # Main switching matrix: all non-postpartum women
-    'annual': {
-        '<18': np.array([
-           [0.9953, 0.    , 0.0002, 0.0012, 0.0002, 0.0017, 0.0014, 0.0001, 0.    , 0.    ],
-           [0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.0525, 0.    , 0.9475, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.307 , 0.    , 0.    , 0.693 , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.5358, 0.    , 0.    , 0.    , 0.3957, 0.0685, 0.    , 0.    , 0.    , 0.    ],
-           [0.3779, 0.    , 0.    , 0.    , 0.0358, 0.5647, 0.0216, 0.    , 0.    , 0.    ],
-           [0.2003, 0.    , 0.    , 0.    , 0.    , 0.    , 0.7997, 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]]),
-        '18-20': np.array([
-           [0.9774, 0.    , 0.0014, 0.0027, 0.0027, 0.0104, 0.0048, 0.0003, 0.    , 0.0003],
-           [0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.3216, 0.    , 0.6784, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.182 , 0.    , 0.    , 0.818 , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.4549, 0.    , 0.    , 0.    , 0.4754, 0.0463, 0.0234, 0.    , 0.    , 0.    ],
-           [0.4389, 0.    , 0.0049, 0.0099, 0.0196, 0.5218, 0.0049, 0.    , 0.    , 0.    ],
-           [0.17  , 0.    , 0.    , 0.    , 0.    , 0.0196, 0.8103, 0.    , 0.    , 0.    ],
-           [0.1607, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.8393, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.4773, 0.    , 0.    , 0.4773, 0.    , 0.    , 0.    , 0.    , 0.    , 0.0453]]),
-        '21-25': np.array([
-           [0.9581, 0.0001, 0.0011, 0.0024, 0.0081, 0.0184, 0.0108, 0.0006, 0.    , 0.0004],
-           [0.4472, 0.5528, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.2376, 0.    , 0.7624, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.1896, 0.    , 0.0094, 0.754 , 0.0094, 0.    , 0.0188, 0.    , 0.    , 0.0188],
-           [0.3715, 0.003 , 0.003 , 0.    , 0.5703, 0.0435, 0.0088, 0.    , 0.    , 0.    ],
-           [0.3777, 0.    , 0.0036, 0.0036, 0.0258, 0.5835, 0.0036, 0.0024, 0.    , 0.    ],
-           [0.137 , 0.    , 0.    , 0.003 , 0.0045, 0.0045, 0.848 , 0.003 , 0.    , 0.    ],
-           [0.1079, 0.    , 0.    , 0.    , 0.0445, 0.    , 0.0225, 0.8251, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.3342, 0.    , 0.    , 0.1826, 0.    , 0.    , 0.    , 0.    , 0.    , 0.4831]]),
-        '26-35': np.array([
-           [0.9462, 0.0001, 0.0018, 0.0013, 0.0124, 0.0209, 0.0139, 0.003 , 0.0001, 0.0002],
-           [0.0939, 0.8581, 0.    , 0.    , 0.    , 0.048 , 0.    , 0.    , 0.    , 0.    ],
-           [0.1061, 0.    , 0.8762, 0.0051, 0.0025, 0.0025, 0.0051, 0.0025, 0.    , 0.    ],
-           [0.1549, 0.    , 0.    , 0.8077, 0.0042, 0.0125, 0.0083, 0.0083, 0.    , 0.0042],
-           [0.3031, 0.0016, 0.0021, 0.0021, 0.6589, 0.0211, 0.0053, 0.0053, 0.    , 0.0005],
-           [0.2746, 0.    , 0.0028, 0.002 , 0.0173, 0.691 , 0.0073, 0.0048, 0.    , 0.0003],
-           [0.1115, 0.0003, 0.0009, 0.0003, 0.0059, 0.0068, 0.8714, 0.0025, 0.0003, 0.    ],
-           [0.0775, 0.    , 0.0015, 0.    , 0.0058, 0.0044, 0.0044, 0.905 , 0.    , 0.0015],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.1581, 0.    , 0.0121, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.8297]]),
-        '>35': np.array([
-           [0.9462, 0.0001, 0.0018, 0.0013, 0.0124, 0.0209, 0.0139, 0.003 , 0.0001, 0.0002],
-           [0.0939, 0.8581, 0.    , 0.    , 0.    , 0.048 , 0.    , 0.    , 0.    , 0.    ],
-           [0.1061, 0.    , 0.8762, 0.0051, 0.0025, 0.0025, 0.0051, 0.0025, 0.    , 0.    ],
-           [0.1549, 0.    , 0.    , 0.8077, 0.0042, 0.0125, 0.0083, 0.0083, 0.    , 0.0042],
-           [0.3031, 0.0016, 0.0021, 0.0021, 0.6589, 0.0211, 0.0053, 0.0053, 0.    , 0.0005],
-           [0.2746, 0.    , 0.0028, 0.002 , 0.0173, 0.691 , 0.0073, 0.0048, 0.    , 0.0003],
-           [0.1115, 0.0003, 0.0009, 0.0003, 0.0059, 0.0068, 0.8714, 0.0025, 0.0003, 0.    ],
-           [0.0775, 0.    , 0.0015, 0.    , 0.0058, 0.0044, 0.0044, 0.905 , 0.    , 0.0015],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.1581, 0.    , 0.0121, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.8297]])
+        # Main switching matrix: all non-postpartum women
+        'annual': {
+            '<18': np.array([
+                [0.9236, 0.0004, 0.0017, 0.0007, 0.0042, 0.0596, 0.0076, 0.0006, 0.    , 0.0017],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
+                [0.1374, 0.    , 0.8571, 0.    , 0.0003, 0.0044, 0.0005, 0.    , 0.    , 0.0001],
+                [0.2815, 0.0001, 0.0003, 0.6995, 0.0007, 0.0164, 0.0012, 0.0001, 0.    , 0.0003],
+                [0.4681, 0.0001, 0.0006, 0.0013, 0.3023, 0.1869, 0.003 , 0.0005, 0.    , 0.0371],
+                [0.3267, 0.0001, 0.0017, 0.0005, 0.0043, 0.6549, 0.009 , 0.0023, 0.    , 0.0005],
+                [0.1937, 0.    , 0.0008, 0.0001, 0.0007, 0.0087, 0.7957, 0.0001, 0.    , 0.0002],
+                [0.4158, 0.0001, 0.0004, 0.0002, 0.0011, 0.0142, 0.0017, 0.5662, 0.    , 0.0004],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ],
+                [0.5988, 0.0001, 0.0006, 0.024 , 0.0186, 0.0258, 0.0027, 0.0002, 0.    , 0.3293]]),
+            '18-20': np.array([
+                [0.8783, 0.0002, 0.0021, 0.0017, 0.0115, 0.0845, 0.0194, 0.0016, 0.    , 0.0006],
+                [0.0599, 0.9362, 0.0001, 0.0001, 0.0004, 0.0027, 0.0006, 0.0001, 0.    , 0.    ],
+                [0.1874, 0.    , 0.8002, 0.0002, 0.0012, 0.0088, 0.002 , 0.0002, 0.    , 0.0001],
+                [0.8023, 0.0001, 0.0012, 0.117 , 0.0068, 0.0498, 0.0109, 0.009 , 0.    , 0.0028],
+                [0.2326, 0.    , 0.0003, 0.0003, 0.7384, 0.025 , 0.0026, 0.0003, 0.    , 0.0004],
+                [0.279 , 0.    , 0.0003, 0.0004, 0.0069, 0.6868, 0.0219, 0.0045, 0.    , 0.0002],
+                [0.2046, 0.    , 0.0002, 0.0018, 0.0058, 0.0224, 0.7647, 0.0002, 0.    , 0.0001],
+                [0.3239, 0.    , 0.0004, 0.0004, 0.0372, 0.1151, 0.0048, 0.5179, 0.    , 0.0002],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ],
+                [0.8974, 0.0002, 0.0017, 0.0016, 0.0093, 0.0693, 0.0156, 0.0013, 0.    , 0.0036]]),
+            '21-25': np.array([
+                [0.8704, 0.0008, 0.0026, 0.0011, 0.0106, 0.0794, 0.0291, 0.0047, 0.    , 0.0012],
+                [0.1535, 0.8357, 0.0002, 0.0001, 0.0009, 0.0067, 0.0024, 0.0004, 0.    , 0.0001],
+                [0.0473, 0.    , 0.8681, 0.    , 0.0333, 0.0408, 0.0047, 0.0004, 0.    , 0.0053],
+                [0.0851, 0.    , 0.0001, 0.8887, 0.0006, 0.0237, 0.0014, 0.0003, 0.    , 0.0001],
+                [0.3553, 0.0002, 0.0027, 0.0002, 0.4916, 0.1088, 0.0297, 0.0111, 0.    , 0.0003],
+                [0.2505, 0.0001, 0.0014, 0.0002, 0.0118, 0.7151, 0.0152, 0.0052, 0.    , 0.0005],
+                [0.1413, 0.0001, 0.0002, 0.0001, 0.0027, 0.0409, 0.8127, 0.0019, 0.    , 0.0001],
+                [0.0687, 0.    , 0.0001, 0.    , 0.0007, 0.0038, 0.0265, 0.9002, 0.    , 0.0001],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ],
+                [0.7042, 0.0004, 0.0254, 0.0005, 0.0214, 0.061 , 0.0145, 0.0024, 0.    , 0.1703]]),
+            '26-35': np.array([
+                [0.875 , 0.0001, 0.0014, 0.0008, 0.0078, 0.0827, 0.0261, 0.0058, 0.0002, 0.0001],
+                [0.0664, 0.8974, 0.0001, 0.    , 0.0005, 0.0342, 0.0012, 0.0003, 0.    , 0.    ],
+                [0.1795, 0.    , 0.8028, 0.0001, 0.0008, 0.0081, 0.0081, 0.0005, 0.    , 0.    ],
+                [0.1613, 0.    , 0.0002, 0.7594, 0.001 , 0.0613, 0.0027, 0.0009, 0.    , 0.013 ],
+                [0.3407, 0.    , 0.0018, 0.0002, 0.4605, 0.1452, 0.0463, 0.0052, 0.0001, 0.    ],
+                [0.2059, 0.0002, 0.0016, 0.0002, 0.0094, 0.7561, 0.0203, 0.0059, 0.0004, 0.    ],
+                [0.1098, 0.    , 0.0007, 0.    , 0.0014, 0.0176, 0.8692, 0.001 , 0.    , 0.0002],
+                [0.0641, 0.    , 0.0013, 0.    , 0.0003, 0.0028, 0.0009, 0.9306, 0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ],
+                [0.3603, 0.    , 0.0003, 0.0002, 0.0017, 0.0172, 0.0052, 0.0338, 0.    , 0.5813]]),
+            '>35': np.array([
+                [0.9342, 0.0001, 0.0009, 0.0001, 0.0034, 0.0482, 0.0118, 0.001 , 0.    , 0.0002],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
+                [0.0867, 0.    , 0.9104, 0.    , 0.0002, 0.0021, 0.0005, 0.    , 0.    , 0.    ],
+                [0.1769, 0.    , 0.0001, 0.8162, 0.0003, 0.0053, 0.0011, 0.0001, 0.    , 0.    ],
+                [0.1985, 0.    , 0.0141, 0.    , 0.6921, 0.066 , 0.0075, 0.0183, 0.    , 0.0033],
+                [0.1747, 0.0003, 0.0005, 0.    , 0.0061, 0.8054, 0.0117, 0.0012, 0.    , 0.    ],
+                [0.0998, 0.    , 0.0013, 0.0002, 0.0061, 0.0315, 0.861 , 0.0001, 0.    , 0.    ],
+                [0.1299, 0.    , 0.0002, 0.    , 0.0148, 0.0037, 0.0008, 0.8504, 0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ],
+                [0.0957, 0.    , 0.    , 0.    , 0.0002, 0.0023, 0.0006, 0.    , 0.    , 0.9012]])
         },
 
-    # Postpartum switching matrix, 1 to 6 months
-    'pp1to6': {
-        '<18': np.array([
-           [0.9014, 0.    , 0.0063, 0.001 , 0.0126, 0.051 , 0.0272, 0.0005, 0.    , 0.    ],
-           [0.    , 0.5   , 0.    , 0.    , 0.    , 0.    , 0.5   , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.4   , 0.    , 0.    , 0.    , 0.6   , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.0714, 0.    , 0.    , 0.    , 0.    , 0.9286, 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]]),
-        '18-20': np.array([
-           [0.8775, 0.0007, 0.0026, 0.0033, 0.0191, 0.0586, 0.0329, 0.0046, 0.    , 0.0007],
-           [0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.75  , 0.25  , 0.    , 0.    , 0.    , 0.    ],
-           [0.0278, 0.    , 0.    , 0.    , 0.    , 0.9722, 0.    , 0.    , 0.    , 0.    ],
-           [0.0312, 0.    , 0.    , 0.    , 0.    , 0.    , 0.9688, 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]]),
-        '21-25': np.array([
-           [0.8538, 0.0004, 0.0055, 0.0037, 0.0279, 0.0721, 0.0343, 0.0022, 0.    , 0.    ],
-           [0.    , 1.0000, 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.9583, 0.    , 0.    , 0.0417, 0.    , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.5   , 0.25  , 0.25  , 0.    , 0.    , 0.    , 0.    ],
-           [0.0244, 0.    , 0.    , 0.    , 0.9512, 0.0244, 0.    , 0.    , 0.    , 0.    ],
-           [0.0672, 0.    , 0.    , 0.    , 0.    , 0.9328, 0.    , 0.    , 0.    , 0.    ],
-           [0.0247, 0.    , 0.    , 0.    , 0.    , 0.0123, 0.963 , 0.    , 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]]),
-        '26-35': np.array([
-           [0.8433, 0.0008, 0.0065, 0.004 , 0.029 , 0.0692, 0.039 , 0.0071, 0.0001, 0.001 ],
-           [0.    , 0.5   , 0.    , 0.    , 0.    , 0.    , 0.5   , 0.    , 0.    , 0.    ],
-           [0.027 , 0.    , 0.9189, 0.    , 0.    , 0.027 , 0.027 , 0.    , 0.    , 0.    ],
-           [0.1667, 0.    , 0.    , 0.6667, 0.    , 0.    , 0.1667, 0.    , 0.    , 0.    ],
-           [0.0673, 0.    , 0.    , 0.    , 0.8654, 0.0288, 0.0385, 0.    , 0.    , 0.    ],
-           [0.0272, 0.    , 0.0039, 0.    , 0.0078, 0.9533, 0.0078, 0.    , 0.    , 0.    ],
-           [0.0109, 0.    , 0.    , 0.    , 0.0036, 0.    , 0.9855, 0.    , 0.    , 0.    ],
-           [0.0256, 0.    , 0.    , 0.    , 0.    , 0.0256, 0.    , 0.9487, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]]),
-        '>35': np.array([
-           [0.8433, 0.0008, 0.0065, 0.004 , 0.029 , 0.0692, 0.039 , 0.0071, 0.0001, 0.001 ],
-           [0.    , 0.5   , 0.    , 0.    , 0.    , 0.    , 0.5   , 0.    , 0.    , 0.    ],
-           [0.027 , 0.    , 0.9189, 0.    , 0.    , 0.027 , 0.027 , 0.    , 0.    , 0.    ],
-           [0.1667, 0.    , 0.    , 0.6667, 0.    , 0.    , 0.1667, 0.    , 0.    , 0.    ],
-           [0.0673, 0.    , 0.    , 0.    , 0.8654, 0.0288, 0.0385, 0.    , 0.    , 0.    ],
-           [0.0272, 0.    , 0.0039, 0.    , 0.0078, 0.9533, 0.0078, 0.    , 0.    , 0.    ],
-           [0.0109, 0.    , 0.    , 0.    , 0.0036, 0.    , 0.9855, 0.    , 0.    , 0.    ],
-           [0.0256, 0.    , 0.    , 0.    , 0.    , 0.0256, 0.    , 0.9487, 0.    , 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000, 0.    ],
-           [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.0000]])
+
+        # Postpartum switching matrix, 1 to 6 months
+        'pp1to6': {
+            '<18': np.array([
+                [0.8316, 0.    , 0.0046, 0.    , 0.0069, 0.1376, 0.018 , 0.0012,0.    , 0.    ],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.0135, 0.    , 0     , 0     , 0.1861, 0.8004, 0.    , 0.    ,0.    , 0.    ], 
+                [0.0036, 0.    , 0.    , 0.    , 0.    , 0.9964, 0.    , 0.    ,0.    , 0.    ], 
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,1.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 1.    ]]),
+            '18-20': np.array([
+                [0.7971, 0.    , 0.0027, 0.    , 0.0046, 0.1534, 0.0383, 0.004, 0.    , 0.    ],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.2151, 0.    , 0.    , 0.    , 0.0337, 0.7016, 0.0496, 0.    ,0.    , 0     ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,1.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 1.    ]]),
+            '21-25': np.array([ 
+                [0.807 , 0.0005, 0.0011, 0.0011, 0.0187, 0.1338, 0.0307, 0.0067,0.    , 0.0004],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.3813, 0.6187, 0.    , 0.    ,0.    , 0.    ],
+                [0.0722, 0.    , 0.    , 0.    , 0.    , 0.9278, 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,1.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 1.    ]]),
+            '26-35': np.array([
+                [0.8582, 0.0007, 0.0019, 0.0001, 0.0118, 0.1083, 0.0151, 0.0039, 0, 0],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.2954, 0.    , 0.    , 0.    , 0.6214, 0.    , 0.    , 0.0832,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.989 , 0.    , 0.0067,0.0043, 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,1.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 1.    ]]),
+            '>35': np.array([
+                [0.8897, 0.    , 0.0035, 0.0004, 0.0012, 0.0733, 0.0194, 0.0099,0.    , 0.0025],
+                [0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 1.    , 0.    , 0.    , 0.    ,0.    , 0.    ],
+                [0.0568, 0.    , 0.    , 0.    , 0.    , 0.9432, 0.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    , 0.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 1.    ,0.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,1.    , 0.    ],
+                [0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    , 0.    ,0.    , 1.    ]])
         },
 
-    # Postpartum initiation vectors, 0 to 1 month
-    'pp0to1': {
-        '<18':   np.array([0.9607, 0.0009, 0.0017, 0.0009, 0.0021, 0.0128, 0.0205, 0.0004, 0.    , 0.    ]),
-        '18-20': np.array([0.9525, 0.0006, 0.0017, 0.0006, 0.0028, 0.0215, 0.0198, 0.0006, 0.    , 0.    ]),
-        '21-25': np.array([0.9379, 0.    , 0.0053, 0.0009, 0.0083, 0.0285, 0.0177, 0.0013, 0.    , 0.    ]),
-        '26-35': np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004 , 0.0022, 0.0004]),
-        '>35':   np.array([0.9254, 0.0002, 0.0036, 0.0007, 0.0102, 0.0265, 0.0268, 0.004 , 0.0022, 0.0004]),
+        # Postpartum initiation vectors, 0 to 1 month 
+        'pp0to1': {
+            '<18': np.array([0.95, 0., 0., 0., 0.0031, 0.0383, 0.0073, 0.0013, 0., 0.]),
+            '18-20': np.array([0.9382, 0., 0., 0., 0.0015, 0.0466, 0.0118, 0.0019, 0., 0.]),
+            '21-25': np.array([0.9583, 0.0006, 0., 0., 0.0003, 0.0343, 0.0053, 0.0013, 0., 0.]),
+            '26-35': np.array([0.9693, 0., 0.0005, 0., 0.0032, 0.0195, 0.0044, 0.0025, 0.0005, 0.]),
+            '>35': np.array([0.9556, 0., 0., 0., 0.0009, 0.0298, 0.0028, 0.0048, 0.006, 0.]),
         }
     }
+
     return raw
 
 
 def barriers():
-    ''' Reasons for nonuse -- taken from DHS '''
+    ''' Reasons for nonuse -- taken from Ethiopia PMA 2019. '''
 
-    barriers = sc.odict({
-      'No need'   :  54.2,
-      'Opposition':  30.5,
-      'Knowledge' :   1.7,
-      'Access'    :   4.5,
-      'Health'    :  12.9,
+    barriers = sc.odict({ #updated based on PMA cross-sectional data
+        'No need': 58.5,
+        'Opposition': 16.6,
+        'Knowledge': 1.28,
+        'Access': 2.73,
+        'Health': 20.9,
     })
 
-    barriers[:] /= barriers[:].sum() # Ensure it adds to 1
+    barriers[:] /= barriers[:].sum()  # Ensure it adds to 1
     return barriers
 
+def barriers_region():
+    '''
+    Returns reasons for nonuse by region
+    '''
+    reasons_region = pd.read_csv(thisdir / 'ethiopia' / 'subnational_data' / 'barriers_region.csv')
+    reasons_region_dict = {}
+    reasons_region_dict['region'] = reasons_region['region'] # Return region names
+    reasons_region_dict['barrier'] = reasons_region['barrier'] # Return the reason for nonuse
+    reasons_region_dict['perc'] = reasons_region['perc'] # Return retuned the percentage
+
+    return reasons_region_dict
 
 
-#%% Make and validate parameters
+def urban_proportion():
+    """Load information about the proportion of people who live in an urban setting"""
+    urban_data = pd.read_csv(thisdir / 'ethiopia' / 'urban.csv')
+    return urban_data["mean"][0]  # Return this value as a float
 
-def make_pars():
+# %% Make and validate parameters
+
+def make_pars(use_empowerment=None, use_education=None, use_partnership=None, use_subnational=None, seed=None):
     '''
     Take all parameters and construct into a dictionary
     '''
 
     # Scalar parameters and filenames
     pars = scalar_pars()
     pars['filenames'] = filenames()
 
     # Demographics and pregnancy outcome
-    pars['age_pyramid']        = age_pyramid()
-    pars['age_mortality']      = age_mortality()
+    pars['age_pyramid'] = age_pyramid()
+    pars['age_mortality'] = age_mortality()
+    pars['urban_prop'] = urban_proportion()
     pars['maternal_mortality'] = maternal_mortality()
-    pars['infant_mortality']   = infant_mortality()
-    pars['miscarriage_rates']  = miscarriage()
-    pars['stillbirth_rate']    = stillbirth()
+    pars['infant_mortality'] = infant_mortality()
+    pars['miscarriage_rates'] = miscarriage()
+    pars['stillbirth_rate'] = stillbirth()
 
     # Fecundity
-    pars['age_fecundity']          = female_age_fecundity()
+    pars['age_fecundity'] = female_age_fecundity()
     pars['fecundity_ratio_nullip'] = fecundity_ratio_nullip()
     pars['lactational_amenorrhea'] = lactational_amenorrhea()
 
     # Pregnancy exposure
-    pars['sexual_activity']    = sexual_activity()
+    pars['sexual_activity'] = sexual_activity()
     pars['sexual_activity_pp'] = sexual_activity_pp()
-    pars['debut_age']          = debut_age()
-    pars['exposure_age']       = exposure_age()
-    pars['exposure_parity']    = exposure_parity()
-    pars['spacing_pref']       = birth_spacing_pref()
+    pars['debut_age'] = debut_age()
+    pars['exposure_age'] = exposure_age()
+    pars['exposure_parity'] = exposure_parity()
+    pars['spacing_pref'] = birth_spacing_pref()
 
     # Contraceptive methods
-    pars['methods']        = methods()
+    pars['methods'] = methods()
     pars['methods']['raw'] = method_probs()
-    pars['barriers']       = barriers()
+    pars['barriers'] = barriers()
+
+    # Regional parameters
+    if use_subnational:
+        pars['region'] = region_proportions()  # This function returns extrapolated and raw data
+        pars['lactational_amenorrhea_region'] = lactational_amenorrhea_region()
+        pars['sexual_activity_region'] = sexual_activity_region()
+        pars['sexual_activity_pp_region'] = sexual_activity_pp_region()
+        pars['debut_age_region'] = debut_age_region()
+        pars['barriers_region'] = barriers_region()
+
+    kwargs = locals()
+    not_implemented_args = ['use_empowerment', 'use_education', 'use_partnership']
+    true_args = [key for key in not_implemented_args if kwargs[key] is True]
+    if true_args:
+        errmsg = f"{true_args} not implemented yet for {pars['location']}"
+        raise NotImplementedError(errmsg)
 
-    return pars
+    return pars
```

### Comparing `fpsim-0.22.0/fpsim/scenarios.py` & `fpsim-0.28.1/fpsim/scenarios.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim/settings.py` & `fpsim-0.28.1/fpsim/settings.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/fpsim.egg-info/PKG-INFO` & `fpsim-0.28.1/fpsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpsim
-Version: 0.22.0
+Version: 0.28.1
 Summary: FPsim: Family Planning Simulator
 Home-page: http://fpsim.org
 Author: Michelle O'Brien, Annie Valente, Cliff Kerr, Sam Buxton, Daniel Klein, Marita Zimmermann
 Author-email: info@fpsim.org
 Keywords: family planning,women's health,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `fpsim-0.22.0/setup.py` & `fpsim-0.28.1/setup.py`

 * *Files identical despite different names*

### Comparing `fpsim-0.22.0/tests/README.rst` & `fpsim-0.28.1/tests/README.rst`

 * *Files identical despite different names*

