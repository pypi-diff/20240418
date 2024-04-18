# Comparing `tmp/psrdb-3.0.4.tar.gz` & `tmp/psrdb-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psrdb-3.0.4.tar", max compression
+gzip compressed data, was "psrdb-3.0.5.tar", max compression
```

## Comparing `psrdb-3.0.4.tar` & `psrdb-3.0.5.tar`

### file list

```diff
@@ -1,38 +1,91 @@
--rw-r--r--   0        0        0    35149 2023-05-30 05:15:57.018989 psrdb-3.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-05-30 05:15:57.018989 psrdb-3.0.4/psrdb/__init__.py
--rw-r--r--   0        0        0    14969 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/data/l_band_gain_calibrators.csv
--rw-r--r--   0        0        0     3147 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/data/molonglo_phasing.txt
--rw-r--r--   0        0        0     1782 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/data/polarisation_calibrators.csv
--rw-r--r--   0        0        0     5680 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/data/s_band_gain_calibrators.csv
--rw-r--r--   0        0        0     5441 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/data/uhf_band_gain_calibrators.csv
--rw-r--r--   0        0        0     2758 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/graphql_client.py
--rw-r--r--   0        0        0     9962 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/graphql_table.py
--rw-r--r--   0        0        0      924 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/load_data.py
--rw-r--r--   0        0        0        0 2023-06-02 01:54:24.872472 psrdb-3.0.4/psrdb/scripts/__init__.py
--rw-r--r--   0        0        0     6338 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/scripts/generate_meerkat_json.py
--rw-r--r--   0        0        0     3764 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/scripts/generate_molonglo_json.py
--rwxr-xr-x   0        0        0     4446 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/scripts/ingest_obs.py
--rwxr-xr-x   0        0        0     2613 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/scripts/psrdb.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.331662 psrdb-3.0.4/psrdb/tables/__init__.py
--rw-r--r--   0        0        0     6182 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/calibration.py
--rw-r--r--   0        0        0    10082 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/ephemeris.py
--rw-r--r--   0        0        0     5761 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/main_project.py
--rw-r--r--   0        0        0    31384 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/tables/observation.py
--rw-r--r--   0        0        0     4779 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/pipeline_image.py
--rw-r--r--   0        0        0    17605 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/pipeline_run.py
--rw-r--r--   0        0        0     7390 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/project.py
--rw-r--r--   0        0        0     6119 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/pulsar.py
--rw-r--r--   0        0        0     7640 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/pulsar_fold_result.py
--rw-r--r--   0        0        0     6381 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/tables/residual.py
--rw-r--r--   0        0        0     5190 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/telescope.py
--rw-r--r--   0        0        0     5419 2023-11-16 01:56:57.828868 psrdb-3.0.4/psrdb/tables/template.py
--rw-r--r--   0        0        0    14872 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/tables/toa.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.335662 psrdb-3.0.4/psrdb/utils/__init__.py
--rw-r--r--   0        0        0     2345 2023-11-07 08:06:35.143673 psrdb-3.0.4/psrdb/utils/ephemeris.py
--rw-r--r--   0        0        0     5879 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/utils/header.py
--rw-r--r--   0        0        0     4044 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/utils/other.py
--rw-r--r--   0        0        0     1318 2023-11-07 08:06:24.335662 psrdb-3.0.4/psrdb/utils/residual.py
--rw-r--r--   0        0        0     1396 2024-04-08 04:00:36.591981 psrdb-3.0.4/psrdb/utils/toa.py
--rw-r--r--   0        0        0      806 2024-03-21 03:33:05.768496 psrdb-3.0.4/psrdb/utils/upload.py
--rw-r--r--   0        0        0     1006 2024-04-08 04:00:36.591981 psrdb-3.0.4/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 05:15:57.018989 psrdb-3.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-30 05:15:57.018989 psrdb-3.0.5/psrdb/__init__.py
+-rw-r--r--   0        0        0    14969 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/l_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     3147 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/molonglo_phasing.txt
+-rw-r--r--   0        0        0     1782 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/polarisation_calibrators.csv
+-rw-r--r--   0        0        0     5680 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/s_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     5441 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/uhf_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     2758 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/graphql_client.py
+-rw-r--r--   0        0        0    10552 2024-04-18 06:36:18.652677 psrdb-3.0.5/psrdb/graphql_table.py
+-rw-r--r--   0        0        0      328 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5549 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/folded_observations.cpython-310.pyc
+-rw-r--r--   0        0        0     1603 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/graphql_join.cpython-310.pyc
+-rw-r--r--   0        0        0     5171 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/processed_observations.cpython-310.pyc
+-rw-r--r--   0        0        0     5954 2023-05-30 05:16:50.102246 psrdb-3.0.5/psrdb/joins/__pycache__/toaed_observations.cpython-310.pyc
+-rw-r--r--   0        0        0      924 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/load_data.py
+-rw-r--r--   0        0        0        0 2023-06-02 01:54:24.872472 psrdb-3.0.5/psrdb/scripts/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-02 03:15:49.753919 psrdb-3.0.5/psrdb/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5405 2023-12-07 08:15:08.840488 psrdb-3.0.5/psrdb/scripts/__pycache__/generate_molonglo_json.cpython-310.pyc
+-rw-r--r--   0        0        0     3611 2023-06-15 01:57:40.726904 psrdb-3.0.5/psrdb/scripts/__pycache__/ingest_obs.cpython-310.pyc
+-rw-r--r--   0        0        0     2182 2023-11-07 08:08:02.995828 psrdb-3.0.5/psrdb/scripts/__pycache__/psrdb.cpython-310.pyc
+-rw-r--r--   0        0        0     6338 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/scripts/generate_meerkat_json.py
+-rw-r--r--   0        0        0     3764 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/scripts/generate_molonglo_json.py
+-rwxr-xr-x   0        0        0     4446 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/scripts/ingest_obs.py
+-rwxr-xr-x   0        0        0     2613 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/scripts/psrdb.py
+-rw-r--r--   0        0        0        0 2023-11-07 08:06:24.331662 psrdb-3.0.5/psrdb/tables/__init__.py
+-rw-r--r--   0        0        0      139 2023-11-07 08:07:03.843712 psrdb-3.0.5/psrdb/tables/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4745 2023-08-30 02:33:29.094412 psrdb-3.0.5/psrdb/tables/__pycache__/basebandings.cpython-310.pyc
+-rw-r--r--   0        0        0     6244 2024-04-18 06:41:23.569219 psrdb-3.0.5/psrdb/tables/__pycache__/calibration.cpython-310.pyc
+-rw-r--r--   0        0        0     4786 2023-08-30 02:33:29.194416 psrdb-3.0.5/psrdb/tables/__pycache__/calibrations.cpython-310.pyc
+-rw-r--r--   0        0        0     4616 2023-08-30 02:33:29.198416 psrdb-3.0.5/psrdb/tables/__pycache__/collections.cpython-310.pyc
+-rw-r--r--   0        0        0     7794 2023-08-30 02:33:29.202416 psrdb-3.0.5/psrdb/tables/__pycache__/ephemerides.cpython-310.pyc
+-rw-r--r--   0        0        0     8683 2024-04-18 06:41:23.541219 psrdb-3.0.5/psrdb/tables/__pycache__/ephemeris.cpython-310.pyc
+-rw-r--r--   0        0        0     5806 2023-08-30 02:33:29.202416 psrdb-3.0.5/psrdb/tables/__pycache__/filterbankings.cpython-310.pyc
+-rw-r--r--   0        0        0     6196 2023-08-30 02:33:29.206416 psrdb-3.0.5/psrdb/tables/__pycache__/foldings.cpython-310.pyc
+-rw-r--r--   0        0        0     4823 2023-08-30 02:33:29.194416 psrdb-3.0.5/psrdb/tables/__pycache__/graphql_query.cpython-310.pyc
+-rw-r--r--   0        0        0     9172 2023-08-30 02:33:29.102413 psrdb-3.0.5/psrdb/tables/__pycache__/graphql_table.cpython-310.pyc
+-rw-r--r--   0        0        0     6152 2023-08-30 02:33:29.206416 psrdb-3.0.5/psrdb/tables/__pycache__/instrumentconfigs.cpython-310.pyc
+-rw-r--r--   0        0        0     5325 2023-08-30 02:33:29.210417 psrdb-3.0.5/psrdb/tables/__pycache__/launches.cpython-310.pyc
+-rw-r--r--   0        0        0     5806 2024-04-18 06:41:23.517219 psrdb-3.0.5/psrdb/tables/__pycache__/main_project.cpython-310.pyc
+-rw-r--r--   0        0        0    20905 2024-04-18 06:41:23.581219 psrdb-3.0.5/psrdb/tables/__pycache__/observation.cpython-310.pyc
+-rw-r--r--   0        0        0     9723 2023-08-30 02:33:29.214417 psrdb-3.0.5/psrdb/tables/__pycache__/observations.cpython-310.pyc
+-rw-r--r--   0        0        0     4708 2024-04-18 06:41:23.701220 psrdb-3.0.5/psrdb/tables/__pycache__/pipeline_image.cpython-310.pyc
+-rw-r--r--   0        0        0    13575 2024-04-18 06:41:23.669220 psrdb-3.0.5/psrdb/tables/__pycache__/pipeline_run.cpython-310.pyc
+-rw-r--r--   0        0        0     5962 2023-08-30 02:33:29.218417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelinefiles.cpython-310.pyc
+-rw-r--r--   0        0        0     5962 2023-08-30 02:33:29.214417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelineimages.cpython-310.pyc
+-rw-r--r--   0        0        0     5800 2023-08-30 02:33:29.218417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelines.cpython-310.pyc
+-rw-r--r--   0        0        0     4960 2023-08-30 02:33:29.222417 psrdb-3.0.5/psrdb/tables/__pycache__/processingcollections.cpython-310.pyc
+-rw-r--r--   0        0        0     7283 2023-08-30 02:33:29.222417 psrdb-3.0.5/psrdb/tables/__pycache__/processings.cpython-310.pyc
+-rw-r--r--   0        0        0     4694 2023-08-30 02:33:29.226417 psrdb-3.0.5/psrdb/tables/__pycache__/programs.cpython-310.pyc
+-rw-r--r--   0        0        0     7073 2024-04-18 06:41:23.529219 psrdb-3.0.5/psrdb/tables/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5641 2023-08-30 02:33:29.226417 psrdb-3.0.5/psrdb/tables/__pycache__/projects.cpython-310.pyc
+-rw-r--r--   0        0        0     5982 2023-11-16 01:57:19.167220 psrdb-3.0.5/psrdb/tables/__pycache__/pulsar.cpython-310.pyc
+-rw-r--r--   0        0        0     5588 2024-04-18 06:41:23.689220 psrdb-3.0.5/psrdb/tables/__pycache__/pulsar_fold_result.cpython-310.pyc
+-rw-r--r--   0        0        0     4654 2023-08-30 02:33:29.230417 psrdb-3.0.5/psrdb/tables/__pycache__/pulsars.cpython-310.pyc
+-rw-r--r--   0        0        0     5117 2023-08-30 02:33:29.230417 psrdb-3.0.5/psrdb/tables/__pycache__/pulsartargets.cpython-310.pyc
+-rw-r--r--   0        0        0     5476 2024-04-18 06:41:23.741220 psrdb-3.0.5/psrdb/tables/__pycache__/residual.cpython-310.pyc
+-rw-r--r--   0        0        0     5747 2023-08-30 02:33:29.234418 psrdb-3.0.5/psrdb/tables/__pycache__/sessions.cpython-310.pyc
+-rw-r--r--   0        0        0     4670 2023-08-30 02:33:29.234418 psrdb-3.0.5/psrdb/tables/__pycache__/targets.cpython-310.pyc
+-rw-r--r--   0        0        0     5339 2024-04-18 06:41:23.509219 psrdb-3.0.5/psrdb/tables/__pycache__/telescope.cpython-310.pyc
+-rw-r--r--   0        0        0     4223 2023-08-30 02:33:29.238417 psrdb-3.0.5/psrdb/tables/__pycache__/telescopes.cpython-310.pyc
+-rw-r--r--   0        0        0     4965 2024-04-18 06:41:23.553219 psrdb-3.0.5/psrdb/tables/__pycache__/template.cpython-310.pyc
+-rw-r--r--   0        0        0     7037 2023-08-30 02:33:29.242418 psrdb-3.0.5/psrdb/tables/__pycache__/templates.cpython-310.pyc
+-rw-r--r--   0        0        0    12044 2024-04-18 06:41:23.717220 psrdb-3.0.5/psrdb/tables/__pycache__/toa.cpython-310.pyc
+-rw-r--r--   0        0        0     7754 2023-08-30 02:33:29.242418 psrdb-3.0.5/psrdb/tables/__pycache__/toas.cpython-310.pyc
+-rw-r--r--   0        0        0     6182 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/calibration.py
+-rw-r--r--   0        0        0    10082 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/ephemeris.py
+-rw-r--r--   0        0        0     5761 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/main_project.py
+-rw-r--r--   0        0        0    31662 2024-04-18 06:36:18.652677 psrdb-3.0.5/psrdb/tables/observation.py
+-rw-r--r--   0        0        0     4779 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pipeline_image.py
+-rw-r--r--   0        0        0    17605 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pipeline_run.py
+-rw-r--r--   0        0        0     7390 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/project.py
+-rw-r--r--   0        0        0     6119 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pulsar.py
+-rw-r--r--   0        0        0     7640 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pulsar_fold_result.py
+-rw-r--r--   0        0        0     6381 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/tables/residual.py
+-rw-r--r--   0        0        0     5190 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/telescope.py
+-rw-r--r--   0        0        0     5419 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/template.py
+-rw-r--r--   0        0        0    15643 2024-04-18 06:36:18.656677 psrdb-3.0.5/psrdb/tables/toa.py
+-rw-r--r--   0        0        0        0 2023-11-07 08:06:24.335662 psrdb-3.0.5/psrdb/utils/__init__.py
+-rw-r--r--   0        0        0      138 2023-11-07 08:07:05.091714 psrdb-3.0.5/psrdb/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3994 2023-12-07 08:15:08.880487 psrdb-3.0.5/psrdb/utils/__pycache__/header.cpython-310.pyc
+-rw-r--r--   0        0        0     3554 2024-04-18 06:41:23.497219 psrdb-3.0.5/psrdb/utils/__pycache__/other.cpython-310.pyc
+-rw-r--r--   0        0        0     1191 2023-11-07 08:08:03.863830 psrdb-3.0.5/psrdb/utils/__pycache__/residual.cpython-310.pyc
+-rw-r--r--   0        0        0     1744 2024-04-18 06:41:23.717220 psrdb-3.0.5/psrdb/utils/__pycache__/toa.cpython-310.pyc
+-rw-r--r--   0        0        0     2345 2023-11-07 08:06:35.143673 psrdb-3.0.5/psrdb/utils/ephemeris.py
+-rw-r--r--   0        0        0     5879 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/utils/header.py
+-rw-r--r--   0        0        0     4044 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/utils/other.py
+-rw-r--r--   0        0        0     1318 2023-11-07 08:06:24.335662 psrdb-3.0.5/psrdb/utils/residual.py
+-rw-r--r--   0        0        0     1944 2024-04-18 06:36:14.244686 psrdb-3.0.5/psrdb/utils/toa.py
+-rw-r--r--   0        0        0      806 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/utils/upload.py
+-rw-r--r--   0        0        0     1006 2024-04-18 06:36:18.656677 psrdb-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.5/PKG-INFO
```

### Comparing `psrdb-3.0.4/LICENSE` & `psrdb-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/data/l_band_gain_calibrators.csv` & `psrdb-3.0.5/psrdb/data/l_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/data/molonglo_phasing.txt` & `psrdb-3.0.5/psrdb/data/molonglo_phasing.txt`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/data/polarisation_calibrators.csv` & `psrdb-3.0.5/psrdb/data/polarisation_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/data/s_band_gain_calibrators.csv` & `psrdb-3.0.5/psrdb/data/s_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/data/uhf_band_gain_calibrators.csv` & `psrdb-3.0.5/psrdb/data/uhf_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/graphql_client.py` & `psrdb-3.0.5/psrdb/graphql_client.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/graphql_table.py` & `psrdb-3.0.5/psrdb/graphql_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 
 
 def generate_graphql_query(table_name, filters, conection_fields, node_fields):
     """Generate a GraphQL query for a table"""
 
     # From filter create query arguments
     arguments = []
+    argument_definitions = []
     for f in filters:
         field = f["field"]
         value = f["value"]
         if value is not None:
+            arguments.append(f'{field}: ${field}')
             if type(value) == str:
-                arguments.append(f'{field}: "{value}"')
+                argument_definitions.append(f'${field}: String')
             elif type(value) == bool:
-                arguments.append(f"{field}: {str(value).lower()}")
+                argument_definitions.append(f"${field}: Boolean")
             elif type(value) == list:
                 value_list = '","'.join(value)
-                arguments.append(f'{field}: ["{value_list}"]')
+                argument_definitions.append(f'${field}: [String]')
             else:
-                arguments.append(f"{field}: {value}")
+                argument_definitions.append(f"${field}: Int")
+    # Prepare the argument definitions to the template format
+    if len(argument_definitions) > 0:
+        argument_definitions = ',\n        '.join(argument_definitions)
+        query_argument_definitions = f"(\n        {argument_definitions}\n    )"
+    else:
+        query_argument_definitions = ""
     # Prepare the arguments to the template format
     if len(arguments) > 0:
         arguments = ',\n        '.join(arguments)
         query_arguments = f"(\n        {arguments}\n    )"
     else:
         query_arguments = ""
 
@@ -36,15 +44,15 @@
     node_fields = "\n                ".join(node_fields)
     conection_fields= "\n        ".join(conection_fields)
 
     # Convert table name to camel case to match graphql query
     query_name = to_camel_case(table_name)
 
     # Combine everything into a query
-    query = f"""query {{
+    query = f"""query {query_name} {query_argument_definitions} {{
     {query_name} {query_arguments} {{
         {conection_fields}
         edges {{
             node {{
                 {node_fields}
             }}
         }}
@@ -155,21 +163,24 @@
         has_next_page = True
         while has_next_page:
             # Append page information to input filters and fields
             filters = copy(input_filters)
             filters.append({"field": "first", "value": paginate_num})
             if cursor is not None:
                 filters.append({"field": "after", "value": cursor})
+            variables = {}
+            for f in filters:
+                variables[f["field"]] = f["value"]
 
             # Generate the query
             query = generate_graphql_query(table_name, filters, connection_fields, input_node_fields)
             self.logger.debug(f"Using query: {query}")
 
             # Send the query
-            payload = {"query": query}
+            payload = {"query": query, "variables": json.dumps(variables)}
             response = self.client.post(payload)
             has_next_page = False
             if response.status_code == 200:
                 content = json.loads(response.content)
                 self.logger.debug(f"Response content: {content}")
                 if "errors" not in content.keys():
                     data = content["data"][to_camel_case(table_name)]
```

### Comparing `psrdb-3.0.4/psrdb/load_data.py` & `psrdb-3.0.5/psrdb/load_data.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/scripts/generate_meerkat_json.py` & `psrdb-3.0.5/psrdb/scripts/generate_meerkat_json.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/scripts/generate_molonglo_json.py` & `psrdb-3.0.5/psrdb/scripts/generate_molonglo_json.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/scripts/ingest_obs.py` & `psrdb-3.0.5/psrdb/scripts/ingest_obs.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/scripts/psrdb.py` & `psrdb-3.0.5/psrdb/scripts/psrdb.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/calibration.py` & `psrdb-3.0.5/psrdb/tables/calibration.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/ephemeris.py` & `psrdb-3.0.5/psrdb/tables/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/main_project.py` & `psrdb-3.0.5/psrdb/tables/main_project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/observation.py` & `psrdb-3.0.5/psrdb/tables/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
             "telescope { name }",
             "project { code }",
             "project { short }",
             "utcStart",
             "beam",
             "band",
             "duration",
+            "foldNchan",
+            "foldNbin",
+            "modeDuration"
         ]
 
     def list(
         self,
         id=None,
         pulsar_name=None,
         telescope_name=None,
@@ -218,24 +221,27 @@
             output_name += "_unprocessed"
         if incomplete:
             output_name += "_incomplete"
         output_name += ".csv"
 
         # Loop over the pulsar_fold_results and dump them as a file
         with open(output_name, "w") as f:
-            f.write("Obs ID,Pulsar Jname,UTC Start,Project Short Name,Beam #,Observing Band,Duration (s),Calibration Location\n")
+            f.write("Obs ID,Pulsar Jname,UTC Start,Project Short Name,Beam #,Observing Band,Duration (s),Mode Duration (s),Nchan,Nbin,Calibration Location\n")
             for observations_dict in observations_dicts:
                 data_line = [
                     str(decode_id(observations_dict["id"])),
                     str(observations_dict["pulsar"]["name"]),
                     str(datetime.strptime(observations_dict['utcStart'], '%Y-%m-%dT%H:%M:%S+00:00').strftime('%Y-%m-%d-%H:%M:%S')),
                     str(observations_dict["project"]["short"]),
                     str(observations_dict["beam"]),
                     str(observations_dict["band"]),
                     str(observations_dict["duration"]),
+                    str(observations_dict["modeDuration"]),
+                    str(observations_dict["foldNchan"]),
+                    str(observations_dict["foldNbin"]),
                     str(observations_dict["calibration"]["location"]),
                 ]
                 f.write(f"{','.join(data_line)}\n")
         return output_name
 
     def create(
         self,
```

### Comparing `psrdb-3.0.4/psrdb/tables/pipeline_image.py` & `psrdb-3.0.5/psrdb/tables/pipeline_image.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/pipeline_run.py` & `psrdb-3.0.5/psrdb/tables/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/project.py` & `psrdb-3.0.5/psrdb/tables/project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/pulsar.py` & `psrdb-3.0.5/psrdb/tables/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/pulsar_fold_result.py` & `psrdb-3.0.5/psrdb/tables/pulsar_fold_result.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/residual.py` & `psrdb-3.0.5/psrdb/tables/residual.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/telescope.py` & `psrdb-3.0.5/psrdb/tables/telescope.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/template.py` & `psrdb-3.0.5/psrdb/tables/template.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/tables/toa.py` & `psrdb-3.0.5/psrdb/tables/toa.py`

 * *Files 21% similar despite different names*

```diff
@@ -104,19 +104,21 @@
     def create(
         self,
         pipeline_run_id,
         project_short,
         ephemeris,
         template_id,
         toa_lines,
-        dmCorrected,
-        minimumNsubs,
-        maximumNsubs,
-        npol,
-        nchan,
+        dmCorrected=False,
+        minimumNsubs=False,
+        maximumNsubs=False,
+        allNsubs=False,
+        modeNsubs=False,
+        npol=1,
+        nchan=1,
     ):
         """Create a new Toa database object.
 
         Parameters
         ----------
         pipeline_run_id : int
             The ID of the PipelineRun database object for this Toa.
@@ -151,26 +153,30 @@
             $projectShort: String!,
             $templateId: Int!,
             $ephemerisText: String!,
             $toaLines: [String]!,
             $dmCorrected: Boolean!,
             $minimumNsubs: Boolean!,
             $maximumNsubs: Boolean!,
+            $allNsubs: Boolean!,
+            $modeNsubs: Boolean!,
             $obsNpol: Int!,
             $obsNchan: Int!,
         ) {
             createToa (input: {
                 pipelineRunId: $pipelineRunId,
                 projectShort: $projectShort,
                 templateId: $templateId,
                 ephemerisText: $ephemerisText,
                 toaLines: $toaLines,
                 dmCorrected: $dmCorrected,
                 minimumNsubs: $minimumNsubs,
                 maximumNsubs: $maximumNsubs,
+                allNsubs: $allNsubs,
+                modeNsubs: $modeNsubs,
                 obsNpol: $obsNpol,
                 obsNchan: $obsNchan,
             }) {
                 toa {
                     id,
                 }
             }
@@ -188,14 +194,16 @@
                 'projectShort': project_short,
                 'templateId': template_id,
                 'ephemerisText': ephemeris_str,
                 'toaLines': toa_chunk,
                 'dmCorrected': dmCorrected,
                 'minimumNsubs': minimumNsubs,
                 'maximumNsubs': maximumNsubs,
+                'allNsubs': allNsubs,
+                'modeNsubs': modeNsubs,
                 "obsNpol": npol,
                 "obsNchan": nchan,
             }
             responses.append(self.mutation_graphql())
         if len(responses) == 0:
             return None
         else:
@@ -233,16 +241,15 @@
     def download(
         self,
         pulsar,
         id=None,
         pipeline_run_id=None,
         project_short=None,
         dm_corrected=None,
-        minimum_nsubs=None,
-        maximum_nsubs=None,
+        nsub_type=None,
         obs_nchan=None,
         npol=None,
     ):
         """Download a file containing ToAs based on the filters.
 
         Parameters
         ----------
@@ -252,18 +259,20 @@
             Filter by the database ID, by default None
         pipeline_run_id : int, optional
             Filter by the pipeline run id, by default None
         project_short : str
             The project short name (e.g PTA).
         dm_corrected : bool, optional
             Filter by if the toa was DM corrected, by default None
-        minimum_nsubs : bool, optional
-            Filter by if the toa was generated with the minimum number of time subbands, by default None
-        maximum_nsubs : bool, optional
-            Filter by if the toa was generated with the maximum number of time subbands, by default None
+        nsub_type : str
+            The method used to calculate the number of subintegrations. The choices are:
+                "1": a single nsub,
+                "max" the maximum number of subints possible for the observation based on the S/N ratio,
+                "mode" the length of each subintegration is equal to the most common observation duration,
+                "all": all available nsubs (no time scrunching).
         obs_nchan : int, optional
             Filter by the number of channels, by default None
         npol : int
             The number of Stokes polarisations.
 
         Returns
         -------
@@ -277,34 +286,38 @@
             {"field": "pulsar", "value": pulsar},
             {"field": "pipelineRunId", "value": pipeline_run_id},
             {"field": "projectShort", "value": project_short},
             {"field": "dmCorrected", "value": dm_corrected},
             {"field": "obsNchan", "value": obs_nchan},
             {"field": "obsNpol", "value": npol},
         ]
-        if minimum_nsubs:
-            filters.append({"field": "minimumNsubs", "value": minimum_nsubs})
-        if maximum_nsubs:
-            filters.append({"field": "maximumNsubs", "value": maximum_nsubs})
+        if nsub_type == "1":
+            filters.append({"field": "minimumNsubs", "value": True})
+        if nsub_type == "max":
+            filters.append({"field": "maximumNsubs", "value": True})
+        if nsub_type == "all":
+            filters.append({"field": "allNsubs", "value": True})
+        if nsub_type == "mode":
+            filters.append({"field": "modeNsubs", "value": True})
 
         self.get_dicts = True
         toa_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names, paginate_num=10000)
 
         # Create the output name
         output_name = f"toa_{pulsar}"
         if id is not None:
             output_name += f"_id{id}"
         if pipeline_run_id is not None:
             output_name += f"_pipeline_run_id{pipeline_run_id}"
+        if project_short is not None:
+            output_name += f"_{project_short}"
         if dm_corrected is not None and dm_corrected:
             output_name += "_dm_corrected"
-        if minimum_nsubs is not None and minimum_nsubs:
-            output_name += "_minimum_nsubs"
-        if maximum_nsubs is not None and maximum_nsubs:
-            output_name += "_maximum_nsubs"
+        if nsub_type is not None:
+            output_name += f"_{nsub_type}_nsub"
         if obs_nchan is not None:
             output_name += f"_nchan{obs_nchan}"
         if npol is not None:
             output_name += f"_npol{npol}"
         output_name += ".tim"
 
         # Loop over the toas and dump them as a file
@@ -349,16 +362,15 @@
         elif args.subcommand == "download":
             return self.download(
                 args.pulsar,
                 args.id,
                 args.pipeline_run_id,
                 args.project,
                 args.dm_corrected,
-                args.minimum_nsubs,
-                args.maximum_nsubs,
+                args.nsub_type,
                 args.nchan,
                 args.npol,
             )
         else:
             raise RuntimeError(f"{args.subcommand} command is not implemented")
 
     @classmethod
@@ -396,16 +408,25 @@
         parser_list.add_argument(
             "--template", metavar="TEMPL", type=int, help="list toa matching the template id [int]"
         )
 
         # create the parser for the "download" command
         parser_download = subs.add_parser("download", help="Download TOAs for a pulsar to a .tim file")
         parser_download.add_argument("pulsar", type=str, help="Name of the pulsar [str]")
-        parser_download.add_argument("--project", type=str, help="The project short (e.g. PTA) [str]")
+        parser_download.add_argument("--project", type=str, help="The project short (e.g. PTA) [str]", required=True)
         parser_download.add_argument("--id", type=int, help="id of the toa [int]")
         parser_download.add_argument("--pipeline_run_id", type=int, help="pipeline_run_id of the toa [int]")
         parser_download.add_argument("--dm_corrected",  action="store_true", help="Return TOAs that have had their DM corrected for each observation [bool]")
-        parser_download.add_argument("--minimum_nsubs", action="store_true", help="Only use TOAs with the minimum number of subints per observation (1) [bool]")
-        parser_download.add_argument("--maximum_nsubs", action="store_true", help="Only use TOAs with the maximum number of subints per observation (can be 1 but is often more) [bool]")
+        parser_download.add_argument(
+            '--nsub_type',
+            type=str,
+            choices=['1', 'max', 'mode', 'all'],
+            required=True,
+            help='The method used to calculate the number of subintegrations. The choices are: '
+                '"1": a single nsub, '
+                '"max" the maximum number of subints possible for the observation based on the S/N ratio, '
+                '"mode" the length of each subintegration is equal to the most common observation duration, '
+                '"all": all available nsubs (no time scrunching).'
+        )
         parser_download.add_argument("--nchan", type=int, help="Only use TOAs with this many subchans (common values are 1,4 and 16) [int]", required=True)
         parser_download.add_argument("--npol", type=int, help="Only use TOAs with this many stokes polarisations (4 for all and 1 for summed) [int]", required=True)
```

### Comparing `psrdb-3.0.4/psrdb/utils/ephemeris.py` & `psrdb-3.0.5/psrdb/utils/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/utils/header.py` & `psrdb-3.0.5/psrdb/utils/header.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/utils/other.py` & `psrdb-3.0.5/psrdb/utils/other.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/utils/residual.py` & `psrdb-3.0.5/psrdb/utils/residual.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/psrdb/utils/toa.py` & `psrdb-3.0.5/psrdb/utils/toa.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from decimal import Decimal, getcontext
 
+def format_float(value, threshold=1e3, decimal_places=2):
+    if abs(value) >= threshold:
+        e_format = "{:.{}e}".format(value, decimal_places)
+        return e_format.replace("0e", "e").replace("0e", "e").replace(".e", "e")  # remove trailing zeros
+    else:
+        return f"{value}"
+
+
 def toa_line_to_dict(toa_line):
     """
     Parse a single line from a .toa file.
 
     Args:
         toa_line (str): A line from a .toa file.
 
@@ -23,23 +31,30 @@
 
     for toa_arg in toa_args[1:]:
         arg, value = toa_arg.split()
         toa_dict[arg] = value
 
     return toa_dict
 
+
 def toa_dict_to_line(toa_dict):
     """
     Convert a dictionary to a line in a .toa file.
 
     Args:
         toa_dict (dict): A dictionary containing the parsed values.
 
     Returns:
         str: A line from a .toa file.
     """
     toa_line = ""
-    toa_line += f"{toa_dict['archive']} {toa_dict['freq_MHz']:.6f} {toa_dict['mjd']}{toa_dict['mjd_err']:>8.3f}  {toa_dict['telescope']} "
+    telescope = toa_dict['telescope']
+    if telescope == "meerkat":
+        telescope = " meerkat "
+    toa_line += f"{toa_dict['archive']} {toa_dict['freq_MHz']:.6f} {toa_dict['mjd']} {toa_dict['mjd_err']:>7.3f} {telescope}"  # noqa: E501
     for key, value in toa_dict.items():
-        if key not in ["archive", "freq_MHz", "mjd", "mjd_err", "telescope"] and value is not None:
-            toa_line += f" -{key} {value}"
+        if key not in ["archive", "freq_MHz", "mjd", "mjd_err", "telescope"]:
+            if isinstance(value, float) and key == "gof":
+                toa_line += f" -{key} {format_float(value, threshold=1e3, decimal_places=2)}"
+            else:
+                toa_line += f" -{key} {value}"
     return toa_line
```

### Comparing `psrdb-3.0.4/psrdb/utils/upload.py` & `psrdb-3.0.5/psrdb/utils/upload.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.4/pyproject.toml` & `psrdb-3.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psrdb"
-version = "3.0.4"
+version = "3.0.5"
 description = "CLI for pulsars.org.au"
 authors = ["GWDC"]
 license = "MIT"
 packages = [{include = "psrdb"}]
 include = ["psrdb/data/molonglo_phasing.txt"]
 
 [tool.poetry.scripts]
```

### Comparing `psrdb-3.0.4/PKG-INFO` & `psrdb-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrdb
-Version: 3.0.4
+Version: 3.0.5
 Summary: CLI for pulsars.org.au
 License: MIT
 Author: GWDC
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

