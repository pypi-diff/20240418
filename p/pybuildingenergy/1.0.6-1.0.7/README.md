# Comparing `tmp/pybuildingenergy-1.0.6.tar.gz` & `tmp/pybuildingenergy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuildingenergy-1.0.6.tar", last modified: Thu Apr  4 20:52:03 2024, max compression
+gzip compressed data, was "pybuildingenergy-1.0.7.tar", last modified: Thu Apr 18 14:29:45 2024, max compression
```

## Comparing `pybuildingenergy-1.0.6.tar` & `pybuildingenergy-1.0.7.tar`

### file list

```diff
@@ -1,98 +1,126 @@
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.914608 pybuildingenergy-1.0.6/
--rw-r--r--   0 dantonucci   (501) staff       (20)      262 2024-03-27 07:15:14.000000 pybuildingenergy-1.0.6/AUTHORS.rst
--rw-r--r--   0 dantonucci   (501) staff       (20)     1500 2024-03-26 10:34:21.000000 pybuildingenergy-1.0.6/CONTRIBUTING.rst
--rw-r--r--   0 dantonucci   (501) staff       (20)      164 2024-03-27 11:27:34.000000 pybuildingenergy-1.0.6/HISTORY.rst
--rw-r--r--   0 dantonucci   (501) staff       (20)     1076 2024-02-22 11:09:38.000000 pybuildingenergy-1.0.6/LICENSE.md
--rw-r--r--   0 dantonucci   (501) staff       (20)      130 2024-03-26 10:59:05.000000 pybuildingenergy-1.0.6/MANIFEST.in
--rw-r--r--   0 dantonucci   (501) staff       (20)    19781 2024-04-04 20:52:03.914469 pybuildingenergy-1.0.6/PKG-INFO
--rw-r--r--   0 dantonucci   (501) staff       (20)    16266 2024-04-04 20:51:35.000000 pybuildingenergy-1.0.6/README.rst
--rw-r--r--   0 dantonucci   (501) staff       (20)     2285 2024-04-04 20:49:04.000000 pybuildingenergy-1.0.6/pyproject.toml
--rw-r--r--   0 dantonucci   (501) staff       (20)     1066 2024-04-04 20:52:03.914969 pybuildingenergy-1.0.6/setup.cfg
--rw-r--r--   0 dantonucci   (501) staff       (20)     1219 2024-03-27 11:24:50.000000 pybuildingenergy-1.0.6/setup.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.807237 pybuildingenergy-1.0.6/src/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.811998 pybuildingenergy-1.0.6/src/pybuildingenergy/
--rw-r--r--   0 dantonucci   (501) staff       (20)      263 2024-03-19 14:52:33.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/__init__.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.814309 pybuildingenergy-1.0.6/src/pybuildingenergy/data/
--rw-r--r--   0 dantonucci   (501) staff       (20)    23766 2024-03-22 13:12:10.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/data/building_archetype.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    24930 2024-03-22 22:29:48.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/data/create_archetype.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     1835 2024-03-14 15:35:13.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/data/profiles.py
--rw-r--r--   0 dantonucci   (501) staff       (20)      314 2024-03-14 11:42:18.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/global_inputs.py
--rw-r--r--   0 dantonucci   (501) staff       (20)      141 2024-03-25 17:32:54.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/pybuildingenergy.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.818187 pybuildingenergy-1.0.6/src/pybuildingenergy/source/
--rw-r--r--   0 dantonucci   (501) staff       (20)       39 2024-03-19 14:52:33.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/__init__.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    11891 2024-04-03 12:16:51.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/calibration.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     9750 2024-04-03 09:16:07.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/calibration_NSGI.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    18020 2024-03-26 14:31:25.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/functions.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    24007 2024-03-26 14:30:13.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/graphs.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    85208 2024-04-03 12:00:12.000000 pybuildingenergy-1.0.6/src/pybuildingenergy/source/utils.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.913804 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/
--rw-r--r--   0 dantonucci   (501) staff       (20)    19781 2024-04-04 20:52:03.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/PKG-INFO
--rw-r--r--   0 dantonucci   (501) staff       (20)     3366 2024-04-04 20:52:03.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/SOURCES.txt
--rw-r--r--   0 dantonucci   (501) staff       (20)        1 2024-04-04 20:52:03.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/dependency_links.txt
--rw-r--r--   0 dantonucci   (501) staff       (20)        1 2024-03-26 11:17:54.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/not-zip-safe
--rw-r--r--   0 dantonucci   (501) staff       (20)      298 2024-04-04 20:52:03.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/requires.txt
--rw-r--r--   0 dantonucci   (501) staff       (20)       17 2024-04-04 20:52:03.000000 pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/top_level.txt
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.821228 pybuildingenergy-1.0.6/tests/
--rw-r--r--   0 dantonucci   (501) staff       (20)       46 2024-02-22 11:09:38.000000 pybuildingenergy-1.0.6/tests/__init__.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.822457 pybuildingenergy-1.0.6/tests/input_data/
--rw-rw-r--   0 dantonucci   (501) staff       (20)        0 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/__init__.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.823115 pybuildingenergy-1.0.6/tests/input_data/__pycache__/
--rw-r--r--   0 dantonucci   (501) staff       (20)      256 2024-03-25 15:39:11.000000 pybuildingenergy-1.0.6/tests/input_data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dantonucci   (501) staff       (20)     1497 2024-03-25 15:39:11.000000 pybuildingenergy-1.0.6/tests/input_data/__pycache__/src.cpython-311.pyc
--rw-r--r--   0 dantonucci   (501) staff       (20)     3748 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/archetype.py
--rw-r--r--   0 dantonucci   (501) staff       (20)    15584 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/archetypes.pickle
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.862059 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/
--rw-rw-r--   0 dantonucci   (501) staff       (20)    35029 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0.idf
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2940690 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Athens.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2904036 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Berlin.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2917369 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Bolzano.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2937801 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2937665 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver2.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2950185 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Madrid.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2920285 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Milan.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  2910501 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Stockholm.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  3100099 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/eplusout.csv
--rw-r--r--   0 dantonucci   (501) staff       (20)      761 2024-03-25 15:25:33.000000 pybuildingenergy-1.0.6/tests/input_data/src.py
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.906480 pybuildingenergy-1.0.6/tests/input_data/weatherdata/
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1594906 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Athens.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1587046 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Berlin.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1582490 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Madrid.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1584636 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Milan.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1584260 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Stockholm.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)   585391 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1864148 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)   575738 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1856268 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)   574988 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1858021 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)   586704 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.csv
--rw-rw-r--   0 dantonucci   (501) staff       (20)  1863968 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.epw
--rw-rw-r--   0 dantonucci   (501) staff       (20)   585133 2024-03-25 15:13:53.000000 pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_52.496_13.414_2005_2020.csv
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.809004 pybuildingenergy-1.0.6/tests/snapshots/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.909640 pybuildingenergy-1.0.6/tests/snapshots/__pycache__/
--rw-r--r--   0 dantonucci   (501) staff       (20)     6210 2024-03-22 21:59:39.000000 pybuildingenergy-1.0.6/tests/snapshots/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.808235 pybuildingenergy-1.0.6/tests/snapshots/test_create_bui_obj/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.910122 pybuildingenergy-1.0.6/tests/snapshots/test_create_bui_obj/test_create_bui_obj/
--rw-r--r--   0 dantonucci   (501) staff       (20)     2413 2024-03-22 21:45:52.000000 pybuildingenergy-1.0.6/tests/snapshots/test_create_bui_obj/test_create_bui_obj/properties_inputs.yml
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.808425 pybuildingenergy-1.0.6/tests/snapshots/test_create_report/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.910550 pybuildingenergy-1.0.6/tests/snapshots/test_create_report/test_plotting_report/
--rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-03-26 09:57:23.000000 pybuildingenergy-1.0.6/tests/snapshots/test_create_report/test_plotting_report/report_generated.yml
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.808639 pybuildingenergy-1.0.6/tests/snapshots/test_simul_newbui_from_archetype/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.910841 pybuildingenergy-1.0.6/tests/snapshots/test_simul_newbui_from_archetype/test_new_bui_from_archetype/
--rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-03-26 09:40:16.000000 pybuildingenergy-1.0.6/tests/snapshots/test_simul_newbui_from_archetype/test_new_bui_from_archetype/report_new_bui_from_archetype_generated.yml
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.808795 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_archetype/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.911125 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_archetype/test_simulate_archetype/
--rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-03-22 22:25:27.000000 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_archetype/test_simulate_archetype/report_from_archetype_generated.yml
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.808925 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_besttest/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.911435 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_besttest/test_best600/
--rw-r--r--   0 dantonucci   (501) staff       (20)     1065 2024-03-25 15:37:10.000000 pybuildingenergy-1.0.6/tests/snapshots/test_simulate_besttest/test_best600/data_best600_athens.json
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.809083 pybuildingenergy-1.0.6/tests/snapshots/test_simulation_new_bui/
-drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-04 20:52:03.912001 pybuildingenergy-1.0.6/tests/snapshots/test_simulation_new_bui/test_simulation/
--rw-r--r--   0 dantonucci   (501) staff       (20)      139 2024-03-20 16:29:41.000000 pybuildingenergy-1.0.6/tests/snapshots/test_simulation_new_bui/test_simulation/annual_results_df.json
--rw-r--r--   0 dantonucci   (501) staff       (20)   977784 2024-03-20 16:29:41.000000 pybuildingenergy-1.0.6/tests/snapshots/test_simulation_new_bui/test_simulation/hourly_sim.json
--rw-r--r--   0 dantonucci   (501) staff       (20)     3506 2024-03-22 14:41:43.000000 pybuildingenergy-1.0.6/tests/test_create_bui_obj.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     3884 2024-03-25 15:55:52.000000 pybuildingenergy-1.0.6/tests/test_create_report.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     5249 2024-03-26 10:10:01.000000 pybuildingenergy-1.0.6/tests/test_simul_newbui_from_archetype.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     2757 2024-03-26 10:10:01.000000 pybuildingenergy-1.0.6/tests/test_simulate_archetype.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     4991 2024-03-26 14:30:53.000000 pybuildingenergy-1.0.6/tests/test_simulate_besttest.py
--rw-r--r--   0 dantonucci   (501) staff       (20)     3695 2024-03-22 21:47:33.000000 pybuildingenergy-1.0.6/tests/test_simulation_new_bui.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.108615 pybuildingenergy-1.0.7/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      264 2024-04-11 12:42:55.000000 pybuildingenergy-1.0.7/AUTHORS.rst
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1500 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 dantonucci   (501) staff       (20)      164 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/HISTORY.rst
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1076 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/LICENSE.md
+-rw-r--r--   0 dantonucci   (501) staff       (20)      130 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/MANIFEST.in
+-rw-r--r--   0 dantonucci   (501) staff       (20)    20795 2024-04-18 14:29:45.108496 pybuildingenergy-1.0.7/PKG-INFO
+-rw-r--r--   0 dantonucci   (501) staff       (20)    17215 2024-04-18 14:05:44.000000 pybuildingenergy-1.0.7/README.rst
+-rw-r--r--   0 dantonucci   (501) staff       (20)     2333 2024-04-18 13:51:55.000000 pybuildingenergy-1.0.7/pyproject.toml
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1066 2024-04-18 14:29:45.108962 pybuildingenergy-1.0.7/setup.cfg
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1219 2024-04-18 14:05:57.000000 pybuildingenergy-1.0.7/setup.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.913303 pybuildingenergy-1.0.7/src/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.918141 pybuildingenergy-1.0.7/src/pybuildingenergy/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      263 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/__init__.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.919722 pybuildingenergy-1.0.7/src/pybuildingenergy/data/
+-rw-r--r--   0 dantonucci   (501) staff       (20)    23766 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/data/building_archetype.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)      395 2024-04-18 12:56:08.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/global_inputs.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)      141 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/pybuildingenergy.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.921682 pybuildingenergy-1.0.7/src/pybuildingenergy/source/
+-rw-r--r--   0 dantonucci   (501) staff       (20)    15970 2024-04-18 12:57:12.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/source/DHW.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)       39 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/source/__init__.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)    18040 2024-04-17 18:14:41.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/source/functions.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)    24007 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/source/graphs.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)    85246 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/src/pybuildingenergy/source/utils.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.107832 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/
+-rw-r--r--   0 dantonucci   (501) staff       (20)    20795 2024-04-18 14:29:44.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/PKG-INFO
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4723 2024-04-18 14:29:44.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/SOURCES.txt
+-rw-r--r--   0 dantonucci   (501) staff       (20)        1 2024-04-18 14:29:44.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/dependency_links.txt
+-rw-r--r--   0 dantonucci   (501) staff       (20)        1 2024-04-18 12:20:55.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/not-zip-safe
+-rw-r--r--   0 dantonucci   (501) staff       (20)      333 2024-04-18 14:29:44.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/requires.txt
+-rw-r--r--   0 dantonucci   (501) staff       (20)       17 2024-04-18 14:29:44.000000 pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/top_level.txt
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.924302 pybuildingenergy-1.0.7/tests/
+-rw-r--r--   0 dantonucci   (501) staff       (20)       46 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/__init__.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.927005 pybuildingenergy-1.0.7/tests/__pycache__/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      289 2024-04-18 12:44:37.000000 pybuildingenergy-1.0.7/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4443 2024-04-18 13:33:02.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_create_bui_obj.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4925 2024-04-18 14:06:41.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_create_report.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4171 2024-04-18 13:09:39.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_dhw.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     6693 2024-04-18 13:33:03.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_simul_newbui_from_archetype.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     3738 2024-04-18 13:39:30.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_simulate_archetype.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     6478 2024-04-18 14:06:41.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4753 2024-04-18 13:50:01.000000 pybuildingenergy-1.0.7/tests/__pycache__/test_simulation_new_bui.cpython-311-pytest-6.2.4.pyc
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.929468 pybuildingenergy-1.0.7/tests/input_data/
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10931 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10902 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Athens.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10907 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Berlin.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10915 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Bolzano.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10921 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Madrid.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10926 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Milan.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10910 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Milano.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10925 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/BESTEST600_iso_vs_energyplus_Stockholm.html
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.960323 pybuildingenergy-1.0.7/tests/input_data/Result/
+-rw-r--r--   0 dantonucci   (501) staff       (20)     6431 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/Yearly_eNeed_gauge.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)      100 2024-04-18 14:22:05.000000 pybuildingenergy-1.0.7/tests/input_data/Result/annual_sim__arch.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)    34545 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/energy_signature.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)   500956 2024-04-18 14:22:05.000000 pybuildingenergy-1.0.7/tests/input_data/Result/hourly_sim__arch.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2368145 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/line_chart.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2436418 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/main_report.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2468974 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/main_report_2.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    14628 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/monthly_heating_cooling_need.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    13637 2024-04-18 14:24:17.000000 pybuildingenergy-1.0.7/tests/input_data/Result/monthly_heating_need.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2469695 2024-04-18 14:19:39.000000 pybuildingenergy-1.0.7/tests/input_data/Result/new_building_.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)    10902 2024-04-18 14:24:43.000000 pybuildingenergy-1.0.7/tests/input_data/Result/testbed600_ISO_vs_Eplus_Athens.html
+-rw-r--r--   0 dantonucci   (501) staff       (20)        0 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/__init__.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.963411 pybuildingenergy-1.0.7/tests/input_data/__pycache__/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      247 2024-04-18 13:33:03.000000 pybuildingenergy-1.0.7/tests/input_data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1488 2024-04-18 13:33:03.000000 pybuildingenergy-1.0.7/tests/input_data/__pycache__/src.cpython-311.pyc
+-rw-r--r--   0 dantonucci   (501) staff       (20)     3748 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/archetype.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)    15584 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/archetypes.pickle
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.028575 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/
+-rw-r--r--   0 dantonucci   (501) staff       (20)    35029 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0.idf
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2940690 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Athens.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2904036 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Berlin.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2917369 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Bolzano.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2937801 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2937665 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver2.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2950185 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Madrid.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2920285 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Milan.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  2910501 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Stockholm.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  3100099 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/eplusout.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)      761 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/src.py
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.097819 pybuildingenergy-1.0.7/tests/input_data/weatherdata/
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1594906 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Athens.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1587046 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Berlin.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1582490 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Madrid.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1584636 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Milan.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1584260 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Stockholm.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)   585391 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1864148 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)   575738 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1856268 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)   574988 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1858021 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)   586704 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.csv
+-rw-r--r--   0 dantonucci   (501) staff       (20)  1863968 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.epw
+-rw-r--r--   0 dantonucci   (501) staff       (20)   585133 2024-04-11 12:40:17.000000 pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_52.496_13.414_2005_2020.csv
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.915369 pybuildingenergy-1.0.7/tests/snapshots/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.914384 pybuildingenergy-1.0.7/tests/snapshots/test_create_bui_obj/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.103976 pybuildingenergy-1.0.7/tests/snapshots/test_create_bui_obj/test_create_bui_obj/
+-rw-r--r--   0 dantonucci   (501) staff       (20)     2413 2024-04-18 12:50:51.000000 pybuildingenergy-1.0.7/tests/snapshots/test_create_bui_obj/test_create_bui_obj/properties_inputs.yml
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.914579 pybuildingenergy-1.0.7/tests/snapshots/test_create_report/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.104272 pybuildingenergy-1.0.7/tests/snapshots/test_create_report/test_plotting_report/
+-rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-04-18 14:08:45.000000 pybuildingenergy-1.0.7/tests/snapshots/test_create_report/test_plotting_report/report_generated.yml
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.914765 pybuildingenergy-1.0.7/tests/snapshots/test_dhw/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.104543 pybuildingenergy-1.0.7/tests/snapshots/test_dhw/test_energy_needs/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      308 2024-04-18 13:08:07.000000 pybuildingenergy-1.0.7/tests/snapshots/test_dhw/test_energy_needs/dhw_test.yml
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.914912 pybuildingenergy-1.0.7/tests/snapshots/test_simul_newbui_from_archetype/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.104835 pybuildingenergy-1.0.7/tests/snapshots/test_simul_newbui_from_archetype/test_new_bui_from_archetype/
+-rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-04-18 13:35:12.000000 pybuildingenergy-1.0.7/tests/snapshots/test_simul_newbui_from_archetype/test_new_bui_from_archetype/report_new_bui_from_archetype_generated.yml
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.915088 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_archetype/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.105163 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_archetype/test_simulate_archetype/
+-rw-r--r--   0 dantonucci   (501) staff       (20)       21 2024-04-18 13:43:13.000000 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_archetype/test_simulate_archetype/report_from_archetype_generated.yml
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.915269 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_besttest/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.105475 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_besttest/test_best600/
+-rw-r--r--   0 dantonucci   (501) staff       (20)     1065 2024-04-18 14:14:13.000000 pybuildingenergy-1.0.7/tests/snapshots/test_simulate_besttest/test_best600/data_best600_athens.json
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:44.915444 pybuildingenergy-1.0.7/tests/snapshots/test_simulation_new_bui/
+drwxr-xr-x   0 dantonucci   (501) staff       (20)        0 2024-04-18 14:29:45.106067 pybuildingenergy-1.0.7/tests/snapshots/test_simulation_new_bui/test_simulation/
+-rw-r--r--   0 dantonucci   (501) staff       (20)      139 2024-04-18 13:57:25.000000 pybuildingenergy-1.0.7/tests/snapshots/test_simulation_new_bui/test_simulation/annual_results_df.json
+-rw-r--r--   0 dantonucci   (501) staff       (20)   977784 2024-04-18 13:57:25.000000 pybuildingenergy-1.0.7/tests/snapshots/test_simulation_new_bui/test_simulation/hourly_sim.json
+-rw-r--r--   0 dantonucci   (501) staff       (20)     3506 2024-04-18 13:32:46.000000 pybuildingenergy-1.0.7/tests/test_create_bui_obj.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     3884 2024-04-18 14:06:29.000000 pybuildingenergy-1.0.7/tests/test_create_report.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     2851 2024-04-18 13:09:16.000000 pybuildingenergy-1.0.7/tests/test_dhw.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     5249 2024-04-18 13:32:51.000000 pybuildingenergy-1.0.7/tests/test_simul_newbui_from_archetype.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     2757 2024-04-18 13:39:14.000000 pybuildingenergy-1.0.7/tests/test_simulate_archetype.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     4991 2024-04-18 14:06:22.000000 pybuildingenergy-1.0.7/tests/test_simulate_besttest.py
+-rw-r--r--   0 dantonucci   (501) staff       (20)     3695 2024-04-18 13:49:50.000000 pybuildingenergy-1.0.7/tests/test_simulation_new_bui.py
```

### Comparing `pybuildingenergy-1.0.6/CONTRIBUTING.rst` & `pybuildingenergy-1.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/LICENSE.md` & `pybuildingenergy-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/PKG-INFO` & `pybuildingenergy-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuildingenergy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Energy Simulation of building usin ISO52016 and more
 Home-page: https://github.com/EURAC-EEBgroup/pyBuildingEnergy
 Author: Daniele Antonucci
 Author-email: Daniele Antonucci <daniele.antonucci@eurac.edu>
 Maintainer-email: Daniele Antonucci <daniele.antonucci@eurac.edu>
 License: MIT License
         
@@ -63,14 +63,16 @@
 Requires-Dist: Pyarrow==13.0.0
 Requires-Dist: pyecharts==2.0.4
 Requires-Dist: geopy==2.4.1
 Requires-Dist: pvlib==0.10.1
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: pyswarms==1.3.0
+Requires-Dist: workalendar==17.0.0
+Requires-Dist: plotly==5.21.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Provides-Extra: gui
 Provides-Extra: cli
 
@@ -95,15 +97,15 @@
 
 The new EPBD recast provides an update on building performance assessment through a methodology that must take into account various aspects such as the thermal characteristics of the building, the use of energy from renewable sources, building automation and control systems, ventilation, cooling, energy recovery, etc.
 
 The methodology should represent the actual operating conditions, allow for the use of measured energy for accuracy and comparability purposes, and be based on hourly or sub-hourly intervals that take into account the variable conditions significantly impacting the operation and performance of the system, as well as internal conditions.
 The energy performance of a building shall be expressed by a numeric indicator of primary energy use per unit of reference floor area per year, in kWh/(m2.y) for the purpose of both energy performance certification and compliance with minimum energy performance requirements. Numeric indicators of final energy use per unit of reference floor area per year, in kWh/(m2.y) and of energy needs according to ISO 52000 in kWh/(m².y) shall be used. The methodology applied for the determination of the energy performance of a building shall be transparent and open to innovation and reflect best practices, in particular from additional indicators.
 Member States shall describe their national calculation methodology based on Annex A of the key European standards on energy performance of buildings, namely EN ISO 52000-1, EN ISO 52003-1, EN ISO 52010-1,EN ISO 52016-1, EN ISO 52018-1,EN 16798-1, EN 52120-1 and EN 17423 or superseding documents. This provision shall not constitute a legal codification of those standards.
 
-**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2017. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
+**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2018. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
 The actual calculation methods for the assessment of building performance are the following:
 
 - [x] the (sensible) energy need for heating and cooling, based on hourly or monthly calculations;
 
 - [ ] the latent energy need for (de-)humidification, based on hourly or monthly calculations;
 
 - [x] the internal temperature, based on hourly calculations;
@@ -113,29 +115,34 @@
 - [ ] the moisture and latent heat load for (de-)humidification, based on hourly calculations;
 
 - [ ] the design sensible heating or cooling load and design latent heat load using an hourly calculation interval;
 
 - [ ] the conditions of the supply air to provide the necessary humidification and dehumidification.
 
 The calculation methods can be used for residential or non-residential buildings, or a part of it, referred to as "the building" or the "assessed object".
-ISO 52016-1:2017 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
-ISO 52016-1:2017 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
-
+ISO 52016-1:2018 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
+ISO 52016-1:2018 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
 
 
 Weather Data
 ------------
 The tool can use wather data coming from 2 main sources:
 
 - pvgis api (https://re.jrc.ec.europa.eu/pvg_tools/en/) - PHOTOVOLTAIC GEOGRAPHICAL INFORMATION SYSTEM
 - .epw file from https://www.ladybug.tools/epwmap/
 
 More details in the example folder
 
 
+Domestic Hot Water - DHW
+------------------------
+- [x] Calculation of volume and energy need for domestic hot water according to ISO 12831-3. 
+- [] Assessment of thermal load based on the type of DHW system
+
+
 Limitations
 ------------
 The library is developed with the intent of demonstrating specific elements of calculation procedures in the relevant standards. It is not intended to replace the regulations but to complement them, as the latter are essential for understanding the calculation. 
 This library is meant to be used for demonstration and testing purposes and is therefore provided as open source, without protection against misuse or inappropriate use.
 
 The information and views set out in this document are those of the authors and do not necessarily reflect the official opinion of the European Union. Neither the European Union institutions and bodies nor any person acting on their behalf may be held responsible for the use that may be made of the information contained herein.
 
@@ -443,15 +450,15 @@
      - YES
    
 More information about coefficients are available `here <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/src/pybuildingenergy/data>`
 
 
 Documentation
 --------------
-
+Check our doc `here <https://pybuildingenergy.readthedocs.io/en/latest/>`
 
 Example
 -------
 
 Here some `Examples <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/examples>` on pybuildingenergy application.
 For more information
 .....
@@ -477,9 +484,19 @@
 Acknowledgment
 ---------------
 This work was carried out within European projects: 
 Infinite - This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 958397, 
 Moderate - Horizon Europe research and innovation programme under grant agreement No 101069834, 
 with the aim of contributing to the development of open products useful for defining plausible scenarios for the decarbonization of the built environment
 
+Reagrding the DHW Calculation: 
+The work was developed using the regulations and results obtained from the spreadsheet created by the EPBCenter.
+
+Reference
+----------
+- EN ISO 52010-1:2018 Energy performance of buildings - External climatic conditions - Part 1: Conversion of climatic data for energy calculations
+- EN ISO 52016-1:2018 Energy performance of buildings - Energy needs for heating and cooling, internal temperatures and sensible and latent heat loads 
+- EN ISO 12831-3:2018 Energy performance of buildings - Method for calculation of the design heat load - Part 3: Domestic hot water systems heat load and characterisation of needs, Module M8-2, M8-3
+
+
```

### Comparing `pybuildingenergy-1.0.6/README.rst` & `pybuildingenergy-1.0.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 The new EPBD recast provides an update on building performance assessment through a methodology that must take into account various aspects such as the thermal characteristics of the building, the use of energy from renewable sources, building automation and control systems, ventilation, cooling, energy recovery, etc.
 
 The methodology should represent the actual operating conditions, allow for the use of measured energy for accuracy and comparability purposes, and be based on hourly or sub-hourly intervals that take into account the variable conditions significantly impacting the operation and performance of the system, as well as internal conditions.
 The energy performance of a building shall be expressed by a numeric indicator of primary energy use per unit of reference floor area per year, in kWh/(m2.y) for the purpose of both energy performance certification and compliance with minimum energy performance requirements. Numeric indicators of final energy use per unit of reference floor area per year, in kWh/(m2.y) and of energy needs according to ISO 52000 in kWh/(m².y) shall be used. The methodology applied for the determination of the energy performance of a building shall be transparent and open to innovation and reflect best practices, in particular from additional indicators.
 Member States shall describe their national calculation methodology based on Annex A of the key European standards on energy performance of buildings, namely EN ISO 52000-1, EN ISO 52003-1, EN ISO 52010-1,EN ISO 52016-1, EN ISO 52018-1,EN 16798-1, EN 52120-1 and EN 17423 or superseding documents. This provision shall not constitute a legal codification of those standards.
 
-**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2017. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
+**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2018. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
 The actual calculation methods for the assessment of building performance are the following:
 
 - [x] the (sensible) energy need for heating and cooling, based on hourly or monthly calculations;
 
 - [ ] the latent energy need for (de-)humidification, based on hourly or monthly calculations;
 
 - [x] the internal temperature, based on hourly calculations;
@@ -37,29 +37,34 @@
 - [ ] the moisture and latent heat load for (de-)humidification, based on hourly calculations;
 
 - [ ] the design sensible heating or cooling load and design latent heat load using an hourly calculation interval;
 
 - [ ] the conditions of the supply air to provide the necessary humidification and dehumidification.
 
 The calculation methods can be used for residential or non-residential buildings, or a part of it, referred to as "the building" or the "assessed object".
-ISO 52016-1:2017 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
-ISO 52016-1:2017 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
-
+ISO 52016-1:2018 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
+ISO 52016-1:2018 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
 
 
 Weather Data
 ------------
 The tool can use wather data coming from 2 main sources:
 
 - pvgis api (https://re.jrc.ec.europa.eu/pvg_tools/en/) - PHOTOVOLTAIC GEOGRAPHICAL INFORMATION SYSTEM
 - .epw file from https://www.ladybug.tools/epwmap/
 
 More details in the example folder
 
 
+Domestic Hot Water - DHW
+------------------------
+- [x] Calculation of volume and energy need for domestic hot water according to ISO 12831-3. 
+- [] Assessment of thermal load based on the type of DHW system
+
+
 Limitations
 ------------
 The library is developed with the intent of demonstrating specific elements of calculation procedures in the relevant standards. It is not intended to replace the regulations but to complement them, as the latter are essential for understanding the calculation. 
 This library is meant to be used for demonstration and testing purposes and is therefore provided as open source, without protection against misuse or inappropriate use.
 
 The information and views set out in this document are those of the authors and do not necessarily reflect the official opinion of the European Union. Neither the European Union institutions and bodies nor any person acting on their behalf may be held responsible for the use that may be made of the information contained herein.
 
@@ -367,15 +372,15 @@
      - YES
    
 More information about coefficients are available `here <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/src/pybuildingenergy/data>`
 
 
 Documentation
 --------------
-
+Check our doc `here <https://pybuildingenergy.readthedocs.io/en/latest/>`
 
 Example
 -------
 
 Here some `Examples <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/examples>` on pybuildingenergy application.
 For more information
 .....
@@ -401,9 +406,19 @@
 Acknowledgment
 ---------------
 This work was carried out within European projects: 
 Infinite - This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 958397, 
 Moderate - Horizon Europe research and innovation programme under grant agreement No 101069834, 
 with the aim of contributing to the development of open products useful for defining plausible scenarios for the decarbonization of the built environment
 
+Reagrding the DHW Calculation: 
+The work was developed using the regulations and results obtained from the spreadsheet created by the EPBCenter.
+
+Reference
+----------
+- EN ISO 52010-1:2018 Energy performance of buildings - External climatic conditions - Part 1: Conversion of climatic data for energy calculations
+- EN ISO 52016-1:2018 Energy performance of buildings - Energy needs for heating and cooling, internal temperatures and sensible and latent heat loads 
+- EN ISO 12831-3:2018 Energy performance of buildings - Method for calculation of the design heat load - Part 3: Domestic hot water systems heat load and characterisation of needs, Module M8-2, M8-3
+
+
```

### Comparing `pybuildingenergy-1.0.6/pyproject.toml` & `pybuildingenergy-1.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Ignore flat-layout.
 [tool.setuptools]
 py-modules = []
 
 [project]
 name = "pybuildingenergy"
-version = "1.0.6"
+version = "1.0.7"
 description = "Energy Simulation of building usin ISO52016 and more"
 license = {file = "LICENSE.md"}
 readme = "README.rst"
 requires-python = ">=3.8.0"
 authors = [{name = "Daniele Antonucci", email = "daniele.antonucci@eurac.edu"}]
 maintainers = [{name = "Daniele Antonucci", email = "daniele.antonucci@eurac.edu"}]
 keywords = [
@@ -36,14 +36,16 @@
     "Pyarrow==13.0.0",
     "pyecharts==2.0.4",
     "geopy==2.4.1",
     "pvlib==0.10.1",
     "scikit-learn>=1.3.2",
     "urllib3==1.26.18",
     "pyswarms==1.3.0",
+    "workalendar==17.0.0",
+    "plotly==5.21.0"
 ]
 
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
```

### Comparing `pybuildingenergy-1.0.6/setup.cfg` & `pybuildingenergy-1.0.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybuildingenergy
-version = 1.0.6
+version = 1.0.7
 description = library to simulate builiding performance
 author = Daniele antonucci
 author_email = daniele.antonucci@eurac.edu
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `pybuildingenergy-1.0.6/setup.py` & `pybuildingenergy-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             author_email='daniele.antonucci@eurac.edu',
             description="Energy simulation of the building using ISO52000",
             long_description=open('README.rst').read(),
             long_description_content_type='text/markdown',
             include_package_data=True,
             keywords='pybuildingenergy',
             url='https://github.com/EURAC-EEBgroup/pyBuildingEnergy',
-            version='1.0.5',
+            version='1.0.7',
         )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
```

### Comparing `pybuildingenergy-1.0.6/src/pybuildingenergy/data/building_archetype.py` & `pybuildingenergy-1.0.7/src/pybuildingenergy/data/building_archetype.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/src/pybuildingenergy/source/graphs.py` & `pybuildingenergy-1.0.7/src/pybuildingenergy/source/graphs.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/src/pybuildingenergy/source/utils.py` & `pybuildingenergy-1.0.7/src/pybuildingenergy/source/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# __author__ = "Daniele Antonucci, Ulrich Filippi Oberagger, Olga Somova"
-# __credits__ = ["Daniele Antonucci", "Ulrich FIlippi Oberagger", "Olga Somova"]
+# __author__ = "Daniele Antonucci, Ulrich Filippi Oberegger, Olga Somova"
+# __credits__ = ["Daniele Antonucci", "Ulrich FIlippi Oberegger", "Olga Somova"]
 # __license__ = "MIT"
 # __version__ = "0.1"
 # __maintainer__ = "Daniele Antonucci"
 
 import requests
 import pandas as pd
 import datetime as dt
@@ -1598,15 +1598,17 @@
                 if Theta_C_set > 995:
                     power_cooling_max_act = 0
                 else:
                     power_cooling_max_act = building_object.__getattribute__(
                         "power_cooling_max"
                     )
 
-                Phi_HC_nd_calc[0] = 0  # the load has three values:  0 no heating e no cooling, 1  heating, 2 cooling
+                Phi_HC_nd_calc[
+                    0
+                ] = 0  # the load has three values:  0 no heating e no cooling, 1  heating, 2 cooling
                 if power_heating_max_act == 0 and power_cooling_max_act == 0:  #
                     nrHCmodes = 1
                 elif power_cooling_max_act == 0:
                     colB_H = 1
                     nrHCmodes = 2
                     Phi_HC_nd_calc[colB_H] = power_heating_max_act
                 elif power_heating_max_act == 0:
```

### Comparing `pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/PKG-INFO` & `pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuildingenergy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Energy Simulation of building usin ISO52016 and more
 Home-page: https://github.com/EURAC-EEBgroup/pyBuildingEnergy
 Author: Daniele Antonucci
 Author-email: Daniele Antonucci <daniele.antonucci@eurac.edu>
 Maintainer-email: Daniele Antonucci <daniele.antonucci@eurac.edu>
 License: MIT License
         
@@ -63,14 +63,16 @@
 Requires-Dist: Pyarrow==13.0.0
 Requires-Dist: pyecharts==2.0.4
 Requires-Dist: geopy==2.4.1
 Requires-Dist: pvlib==0.10.1
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: pyswarms==1.3.0
+Requires-Dist: workalendar==17.0.0
+Requires-Dist: plotly==5.21.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Provides-Extra: gui
 Provides-Extra: cli
 
@@ -95,15 +97,15 @@
 
 The new EPBD recast provides an update on building performance assessment through a methodology that must take into account various aspects such as the thermal characteristics of the building, the use of energy from renewable sources, building automation and control systems, ventilation, cooling, energy recovery, etc.
 
 The methodology should represent the actual operating conditions, allow for the use of measured energy for accuracy and comparability purposes, and be based on hourly or sub-hourly intervals that take into account the variable conditions significantly impacting the operation and performance of the system, as well as internal conditions.
 The energy performance of a building shall be expressed by a numeric indicator of primary energy use per unit of reference floor area per year, in kWh/(m2.y) for the purpose of both energy performance certification and compliance with minimum energy performance requirements. Numeric indicators of final energy use per unit of reference floor area per year, in kWh/(m2.y) and of energy needs according to ISO 52000 in kWh/(m².y) shall be used. The methodology applied for the determination of the energy performance of a building shall be transparent and open to innovation and reflect best practices, in particular from additional indicators.
 Member States shall describe their national calculation methodology based on Annex A of the key European standards on energy performance of buildings, namely EN ISO 52000-1, EN ISO 52003-1, EN ISO 52010-1,EN ISO 52016-1, EN ISO 52018-1,EN 16798-1, EN 52120-1 and EN 17423 or superseding documents. This provision shall not constitute a legal codification of those standards.
 
-**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2017. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
+**pyBuildingEnergy** aims to provide an assessment of building performance both in terms of energy and comfort. In this initial release, it is possible to assess the energy performance of the building using ISO 52106-1:2018. Additional modules will be added for a more comprehensive evaluation of performance, assessing ventilation, renewable energies, systems, etc.
 The actual calculation methods for the assessment of building performance are the following:
 
 - [x] the (sensible) energy need for heating and cooling, based on hourly or monthly calculations;
 
 - [ ] the latent energy need for (de-)humidification, based on hourly or monthly calculations;
 
 - [x] the internal temperature, based on hourly calculations;
@@ -113,29 +115,34 @@
 - [ ] the moisture and latent heat load for (de-)humidification, based on hourly calculations;
 
 - [ ] the design sensible heating or cooling load and design latent heat load using an hourly calculation interval;
 
 - [ ] the conditions of the supply air to provide the necessary humidification and dehumidification.
 
 The calculation methods can be used for residential or non-residential buildings, or a part of it, referred to as "the building" or the "assessed object".
-ISO 52016-1:2017 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
-ISO 52016-1:2017 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
-
+ISO 52016-1:2018 also contains specifications for the assessment of thermal zones in the building or in the part of a building. The calculations are performed per thermal zone. In the calculations, the thermal zones can be assumed to be thermally coupled or not.
+ISO 52016-1:2018 is applicable to buildings at the design stage, to new buildings after construction and to existing buildings in the use phase
 
 
 Weather Data
 ------------
 The tool can use wather data coming from 2 main sources:
 
 - pvgis api (https://re.jrc.ec.europa.eu/pvg_tools/en/) - PHOTOVOLTAIC GEOGRAPHICAL INFORMATION SYSTEM
 - .epw file from https://www.ladybug.tools/epwmap/
 
 More details in the example folder
 
 
+Domestic Hot Water - DHW
+------------------------
+- [x] Calculation of volume and energy need for domestic hot water according to ISO 12831-3. 
+- [] Assessment of thermal load based on the type of DHW system
+
+
 Limitations
 ------------
 The library is developed with the intent of demonstrating specific elements of calculation procedures in the relevant standards. It is not intended to replace the regulations but to complement them, as the latter are essential for understanding the calculation. 
 This library is meant to be used for demonstration and testing purposes and is therefore provided as open source, without protection against misuse or inappropriate use.
 
 The information and views set out in this document are those of the authors and do not necessarily reflect the official opinion of the European Union. Neither the European Union institutions and bodies nor any person acting on their behalf may be held responsible for the use that may be made of the information contained herein.
 
@@ -443,15 +450,15 @@
      - YES
    
 More information about coefficients are available `here <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/src/pybuildingenergy/data>`
 
 
 Documentation
 --------------
-
+Check our doc `here <https://pybuildingenergy.readthedocs.io/en/latest/>`
 
 Example
 -------
 
 Here some `Examples <https://github.com/EURAC-EEBgroup/pyBuildingEnergy/tree/master/examples>` on pybuildingenergy application.
 For more information
 .....
@@ -477,9 +484,19 @@
 Acknowledgment
 ---------------
 This work was carried out within European projects: 
 Infinite - This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 958397, 
 Moderate - Horizon Europe research and innovation programme under grant agreement No 101069834, 
 with the aim of contributing to the development of open products useful for defining plausible scenarios for the decarbonization of the built environment
 
+Reagrding the DHW Calculation: 
+The work was developed using the regulations and results obtained from the spreadsheet created by the EPBCenter.
+
+Reference
+----------
+- EN ISO 52010-1:2018 Energy performance of buildings - External climatic conditions - Part 1: Conversion of climatic data for energy calculations
+- EN ISO 52016-1:2018 Energy performance of buildings - Energy needs for heating and cooling, internal temperatures and sensible and latent heat loads 
+- EN ISO 12831-3:2018 Energy performance of buildings - Method for calculation of the design heat load - Part 3: Domestic hot water systems heat load and characterisation of needs, Module M8-2, M8-3
+
+
```

### Comparing `pybuildingenergy-1.0.6/src/pybuildingenergy.egg-info/SOURCES.txt` & `pybuildingenergy-1.0.7/src/pybuildingenergy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -13,33 +13,58 @@
 src/pybuildingenergy.egg-info/PKG-INFO
 src/pybuildingenergy.egg-info/SOURCES.txt
 src/pybuildingenergy.egg-info/dependency_links.txt
 src/pybuildingenergy.egg-info/not-zip-safe
 src/pybuildingenergy.egg-info/requires.txt
 src/pybuildingenergy.egg-info/top_level.txt
 src/pybuildingenergy/data/building_archetype.py
-src/pybuildingenergy/data/create_archetype.py
-src/pybuildingenergy/data/profiles.py
+src/pybuildingenergy/source/DHW.py
 src/pybuildingenergy/source/__init__.py
-src/pybuildingenergy/source/calibration.py
-src/pybuildingenergy/source/calibration_NSGI.py
 src/pybuildingenergy/source/functions.py
 src/pybuildingenergy/source/graphs.py
 src/pybuildingenergy/source/utils.py
 tests/__init__.py
 tests/test_create_bui_obj.py
 tests/test_create_report.py
+tests/test_dhw.py
 tests/test_simul_newbui_from_archetype.py
 tests/test_simulate_archetype.py
 tests/test_simulate_besttest.py
 tests/test_simulation_new_bui.py
+tests/__pycache__/__init__.cpython-311.pyc
+tests/__pycache__/test_create_bui_obj.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_create_report.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_dhw.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_simul_newbui_from_archetype.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_simulate_archetype.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc
+tests/__pycache__/test_simulation_new_bui.cpython-311-pytest-6.2.4.pyc
+tests/input_data/BESTEST600_iso_vs_energyplus.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Athens.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Berlin.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Bolzano.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Madrid.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Milan.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Milano.html
+tests/input_data/BESTEST600_iso_vs_energyplus_Stockholm.html
 tests/input_data/__init__.py
 tests/input_data/archetype.py
 tests/input_data/archetypes.pickle
 tests/input_data/src.py
+tests/input_data/Result/Yearly_eNeed_gauge.html
+tests/input_data/Result/annual_sim__arch.csv
+tests/input_data/Result/energy_signature.html
+tests/input_data/Result/hourly_sim__arch.csv
+tests/input_data/Result/line_chart.html
+tests/input_data/Result/main_report.html
+tests/input_data/Result/main_report_2.html
+tests/input_data/Result/monthly_heating_cooling_need.html
+tests/input_data/Result/monthly_heating_need.html
+tests/input_data/Result/new_building_.html
+tests/input_data/Result/testbed600_ISO_vs_Eplus_Athens.html
 tests/input_data/__pycache__/__init__.cpython-311.pyc
 tests/input_data/__pycache__/src.cpython-311.pyc
 tests/input_data/energyPlus_data/Case600_V22.1.0.idf
 tests/input_data/energyPlus_data/Case600_V22.1.0out_Athens.csv
 tests/input_data/energyPlus_data/Case600_V22.1.0out_Berlin.csv
 tests/input_data/energyPlus_data/Case600_V22.1.0out_Bolzano.csv
 tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver.csv
@@ -58,15 +83,15 @@
 tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.csv
 tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.epw
 tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.csv
 tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.epw
 tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.csv
 tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.epw
 tests/input_data/weatherdata/tmy_52.496_13.414_2005_2020.csv
-tests/snapshots/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc
 tests/snapshots/test_create_bui_obj/test_create_bui_obj/properties_inputs.yml
 tests/snapshots/test_create_report/test_plotting_report/report_generated.yml
+tests/snapshots/test_dhw/test_energy_needs/dhw_test.yml
 tests/snapshots/test_simul_newbui_from_archetype/test_new_bui_from_archetype/report_new_bui_from_archetype_generated.yml
 tests/snapshots/test_simulate_archetype/test_simulate_archetype/report_from_archetype_generated.yml
 tests/snapshots/test_simulate_besttest/test_best600/data_best600_athens.json
 tests/snapshots/test_simulation_new_bui/test_simulation/annual_results_df.json
 tests/snapshots/test_simulation_new_bui/test_simulation/hourly_sim.json
```

### Comparing `pybuildingenergy-1.0.6/tests/input_data/__pycache__/src.cpython-311.pyc` & `pybuildingenergy-1.0.7/tests/input_data/__pycache__/src.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d970166 (Mon Mar 25 15:25:33 2024 UTC)
+moddate:  0x31da1766 (Thu Apr 11 12:40:17 2024 UTC)
 files sz: 761
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
@@ -26,19 +26,19 @@
                 20 LOAD_NAME                0 (os)
                 22 LOAD_ATTR                2 (getenv)
                 32 LOAD_CONST               2 ('TOXFILESDIR')
                 34 PRECALL                  1
                 38 CALL                     1
                 48 STORE_NAME               3 (main_directory_)
    
-     6          50 LOAD_CONST               3 (<code object ensure_directory_exists, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/input_data/src.py", line 6>)
+     6          50 LOAD_CONST               3 (<code object ensure_directory_exists, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/input_data/src.py", line 6>)
                 52 MAKE_FUNCTION            0
                 54 STORE_NAME               4 (ensure_directory_exists)
    
-    17          56 LOAD_CONST               4 (<code object get_buildings_demos, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/input_data/src.py", line 17>)
+    17          56 LOAD_CONST               4 (<code object get_buildings_demos, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/input_data/src.py", line 17>)
                 58 MAKE_FUNCTION            0
                 60 STORE_NAME               5 (get_buildings_demos)
                 62 LOAD_CONST               1 (None)
                 64 RETURN_VALUE
    consts
       0
       None
@@ -102,15 +102,15 @@
             "' created."
             "' already exists."
             None
          names      ('os', 'path', 'exists', 'makedirs', 'print')
          varnames   ('directory',)
          freevars   ()
          cellvars   ()
-         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/input_data/src.py'
+         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/input_data/src.py'
          name       'ensure_directory_exists'
          firstlineno 6
          lnotab 0x02053e0128012a02
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
@@ -173,19 +173,19 @@
             '/archetypes.pickle'
             'rb'
             None
          names      ('open', 'pickle', 'load')
          varnames   ('main_directory_', 'pickle_file_path', 'f', 'archetypes')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/input_data/src.py'
+         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/input_data/src.py'
          name       'get_buildings_demos'
          firstlineno 17
          lnotab 0x02050a01220128ff2e03
    names      ('os', 'pickle', 'getenv', 'main_directory_', 'ensure_directory_exists', 'get_buildings_demos')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/input_data/src.py'
+   filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/input_data/src.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201080108022002060b
```

### Comparing `pybuildingenergy-1.0.6/tests/input_data/archetype.py` & `pybuildingenergy-1.0.7/tests/input_data/archetype.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/archetypes.pickle` & `pybuildingenergy-1.0.7/tests/input_data/archetypes.pickle`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0.idf` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0.idf`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Athens.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Athens.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Berlin.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Berlin.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Bolzano.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Bolzano.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver2.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Denver2.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Madrid.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Madrid.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Milan.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Milan.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/Case600_V22.1.0out_Stockholm.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/Case600_V22.1.0out_Stockholm.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/energyPlus_data/eplusout.csv` & `pybuildingenergy-1.0.7/tests/input_data/energyPlus_data/eplusout.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/src.py` & `pybuildingenergy-1.0.7/tests/input_data/src.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Athens.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Athens.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Berlin.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Berlin.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Madrid.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Madrid.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Milan.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Milan.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/2020_Stockholm.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/2020_Stockholm.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.csv` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_37.116_14.561_2005_2020.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.csv` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_39.783_-104.892_2005_2015.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.csv` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_46.491_11.332_2005_2020.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.csv` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.epw` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_47.360_2.080_2005_2020.epw`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/input_data/weatherdata/tmy_52.496_13.414_2005_2020.csv` & `pybuildingenergy-1.0.7/tests/input_data/weatherdata/tmy_52.496_13.414_2005_2020.csv`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/snapshots/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc` & `pybuildingenergy-1.0.7/tests/__pycache__/test_simulate_besttest.cpython-311-pytest-6.2.4.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0xd657fd65 (Fri Mar 22 10:05:10 2024 UTC)
-files sz: 4881
+moddate:  0xde282166 (Thu Apr 18 14:06:22 2024 UTC)
+files sz: 4991
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 3
    flags     : 0
    code
       0x9700640064016c005a01640064016c026d03630201006d045a05010064
       0064026c066d075a070100640064036c086d095a090100640064046c0a6d
-      0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d105a
-      100100640064016c115a12640064016c135a1365136a1400000000000000
-      00a015000000000000000000000000000000000000000065136a14000000
-      0000000000a01600000000000000000000000000000000000000006517a6
-      010000ab010000000000000000a6010000ab0100000000000000005a1802
-      00650ca6000000ab0000000000000000005a196407840065194400a60000
-      00ab0000000000000000006400190000000000000000005a1a64085a1b64
-      095a1c640a5a1d640b5a1e640c5a1f640d5a20640e84005a2164015300
+      0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f010064
+      0064016c105a11640064016c125a12640064016c135a13640764086c146d
+      155a156d165a160100020065166515a6010000ab0100000000000000005a
+      176409840065174400a6000000ab00000000000000000064001900000000
+      00000000005a18640a5a19640b5a1a640c5a1b6515640d7a0000005a1c65
+      15640e7a0000005a1d6515640f7a0000005a1e641084005a1f64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (builtins)
                  8 STORE_NAME               1 (@py_builtins)
                 10 LOAD_CONST               0 (0)
@@ -43,115 +41,123 @@
                 42 LOAD_CONST               3 (('Buildings_from_dictionary',))
                 44 IMPORT_NAME              8 (src.pybuildingenergy.data.building_archetype)
                 46 IMPORT_FROM              9 (Buildings_from_dictionary)
                 48 STORE_NAME               9 (Buildings_from_dictionary)
                 50 POP_TOP
    
      3          52 LOAD_CONST               0 (0)
-                54 LOAD_CONST               4 (('ePlus_shape_data', 'get_buildings_demos'))
+                54 LOAD_CONST               4 (('ePlus_shape_data',))
                 56 IMPORT_NAME             10 (src.pybuildingenergy.source.functions)
                 58 IMPORT_FROM             11 (ePlus_shape_data)
                 60 STORE_NAME              11 (ePlus_shape_data)
-                62 IMPORT_FROM             12 (get_buildings_demos)
-                64 STORE_NAME              12 (get_buildings_demos)
-                66 POP_TOP
-   
-     4          68 LOAD_CONST               0 (0)
-                70 LOAD_CONST               5 (('bar_chart_single',))
-                72 IMPORT_NAME             13 (src.pybuildingenergy.source.graphs)
-                74 IMPORT_FROM             14 (bar_chart_single)
-                76 STORE_NAME              14 (bar_chart_single)
-                78 POP_TOP
-   
-     5          80 LOAD_CONST               0 (0)
-                82 LOAD_CONST               6 (('ThemeType',))
-                84 IMPORT_NAME             15 (pyecharts.globals)
-                86 IMPORT_FROM             16 (ThemeType)
-                88 STORE_NAME              16 (ThemeType)
-                90 POP_TOP
-   
-     6          92 LOAD_CONST               0 (0)
-                94 LOAD_CONST               1 (None)
-                96 IMPORT_NAME             17 (pandas)
-                98 STORE_NAME              18 (pd)
-   
-     7         100 LOAD_CONST               0 (0)
-               102 LOAD_CONST               1 (None)
-               104 IMPORT_NAME             19 (os)
-               106 STORE_NAME              19 (os)
-   
-     9         108 LOAD_NAME               19 (os)
-               110 LOAD_ATTR               20 (path)
-               120 LOAD_METHOD             21 (dirname)
-               142 LOAD_NAME               19 (os)
-               144 LOAD_ATTR               20 (path)
-               154 LOAD_METHOD             22 (realpath)
-               176 LOAD_NAME               23 (__file__)
-               178 PRECALL                  1
-               182 CALL                     1
-               192 PRECALL                  1
-               196 CALL                     1
-               206 STORE_NAME              24 (main_directory_)
-   
-    10         208 PUSH_NULL
-               210 LOAD_NAME               12 (get_buildings_demos)
-               212 PRECALL                  0
-               216 CALL                     0
-               226 STORE_NAME              25 (demo_buis)
+                62 POP_TOP
    
-    11         228 LOAD_CONST               7 (<code object <listcomp>, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/snapshots/test_simulate_besttest.py", line 11>)
+     4          64 LOAD_CONST               0 (0)
+                66 LOAD_CONST               5 (('bar_chart_single',))
+                68 IMPORT_NAME             12 (src.pybuildingenergy.source.graphs)
+                70 IMPORT_FROM             13 (bar_chart_single)
+                72 STORE_NAME              13 (bar_chart_single)
+                74 POP_TOP
+   
+     5          76 LOAD_CONST               0 (0)
+                78 LOAD_CONST               6 (('ThemeType',))
+                80 IMPORT_NAME             14 (pyecharts.globals)
+                82 IMPORT_FROM             15 (ThemeType)
+                84 STORE_NAME              15 (ThemeType)
+                86 POP_TOP
+   
+     6          88 LOAD_CONST               0 (0)
+                90 LOAD_CONST               1 (None)
+                92 IMPORT_NAME             16 (pandas)
+                94 STORE_NAME              17 (pd)
+   
+     7          96 LOAD_CONST               0 (0)
+                98 LOAD_CONST               1 (None)
+               100 IMPORT_NAME             18 (os)
+               102 STORE_NAME              18 (os)
+   
+     8         104 LOAD_CONST               0 (0)
+               106 LOAD_CONST               1 (None)
+               108 IMPORT_NAME             19 (pickle)
+               110 STORE_NAME              19 (pickle)
+   
+     9         112 LOAD_CONST               7 (1)
+               114 LOAD_CONST               8 (('main_directory_', 'get_buildings_demos'))
+               116 IMPORT_NAME             20 (input_data.src)
+               118 IMPORT_FROM             21 (main_directory_)
+               120 STORE_NAME              21 (main_directory_)
+               122 IMPORT_FROM             22 (get_buildings_demos)
+               124 STORE_NAME              22 (get_buildings_demos)
+               126 POP_TOP
+   
+    11         128 PUSH_NULL
+               130 LOAD_NAME               22 (get_buildings_demos)
+               132 LOAD_NAME               21 (main_directory_)
+               134 PRECALL                  1
+               138 CALL                     1
+               148 STORE_NAME              23 (demo_buis)
+   
+    13         150 LOAD_CONST               9 (<code object <listcomp>, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/test_simulate_besttest.py", line 13>)
+               152 MAKE_FUNCTION            0
+               154 LOAD_NAME               23 (demo_buis)
+               156 GET_ITER
+               158 PRECALL                  0
+               162 CALL                     0
+               172 LOAD_CONST               0 (0)
+               174 BINARY_SUBSCR
+               184 STORE_NAME              24 (bt_600)
+   
+    14         186 LOAD_CONST              10 ('pvgis')
+               188 STORE_NAME              25 (weather_type)
+   
+    15         190 LOAD_CONST              11 (44.78)
+               192 STORE_NAME              26 (latitude_bui)
+   
+    16         194 LOAD_CONST              12 (9.78)
+               196 STORE_NAME              27 (longitude_bui)
+   
+    17         198 LOAD_NAME               21 (main_directory_)
+               200 LOAD_CONST              13 ('/energyPlus_data/Case600_V22.1.0out_Athens.csv')
+               202 BINARY_OP                0 (+)
+               206 STORE_NAME              28 (path_epls_file)
+   
+    18         208 LOAD_NAME               21 (main_directory_)
+               210 LOAD_CONST              14 ('/weatherdata/2020_Athens.epw')
+               212 BINARY_OP                0 (+)
+               216 STORE_NAME              29 (path_weather_file_)
+   
+    19         218 LOAD_NAME               21 (main_directory_)
+               220 LOAD_CONST              15 ('/Result/testbed600_ISO_vs_Eplus_Athens.html')
+               222 BINARY_OP                0 (+)
+               226 STORE_NAME              30 (path_chart_name)
+   
+    23         228 LOAD_CONST              16 (<code object test_best600, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/test_simulate_besttest.py", line 23>)
                230 MAKE_FUNCTION            0
-               232 LOAD_NAME               25 (demo_buis)
-               234 GET_ITER
-               236 PRECALL                  0
-               240 CALL                     0
-               250 LOAD_CONST               0 (0)
-               252 BINARY_SUBSCR
-               262 STORE_NAME              26 (bt_600)
-   
-    12         264 LOAD_CONST               8 ('pvgis')
-               266 STORE_NAME              27 (weather_type)
-   
-    13         268 LOAD_CONST               9 (44.78)
-               270 STORE_NAME              28 (latitude_bui)
-   
-    14         272 LOAD_CONST              10 (9.78)
-               274 STORE_NAME              29 (longitude_bui)
-   
-    15         276 LOAD_CONST              11 ('/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/examples/energyPlus_data/Case600_V22.1.0out_Athens.csv')
-               278 STORE_NAME              30 (path_epls_file)
-   
-    16         280 LOAD_CONST              12 ('/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/examples/weatherdata/2020_Athens.epw')
-               282 STORE_NAME              31 (path_weather_file_)
-   
-    17         284 LOAD_CONST              13 ('/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/Result_test/testbed600_ISO_vs_Eplus_Athens.html')
-               286 STORE_NAME              32 (path_chart_name)
-   
-    21         288 LOAD_CONST              14 (<code object test_best600, file "/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/snapshots/test_simulate_besttest.py", line 21>)
-               290 MAKE_FUNCTION            0
-               292 STORE_NAME              33 (test_best600)
-               294 LOAD_CONST               1 (None)
-               296 RETURN_VALUE
+               232 STORE_NAME              31 (test_best600)
+               234 LOAD_CONST               1 (None)
+               236 RETURN_VALUE
    consts
       0
       None
       ('ISO52016',)
       ('Buildings_from_dictionary',)
-      ('ePlus_shape_data', 'get_buildings_demos')
+      ('ePlus_shape_data',)
       ('bar_chart_single',)
       ('ThemeType',)
+      1
+      ('main_directory_', 'get_buildings_demos')
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970067007c005d107d017c0164001900000000000000000064016b0200
             000000af0e7c0191028c115300
-          11           0 RESUME                   0
+          13           0 RESUME                   0
                        2 BUILD_LIST               0
                        4 LOAD_FAST                0 (.0)
                  >>    6 FOR_ITER                16 (to 40)
                        8 STORE_FAST               1 (bui)
                       10 LOAD_FAST                1 (bui)
                       12 LOAD_CONST               0 ('building_type')
                       14 BINARY_SUBSCR
@@ -165,24 +171,24 @@
          consts
             'building_type'
             'BestTest600'
          names      ()
          varnames   ('.0', 'bui')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/snapshots/test_simulate_besttest.py'
+         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/test_simulate_besttest.py'
          name       '<listcomp>'
-         firstlineno 11
+         firstlineno 13
          lnotab 0x
       'pvgis'
       44.78
       9.78
-      '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/examples/energyPlus_data/Case600_V22.1.0out_Athens.csv'
-      '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/examples/weatherdata/2020_Athens.epw'
-      '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/Result_test/testbed600_ISO_vs_Eplus_Athens.html'
+      '/energyPlus_data/Case600_V22.1.0out_Athens.csv'
+      '/weatherdata/2020_Athens.epw'
+      '/Result/testbed600_ISO_vs_Eplus_Athens.html'
       code
          argcount  : 1
          nlocals   : 18
          stacksize : 7
          flags     : 3
          code
             0x9700740100000000000000000000740200000000000000000000a60100
@@ -198,306 +204,385 @@
             000100740f00000000000000000000a6000000ab000000000000000000a0
             0800000000000000000000000000000000000000007c0174060000000000
             0000000000741200000000000000000000ac08a6030000ab030000000000
             0000005c0200007d027d037c03640919000000000000000000a00a000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00640a7a0b00007d047c03640b19000000000000000000a00a0000000000
             000000000000000000000000000000a6000000ab00000000000000000064
-            0a7a0b00007d057c02640c19000000000000000000a00b00000000000000
-            00000000000000000000000000640da6010000ab010000000000000000a0
-            0c0000000000000000000000000000000000000000a6000000ab00000000
-            0000000000640e7c01a00d00000000000000000000000000000000000000
-            00640fa6010000ab0100000000000000007a0500007a0b00007d067c0264
-            1019000000000000000000a00b0000000000000000000000000000000000
-            000000640da6010000ab010000000000000000a00c000000000000000000
-            0000000000000000000000a6000000ab000000000000000000640e7c01a0
-            0d0000000000000000000000000000000000000000640fa6010000ab0100
-            000000000000007a0500007a0b00007d077c026411190000000000000000
-            00a00b0000000000000000000000000000000000000000640da6010000ab
-            010000000000000000a00e00000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d087c066a0f00000000000000007d
-            097420000000000000000000007d0a742300000000000000000000742500
-            0000000000000000006a1300000000000000007c0aa6010000ab01000000
-            00000000007c01a00d000000000000000000000000000000000000000064
-            0fa6010000ab010000000000000000a6020000ab0200000000000000007d
-            0b7c0b6412190000000000000000007d0c7c0b6413190000000000000000
-            007d0d7c0b6414190000000000000000007d0e7c066a0f00000000000000
-            007d097425000000000000000000006a1400000000000000007c097c0c7c
-            0d64159c02ac16a6020000ab0200000000000000007d0f74250000000000
-            00000000006a1500000000000000007c067c0f6417190000000000000000
-            007c077c0f64181900000000000000000067046413ac19a6020000ab0200
-            000000000000007d107c10a0160000000000000000000000000000000000
-            0000006414a6010000ab0100000000000000007d10742f00000000000000
-            0000007c106a180000000000000000a01900000000000000000000000000
-            00000000000000a6000000ab0000000000000000007c106a1a0000000000
-            0000006a1b0000000000000000a019000000000000000000000000000000
-            0000000000a6000000ab0000000000000000007438000000000000000000
-            006a1d0000000000000000ac1aa6030000ab0300000000000000007d117c
-            11a01e0000000000000000000000000000000000000000743e0000000000
-            0000000000a6010000ab01000000000000000001007c00a0200000000000
-            0000000000000000000000000000007c10a0210000000000000000000000
-            000000000000000000a6000000ab000000000000000000641ba6020000ab
-            0200000000000000005300
-          21           0 RESUME                   0
+            0a7a0b00007d0509007c02640c19000000000000000000a00b0000000000
+            000000000000000000000000000000640da6010000ab0100000000000000
+            00a00c0000000000000000000000000000000000000000a6000000ab0000
+            00000000000000640e7c01a00d0000000000000000000000000000000000
+            000000640fa6010000ab0100000000000000007a0500007a0b00007d067c
+            02641019000000000000000000a00b000000000000000000000000000000
+            0000000000640da6010000ab010000000000000000a00c00000000000000
+            00000000000000000000000000a6000000ab000000000000000000640e7c
+            01a00d0000000000000000000000000000000000000000640fa6010000ab
+            0100000000000000007a0500007a0b00007d077c02641119000000000000
+            000000a00b0000000000000000000000000000000000000000640da60100
+            00ab010000000000000000a00e0000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d086ec0230001007c02640c19
+            000000000000000000a00b00000000000000000000000000000000000000
+            006412a6010000ab010000000000000000a00c0000000000000000000000
+            000000000000000000a6000000ab000000000000000000640e7c01a00d00
+            00000000000000000000000000000000000000640fa6010000ab01000000
+            00000000007a0500007a0b00007d067c02641019000000000000000000a0
+            0b00000000000000000000000000000000000000006412a6010000ab0100
+            00000000000000a00c0000000000000000000000000000000000000000a6
+            000000ab000000000000000000640e7c01a00d0000000000000000000000
+            000000000000000000640fa6010000ab0100000000000000007a0500007a
+            0b00007d077c02641119000000000000000000a00b000000000000000000
+            00000000000000000000006412a6010000ab010000000000000000a00e00
+            00000000000000000000000000000000000000a6000000ab000000000000
+            0000007d0859006e037803590077017c066a0f00000000000000007d0974
+            20000000000000000000007d0a7423000000000000000000007425000000
+            000000000000006a1300000000000000007c0aa6010000ab010000000000
+            0000007c01a00d0000000000000000000000000000000000000000640fa6
+            010000ab010000000000000000a6020000ab0200000000000000007d0b7c
+            0b6413190000000000000000007d0c7c0b6414190000000000000000007d
+            0d7c0b6415190000000000000000007d0e7c066a0f00000000000000007d
+            097425000000000000000000006a1400000000000000007c097c0c7c0d64
+            169c02ac17a6020000ab0200000000000000007d0f742500000000000000
+            0000006a1500000000000000007c067c0f6418190000000000000000007c
+            077c0f64191900000000000000000067046414ac1aa6020000ab02000000
+            00000000007d107c10a01600000000000000000000000000000000000000
+            006415a6010000ab0100000000000000007d10742f000000000000000000
+            007c106a180000000000000000a019000000000000000000000000000000
+            0000000000a6000000ab0000000000000000007c106a1a00000000000000
+            006a1b0000000000000000a0190000000000000000000000000000000000
+            000000a6000000ab0000000000000000007438000000000000000000006a
+            1d0000000000000000ac1ba6030000ab0300000000000000007d117c11a0
+            1e0000000000000000000000000000000000000000743e00000000000000
+            000000a6010000ab01000000000000000001007c00a02000000000000000
+            000000000000000000000000007c10a02100000000000000000000000000
+            00000000000000a6000000ab000000000000000000641ca6020000ab0200
+            000000000000005300
+          23           0 RESUME                   0
          
-          35           2 LOAD_GLOBAL              1 (NULL + Buildings_from_dictionary)
+          37           2 LOAD_GLOBAL              1 (NULL + Buildings_from_dictionary)
                       14 LOAD_GLOBAL              2 (bt_600)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               1 (BUI)
          
-          36          42 LOAD_FAST                1 (BUI)
+          38          42 LOAD_FAST                1 (BUI)
                       44 LOAD_METHOD              2 (__setattr__)
                       66 LOAD_CONST               1 ('weather_source')
                       68 LOAD_GLOBAL              6 (weather_type)
                       80 PRECALL                  2
                       84 CALL                     2
                       94 POP_TOP
          
-          38          96 LOAD_GLOBAL              6 (weather_type)
+          40          96 LOAD_GLOBAL              6 (weather_type)
                      108 LOAD_CONST               2 (('pvgis', 'epw'))
                      110 CONTAINS_OP              1
                      112 POP_JUMP_FORWARD_IF_FALSE    15 (to 144)
          
-          39         114 LOAD_GLOBAL              9 (NULL + ValueError)
+          41         114 LOAD_GLOBAL              9 (NULL + ValueError)
                      126 LOAD_CONST               3 ("weather_type must be 'pvgis' or 'epw'")
                      128 PRECALL                  1
                      132 CALL                     1
                      142 RAISE_VARARGS            1
          
-          41     >>  144 LOAD_GLOBAL              6 (weather_type)
+          43     >>  144 LOAD_GLOBAL              6 (weather_type)
                      156 LOAD_CONST               4 ('pvgis')
                      158 COMPARE_OP               2 (==)
                      164 POP_JUMP_FORWARD_IF_FALSE    68 (to 302)
          
-          42         166 LOAD_GLOBAL             10 (latitude_bui)
+          44         166 LOAD_GLOBAL             10 (latitude_bui)
                      178 POP_JUMP_FORWARD_IF_NONE    27 (to 234)
          
-          43         180 LOAD_FAST                1 (BUI)
+          45         180 LOAD_FAST                1 (BUI)
                      182 LOAD_METHOD              2 (__setattr__)
                      204 LOAD_CONST               6 ('latitude')
                      206 LOAD_GLOBAL             10 (latitude_bui)
                      218 PRECALL                  2
                      222 CALL                     2
                      232 POP_TOP
          
-          44     >>  234 LOAD_GLOBAL             12 (longitude_bui)
+          46     >>  234 LOAD_GLOBAL             12 (longitude_bui)
                      246 POP_JUMP_FORWARD_IF_NONE    27 (to 302)
          
-          45         248 LOAD_FAST                1 (BUI)
+          47         248 LOAD_FAST                1 (BUI)
                      250 LOAD_METHOD              2 (__setattr__)
                      272 LOAD_CONST               7 ('longitude')
                      274 LOAD_GLOBAL             12 (longitude_bui)
                      286 PRECALL                  2
                      290 CALL                     2
                      300 POP_TOP
          
-          56     >>  302 LOAD_GLOBAL             15 (NULL + ISO52016)
+          58     >>  302 LOAD_GLOBAL             15 (NULL + ISO52016)
                      314 PRECALL                  0
                      318 CALL                     0
                      328 LOAD_METHOD              8 (Temperature_and_Energy_needs_calculation)
                      350 LOAD_FAST                1 (BUI)
                      352 LOAD_GLOBAL              6 (weather_type)
                      364 LOAD_GLOBAL             18 (path_weather_file_)
                      376 KW_NAMES                 8
                      378 PRECALL                  3
                      382 CALL                     3
                      392 UNPACK_SEQUENCE          2
                      396 STORE_FAST               2 (hourly_results)
                      398 STORE_FAST               3 (annual_results_df)
          
-          60         400 LOAD_FAST                3 (annual_results_df)
+          62         400 LOAD_FAST                3 (annual_results_df)
                      402 LOAD_CONST               9 ('Q_H_annual_per_sqm')
                      404 BINARY_SUBSCR
                      414 LOAD_METHOD             10 (squeeze)
                      436 PRECALL                  0
                      440 CALL                     0
                      450 LOAD_CONST              10 (1000)
                      452 BINARY_OP               11 (/)
                      456 STORE_FAST               4 (ISO52016_annual_heating)
          
-          61         458 LOAD_FAST                3 (annual_results_df)
+          63         458 LOAD_FAST                3 (annual_results_df)
                      460 LOAD_CONST              11 ('Q_C_annual_per_sqm')
                      462 BINARY_SUBSCR
                      472 LOAD_METHOD             10 (squeeze)
                      494 PRECALL                  0
                      498 CALL                     0
                      508 LOAD_CONST              10 (1000)
                      510 BINARY_OP               11 (/)
                      514 STORE_FAST               5 (ISO52016_annual_cooling)
          
-          62         516 LOAD_FAST                2 (hourly_results)
-                     518 LOAD_CONST              12 ('Q_H')
-                     520 BINARY_SUBSCR
-                     530 LOAD_METHOD             11 (resample)
-                     552 LOAD_CONST              13 ('ME')
-                     554 PRECALL                  1
-                     558 CALL                     1
-                     568 LOAD_METHOD             12 (sum)
-                     590 PRECALL                  0
-                     594 CALL                     0
-                     604 LOAD_CONST              14 (1000.0)
-                     606 LOAD_FAST                1 (BUI)
-                     608 LOAD_METHOD             13 (__getattribute__)
-                     630 LOAD_CONST              15 ('a_use')
-                     632 PRECALL                  1
-                     636 CALL                     1
-                     646 BINARY_OP                5 (*)
-                     650 BINARY_OP               11 (/)
-                     654 STORE_FAST               6 (ISO52016_monthly_heating_in_kWh_per_sqm)
-         
-          63         656 LOAD_FAST                2 (hourly_results)
-                     658 LOAD_CONST              16 ('Q_C')
-                     660 BINARY_SUBSCR
-                     670 LOAD_METHOD             11 (resample)
-                     692 LOAD_CONST              13 ('ME')
-                     694 PRECALL                  1
-                     698 CALL                     1
-                     708 LOAD_METHOD             12 (sum)
-                     730 PRECALL                  0
-                     734 CALL                     0
-                     744 LOAD_CONST              14 (1000.0)
-                     746 LOAD_FAST                1 (BUI)
-                     748 LOAD_METHOD             13 (__getattribute__)
-                     770 LOAD_CONST              15 ('a_use')
-                     772 PRECALL                  1
-                     776 CALL                     1
-                     786 BINARY_OP                5 (*)
-                     790 BINARY_OP               11 (/)
-                     794 STORE_FAST               7 (ISO52016_monthly_cooling_in_kWh_per_sqm)
-         
-          64         796 LOAD_FAST                2 (hourly_results)
-                     798 LOAD_CONST              17 ('T_op')
-                     800 BINARY_SUBSCR
-                     810 LOAD_METHOD             11 (resample)
-                     832 LOAD_CONST              13 ('ME')
-                     834 PRECALL                  1
-                     838 CALL                     1
-                     848 LOAD_METHOD             14 (mean)
-                     870 PRECALL                  0
-                     874 CALL                     0
-                     884 STORE_FAST               8 (ISO52016_monthly_T_op)
-         
-          65         886 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
-                     888 LOAD_ATTR               15 (index)
-                     898 STORE_FAST               9 (index)
-         
-          68         900 LOAD_GLOBAL             32 (path_epls_file)
-                     912 STORE_FAST              10 (dir_energy_plus)
-         
-          69         914 LOAD_GLOBAL             35 (NULL + ePlus_shape_data)
-                     926 LOAD_GLOBAL             37 (NULL + pd)
-                     938 LOAD_ATTR               19 (read_csv)
-                     948 LOAD_FAST               10 (dir_energy_plus)
-                     950 PRECALL                  1
-                     954 CALL                     1
-                     964 LOAD_FAST                1 (BUI)
-                     966 LOAD_METHOD             13 (__getattribute__)
-                     988 LOAD_CONST              15 ('a_use')
-                     990 PRECALL                  1
-                     994 CALL                     1
-                    1004 PRECALL                  2
-                    1008 CALL                     2
-                    1018 STORE_FAST              11 (eplus_data)
-         
-          70        1020 LOAD_FAST               11 (eplus_data)
-                    1022 LOAD_CONST              18 (0)
-                    1024 BINARY_SUBSCR
-                    1034 STORE_FAST              12 (EnergyPlus_monthly_heating_in_kWh_per_sqm)
-         
-          71        1036 LOAD_FAST               11 (eplus_data)
-                    1038 LOAD_CONST              19 (1)
-                    1040 BINARY_SUBSCR
-                    1050 STORE_FAST              13 (EnergyPlus_monthly_cooling_in_kWh_per_sqm)
-         
-          72        1052 LOAD_FAST               11 (eplus_data)
-                    1054 LOAD_CONST              20 (2)
-                    1056 BINARY_SUBSCR
-                    1066 STORE_FAST              14 (ep_monthly_T_op)
-         
-          73        1068 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
-                    1070 LOAD_ATTR               15 (index)
-                    1080 STORE_FAST               9 (index)
-         
-          75        1082 LOAD_GLOBAL             37 (NULL + pd)
-                    1094 LOAD_ATTR               20 (DataFrame)
-                    1104 LOAD_FAST                9 (index)
-                    1106 LOAD_FAST               12 (EnergyPlus_monthly_heating_in_kWh_per_sqm)
-                    1108 LOAD_FAST               13 (EnergyPlus_monthly_cooling_in_kWh_per_sqm)
-                    1110 LOAD_CONST              21 (('Q_H EnergyPlus', 'Q_C EnergyPlus'))
-                    1112 BUILD_CONST_KEY_MAP      2
-                    1114 KW_NAMES                22
-                    1116 PRECALL                  2
-                    1120 CALL                     2
-                    1130 STORE_FAST              15 (df_ep_monthly)
-         
-          79        1132 LOAD_GLOBAL             37 (NULL + pd)
-                    1144 LOAD_ATTR               21 (concat)
-                    1154 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
-                    1156 LOAD_FAST               15 (df_ep_monthly)
-                    1158 LOAD_CONST              23 ('Q_H EnergyPlus')
-                    1160 BINARY_SUBSCR
-                    1170 LOAD_FAST                7 (ISO52016_monthly_cooling_in_kWh_per_sqm)
-                    1172 LOAD_FAST               15 (df_ep_monthly)
-                    1174 LOAD_CONST              24 ('Q_C EnergyPlus')
-                    1176 BINARY_SUBSCR
-                    1186 BUILD_LIST               4
-                    1188 LOAD_CONST              19 (1)
-                    1190 KW_NAMES                25
-                    1192 PRECALL                  2
-                    1196 CALL                     2
-                    1206 STORE_FAST              16 (df_barplot)
-         
-          80        1208 LOAD_FAST               16 (df_barplot)
-                    1210 LOAD_METHOD             22 (round)
-                    1232 LOAD_CONST              20 (2)
-                    1234 PRECALL                  1
-                    1238 CALL                     1
-                    1248 STORE_FAST              16 (df_barplot)
-         
-          83        1250 LOAD_GLOBAL             47 (NULL + bar_chart_single)
-         
-          84        1262 LOAD_FAST               16 (df_barplot)
-                    1264 LOAD_ATTR               24 (columns)
-                    1274 LOAD_METHOD             25 (tolist)
-                    1296 PRECALL                  0
-                    1300 CALL                     0
-         
-          85        1310 LOAD_FAST               16 (df_barplot)
-                    1312 LOAD_ATTR               26 (values)
-                    1322 LOAD_ATTR               27 (T)
-                    1332 LOAD_METHOD             25 (tolist)
-                    1354 PRECALL                  0
-                    1358 CALL                     0
-         
-          86        1368 LOAD_GLOBAL             56 (ThemeType)
-                    1380 LOAD_ATTR               29 (SHINE)
-         
-          83        1390 KW_NAMES                26
-                    1392 PRECALL                  3
-                    1396 CALL                     3
-                    1406 STORE_FAST              17 (graph)
-         
-          88        1408 LOAD_FAST               17 (graph)
-                    1410 LOAD_METHOD             30 (render)
-                    1432 LOAD_GLOBAL             62 (path_chart_name)
-                    1444 PRECALL                  1
-                    1448 CALL                     1
-                    1458 POP_TOP
-         
-          90        1460 LOAD_FAST                0 (snapshot)
-                    1462 LOAD_METHOD             32 (assert_match)
-                    1484 LOAD_FAST               16 (df_barplot)
-                    1486 LOAD_METHOD             33 (to_json)
-                    1508 PRECALL                  0
-                    1512 CALL                     0
-                    1522 LOAD_CONST              27 ('data_best600_athens.json')
-                    1524 PRECALL                  2
-                    1528 CALL                     2
-                    1538 RETURN_VALUE
+          64         516 NOP
+         
+          65         518 LOAD_FAST                2 (hourly_results)
+                     520 LOAD_CONST              12 ('Q_H')
+                     522 BINARY_SUBSCR
+                     532 LOAD_METHOD             11 (resample)
+                     554 LOAD_CONST              13 ('ME')
+                     556 PRECALL                  1
+                     560 CALL                     1
+                     570 LOAD_METHOD             12 (sum)
+                     592 PRECALL                  0
+                     596 CALL                     0
+                     606 LOAD_CONST              14 (1000.0)
+                     608 LOAD_FAST                1 (BUI)
+                     610 LOAD_METHOD             13 (__getattribute__)
+                     632 LOAD_CONST              15 ('a_use')
+                     634 PRECALL                  1
+                     638 CALL                     1
+                     648 BINARY_OP                5 (*)
+                     652 BINARY_OP               11 (/)
+                     656 STORE_FAST               6 (ISO52016_monthly_heating_in_kWh_per_sqm)
+         
+          66         658 LOAD_FAST                2 (hourly_results)
+                     660 LOAD_CONST              16 ('Q_C')
+                     662 BINARY_SUBSCR
+                     672 LOAD_METHOD             11 (resample)
+                     694 LOAD_CONST              13 ('ME')
+                     696 PRECALL                  1
+                     700 CALL                     1
+                     710 LOAD_METHOD             12 (sum)
+                     732 PRECALL                  0
+                     736 CALL                     0
+                     746 LOAD_CONST              14 (1000.0)
+                     748 LOAD_FAST                1 (BUI)
+                     750 LOAD_METHOD             13 (__getattribute__)
+                     772 LOAD_CONST              15 ('a_use')
+                     774 PRECALL                  1
+                     778 CALL                     1
+                     788 BINARY_OP                5 (*)
+                     792 BINARY_OP               11 (/)
+                     796 STORE_FAST               7 (ISO52016_monthly_cooling_in_kWh_per_sqm)
+         
+          67         798 LOAD_FAST                2 (hourly_results)
+                     800 LOAD_CONST              17 ('T_op')
+                     802 BINARY_SUBSCR
+                     812 LOAD_METHOD             11 (resample)
+                     834 LOAD_CONST              13 ('ME')
+                     836 PRECALL                  1
+                     840 CALL                     1
+                     850 LOAD_METHOD             14 (mean)
+                     872 PRECALL                  0
+                     876 CALL                     0
+                     886 STORE_FAST               8 (ISO52016_monthly_T_op)
+                     888 JUMP_FORWARD           192 (to 1274)
+                 >>  890 PUSH_EXC_INFO
+         
+          68         892 POP_TOP
+         
+          69         894 LOAD_FAST                2 (hourly_results)
+                     896 LOAD_CONST              12 ('Q_H')
+                     898 BINARY_SUBSCR
+                     908 LOAD_METHOD             11 (resample)
+                     930 LOAD_CONST              18 ('M')
+                     932 PRECALL                  1
+                     936 CALL                     1
+                     946 LOAD_METHOD             12 (sum)
+                     968 PRECALL                  0
+                     972 CALL                     0
+                     982 LOAD_CONST              14 (1000.0)
+                     984 LOAD_FAST                1 (BUI)
+                     986 LOAD_METHOD             13 (__getattribute__)
+                    1008 LOAD_CONST              15 ('a_use')
+                    1010 PRECALL                  1
+                    1014 CALL                     1
+                    1024 BINARY_OP                5 (*)
+                    1028 BINARY_OP               11 (/)
+                    1032 STORE_FAST               6 (ISO52016_monthly_heating_in_kWh_per_sqm)
+         
+          70        1034 LOAD_FAST                2 (hourly_results)
+                    1036 LOAD_CONST              16 ('Q_C')
+                    1038 BINARY_SUBSCR
+                    1048 LOAD_METHOD             11 (resample)
+                    1070 LOAD_CONST              18 ('M')
+                    1072 PRECALL                  1
+                    1076 CALL                     1
+                    1086 LOAD_METHOD             12 (sum)
+                    1108 PRECALL                  0
+                    1112 CALL                     0
+                    1122 LOAD_CONST              14 (1000.0)
+                    1124 LOAD_FAST                1 (BUI)
+                    1126 LOAD_METHOD             13 (__getattribute__)
+                    1148 LOAD_CONST              15 ('a_use')
+                    1150 PRECALL                  1
+                    1154 CALL                     1
+                    1164 BINARY_OP                5 (*)
+                    1168 BINARY_OP               11 (/)
+                    1172 STORE_FAST               7 (ISO52016_monthly_cooling_in_kWh_per_sqm)
+         
+          71        1174 LOAD_FAST                2 (hourly_results)
+                    1176 LOAD_CONST              17 ('T_op')
+                    1178 BINARY_SUBSCR
+                    1188 LOAD_METHOD             11 (resample)
+                    1210 LOAD_CONST              18 ('M')
+                    1212 PRECALL                  1
+                    1216 CALL                     1
+                    1226 LOAD_METHOD             14 (mean)
+                    1248 PRECALL                  0
+                    1252 CALL                     0
+                    1262 STORE_FAST               8 (ISO52016_monthly_T_op)
+                    1264 POP_EXCEPT
+                    1266 JUMP_FORWARD             3 (to 1274)
+                 >> 1268 COPY                     3
+                    1270 POP_EXCEPT
+                    1272 RERAISE                  1
+         
+          73     >> 1274 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
+                    1276 LOAD_ATTR               15 (index)
+                    1286 STORE_FAST               9 (index)
+         
+          76        1288 LOAD_GLOBAL             32 (path_epls_file)
+                    1300 STORE_FAST              10 (dir_energy_plus)
+         
+          77        1302 LOAD_GLOBAL             35 (NULL + ePlus_shape_data)
+                    1314 LOAD_GLOBAL             37 (NULL + pd)
+                    1326 LOAD_ATTR               19 (read_csv)
+                    1336 LOAD_FAST               10 (dir_energy_plus)
+                    1338 PRECALL                  1
+                    1342 CALL                     1
+                    1352 LOAD_FAST                1 (BUI)
+                    1354 LOAD_METHOD             13 (__getattribute__)
+                    1376 LOAD_CONST              15 ('a_use')
+                    1378 PRECALL                  1
+                    1382 CALL                     1
+                    1392 PRECALL                  2
+                    1396 CALL                     2
+                    1406 STORE_FAST              11 (eplus_data)
+         
+          78        1408 LOAD_FAST               11 (eplus_data)
+                    1410 LOAD_CONST              19 (0)
+                    1412 BINARY_SUBSCR
+                    1422 STORE_FAST              12 (EnergyPlus_monthly_heating_in_kWh_per_sqm)
+         
+          79        1424 LOAD_FAST               11 (eplus_data)
+                    1426 LOAD_CONST              20 (1)
+                    1428 BINARY_SUBSCR
+                    1438 STORE_FAST              13 (EnergyPlus_monthly_cooling_in_kWh_per_sqm)
+         
+          80        1440 LOAD_FAST               11 (eplus_data)
+                    1442 LOAD_CONST              21 (2)
+                    1444 BINARY_SUBSCR
+                    1454 STORE_FAST              14 (ep_monthly_T_op)
+         
+          81        1456 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
+                    1458 LOAD_ATTR               15 (index)
+                    1468 STORE_FAST               9 (index)
+         
+          83        1470 LOAD_GLOBAL             37 (NULL + pd)
+                    1482 LOAD_ATTR               20 (DataFrame)
+                    1492 LOAD_FAST                9 (index)
+                    1494 LOAD_FAST               12 (EnergyPlus_monthly_heating_in_kWh_per_sqm)
+                    1496 LOAD_FAST               13 (EnergyPlus_monthly_cooling_in_kWh_per_sqm)
+                    1498 LOAD_CONST              22 (('Q_H EnergyPlus', 'Q_C EnergyPlus'))
+                    1500 BUILD_CONST_KEY_MAP      2
+                    1502 KW_NAMES                23
+                    1504 PRECALL                  2
+                    1508 CALL                     2
+                    1518 STORE_FAST              15 (df_ep_monthly)
+         
+          87        1520 LOAD_GLOBAL             37 (NULL + pd)
+                    1532 LOAD_ATTR               21 (concat)
+                    1542 LOAD_FAST                6 (ISO52016_monthly_heating_in_kWh_per_sqm)
+                    1544 LOAD_FAST               15 (df_ep_monthly)
+                    1546 LOAD_CONST              24 ('Q_H EnergyPlus')
+                    1548 BINARY_SUBSCR
+                    1558 LOAD_FAST                7 (ISO52016_monthly_cooling_in_kWh_per_sqm)
+                    1560 LOAD_FAST               15 (df_ep_monthly)
+                    1562 LOAD_CONST              25 ('Q_C EnergyPlus')
+                    1564 BINARY_SUBSCR
+                    1574 BUILD_LIST               4
+                    1576 LOAD_CONST              20 (1)
+                    1578 KW_NAMES                26
+                    1580 PRECALL                  2
+                    1584 CALL                     2
+                    1594 STORE_FAST              16 (df_barplot)
+         
+          88        1596 LOAD_FAST               16 (df_barplot)
+                    1598 LOAD_METHOD             22 (round)
+                    1620 LOAD_CONST              21 (2)
+                    1622 PRECALL                  1
+                    1626 CALL                     1
+                    1636 STORE_FAST              16 (df_barplot)
+         
+          91        1638 LOAD_GLOBAL             47 (NULL + bar_chart_single)
+         
+          92        1650 LOAD_FAST               16 (df_barplot)
+                    1652 LOAD_ATTR               24 (columns)
+                    1662 LOAD_METHOD             25 (tolist)
+                    1684 PRECALL                  0
+                    1688 CALL                     0
+         
+          93        1698 LOAD_FAST               16 (df_barplot)
+                    1700 LOAD_ATTR               26 (values)
+                    1710 LOAD_ATTR               27 (T)
+                    1720 LOAD_METHOD             25 (tolist)
+                    1742 PRECALL                  0
+                    1746 CALL                     0
+         
+          94        1756 LOAD_GLOBAL             56 (ThemeType)
+                    1768 LOAD_ATTR               29 (SHINE)
+         
+          91        1778 KW_NAMES                27
+                    1780 PRECALL                  3
+                    1784 CALL                     3
+                    1794 STORE_FAST              17 (graph)
+         
+          96        1796 LOAD_FAST               17 (graph)
+                    1798 LOAD_METHOD             30 (render)
+                    1820 LOAD_GLOBAL             62 (path_chart_name)
+                    1832 PRECALL                  1
+                    1836 CALL                     1
+                    1846 POP_TOP
+         
+          98        1848 LOAD_FAST                0 (snapshot)
+                    1850 LOAD_METHOD             32 (assert_match)
+                    1872 LOAD_FAST               16 (df_barplot)
+                    1874 LOAD_METHOD             33 (to_json)
+                    1896 PRECALL                  0
+                    1900 CALL                     0
+                    1910 LOAD_CONST              28 ('data_best600_athens.json')
+                    1912 PRECALL                  2
+                    1916 CALL                     2
+                    1926 RETURN_VALUE
+         ExceptionTable:
+           518 to 886 -> 890 [0]
+           890 to 1262 -> 1268 [1] lasti
          consts
             "\n    Simualte besttest600 with different weather file and comparing data with the onew coming from energy plus\n    Param\n    ------\n    name_chart: name file to save the result of simulation\n    weather_type: Specify the data source for weather data. If using the PVGIS website, indicate 'pvgis'; if loading an EPW file from the path_weather_file_, indicate 'epw'.\n    latitude: mandatory if weather_type is 'pvgis'\n    longitude:  mandatory if weather_type is 'epw'\n    path_epls_file: specifc thte path of the energy plus simulation file \n    path_weather_file_: if weather_type ='epw', specify the folder where the epw file is uploaded.\n    eplus_file_name: name of the epw file \n    "
             'weather_source'
             ('pvgis', 'epw')
             "weather_type must be 'pvgis' or 'epw'"
             'pvgis'
             None
@@ -509,38 +594,39 @@
             'Q_C_annual_per_sqm'
             'Q_H'
             'ME'
             1000.0
             'a_use'
             'Q_C'
             'T_op'
+            'M'
             0
             1
             2
             ('Q_H EnergyPlus', 'Q_C EnergyPlus')
             ('index', 'data')
             'Q_H EnergyPlus'
             'Q_C EnergyPlus'
             ('axis',)
             ('y_name', 'y_data_plot', 'theme_type')
             'data_best600_athens.json'
          names      ('Buildings_from_dictionary', 'bt_600', '__setattr__', 'weather_type', 'ValueError', 'latitude_bui', 'longitude_bui', 'ISO52016', 'Temperature_and_Energy_needs_calculation', 'path_weather_file_', 'squeeze', 'resample', 'sum', '__getattribute__', 'mean', 'index', 'path_epls_file', 'ePlus_shape_data', 'pd', 'read_csv', 'DataFrame', 'concat', 'round', 'bar_chart_single', 'columns', 'tolist', 'values', 'T', 'ThemeType', 'SHINE', 'render', 'path_chart_name', 'assert_match', 'to_json')
          varnames   ('snapshot', 'BUI', 'hourly_results', 'annual_results_df', 'ISO52016_annual_heating', 'ISO52016_annual_cooling', 'ISO52016_monthly_heating_in_kWh_per_sqm', 'ISO52016_monthly_cooling_in_kWh_per_sqm', 'ISO52016_monthly_T_op', 'index', 'dir_energy_plus', 'eplus_data', 'EnergyPlus_monthly_heating_in_kWh_per_sqm', 'EnergyPlus_monthly_cooling_in_kWh_per_sqm', 'ep_monthly_T_op', 'df_ep_monthly', 'df_barplot', 'graph')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/snapshots/test_simulate_besttest.py'
+         filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/test_simulate_besttest.py'
          name       'test_best600'
-         firstlineno 21
+         firstlineno 23
          lnotab
-            0x020e2801360212011e0216010e0136010e01360b62043a013a018c018c
-            015a010e030e016a011001100110010e0232044c012a030c0130013a0116
-            fd12053402
-   names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'src.pybuildingenergy.source.utils', 'ISO52016', 'src.pybuildingenergy.data.building_archetype', 'Buildings_from_dictionary', 'src.pybuildingenergy.source.functions', 'ePlus_shape_data', 'get_buildings_demos', 'src.pybuildingenergy.source.graphs', 'bar_chart_single', 'pyecharts.globals', 'ThemeType', 'pandas', 'pd', 'os', 'path', 'dirname', 'realpath', '__file__', 'main_directory_', 'demo_buis', 'bt_600', 'weather_type', 'latitude_bui', 'longitude_bui', 'path_epls_file', 'path_weather_file_', 'path_chart_name', 'test_best600')
+            0x020e2801360212011e0216010e0136010e01360b62043a013a0102018c
+            018c015e0102018c018c0164020e030e016a011001100110010e0232044c
+            012a030c0130013a0116fd12053402
+   names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'src.pybuildingenergy.source.utils', 'ISO52016', 'src.pybuildingenergy.data.building_archetype', 'Buildings_from_dictionary', 'src.pybuildingenergy.source.functions', 'ePlus_shape_data', 'src.pybuildingenergy.source.graphs', 'bar_chart_single', 'pyecharts.globals', 'ThemeType', 'pandas', 'pd', 'os', 'pickle', 'input_data.src', 'main_directory_', 'get_buildings_demos', 'demo_buis', 'bt_600', 'weather_type', 'latitude_bui', 'longitude_bui', 'path_epls_file', 'path_weather_file_', 'path_chart_name', 'test_best600')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/MODERATE/pyBuildingEnergy/pybuildingenergy/tests/snapshots/test_simulate_besttest.py'
+   filename   '/Users/dantonucci/Library/CloudStorage/OneDrive-ScientificNetworkSouthTyrol/00_GitHubProject/pyBuildingEnergy/tests/test_simulate_besttest.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020126010c0110010c010c01080108026401140124010401040104
-      01040104010404
+      0x00ff020126010c010c010c010c01080108010801100216022401040104
+      0104010a010a010a04
```

### Comparing `pybuildingenergy-1.0.6/tests/snapshots/test_create_bui_obj/test_create_bui_obj/properties_inputs.yml` & `pybuildingenergy-1.0.7/tests/snapshots/test_create_bui_obj/test_create_bui_obj/properties_inputs.yml`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/snapshots/test_simulate_besttest/test_best600/data_best600_athens.json` & `pybuildingenergy-1.0.7/tests/snapshots/test_simulate_besttest/test_best600/data_best600_athens.json`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/snapshots/test_simulation_new_bui/test_simulation/hourly_sim.json` & `pybuildingenergy-1.0.7/tests/snapshots/test_simulation_new_bui/test_simulation/hourly_sim.json`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_create_bui_obj.py` & `pybuildingenergy-1.0.7/tests/test_create_bui_obj.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_create_report.py` & `pybuildingenergy-1.0.7/tests/test_create_report.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_simul_newbui_from_archetype.py` & `pybuildingenergy-1.0.7/tests/test_simul_newbui_from_archetype.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_simulate_archetype.py` & `pybuildingenergy-1.0.7/tests/test_simulate_archetype.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_simulate_besttest.py` & `pybuildingenergy-1.0.7/tests/test_simulate_besttest.py`

 * *Files identical despite different names*

### Comparing `pybuildingenergy-1.0.6/tests/test_simulation_new_bui.py` & `pybuildingenergy-1.0.7/tests/test_simulation_new_bui.py`

 * *Files identical despite different names*

