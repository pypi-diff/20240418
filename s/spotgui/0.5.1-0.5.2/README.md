# Comparing `tmp/spotgui-0.5.1.tar.gz` & `tmp/spotgui-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotgui-0.5.1.tar", last modified: Wed Apr 17 20:48:33 2024, max compression
+gzip compressed data, was "spotgui-0.5.2.tar", last modified: Thu Apr 18 21:13:41 2024, max compression
```

## Comparing `spotgui-0.5.1.tar` & `spotgui-0.5.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.646877 spotgui-0.5.1/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.578486 spotgui-0.5.1/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.581374 spotgui-0.5.1/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotgui-0.5.1/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotgui-0.5.1/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotgui-0.5.1/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.581531 spotgui-0.5.1/.vscode/
--rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotgui-0.5.1/.vscode/settings.json
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotgui-0.5.1/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)      131 2024-02-13 13:06:51.000000 spotgui-0.5.1/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-17 20:48:33.646651 spotgui-0.5.1/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotgui-0.5.1/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.582707 spotgui-0.5.1/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.583680 spotgui-0.5.1/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/plot-progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/surrogate-plot.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.584649 spotgui-0.5.1/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotgui-0.5.1/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-04-17 20:40:08.000000 spotgui-0.5.1/makeSpotGUI.sh
--rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotgui-0.5.1/mkdocs.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-17 20:38:56.000000 spotgui-0.5.1/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-17 20:48:33.646912 spotgui-0.5.1/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.585434 spotgui-0.5.1/spotPythonGUI/
--rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/00_test_spotGUI.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.585585 spotgui-0.5.1/spotPythonGUI/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotPythonGUI/spotPythonGUI.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.621537 spotgui-0.5.1/spotPythonGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/README.txt
--rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data.csv
--rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data.pkl
--rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data_sensitive.pkl
--rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.arff
--rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.csv
--rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.pkl
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.622323 spotgui-0.5.1/spotPythonGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.json
--rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.622774 spotgui-0.5.1/spotRiverGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.626288 spotgui-0.5.1/spotRiverGUI/db_dicts/
--rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/0001_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/000_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)   128965 2024-04-17 20:41:09.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/spotRiver_db_default.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.638829 spotgui-0.5.1/spotRiverGUI/demos/
--rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_demo_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.639033 spotgui-0.5.1/spotRiverGUI/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    63958 2024-04-17 20:47:54.000000 spotgui-0.5.1/spotRiverGUI/spotRiverGUI.py
--rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/spotRiverGUI_v01.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.642888 spotgui-0.5.1/spotRiverGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userData/PhishingData.csv
--rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotgui-0.5.1/spotRiverGUI/userData/PhishingData_license.txt
--rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
--rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotgui-0.5.1/spotRiverGUI/userData/phishingRiver.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userData/user_data.csv
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.643942 spotgui-0.5.1/spotRiverGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.290888 spotgui-0.5.1/spotRiverGUI/userPrepModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.291356 spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1143 2024-04-17 20:48:37.291238 spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_Bikes_river.py
--rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
--rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.579873 spotgui-0.5.1/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.579714 spotgui-0.5.1/src/spotGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644435 spotgui-0.5.1/src/spotGUI/ctk/
--rw-r--r--   0 bartz      (501) staff       (20)      720 2024-04-17 20:48:15.000000 spotgui-0.5.1/src/spotGUI/ctk/CTk.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644540 spotgui-0.5.1/src/spotGUI/eda/
--rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotgui-0.5.1/src/spotGUI/eda/pairplot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644918 spotgui-0.5.1/src/spotGUI/tuner/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.645388 spotgui-0.5.1/src/spotGUI/tuner/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)    29347 2024-04-08 13:05:32.000000 spotgui-0.5.1/src/spotGUI/tuner/spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/spot_00experiment.pickle
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.646325 spotgui-0.5.1/src/spotgui.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2365 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.291979 spotgui-0.5.1/test/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.292406 spotgui-0.5.1/test/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1921 2024-04-17 20:48:37.292321 spotgui-0.5.1/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1255 2024-04-04 08:28:25.000000 spotgui-0.5.1/test/test_spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotgui-0.5.1/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.947694 spotgui-0.5.2/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.852115 spotgui-0.5.2/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.856253 spotgui-0.5.2/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotgui-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotgui-0.5.2/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotgui-0.5.2/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.856522 spotgui-0.5.2/.vscode/
+-rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotgui-0.5.2/.vscode/settings.json
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotgui-0.5.2/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      168 2024-04-18 16:28:24.000000 spotgui-0.5.2/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-18 21:13:41.947445 spotgui-0.5.2/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotgui-0.5.2/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.857881 spotgui-0.5.2/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.859041 spotgui-0.5.2/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/plot-progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/surrogate-plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.860132 spotgui-0.5.2/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotgui-0.5.2/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-04-17 20:40:08.000000 spotgui-0.5.2/makeSpotGUI.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotgui-0.5.2/mkdocs.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-18 14:29:23.000000 spotgui-0.5.2/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-18 21:13:41.947730 spotgui-0.5.2/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.860701 spotgui-0.5.2/spotPythonGUI/
+-rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/00_test_spotGUI.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.861078 spotgui-0.5.2/spotPythonGUI/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotPythonGUI/spotPythonGUI.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.905448 spotgui-0.5.2/spotPythonGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/README.txt
+-rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data.pkl
+-rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data_sensitive.pkl
+-rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.arff
+-rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.pkl
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.906156 spotgui-0.5.2/spotPythonGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.json
+-rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.906808 spotgui-0.5.2/spotRiverGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.911871 spotgui-0.5.2/spotRiverGUI/db_dicts/
+-rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/0001_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/000_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)   248782 2024-04-18 21:11:09.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/spotRiver_db_default.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.926753 spotgui-0.5.2/spotRiverGUI/demos/
+-rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_demo_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)    46380 2024-04-18 21:05:08.000000 spotgui-0.5.2/spotRiverGUI/spotRiverGUI.py
+-rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/spotRiverGUI_v01.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.940292 spotgui-0.5.2/spotRiverGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userData/PhishingData.csv
+-rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotgui-0.5.2/spotRiverGUI/userData/PhishingData_license.txt
+-rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotgui-0.5.2/spotRiverGUI/userData/phishingRiver.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userData/user_data.csv
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.942291 spotgui-0.5.2/spotRiverGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userModel/__init__.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.919571 spotgui-0.5.2/spotRiverGUI/userPrepModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/__init__.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.920542 spotgui-0.5.2/spotRiverGUI/userPrepModel/__pycache__/
+-rw-r--r--   0 bartz      (501) staff       (20)     1143 2024-04-18 21:13:45.920358 spotgui-0.5.2/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc
+-rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_Bikes_river.py
+-rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.853555 spotgui-0.5.2/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.853427 spotgui-0.5.2/src/spotGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943085 spotgui-0.5.2/src/spotGUI/ctk/
+-rw-r--r--   0 bartz      (501) staff       (20)    16944 2024-04-18 19:48:47.000000 spotgui-0.5.2/src/spotGUI/ctk/CTk.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943651 spotgui-0.5.2/src/spotGUI/ctk/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.2/src/spotGUI/ctk/images/spotlogo.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943870 spotgui-0.5.2/src/spotGUI/eda/
+-rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotgui-0.5.2/src/spotGUI/eda/pairplot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.945526 spotgui-0.5.2/src/spotGUI/tuner/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.946035 spotgui-0.5.2/src/spotGUI/tuner/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29286 2024-04-18 19:34:33.000000 spotgui-0.5.2/src/spotGUI/tuner/spotRun.py
+-rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/spot_00experiment.pickle
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.947090 spotgui-0.5.2/src/spotgui.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2368 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.922270 spotgui-0.5.2/test/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.922782 spotgui-0.5.2/test/__pycache__/
+-rw-r--r--   0 bartz      (501) staff       (20)     1921 2024-04-18 21:13:45.922677 spotgui-0.5.2/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc
+-rw-r--r--   0 bartz      (501) staff       (20)     1255 2024-04-04 08:28:25.000000 spotgui-0.5.2/test/test_spotRun.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotgui-0.5.2/tox.ini
```

### Comparing `spotgui-0.5.1/.github/workflows/test.yml` & `spotgui-0.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/.gitignore` & `spotgui-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/.vscode/settings.json` & `spotgui-0.5.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/LICENSE.txt` & `spotgui-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/PKG-INFO` & `spotgui-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotgui
-Version: 0.5.1
+Version: 0.5.2
 Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotgui-0.5.1/README.md` & `spotgui-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/about.md` & `spotgui-0.5.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/examples.md` & `spotgui-0.5.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/gen_ref_pages.py` & `spotgui-0.5.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/images/favicon.png` & `spotgui-0.5.2/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/images/plot-progress.png` & `spotgui-0.5.2/docs/images/plot-progress.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/images/spotlogo.png` & `spotgui-0.5.2/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/docs/images/surrogate-plot.png` & `spotgui-0.5.2/docs/images/surrogate-plot.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/img/favicon.png` & `spotgui-0.5.2/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/img/spotLogo.png` & `spotgui-0.5.2/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/mkdocs.yml` & `spotgui-0.5.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/pyproject.toml` & `spotgui-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotgui"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotgui - GUI for the Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotgui-0.5.1/spotPythonGUI/00_test_spotGUI.ipynb` & `spotgui-0.5.2/spotPythonGUI/00_test_spotGUI.ipynb`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/images/spotlogo.png` & `spotgui-0.5.2/spotPythonGUI/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/spotPythonGUI.py` & `spotgui-0.5.2/spotPythonGUI/spotPythonGUI.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/README.txt` & `spotgui-0.5.2/spotPythonGUI/userData/README.txt`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/data.csv` & `spotgui-0.5.2/spotPythonGUI/userData/data.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/data.pkl` & `spotgui-0.5.2/spotPythonGUI/userData/data.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/data_sensitive.pkl` & `spotgui-0.5.2/spotPythonGUI/userData/data_sensitive.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/diabetes.arff` & `spotgui-0.5.2/spotPythonGUI/userData/diabetes.arff`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/diabetes.csv` & `spotgui-0.5.2/spotPythonGUI/userData/diabetes.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userData/diabetes.pkl` & `spotgui-0.5.2/spotPythonGUI/userData/diabetes.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.json` & `spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.py` & `spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/db_dicts/0001_spotRiver_db.json` & `spotgui-0.5.2/spotRiverGUI/db_dicts/0001_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/db_dicts/000_spotRiver_db.json` & `spotgui-0.5.2/spotRiverGUI/db_dicts/000_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/db_dicts/spotRiver_db.json` & `spotgui-0.5.2/spotRiverGUI/db_dicts/spotRiver_db.json`

 * *Files 26% similar despite different names*

```diff
@@ -9,7 +9,20 @@
 {"data": {"id": "0011_1712582053.3642502", "result": "Results for 0011_1712582053.3642502: Finally, the best value is 49092.626894429006 at [ 4.63529627e-03 -2.21528408e-01  1.91626325e-02  1.30000000e+01].", "fun_control": {"PREFIX": "0011", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/0011_bartz10_2024-04-08_15-14-05", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.00614640280907866, 0.907236745286742, 0.013701435486708036, 12.0], [0.0061453615911764865, 0.9072367812154017, 0.013703275082409747, 12.0], [0.006129996864963464, 0.9072422649768427, 0.015689324614936842, 12.0], [0.007729454383435174, 0.9072386414315836, 0.01423661186284622, 12.0], [0.00849988305832269, -0.2624080408871876, 0.02, 13.0], [0.006473363789700801, 0.9072410989707684, 0.014290904952659115, 12.0], [0.00789610505717209, -0.23509124410557922, 0.02, 13.0], [0.0, -0.23741774992516046, 0.02, 13.0], [0.008229252019576068, 0.9073322995475779, 0.014123029532185083, 12.0], [0.007764244387675478, 0.9074029467392795, 0.01444562119477221, 12.0], [0.01, -0.34492752645793284, 0.013014243418533411, 13.0], [0.007069221948104332, 0.9082484154757392, 0.02, 12.0], [0.009591721961340685, -0.23869141056245657, 0.018579548773751505, 13.0], [0.00586926925439178, -0.23877062155947118, 0.02, 13.0], [0.0030084743687284914, -0.23812028214782194, 0.02, 13.0], [0.004047426214272552, -0.2375093598817126, 0.02, 13.0], [0.004057923211001897, -0.2369217134845787, 0.02, 13.0], [0.004503349294623389, -0.2363386530116154, 0.02, 13.0], [0.0026189518445567882, 0.9248805772644714, 0.02, 12.0], [0.004697752267928726, 0.9593987638352577, 0.02, 12.0], [0.007179565865669419, 0.9463227461630754, 0.02, 12.0], [0.007369592779890063, 0.9464187731448722, 0.02, 12.0], [0.00827567330746704, -0.23594310199507745, 0.02, 13.0], [0.008145870635232555, 0.9459080214874698, 0.02, 12.0], [0.006933530502234274, -0.23496250937363736, 0.015330779627003507, 13.0]], "y": [49092.626894429006, 93216.0612089007, 111455.49507642689, 73889.69967304362, 64484.55237722101, 63444.83662368577, 63442.149504635156, 60083.45681212693, 62471.162280324614, 55526.29140110908, 62375.433127082586, 55512.16917977503, 55508.93954243419, 62668.27277508465, 62104.09021414286, 64995.422293362666, 55410.122204500636, 56680.16208468794, 55492.317731482486, 55491.35698626022, 55489.89043955538, 55488.70213992095, 55487.53914011822, 55398.31660670533, 55394.4687808012, 55394.25088003774, 55393.45882072059, 55482.84626103966, 55392.01562330214, 60791.379473268484], "counter": 30, "min_y": 49092.626894429006, "min_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_y": 49092.626894429006, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.00614640280907866, 0.907236745286742, 0.013701435486708036, 12.0], [0.0061453615911764865, 0.9072367812154017, 0.013703275082409747, 12.0], [0.006129996864963464, 0.9072422649768427, 0.015689324614936842, 12.0], [0.007729454383435174, 0.9072386414315836, 0.01423661186284622, 12.0], [0.00849988305832269, -0.2624080408871876, 0.02, 13.0], [0.006473363789700801, 0.9072410989707684, 0.014290904952659115, 12.0], [0.00789610505717209, -0.23509124410557922, 0.02, 13.0], [0.0, -0.23741774992516046, 0.02, 13.0], [0.008229252019576068, 0.9073322995475779, 0.014123029532185083, 12.0], [0.007764244387675478, 0.9074029467392795, 0.01444562119477221, 12.0], [0.01, -0.34492752645793284, 0.013014243418533411, 13.0], [0.007069221948104332, 0.9082484154757392, 0.02, 12.0], [0.009591721961340685, -0.23869141056245657, 0.018579548773751505, 13.0], [0.00586926925439178, -0.23877062155947118, 0.02, 13.0], [0.0030084743687284914, -0.23812028214782194, 0.02, 13.0], [0.004047426214272552, -0.2375093598817126, 0.02, 13.0], [0.004057923211001897, -0.2369217134845787, 0.02, 13.0], [0.004503349294623389, -0.2363386530116154, 0.02, 13.0], [0.0026189518445567882, 0.9248805772644714, 0.02, 12.0], [0.004697752267928726, 0.9593987638352577, 0.02, 12.0], [0.007179565865669419, 0.9463227461630754, 0.02, 12.0], [0.007369592779890063, 0.9464187731448722, 0.02, 12.0], [0.00827567330746704, -0.23594310199507745, 0.02, 13.0], [0.008145870635232555, 0.9459080214874698, 0.02, 12.0], [0.006933530502234274, -0.23496250937363736, 0.015330779627003507, 13.0]], "mean_y": [49092.626894429006, 93216.0612089007, 111455.49507642689, 73889.69967304362, 64484.55237722101, 63444.83662368577, 63442.149504635156, 60083.45681212693, 62471.162280324614, 55526.29140110908, 62375.433127082586, 55512.16917977503, 55508.93954243419, 62668.27277508465, 62104.09021414286, 64995.422293362666, 55410.122204500636, 56680.16208468794, 55492.317731482486, 55491.35698626022, 55489.89043955538, 55488.70213992095, 55487.53914011822, 55398.31660670533, 55394.4687808012, 55394.25088003774, 55393.45882072059, 55482.84626103966, 55392.01562330214, 60791.379473268484], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "0011_1712583296.904823", "result": "Results for 0011_1712583296.904823: Finally, the best value is 49138.99118166437 at [ 7.19608023e-03 -6.84607006e-01  1.61355271e-02  1.20000000e+01].", "fun_control": {"PREFIX": "0011", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/0011_p040025_2024-04-08_15-34-37", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 6, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.00719608022791976, -0.6846070062674076, 0.016135527069553394, 12.0], [0.0030401568315249496, -0.6040315022185911, 0.007576074172914321, 12.0], [0.008633742397344997, 0.036702435629604624, 0.0025422602251064822, 12.0], [0.0036262640065043146, 0.9287456788749682, 0.0049853543345900865, 11.0], [0.005120987902458055, 0.5893639371311936, 0.011136103759369739, 13.0], [0.0012807406253048876, -0.05530133108024815, 0.01842366826642365, 12.0], [0.007792330004030803, -0.689610571404427, 0.01666708915182653, 12.0], [0.007744716040407038, -0.6925562272419424, 0.016979952349320086, 12.0], [0.0017844140821041928, -0.08954143074995509, 0.004413318194434632, 12.0], [0.007831039704643558, -0.6945236912883185, 0.01718896692037227, 12.0], [0.003809067132567191, -0.6972611373861497, 0.019436047572234726, 12.0], [0.009131446485647253, -0.6994114063895233, 0.009877649400942646, 12.0], [0.008909272005089196, -0.6959899349122515, 0.015700664568689994, 12.0], [0.0078065524861928755, -0.6957824639369029, 0.019536573860744588, 12.0], [0.0020536976971001313, -0.6955475402337593, 0.007142495263480954, 12.0], [0.005208110175496896, -0.6949971474715064, 0.01805582539759546, 12.0], [0.004319434764043885, -0.6949189067870749, 0.02, 12.0], [0.005481407140467216, -0.694760909566854, 0.02, 12.0], [0.0038955262065404335, -0.6943470935046051, 0.02, 12.0], [0.0021561206936889957, -0.6935785653753979, 0.02, 12.0], [0.005677373211343897, -0.6922696126962893, 0.02, 12.0], [0.007001440420017905, -0.6899997884167285, 0.02, 12.0], [0.009626828976650357, -0.6850154983173585, 0.02, 12.0], [0.006981593373295948, -0.6681495668814705, 0.02, 12.0], [0.003922685553379487, -0.6694049496690428, 0.02, 12.0], [0.01, -0.6695692290761467, 0.02, 12.0], [0.01, -0.6697187625125982, 0.02, 12.0], [0.007731835581564724, -0.6698834824639371, 0.02, 12.0], [0.006865881300811069, -0.6700521002972565, 0.02, 12.0], [0.009299119146572908, -0.03574835657173338, 0.02, 12.0]], "y": [49138.99118166437, 80893.1163446481, 114162.70628116961, 95051.70002655852, 69177.49855822364, 56873.311169727254, 58901.04809525298, 58488.92381246161, 99715.83722725316, 58216.49336189274, 55991.83398568038, 73107.99394327424, 60276.35088165927, 55894.01872869484, 83782.22049029358, 57248.30789562812, 55531.24212472715, 55529.067605181575, 55527.531807634135, 55526.25280727963, 55524.323874456975, 55522.79924607483, 55521.00941750175, 55519.18931328442, 55518.855137189756, 55517.12631391772, 55516.372145243084, 55516.01404342042, 55515.49257961302, 55466.129504867975], "counter": 30, "min_y": 49138.99118166437, "min_X": [0.00719608022791976, -0.6846070062674076, 0.016135527069553394, 12.0], "min_mean_X": [0.00719608022791976, -0.6846070062674076, 0.016135527069553394, 12.0], "min_mean_y": 49138.99118166437, "mean_X": [[0.00719608022791976, -0.6846070062674076, 0.016135527069553394, 12.0], [0.0030401568315249496, -0.6040315022185911, 0.007576074172914321, 12.0], [0.008633742397344997, 0.036702435629604624, 0.0025422602251064822, 12.0], [0.0036262640065043146, 0.9287456788749682, 0.0049853543345900865, 11.0], [0.005120987902458055, 0.5893639371311936, 0.011136103759369739, 13.0], [0.0012807406253048876, -0.05530133108024815, 0.01842366826642365, 12.0], [0.007792330004030803, -0.689610571404427, 0.01666708915182653, 12.0], [0.007744716040407038, -0.6925562272419424, 0.016979952349320086, 12.0], [0.0017844140821041928, -0.08954143074995509, 0.004413318194434632, 12.0], [0.007831039704643558, -0.6945236912883185, 0.01718896692037227, 12.0], [0.003809067132567191, -0.6972611373861497, 0.019436047572234726, 12.0], [0.009131446485647253, -0.6994114063895233, 0.009877649400942646, 12.0], [0.008909272005089196, -0.6959899349122515, 0.015700664568689994, 12.0], [0.0078065524861928755, -0.6957824639369029, 0.019536573860744588, 12.0], [0.0020536976971001313, -0.6955475402337593, 0.007142495263480954, 12.0], [0.005208110175496896, -0.6949971474715064, 0.01805582539759546, 12.0], [0.004319434764043885, -0.6949189067870749, 0.02, 12.0], [0.005481407140467216, -0.694760909566854, 0.02, 12.0], [0.0038955262065404335, -0.6943470935046051, 0.02, 12.0], [0.0021561206936889957, -0.6935785653753979, 0.02, 12.0], [0.005677373211343897, -0.6922696126962893, 0.02, 12.0], [0.007001440420017905, -0.6899997884167285, 0.02, 12.0], [0.009626828976650357, -0.6850154983173585, 0.02, 12.0], [0.006981593373295948, -0.6681495668814705, 0.02, 12.0], [0.003922685553379487, -0.6694049496690428, 0.02, 12.0], [0.01, -0.6695692290761467, 0.02, 12.0], [0.01, -0.6697187625125982, 0.02, 12.0], [0.007731835581564724, -0.6698834824639371, 0.02, 12.0], [0.006865881300811069, -0.6700521002972565, 0.02, 12.0], [0.009299119146572908, -0.03574835657173338, 0.02, 12.0]], "mean_y": [49138.99118166437, 80893.1163446481, 114162.70628116961, 95051.70002655852, 69177.49855822364, 56873.311169727254, 58901.04809525298, 58488.92381246161, 99715.83722725316, 58216.49336189274, 55991.83398568038, 73107.99394327424, 60276.35088165927, 55894.01872869484, 83782.22049029358, 57248.30789562812, 55531.24212472715, 55529.067605181575, 55527.531807634135, 55526.25280727963, 55524.323874456975, 55522.79924607483, 55521.00941750175, 55519.18931328442, 55518.855137189756, 55517.12631391772, 55516.372145243084, 55516.01404342042, 55515.49257961302, 55466.129504867975], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "000_1713376338.834367", "result": "Results for 000_1713376338.834367: Finally, the best value is 475697.8999644927 at [6.5097773e-03 9.0715451e-01 2.0000000e-02 1.2000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-17_19-52-12", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145262664645979, 0.9072367143924788, 0.013162742524562463, 12.0], [0.006144501454580373, 0.9072369027054826, 0.015477170051869799, 12.0], [0.007729874771461144, 0.9072368990845396, 0.014187757227531099, 12.0], [0.0073423312109991935, -0.2630517031151739, 0.02, 13.0], [0.007453781117137888, 0.9072405423662437, 0.014210525580741974, 12.0], [0.0024150114751207807, -0.24471463642678074, 0.02, 13.0], [0.006771224320969215, -0.2451162846260436, 0.02, 13.0], [0.00019177880267834738, -0.24495011812373355, 0.019279879392758367, 13.0], [0.01, -0.24494378678321996, 0.02, 13.0], [0.01, -0.24465919194476046, 0.02, 13.0], [0.0017763465426160491, -0.2444110396797722, 0.011294474511639783, 13.0], [0.006919681187530084, 0.9072397245332889, 0.013415919840462837, 12.0], [0.0069196835230138695, 0.9072377624023926, 0.013416032000833984, 12.0], [0.0069196827260243985, 0.9072378996479578, 0.013416135708492429, 12.0], [0.006919682446898545, 0.9072378965773439, 0.013416238454558116, 12.0], [0.0069196821451389225, 0.9072378961198646, 0.013416341307142216, 12.0], [0.006919681587838023, 0.9072378975232593, 0.01341644522838692, 12.0], [0.006919681303370059, 0.9072378958931041, 0.013416549826199272, 12.0], [0.006919681573420602, 0.9072378975946622, 0.013416655169843809, 12.0], [0.008863906331911585, 0.9072379636818124, 0.015490378487900478, 12.0], [0.0062065706901347955, 0.90723561425858, 0.013089864192586847, 12.0], [0.006206707521673508, 0.9072426497490849, 0.013091199052724186, 12.0], [0.009131440518517001, 0.9072314843282391, 0.016777367227508454, 12.0], [0.006509777298826815, 0.9071545100124566, 0.02, 12.0], [0.005642382115145721, 0.9058892326904646, 0.02, 12.0]], "y": [495715.30301175296, 1028781.8853182528, 1195926.3482211772, 791704.1296318508, 650349.5120075233, 650368.461405819, 581323.2172666056, 618217.2760177538, 478498.4205094595, 617543.9136535891, 478647.36709080223, 478477.400440405, 493477.9873124843, 478350.2845636698, 478349.5954129688, 720335.744386252, 642177.3281814052, 642173.754512358, 642170.4437433786, 642167.1641731495, 642163.8812213818, 642160.5641742123, 642157.2255774959, 642153.8631589635, 580856.3470166868, 652746.0475152271, 652702.3064251711, 547299.5335861085, 475697.8999644927, 475734.9991441419], "counter": 30, "min_y": 475697.8999644927, "min_X": [0.006509777298826815, 0.9071545100124566, 0.02, 12.0], "min_mean_X": [0.006509777298826815, 0.9071545100124566, 0.02, 12.0], "min_mean_y": 475697.8999644927, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145262664645979, 0.9072367143924788, 0.013162742524562463, 12.0], [0.006144501454580373, 0.9072369027054826, 0.015477170051869799, 12.0], [0.007729874771461144, 0.9072368990845396, 0.014187757227531099, 12.0], [0.0073423312109991935, -0.2630517031151739, 0.02, 13.0], [0.007453781117137888, 0.9072405423662437, 0.014210525580741974, 12.0], [0.0024150114751207807, -0.24471463642678074, 0.02, 13.0], [0.006771224320969215, -0.2451162846260436, 0.02, 13.0], [0.00019177880267834738, -0.24495011812373355, 0.019279879392758367, 13.0], [0.01, -0.24494378678321996, 0.02, 13.0], [0.01, -0.24465919194476046, 0.02, 13.0], [0.0017763465426160491, -0.2444110396797722, 0.011294474511639783, 13.0], [0.006919681187530084, 0.9072397245332889, 0.013415919840462837, 12.0], [0.0069196835230138695, 0.9072377624023926, 0.013416032000833984, 12.0], [0.0069196827260243985, 0.9072378996479578, 0.013416135708492429, 12.0], [0.006919682446898545, 0.9072378965773439, 0.013416238454558116, 12.0], [0.0069196821451389225, 0.9072378961198646, 0.013416341307142216, 12.0], [0.006919681587838023, 0.9072378975232593, 0.01341644522838692, 12.0], [0.006919681303370059, 0.9072378958931041, 0.013416549826199272, 12.0], [0.006919681573420602, 0.9072378975946622, 0.013416655169843809, 12.0], [0.008863906331911585, 0.9072379636818124, 0.015490378487900478, 12.0], [0.0062065706901347955, 0.90723561425858, 0.013089864192586847, 12.0], [0.006206707521673508, 0.9072426497490849, 0.013091199052724186, 12.0], [0.009131440518517001, 0.9072314843282391, 0.016777367227508454, 12.0], [0.006509777298826815, 0.9071545100124566, 0.02, 12.0], [0.005642382115145721, 0.9058892326904646, 0.02, 12.0]], "mean_y": [495715.30301175296, 1028781.8853182528, 1195926.3482211772, 791704.1296318508, 650349.5120075233, 650368.461405819, 581323.2172666056, 618217.2760177538, 478498.4205094595, 617543.9136535891, 478647.36709080223, 478477.400440405, 493477.9873124843, 478350.2845636698, 478349.5954129688, 720335.744386252, 642177.3281814052, 642173.754512358, 642170.4437433786, 642167.1641731495, 642163.8812213818, 642160.5641742123, 642157.2255774959, 642153.8631589635, 580856.3470166868, 652746.0475152271, 652702.3064251711, 547299.5335861085, 475697.8999644927, 475734.9991441419], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "001_1713378173.903429", "result": "Results for 001_1713378173.903429: Finally, the best value is 475442.85806873086 at [1.00000000e-02 9.55930062e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "001", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/001_bartz10_2024-04-17_20-22-46", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.00614520274891448, 0.9072367573106274, 0.01316308872115215, 12.0], [0.006140159984972868, 0.9072377774339726, 0.015476096171648397, 12.0], [0.007729801332590411, 0.9072373093134973, 0.014187265896945283, 12.0], [0.007342321606458159, -0.2630515858090087, 0.02, 13.0], [0.008150000247945585, 0.907245283370693, 0.01428673076089107, 12.0], [0.0024194006855968223, -0.24472858882554896, 0.02, 13.0], [0.008921453381733347, 0.9073104968953211, 0.02, 12.0], [0.01, -0.25107836130062766, 0.02, 13.0], [0.007274367409976721, -0.2496919215927854, 0.02, 13.0], [0.004621491433736333, -0.24874730395977085, 0.01993580179774948, 13.0], [0.004036096218903718, -0.24806281332964364, 0.02, 13.0], [0.01, -0.24753594623144917, 0.02, 13.0], [0.0016677933327231198, -0.24712032910526766, 0.02, 13.0], [0.01, 0.9094605697983313, 0.02, 12.0], [0.005244423324637369, -0.24824969205367567, 0.02, 13.0], [0.007731670921862507, -0.24780463666052507, 0.01893371276591512, 13.0], [0.0031176085478997464, -0.24757340970593075, 0.02, 13.0], [0.007255968217894876, -0.24722912192323748, 0.02, 13.0], [0.004403830153628333, -0.24692697626588364, 0.02, 13.0], [0.01, 0.9472054252109227, 0.02, 12.0], [0.01, 0.9559300616911349, 0.02, 12.0], [0.008123569469719235, 0.9555559747851857, 0.02, 12.0], [0.01, 0.9551761542443105, 0.02, 12.0], [0.01, 0.954817078499404, 0.02, 12.0], [0.002481292314446936, 0.9544649529252911, 0.02, 12.0]], "y": [495715.3029471603, 1028781.8852915328, 1195926.3482179178, 791704.1296370823, 650349.5119972338, 650357.1896282742, 581352.7255286095, 618232.0531961464, 478498.4205653932, 615235.5316337625, 478647.2286382193, 475602.89013680076, 478365.13932720345, 478468.73680781416, 479856.24444493133, 478591.86276786466, 478356.56141238764, 478682.5135433288, 475555.3634094125, 478544.90014872595, 500542.97757204936, 478626.71942561405, 478463.4951529148, 478574.68234141637, 475463.9809198616, 475442.85806873086, 475517.39333573927, 475444.6833295286, 475445.5526709407, 475741.43305638083], "counter": 30, "min_y": 475442.85806873086, "min_X": [0.01, 0.9559300616911349, 0.02, 12.0], "min_mean_X": [0.01, 0.9559300616911349, 0.02, 12.0], "min_mean_y": 475442.85806873086, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.00614520274891448, 0.9072367573106274, 0.01316308872115215, 12.0], [0.006140159984972868, 0.9072377774339726, 0.015476096171648397, 12.0], [0.007729801332590411, 0.9072373093134973, 0.014187265896945283, 12.0], [0.007342321606458159, -0.2630515858090087, 0.02, 13.0], [0.008150000247945585, 0.907245283370693, 0.01428673076089107, 12.0], [0.0024194006855968223, -0.24472858882554896, 0.02, 13.0], [0.008921453381733347, 0.9073104968953211, 0.02, 12.0], [0.01, -0.25107836130062766, 0.02, 13.0], [0.007274367409976721, -0.2496919215927854, 0.02, 13.0], [0.004621491433736333, -0.24874730395977085, 0.01993580179774948, 13.0], [0.004036096218903718, -0.24806281332964364, 0.02, 13.0], [0.01, -0.24753594623144917, 0.02, 13.0], [0.0016677933327231198, -0.24712032910526766, 0.02, 13.0], [0.01, 0.9094605697983313, 0.02, 12.0], [0.005244423324637369, -0.24824969205367567, 0.02, 13.0], [0.007731670921862507, -0.24780463666052507, 0.01893371276591512, 13.0], [0.0031176085478997464, -0.24757340970593075, 0.02, 13.0], [0.007255968217894876, -0.24722912192323748, 0.02, 13.0], [0.004403830153628333, -0.24692697626588364, 0.02, 13.0], [0.01, 0.9472054252109227, 0.02, 12.0], [0.01, 0.9559300616911349, 0.02, 12.0], [0.008123569469719235, 0.9555559747851857, 0.02, 12.0], [0.01, 0.9551761542443105, 0.02, 12.0], [0.01, 0.954817078499404, 0.02, 12.0], [0.002481292314446936, 0.9544649529252911, 0.02, 12.0]], "mean_y": [495715.3029471603, 1028781.8852915328, 1195926.3482179178, 791704.1296370823, 650349.5119972338, 650357.1896282742, 581352.7255286095, 618232.0531961464, 478498.4205653932, 615235.5316337625, 478647.2286382193, 475602.89013680076, 478365.13932720345, 478468.73680781416, 479856.24444493133, 478591.86276786466, 478356.56141238764, 478682.5135433288, 475555.3634094125, 478544.90014872595, 500542.97757204936, 478626.71942561405, 478463.4951529148, 478574.68234141637, 475463.9809198616, 475442.85806873086, 475517.39333573927, 475444.6833295286, 475445.5526709407, 475741.43305638083], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "000112_1713378298.61094", "result": "Results for 000112_1713378298.61094: Finally, the best value is 475450.4992975737 at [9.79614523e-03 9.56077873e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000112", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000112_bartz10_2024-04-17_20-24-51", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061456978094570755, 0.9072367329225511, 0.01316274420364091, 12.0], [0.00612866736615691, 0.9072424642985943, 0.015478346780712412, 12.0], [0.007729648809427371, 0.9072393831858722, 0.014188387316618017, 12.0], [0.007342335731786966, -0.2630518588876364, 0.02, 13.0], [0.008149838630735217, 0.9072476589567693, 0.014288174205044185, 12.0], [0.0024207949843279095, -0.2447316448350897, 0.02, 13.0], [0.00596726248817429, 0.907455065096563, 0.02, 12.0], [0.003913141979674186, -0.25106580449246496, 0.02, 13.0], [0.003220261640985554, 0.9109744615801779, 0.02, 12.0], [0.009631137503873467, -0.25144951885839384, 0.02, 13.0], [0.006871568668011904, -0.2501970380853746, 0.017861925268531448, 13.0], [0.003955340655974394, -0.2495318710482366, 0.02, 13.0], [0.008470181474491151, -0.24870627855964786, 0.02, 13.0], [0.00401505222049265, -0.24801161575713837, 0.017124691193337403, 13.0], [0.0, 0.9473808042690327, 0.02, 12.0], [0.0014669903379528992, 0.9562564277182433, 0.02, 12.0], [0.009796145230083998, 0.956077872731367, 0.02, 12.0], [0.0, 0.9556498305209826, 0.02, 12.0], [0.0022780557216195776, 0.9551354157880186, 0.02, 12.0], [0.003120781872753028, 0.9546319098117204, 0.02, 12.0], [0.0048597862561232715, 0.9541444353338169, 0.006360002238284238, 12.0], [0.0050054196687566764, -0.26471980130472483, 0.02, 13.0], [0.0011837152627398875, -0.26428754682329575, 0.02, 13.0], [0.0013622614130950924, -0.2638368239900576, 0.02, 13.0], [0.00019365777147082032, -0.2633951304744289, 0.017362973614046977, 13.0]], "y": [495715.30291950295, 1028781.8852733849, 1195926.3482190212, 791704.1296192281, 650349.5119691989, 650368.3897403397, 581291.6698102839, 618198.3291988001, 478498.4206755073, 615192.4455013577, 478647.18132756295, 475718.4601344711, 478603.9592574051, 475817.7295096724, 478380.51237974945, 524510.782319411, 478598.5889437638, 478419.42595110834, 542163.6532688641, 475855.9478654892, 475776.89617010514, 475450.4992975737, 475835.9280775567, 475747.78466612985, 475715.93580011703, 947051.0641909007, 478594.16094721114, 478743.07916109636, 478734.98154414986, 536583.0128412006], "counter": 30, "min_y": 475450.4992975737, "min_X": [0.009796145230083998, 0.956077872731367, 0.02, 12.0], "min_mean_X": [0.009796145230083998, 0.956077872731367, 0.02, 12.0], "min_mean_y": 475450.4992975737, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061456978094570755, 0.9072367329225511, 0.01316274420364091, 12.0], [0.00612866736615691, 0.9072424642985943, 0.015478346780712412, 12.0], [0.007729648809427371, 0.9072393831858722, 0.014188387316618017, 12.0], [0.007342335731786966, -0.2630518588876364, 0.02, 13.0], [0.008149838630735217, 0.9072476589567693, 0.014288174205044185, 12.0], [0.0024207949843279095, -0.2447316448350897, 0.02, 13.0], [0.00596726248817429, 0.907455065096563, 0.02, 12.0], [0.003913141979674186, -0.25106580449246496, 0.02, 13.0], [0.003220261640985554, 0.9109744615801779, 0.02, 12.0], [0.009631137503873467, -0.25144951885839384, 0.02, 13.0], [0.006871568668011904, -0.2501970380853746, 0.017861925268531448, 13.0], [0.003955340655974394, -0.2495318710482366, 0.02, 13.0], [0.008470181474491151, -0.24870627855964786, 0.02, 13.0], [0.00401505222049265, -0.24801161575713837, 0.017124691193337403, 13.0], [0.0, 0.9473808042690327, 0.02, 12.0], [0.0014669903379528992, 0.9562564277182433, 0.02, 12.0], [0.009796145230083998, 0.956077872731367, 0.02, 12.0], [0.0, 0.9556498305209826, 0.02, 12.0], [0.0022780557216195776, 0.9551354157880186, 0.02, 12.0], [0.003120781872753028, 0.9546319098117204, 0.02, 12.0], [0.0048597862561232715, 0.9541444353338169, 0.006360002238284238, 12.0], [0.0050054196687566764, -0.26471980130472483, 0.02, 13.0], [0.0011837152627398875, -0.26428754682329575, 0.02, 13.0], [0.0013622614130950924, -0.2638368239900576, 0.02, 13.0], [0.00019365777147082032, -0.2633951304744289, 0.017362973614046977, 13.0]], "mean_y": [495715.30291950295, 1028781.8852733849, 1195926.3482190212, 791704.1296192281, 650349.5119691989, 650368.3897403397, 581291.6698102839, 618198.3291988001, 478498.4206755073, 615192.4455013577, 478647.18132756295, 475718.4601344711, 478603.9592574051, 475817.7295096724, 478380.51237974945, 524510.782319411, 478598.5889437638, 478419.42595110834, 542163.6532688641, 475855.9478654892, 475776.89617010514, 475450.4992975737, 475835.9280775567, 475747.78466612985, 475715.93580011703, 947051.0641909007, 478594.16094721114, 478743.07916109636, 478734.98154414986, 536583.0128412006], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "000_1713384849.9657128", "result": "Results for 000_1713384849.9657128: Finally, the best value is 475448.3434750501 at [9.85092495e-03 9.56080487e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-17_22-14-02", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061452644255907095, 0.9072367161492362, 0.013162742885295764, 12.0], [0.006128480932647417, 0.9072424647295819, 0.015478235023145772, 12.0], [0.007729652430687734, 0.9072393727760801, 0.014188333694331349, 12.0], [0.007342334549240134, -0.263051846061673, 0.02, 13.0], [0.008149823423713355, 0.9072476437512365, 0.014288096124720168, 12.0], [0.002415526853837616, -0.24473165569312125, 0.02, 13.0], [0.00596695702056377, 0.9074552521352073, 0.02, 12.0], [0.00391338470697982, -0.2510658179185966, 0.02, 13.0], [0.0032190906977868916, 0.910977873568587, 0.02, 12.0], [0.009615799129099665, -0.251448664603145, 0.02, 13.0], [0.006871571549687478, -0.2501960749510464, 0.017861927361674357, 13.0], [0.00396298384278053, -0.2495311860237338, 0.02, 13.0], [0.008493926090613406, -0.248705329642635, 0.02, 13.0], [0.00401504521901348, -0.2480107045484442, 0.01712468842797665, 13.0], [0.0022693597646003066, 0.9474026532802666, 0.02, 12.0], [0.002581054192623153, 0.956267066171554, 0.02, 12.0], [0.009850924948393772, 0.9560804869495009, 0.02, 12.0], [0.00798192222921999, 0.9556473634510392, 0.02, 12.0], [0.002208452546210015, 0.9551513112441312, 0.02, 12.0], [0.0, 0.9546402318617693, 0.02, 12.0], [0.0038586664870226737, 0.9541455948245179, 0.02, 12.0], [0.006532759027733677, 0.9536737692847267, 0.014960320614761588, 12.0], [0.009158731588643373, 0.954523029034684, 0.02, 12.0], [0.0, 0.9545717072033338, 0.02, 12.0], [0.0, 0.9545534844289368, 0.02, 12.0]], "y": [495715.3029674892, 1028781.8853009613, 1195926.3482290679, 791704.129640242, 650349.5119902183, 650368.4496156994, 581294.7302496836, 618199.9415650297, 478498.4206963104, 615194.7766193249, 478647.38806843245, 475718.47167354525, 478603.94975343224, 475817.7671977579, 478381.11220179737, 524510.7310888834, 478598.28736182797, 478418.491899237, 542163.718583719, 475766.8473536951, 475733.1554726683, 475448.3434750501, 475522.73020595, 475750.4773632681, 475838.37237908476, 475688.1592264548, 595556.4692914279, 475479.27525955805, 475838.5383022585, 475838.58240408736], "counter": 30, "min_y": 475448.3434750501, "min_X": [0.009850924948393772, 0.9560804869495009, 0.02, 12.0], "min_mean_X": [0.009850924948393772, 0.9560804869495009, 0.02, 12.0], "min_mean_y": 475448.3434750501, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061452644255907095, 0.9072367161492362, 0.013162742885295764, 12.0], [0.006128480932647417, 0.9072424647295819, 0.015478235023145772, 12.0], [0.007729652430687734, 0.9072393727760801, 0.014188333694331349, 12.0], [0.007342334549240134, -0.263051846061673, 0.02, 13.0], [0.008149823423713355, 0.9072476437512365, 0.014288096124720168, 12.0], [0.002415526853837616, -0.24473165569312125, 0.02, 13.0], [0.00596695702056377, 0.9074552521352073, 0.02, 12.0], [0.00391338470697982, -0.2510658179185966, 0.02, 13.0], [0.0032190906977868916, 0.910977873568587, 0.02, 12.0], [0.009615799129099665, -0.251448664603145, 0.02, 13.0], [0.006871571549687478, -0.2501960749510464, 0.017861927361674357, 13.0], [0.00396298384278053, -0.2495311860237338, 0.02, 13.0], [0.008493926090613406, -0.248705329642635, 0.02, 13.0], [0.00401504521901348, -0.2480107045484442, 0.01712468842797665, 13.0], [0.0022693597646003066, 0.9474026532802666, 0.02, 12.0], [0.002581054192623153, 0.956267066171554, 0.02, 12.0], [0.009850924948393772, 0.9560804869495009, 0.02, 12.0], [0.00798192222921999, 0.9556473634510392, 0.02, 12.0], [0.002208452546210015, 0.9551513112441312, 0.02, 12.0], [0.0, 0.9546402318617693, 0.02, 12.0], [0.0038586664870226737, 0.9541455948245179, 0.02, 12.0], [0.006532759027733677, 0.9536737692847267, 0.014960320614761588, 12.0], [0.009158731588643373, 0.954523029034684, 0.02, 12.0], [0.0, 0.9545717072033338, 0.02, 12.0], [0.0, 0.9545534844289368, 0.02, 12.0]], "mean_y": [495715.3029674892, 1028781.8853009613, 1195926.3482290679, 791704.129640242, 650349.5119902183, 650368.4496156994, 581294.7302496836, 618199.9415650297, 478498.4206963104, 615194.7766193249, 478647.38806843245, 475718.47167354525, 478603.94975343224, 475817.7671977579, 478381.11220179737, 524510.7310888834, 478598.28736182797, 478418.491899237, 542163.718583719, 475766.8473536951, 475733.1554726683, 475448.3434750501, 475522.73020595, 475750.4773632681, 475838.37237908476, 475688.1592264548, 595556.4692914279, 475479.27525955805, 475838.5383022585, 475838.58240408736], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
 {"data": {"id": "000_1713386469.116441", "result": "Results for 000_1713386469.116441: Finally, the best value is 475449.4395934521 at [1.00000000e-02 9.53211618e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-17_22-41-02", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145347898871282, 0.9072367168233831, 0.013162742559417562, 12.0], [0.006144694600813559, 0.9072368940473228, 0.015476652124271658, 12.0], [0.007729888586866125, 0.9072369163842008, 0.014187481710137147, 12.0], [0.00734232802597162, -0.26305163060602543, 0.02, 13.0], [0.008137080974643631, 0.907244955624418, 0.014287216451035097, 12.0], [0.0025356196236077854, -0.24472899466591364, 0.02, 13.0], [0.008921500704026726, 0.9072842218773548, 0.02, 12.0], [0.01, -0.25107876402014445, 0.02, 13.0], [0.0030069184373637163, -0.24969234502677895, 0.012558431776310533, 13.0], [0.006558417412078466, 0.9075256545739324, 0.02, 12.0], [0.005213313254238405, 0.9088105732373747, 0.02, 12.0], [0.00956698685158153, 0.9147010074774165, 0.02, 12.0], [0.01, 0.9345221504917077, 0.02, 12.0], [0.002634368248279207, 0.9504168652092906, 0.02, 12.0], [0.001904024409353247, 0.9528661950002463, 0.02, 12.0], [0.01, 0.9532116177687526, 0.02, 12.0], [0.005966301956177431, 0.9530853907769631, 0.02, 12.0], [0.002307154304539484, 0.9527717612385928, 0.02, 12.0], [0.004813498861448248, 0.9523891152196099, 0.02, 12.0], [0.008654341942326978, 0.9519908880111352, 0.02, 12.0], [0.008805612454000676, 0.9515954989468821, 0.02, 12.0], [0.006492172287180824, 0.9512057064348598, 0.02, 12.0], [2.6957855531690826e-05, 0.95072143093402, 0.019652020296256206, 12.0], [0.0053100988776196454, 0.9503748603349902, 0.02, 12.0], [0.009189323015485994, 0.9500317863804595, 0.02, 12.0]], "y": [495715.30295120884, 1028781.88528604, 1195926.3482218175, 791704.1296281865, 650349.5119809732, 650368.4569554873, 581337.360677842, 618225.5608804307, 478498.4204129208, 615221.538466224, 478642.66919646953, 475602.9519056739, 478365.14031713357, 674686.0715662829, 475695.0928084309, 475744.76276604674, 475559.6670859043, 475494.6878675991, 475745.22714403475, 475767.95525551954, 475449.4395934521, 475608.02416118234, 475752.3654088386, 475654.9449331209, 475505.1975464108, 475500.21908069035, 475591.9402750933, 482836.3836809121, 475640.33543740766, 475488.948424452], "counter": 30, "min_y": 475449.4395934521, "min_X": [0.01, 0.9532116177687526, 0.02, 12.0], "min_mean_X": [0.01, 0.9532116177687526, 0.02, 12.0], "min_mean_y": 475449.4395934521, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145347898871282, 0.9072367168233831, 0.013162742559417562, 12.0], [0.006144694600813559, 0.9072368940473228, 0.015476652124271658, 12.0], [0.007729888586866125, 0.9072369163842008, 0.014187481710137147, 12.0], [0.00734232802597162, -0.26305163060602543, 0.02, 13.0], [0.008137080974643631, 0.907244955624418, 0.014287216451035097, 12.0], [0.0025356196236077854, -0.24472899466591364, 0.02, 13.0], [0.008921500704026726, 0.9072842218773548, 0.02, 12.0], [0.01, -0.25107876402014445, 0.02, 13.0], [0.0030069184373637163, -0.24969234502677895, 0.012558431776310533, 13.0], [0.006558417412078466, 0.9075256545739324, 0.02, 12.0], [0.005213313254238405, 0.9088105732373747, 0.02, 12.0], [0.00956698685158153, 0.9147010074774165, 0.02, 12.0], [0.01, 0.9345221504917077, 0.02, 12.0], [0.002634368248279207, 0.9504168652092906, 0.02, 12.0], [0.001904024409353247, 0.9528661950002463, 0.02, 12.0], [0.01, 0.9532116177687526, 0.02, 12.0], [0.005966301956177431, 0.9530853907769631, 0.02, 12.0], [0.002307154304539484, 0.9527717612385928, 0.02, 12.0], [0.004813498861448248, 0.9523891152196099, 0.02, 12.0], [0.008654341942326978, 0.9519908880111352, 0.02, 12.0], [0.008805612454000676, 0.9515954989468821, 0.02, 12.0], [0.006492172287180824, 0.9512057064348598, 0.02, 12.0], [2.6957855531690826e-05, 0.95072143093402, 0.019652020296256206, 12.0], [0.0053100988776196454, 0.9503748603349902, 0.02, 12.0], [0.009189323015485994, 0.9500317863804595, 0.02, 12.0]], "mean_y": [495715.30295120884, 1028781.88528604, 1195926.3482218175, 791704.1296281865, 650349.5119809732, 650368.4569554873, 581337.360677842, 618225.5608804307, 478498.4204129208, 615221.538466224, 478642.66919646953, 475602.9519056739, 478365.14031713357, 674686.0715662829, 475695.0928084309, 475744.76276604674, 475559.6670859043, 475494.6878675991, 475745.22714403475, 475767.95525551954, 475449.4395934521, 475608.02416118234, 475752.3654088386, 475654.9449331209, 475505.1975464108, 475500.21908069035, 475591.9402750933, 482836.3836809121, 475640.33543740766, 475488.948424452], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000121_1713450624.271904", "result": "Results for 000121_1713450624.271904: Finally, the best value is 475560.25182977517 at [1.00000000e-02 9.07441446e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000121", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000121_bartz10_2024-04-18_16-30-15", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144726252052235, 0.907236719152837, 0.013162736511854746, 12.0], [0.0061439708471784545, 0.9072368907122984, 0.015477024680474634, 12.0], [0.007729877226710211, 0.907236903416045, 0.014187675820520605, 12.0], [0.00641986570827601, -0.26317033379425736, 0.01741847140136336, 13.0], [0.006567015025872191, 0.9072369071125329, 0.014268775582432251, 12.0], [0.003239840226433991, -0.23920495376591247, 0.01605423735598671, 13.0], [0.003639635748769364, -0.24349959304471158, 0.02, 13.0], [0.0020931933092963495, -0.24297194230247304, 0.02, 13.0], [0.0033398296192361705, -0.2424585335234705, 0.02, 13.0], [0.0025498684077849294, -0.24201317718645027, 0.02, 13.0], [0.007992706485908725, -0.24163153194597736, 0.02, 13.0], [0.0018442398103641108, -0.24129948900797968, 0.01999290912031645, 13.0], [0.008344618321176063, -0.24101762844115185, 0.02, 13.0], [0.01, -0.24076500551281688, 0.02, 13.0], [0.01, -0.24053994738273862, 0.02, 13.0], [0.006822476164178637, -0.24033731825718505, 0.02, 13.0], [0.009108418210296561, 0.9072431872221386, 0.02, 12.0], [0.01, 0.9074414461572224, 0.02, 12.0], [0.007299097800226044, 0.9113456917982219, 0.016952703621294512, 12.0], [0.004980852847362808, -0.24345471801325588, 0.02, 13.0], [0.008635205897431705, -0.24326885189037267, 0.02, 13.0], [0.003636578598798305, -0.24309411911251744, 0.02, 13.0], [0.006298574112039975, -0.24292799085356934, 0.02, 13.0], [0.007600905084729991, -0.24277178326946972, 0.02, 13.0], [0.003737912230384629, -0.2426231308902172, 0.02, 13.0]], "y": [495715.3029291629, 1028781.8852800191, 1195926.3482297296, 791704.1296307535, 650349.511987787, 650368.6780551545, 581327.209822583, 618219.7239773851, 535008.594197846, 615833.5717679879, 569341.5599502315, 478596.37022913736, 478655.7754569195, 478605.6137926972, 478635.53377079644, 478421.0307771711, 478803.2278028892, 478405.7350913603, 478340.16564252455, 478339.6206581543, 478463.8171028113, 475595.7167458335, 475560.25182977517, 543023.6162481415, 478543.6317511624, 478399.78365613363, 478595.50835195376, 478490.6484819427, 478439.166312717, 478590.39146631665], "counter": 30, "min_y": 475560.25182977517, "min_X": [0.01, 0.9074414461572224, 0.02, 12.0], "min_mean_X": [0.01, 0.9074414461572224, 0.02, 12.0], "min_mean_y": 475560.25182977517, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144726252052235, 0.907236719152837, 0.013162736511854746, 12.0], [0.0061439708471784545, 0.9072368907122984, 0.015477024680474634, 12.0], [0.007729877226710211, 0.907236903416045, 0.014187675820520605, 12.0], [0.00641986570827601, -0.26317033379425736, 0.01741847140136336, 13.0], [0.006567015025872191, 0.9072369071125329, 0.014268775582432251, 12.0], [0.003239840226433991, -0.23920495376591247, 0.01605423735598671, 13.0], [0.003639635748769364, -0.24349959304471158, 0.02, 13.0], [0.0020931933092963495, -0.24297194230247304, 0.02, 13.0], [0.0033398296192361705, -0.2424585335234705, 0.02, 13.0], [0.0025498684077849294, -0.24201317718645027, 0.02, 13.0], [0.007992706485908725, -0.24163153194597736, 0.02, 13.0], [0.0018442398103641108, -0.24129948900797968, 0.01999290912031645, 13.0], [0.008344618321176063, -0.24101762844115185, 0.02, 13.0], [0.01, -0.24076500551281688, 0.02, 13.0], [0.01, -0.24053994738273862, 0.02, 13.0], [0.006822476164178637, -0.24033731825718505, 0.02, 13.0], [0.009108418210296561, 0.9072431872221386, 0.02, 12.0], [0.01, 0.9074414461572224, 0.02, 12.0], [0.007299097800226044, 0.9113456917982219, 0.016952703621294512, 12.0], [0.004980852847362808, -0.24345471801325588, 0.02, 13.0], [0.008635205897431705, -0.24326885189037267, 0.02, 13.0], [0.003636578598798305, -0.24309411911251744, 0.02, 13.0], [0.006298574112039975, -0.24292799085356934, 0.02, 13.0], [0.007600905084729991, -0.24277178326946972, 0.02, 13.0], [0.003737912230384629, -0.2426231308902172, 0.02, 13.0]], "mean_y": [495715.3029291629, 1028781.8852800191, 1195926.3482297296, 791704.1296307535, 650349.511987787, 650368.6780551545, 581327.209822583, 618219.7239773851, 535008.594197846, 615833.5717679879, 569341.5599502315, 478596.37022913736, 478655.7754569195, 478605.6137926972, 478635.53377079644, 478421.0307771711, 478803.2278028892, 478405.7350913603, 478340.16564252455, 478339.6206581543, 478463.8171028113, 475595.7167458335, 475560.25182977517, 543023.6162481415, 478543.6317511624, 478399.78365613363, 478595.50835195376, 478490.6484819427, 478439.166312717, 478590.39146631665], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000121_1713450815.4077508", "result": "Results for 000121_1713450815.4077508: Finally, the best value is 3728.5708107865703 at [ 3.60490877e-04 -1.55957077e-01  2.85071227e-03  1.30000000e+01].", "fun_control": {"PREFIX": "000121", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 9, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "Bikes", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 182470, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000121_bartz10_2024-04-18_16-30-46", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006140801912478333, 0.11193948635945056, 0.011535573525087193, 12.0], [0.006877196152592707, 0.11211153063828332, 0.011429461720753601, 12.0], [0.006876954878542373, 0.11216807350497585, 0.011429790396504763, 12.0], [0.0047519829552260095, 0.09964889781835347, 0.011429438610271144, 12.0]], "y": [54219.846919502816, 3780.843109771833, 3728.5708107865703, 3824.7311293404923, 3795.744199044163, 3800.125520884503, 3807.260432486679, 3807.3096426707557, 3785.893246470614], "counter": 9, "min_y": 3728.5708107865703, "min_X": [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], "min_mean_X": [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], "min_mean_y": 3728.5708107865703, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006140801912478333, 0.11193948635945056, 0.011535573525087193, 12.0], [0.006877196152592707, 0.11211153063828332, 0.011429461720753601, 12.0], [0.006876954878542373, 0.11216807350497585, 0.011429790396504763, 12.0], [0.0047519829552260095, 0.09964889781835347, 0.011429438610271144, 12.0]], "mean_y": [54219.846919502816, 3780.843109771833, 3728.5708107865703, 3824.7311293404923, 3795.744199044163, 3800.125520884503, 3807.260432486679, 3807.3096426707557, 3785.893246470614], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "0001234_1713452091.353631", "result": "Results for 0001234_1713452091.353631: Finally, the best value is 475445.5574435826 at [9.92163677e-03 9.56085168e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "0001234", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/0001234_bartz10_2024-04-18_16-54-44", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144801580152995, 0.9072367136939526, 0.013162658779253218, 12.0], [0.006128223909860443, 0.9072424798601426, 0.0154784027901522, 12.0], [0.007729667195487804, 0.9072393880537699, 0.014188403235518576, 12.0], [0.007342337050145597, -0.2630518596869404, 0.02, 13.0], [0.008149837591944369, 0.907247490103691, 0.014288075380925832, 12.0], [0.002420574110914539, -0.2447319940060909, 0.02, 13.0], [0.005966960971599471, 0.9074549309849976, 0.02, 12.0], [0.003912867038879993, -0.25106592608331757, 0.02, 13.0], [0.003192104175139294, 0.9109733854215633, 0.02, 12.0], [0.009637392827342762, -0.2514499222629188, 0.02, 13.0], [0.006871567837597975, -0.25019743308860304, 0.017861924923312452, 13.0], [0.0039528506148702415, -0.24953217979818076, 0.02, 13.0], [0.008503431362442236, -0.24870662059021062, 0.02, 13.0], [0.004015055037600275, -0.24801197376865744, 0.01712469253556796, 13.0], [0.0053241065684404175, 0.9473748715468628, 0.02, 12.0], [0.002913148800446845, 0.9562900263664182, 0.02, 12.0], [0.0099216367652004, 0.9560851683860944, 0.02, 12.0], [0.007982422668216362, 0.955645496496282, 0.02, 12.0], [0.002234083957892506, 0.9551463498067652, 0.02, 12.0], [0.0, 0.9546339092998594, 0.02, 12.0], [0.0048601935980997395, 0.9541384613994356, 0.006358858948568509, 12.0], [0.005674960872590371, -0.2647280679087645, 0.02, 13.0], [0.0013072063366229708, -0.26429655697335747, 0.02, 13.0], [0.0013498338047851644, -0.2638453271527418, 0.017515479781284562, 13.0], [0.0046515496913720564, -0.26115158366940505, 0.02, 13.0]], "y": [495715.3030458777, 1028781.885286998, 1195926.3482165677, 791704.129619742, 650349.5120537559, 650371.2065761983, 581290.1569408068, 618197.849753461, 478498.420618228, 615195.3956796824, 478647.1908403995, 475718.47228583856, 478603.9703231787, 475818.83698354935, 478380.2678801726, 524510.7914006669, 478598.6874074032, 478418.12202551716, 542163.621333173, 475647.04887726245, 475720.06877354765, 475445.5574435826, 475522.71507895074, 475749.48360565875, 475838.38768382877, 947117.2756612758, 478567.9079255225, 478738.2551644135, 532896.2000807131, 478599.4065071877], "counter": 30, "min_y": 475445.5574435826, "min_X": [0.0099216367652004, 0.9560851683860944, 0.02, 12.0], "min_mean_X": [0.0099216367652004, 0.9560851683860944, 0.02, 12.0], "min_mean_y": 475445.5574435826, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144801580152995, 0.9072367136939526, 0.013162658779253218, 12.0], [0.006128223909860443, 0.9072424798601426, 0.0154784027901522, 12.0], [0.007729667195487804, 0.9072393880537699, 0.014188403235518576, 12.0], [0.007342337050145597, -0.2630518596869404, 0.02, 13.0], [0.008149837591944369, 0.907247490103691, 0.014288075380925832, 12.0], [0.002420574110914539, -0.2447319940060909, 0.02, 13.0], [0.005966960971599471, 0.9074549309849976, 0.02, 12.0], [0.003912867038879993, -0.25106592608331757, 0.02, 13.0], [0.003192104175139294, 0.9109733854215633, 0.02, 12.0], [0.009637392827342762, -0.2514499222629188, 0.02, 13.0], [0.006871567837597975, -0.25019743308860304, 0.017861924923312452, 13.0], [0.0039528506148702415, -0.24953217979818076, 0.02, 13.0], [0.008503431362442236, -0.24870662059021062, 0.02, 13.0], [0.004015055037600275, -0.24801197376865744, 0.01712469253556796, 13.0], [0.0053241065684404175, 0.9473748715468628, 0.02, 12.0], [0.002913148800446845, 0.9562900263664182, 0.02, 12.0], [0.0099216367652004, 0.9560851683860944, 0.02, 12.0], [0.007982422668216362, 0.955645496496282, 0.02, 12.0], [0.002234083957892506, 0.9551463498067652, 0.02, 12.0], [0.0, 0.9546339092998594, 0.02, 12.0], [0.0048601935980997395, 0.9541384613994356, 0.006358858948568509, 12.0], [0.005674960872590371, -0.2647280679087645, 0.02, 13.0], [0.0013072063366229708, -0.26429655697335747, 0.02, 13.0], [0.0013498338047851644, -0.2638453271527418, 0.017515479781284562, 13.0], [0.0046515496913720564, -0.26115158366940505, 0.02, 13.0]], "mean_y": [495715.3030458777, 1028781.885286998, 1195926.3482165677, 791704.129619742, 650349.5120537559, 650371.2065761983, 581290.1569408068, 618197.849753461, 478498.420618228, 615195.3956796824, 478647.1908403995, 475718.47228583856, 478603.9703231787, 475818.83698354935, 478380.2678801726, 524510.7914006669, 478598.6874074032, 478418.12202551716, 542163.621333173, 475647.04887726245, 475720.06877354765, 475445.5574435826, 475522.71507895074, 475749.48360565875, 475838.38768382877, 947117.2756612758, 478567.9079255225, 478738.2551644135, 532896.2000807131, 478599.4065071877], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "123432_1713458124.960141", "result": "Results for 123432_1713458124.960141: Finally, the best value is 475449.1712832497 at [1.00000000e-02 9.53322439e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "123432", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/123432_bartz10_2024-04-18_18-35-17", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144963014820633, 0.9072367288445962, 0.013162738415445598, 12.0], [0.006144394334068068, 0.907236901957131, 0.015477035904030816, 12.0], [0.007729857537476497, 0.9072369131736734, 0.014187674009365655, 12.0], [0.007342325021970644, -0.2630516805847876, 0.02, 13.0], [0.008137067898739562, 0.9072449014060029, 0.014287334616178968, 12.0], [0.002414809930862277, -0.24473003224479586, 0.02, 13.0], [0.008921462554244225, 0.9072839168377309, 0.02, 12.0], [0.01, -0.2510792153174229, 0.02, 13.0], [0.0030069192249041914, -0.24969242952424142, 0.01255843261435827, 13.0], [0.01, 0.9087870878424061, 0.02, 12.0], [0.01, 0.9146801602378675, 0.02, 12.0], [0.007053118813919316, 0.9366906594901264, 0.02, 12.0], [0.01, 0.9533224386959488, 0.02, 12.0], [0.00676337879154612, 0.9554443231134173, 0.018722271943766813, 12.0], [0.004665143374632263, 0.9528151273001463, 0.017199309817893724, 12.0], [0.01, 0.9493861903280929, 0.02, 12.0], [0.01, 0.9497208866175187, 0.02, 12.0], [0.0045308783610529665, 0.9497476856048175, 0.02, 12.0], [0.007641109358191609, 0.9495882135215781, 0.02, 12.0], [0.003644656670516397, 0.9493175412021083, 0.02, 12.0], [0.01, 0.9489737364341414, 0.02, 12.0], [0.005603368817111942, 0.9485882838253408, 0.02, 12.0], [0.01, 0.9481717641848016, 0.02, 12.0], [0.01, 0.9477411779092288, 0.02, 12.0], [0.005355426507860092, 0.9473779714758325, 0.019407678519999753, 12.0]], "y": [495715.30292177614, 1028781.8852887875, 1195926.3482279899, 791704.129641499, 650349.511995873, 650368.6068061803, 581326.8866127648, 618219.7792018387, 478498.4206539635, 615218.0120126597, 478647.41231845133, 475602.9541327788, 478365.1414345859, 674686.0430614626, 475556.9939688354, 475542.7264743371, 475605.07097257377, 475449.1712832497, 502070.3249887467, 537003.8609395038, 475458.70117949054, 475457.89083169436, 475672.42982512934, 475550.77297341626, 475708.2458237673, 475459.6997354128, 475633.1531331995, 475461.6413610743, 475462.68385291856, 487641.9562151354], "counter": 30, "min_y": 475449.1712832497, "min_X": [0.01, 0.9533224386959488, 0.02, 12.0], "min_mean_X": [0.01, 0.9533224386959488, 0.02, 12.0], "min_mean_y": 475449.1712832497, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006144963014820633, 0.9072367288445962, 0.013162738415445598, 12.0], [0.006144394334068068, 0.907236901957131, 0.015477035904030816, 12.0], [0.007729857537476497, 0.9072369131736734, 0.014187674009365655, 12.0], [0.007342325021970644, -0.2630516805847876, 0.02, 13.0], [0.008137067898739562, 0.9072449014060029, 0.014287334616178968, 12.0], [0.002414809930862277, -0.24473003224479586, 0.02, 13.0], [0.008921462554244225, 0.9072839168377309, 0.02, 12.0], [0.01, -0.2510792153174229, 0.02, 13.0], [0.0030069192249041914, -0.24969242952424142, 0.01255843261435827, 13.0], [0.01, 0.9087870878424061, 0.02, 12.0], [0.01, 0.9146801602378675, 0.02, 12.0], [0.007053118813919316, 0.9366906594901264, 0.02, 12.0], [0.01, 0.9533224386959488, 0.02, 12.0], [0.00676337879154612, 0.9554443231134173, 0.018722271943766813, 12.0], [0.004665143374632263, 0.9528151273001463, 0.017199309817893724, 12.0], [0.01, 0.9493861903280929, 0.02, 12.0], [0.01, 0.9497208866175187, 0.02, 12.0], [0.0045308783610529665, 0.9497476856048175, 0.02, 12.0], [0.007641109358191609, 0.9495882135215781, 0.02, 12.0], [0.003644656670516397, 0.9493175412021083, 0.02, 12.0], [0.01, 0.9489737364341414, 0.02, 12.0], [0.005603368817111942, 0.9485882838253408, 0.02, 12.0], [0.01, 0.9481717641848016, 0.02, 12.0], [0.01, 0.9477411779092288, 0.02, 12.0], [0.005355426507860092, 0.9473779714758325, 0.019407678519999753, 12.0]], "mean_y": [495715.30292177614, 1028781.8852887875, 1195926.3482279899, 791704.129641499, 650349.511995873, 650368.6068061803, 581326.8866127648, 618219.7792018387, 478498.4206539635, 615218.0120126597, 478647.41231845133, 475602.9541327788, 478365.1414345859, 674686.0430614626, 475556.9939688354, 475542.7264743371, 475605.07097257377, 475449.1712832497, 502070.3249887467, 537003.8609395038, 475458.70117949054, 475457.89083169436, 475672.42982512934, 475550.77297341626, 475708.2458237673, 475459.6997354128, 475633.1531331995, 475461.6413610743, 475462.68385291856, 487641.9562151354], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "123432_1713458136.655529", "result": "Results for 123432_1713458136.655529: Finally, the best value is 49092.62616040038 at [ 4.63529627e-03 -2.21528408e-01  1.91626325e-02  1.30000000e+01].", "fun_control": {"PREFIX": "123432", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/123432_bartz10_2024-04-18_18-35-28", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061450589599621845, 0.9072367093682105, 0.01369926419221713, 12.0], [0.006145149157628194, 0.9072367430463045, 0.013779485932705173, 12.0], [0.006129160227554793, 0.9072418145318983, 0.01573703600595811, 12.0], [0.007729295520851236, 0.9072384955793189, 0.014271064455182777, 12.0], [0.008499914716176078, -0.26241437045598254, 0.02, 13.0], [0.006467617121261838, 0.9072385734197509, 0.014325783583633851, 12.0], [0.008658243793130274, -0.23510548742649154, 0.02, 13.0], [0.005529112887507462, -0.23743906721477506, 0.00915025681708915, 13.0], [0.008238375304126196, 0.9072419683259927, 0.012139084042128219, 12.0], [0.0010756513906215106, 0.9072394161713688, 0.01690204711893588, 12.0], [2.7733278600650288e-05, 0.9072410090355738, 0.014589557822262572, 12.0], [2.7683331452378638e-05, 0.9072423800504225, 0.014589776133867997, 12.0], [2.7633645473070038e-05, 0.9072443879120764, 0.014590034703446927, 12.0], [2.7583055926258616e-05, 0.9072473354242185, 0.014590352040116385, 12.0], [2.7530418164716645e-05, 0.9072516724759863, 0.014590753527567217, 12.0], [2.7477027754068237e-05, 0.9072580747789413, 0.014591279518711702, 12.0], [0.0007046537471847327, 0.9072674562733481, 0.018528648467821592, 12.0], [0.006017188373505261, 0.907389701857427, 0.02, 12.0], [0.0, 0.9081946376375785, 0.02, 12.0], [0.003364920206272184, 0.9130235431067293, 0.02, 12.0], [0.006412995480555443, -0.2519082061525501, 0.02, 13.0], [0.00509637933691491, -0.2529029493484723, 0.02, 13.0], [0.01, -0.25339952958944406, 0.02, 13.0], [0.0058808568820970224, -0.25364007739562056, 0.02, 13.0], [0.0, 0.938547109961377, 0.02, 12.0]], "y": [49092.62616040038, 93216.06118251584, 111455.49510718389, 73889.69965999502, 64484.552387470896, 63448.90561746653, 63300.76370177736, 60010.61759999618, 62410.43125092704, 55526.29190183449, 62314.58993687014, 55512.04346974347, 75413.1453612064, 66653.71634540513, 58361.78816154475, 61859.281953485915, 61858.33271744233, 61857.34343676176, 61856.28367949924, 61855.11029067557, 61853.75368500522, 56619.82243314782, 55400.132636267634, 55400.01429650527, 55398.221785301226, 55485.76132391031, 55485.31503508148, 55483.91653029031, 55483.89640820163, 55393.28498082949], "counter": 30, "min_y": 49092.62616040038, "min_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_y": 49092.62616040038, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061450589599621845, 0.9072367093682105, 0.01369926419221713, 12.0], [0.006145149157628194, 0.9072367430463045, 0.013779485932705173, 12.0], [0.006129160227554793, 0.9072418145318983, 0.01573703600595811, 12.0], [0.007729295520851236, 0.9072384955793189, 0.014271064455182777, 12.0], [0.008499914716176078, -0.26241437045598254, 0.02, 13.0], [0.006467617121261838, 0.9072385734197509, 0.014325783583633851, 12.0], [0.008658243793130274, -0.23510548742649154, 0.02, 13.0], [0.005529112887507462, -0.23743906721477506, 0.00915025681708915, 13.0], [0.008238375304126196, 0.9072419683259927, 0.012139084042128219, 12.0], [0.0010756513906215106, 0.9072394161713688, 0.01690204711893588, 12.0], [2.7733278600650288e-05, 0.9072410090355738, 0.014589557822262572, 12.0], [2.7683331452378638e-05, 0.9072423800504225, 0.014589776133867997, 12.0], [2.7633645473070038e-05, 0.9072443879120764, 0.014590034703446927, 12.0], [2.7583055926258616e-05, 0.9072473354242185, 0.014590352040116385, 12.0], [2.7530418164716645e-05, 0.9072516724759863, 0.014590753527567217, 12.0], [2.7477027754068237e-05, 0.9072580747789413, 0.014591279518711702, 12.0], [0.0007046537471847327, 0.9072674562733481, 0.018528648467821592, 12.0], [0.006017188373505261, 0.907389701857427, 0.02, 12.0], [0.0, 0.9081946376375785, 0.02, 12.0], [0.003364920206272184, 0.9130235431067293, 0.02, 12.0], [0.006412995480555443, -0.2519082061525501, 0.02, 13.0], [0.00509637933691491, -0.2529029493484723, 0.02, 13.0], [0.01, -0.25339952958944406, 0.02, 13.0], [0.0058808568820970224, -0.25364007739562056, 0.02, 13.0], [0.0, 0.938547109961377, 0.02, 12.0]], "mean_y": [49092.62616040038, 93216.06118251584, 111455.49510718389, 73889.69965999502, 64484.552387470896, 63448.90561746653, 63300.76370177736, 60010.61759999618, 62410.43125092704, 55526.29190183449, 62314.58993687014, 55512.04346974347, 75413.1453612064, 66653.71634540513, 58361.78816154475, 61859.281953485915, 61858.33271744233, 61857.34343676176, 61856.28367949924, 61855.11029067557, 61853.75368500522, 56619.82243314782, 55400.132636267634, 55400.01429650527, 55398.221785301226, 55485.76132391031, 55485.31503508148, 55483.91653029031, 55483.89640820163, 55393.28498082949], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "00045_1713458978.990674", "result": "Results for 00045_1713458978.990674: Finally, the best value is 6865.176466908466 at [5.05000000e+02 1.70000000e+01 2.93914361e-07 9.21260735e-02\n 2.00000000e+00 0.00000000e+00 9.27551686e-01 1.00000000e+00\n 4.00000000e+00 1.00000000e+00 9.12584547e+02 5.00000000e+00\n 1.00000000e+00 0.00000000e+00 0.00000000e+00].", "fun_control": {"PREFIX": "00045", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "tree.HoeffdingTreeRegressor", "counter": 5, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "Bikes", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [10.0, 2.0, 1e-08, 0.01, 0.0, 0.0, 0.9, 0.0, 2.0, 0.0, 100.0, 3.0, 0.0, 0.0, 0.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "max_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 182470, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/00045_bartz10_2024-04-18_18-44-22", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [1000.0, 20.0, 1e-06, 0.1, 2.0, 2.0, 0.99, 2.0, 10.0, 1.0, 1000.0, 8.0, 1.0, 1.0, 1.0], "var_name": ["grace_period", "max_depth", "delta", "tau", "leaf_prediction", "leaf_model", "model_selector_decay", "splitter", "min_samples_split", "binary_split", "max_size", "memory_estimate_period", "stop_mem_management", "remove_poor_attrs", "merit_preprune"], "var_type": ["int", "int", "float", "float", "factor", "factor", "float", "factor", "int", "factor", "float", "int", "factor", "factor", "factor"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"grace_period": {"type": "int", "default": 200, "transform": "None", "lower": 10, "upper": 1000}, "max_depth": {"type": "int", "default": 20, "transform": "transform_power_2_int", "lower": 2, "upper": 20}, "delta": {"type": "float", "default": 1e-07, "transform": "None", "lower": 1e-08, "upper": 1e-06}, "tau": {"type": "float", "default": 0.05, "transform": "None", "lower": 0.01, "upper": 0.1}, "leaf_prediction": {"levels": ["mean", "model", "adaptive"], "type": "factor", "default": "mean", "transform": "None", "core_model_parameter_type": "str", "lower": 0, "upper": 2}, "leaf_model": {"levels": ["LinearRegression", "PARegressor", "Perceptron"], "type": "factor", "default": "LinearRegression", "transform": "None", "class_name": "river.linear_model", "core_model_parameter_type": "instance()", "lower": 0, "upper": 2}, "model_selector_decay": {"type": "float", "default": 0.95, "transform": "None", "lower": 0.9, "upper": 0.99}, "splitter": {"levels": ["EBSTSplitter", "TEBSTSplitter", "QOSplitter"], "type": "factor", "default": "EBSTSplitter", "transform": "None", "class_name": "river.tree.splitter", "core_model_parameter_type": "instance()", "lower": 0, "upper": 2}, "min_samples_split": {"type": "int", "default": 5, "transform": "None", "lower": 2, "upper": 10}, "binary_split": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "max_size": {"type": "float", "default": 500.0, "transform": "None", "lower": 100.0, "upper": 1000.0}, "memory_estimate_period": {"type": "int", "default": 6, "transform": "transform_power_10_int", "lower": 3, "upper": 8}, "stop_mem_management": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "remove_poor_attrs": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "merit_preprune": {"levels": [0, 1], "type": "factor", "default": 1, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}}, "core_model_hyper_dict_default": {"grace_period": {"type": "int", "default": 200, "transform": "None", "lower": 10, "upper": 1000}, "max_depth": {"type": "int", "default": 20, "transform": "transform_power_2_int", "lower": 2, "upper": 20}, "delta": {"type": "float", "default": 1e-07, "transform": "None", "lower": 1e-08, "upper": 1e-06}, "tau": {"type": "float", "default": 0.05, "transform": "None", "lower": 0.01, "upper": 0.1}, "leaf_prediction": {"levels": ["mean", "model", "adaptive"], "type": "factor", "default": "mean", "transform": "None", "core_model_parameter_type": "str", "lower": 0, "upper": 2}, "leaf_model": {"levels": ["LinearRegression", "PARegressor", "Perceptron"], "type": "factor", "default": "LinearRegression", "transform": "None", "class_name": "river.linear_model", "core_model_parameter_type": "instance()", "lower": 0, "upper": 2}, "model_selector_decay": {"type": "float", "default": 0.95, "transform": "None", "lower": 0.9, "upper": 0.99}, "splitter": {"levels": ["EBSTSplitter", "TEBSTSplitter", "QOSplitter"], "type": "factor", "default": "EBSTSplitter", "transform": "None", "class_name": "river.tree.splitter", "core_model_parameter_type": "instance()", "lower": 0, "upper": 2}, "min_samples_split": {"type": "int", "default": 5, "transform": "None", "lower": 2, "upper": 10}, "binary_split": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "max_size": {"type": "float", "default": 500.0, "transform": "None", "lower": 100.0, "upper": 1000.0}, "memory_estimate_period": {"type": "int", "default": 6, "transform": "transform_power_10_int", "lower": 3, "upper": 8}, "stop_mem_management": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "remove_poor_attrs": {"levels": [0, 1], "type": "factor", "default": 0, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}, "merit_preprune": {"levels": [0, 1], "type": "factor", "default": 1, "transform": "None", "core_model_parameter_type": "bool", "lower": 0, "upper": 1}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 15, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["int", "int", "float", "float", "factor", "factor", "float", "factor", "int", "factor", "float", "int", "factor", "factor", "factor"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [10.0, 2.0, 1e-08, 0.01, 0.0, 0.0, 0.9, 0.0, 2.0, 0.0, 100.0, 3.0, 0.0, 0.0, 0.0], "k": 15, "upper": [1000.0, 20.0, 1e-06, 0.1, 2.0, 2.0, 0.99, 2.0, 10.0, 1.0, 1000.0, 8.0, 1.0, 1.0, 1.0], "var_type": ["int", "int", "float", "float", "factor", "factor", "float", "factor", "int", "factor", "float", "int", "factor", "factor", "factor"], "var_name": ["grace_period", "max_depth", "delta", "tau", "leaf_prediction", "leaf_model", "model_selector_decay", "splitter", "min_samples_split", "binary_split", "max_size", "memory_estimate_period", "stop_mem_management", "remove_poor_attrs", "merit_preprune"], "all_lower": [10.0, 2.0, 1e-08, 0.01, 0.0, 0.0, 0.9, 0.0, 2.0, 0.0, 100.0, 3.0, 0.0, 0.0, 0.0], "all_upper": [1000.0, 20.0, 1e-06, 0.1, 2.0, 2.0, 0.99, 2.0, 10.0, 1.0, 1000.0, 8.0, 1.0, 1.0, 1.0], "ident": [false, false, false, false, false, false, false, false, false, false, false, false, false, false, false], "red_dim": 0, "all_var_type": ["int", "int", "float", "float", "factor", "factor", "float", "factor", "int", "factor", "float", "int", "factor", "factor", "factor"], "all_var_name": ["grace_period", "max_depth", "delta", "tau", "leaf_prediction", "leaf_model", "model_selector_decay", "splitter", "min_samples_split", "binary_split", "max_size", "memory_estimate_period", "stop_mem_management", "remove_poor_attrs", "merit_preprune"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[10.0, 1000.0], [2.0, 20.0], [1e-08, 1e-06], [0.01, 0.1], [0.0, 2.0], [0.0, 2.0], [0.9, 0.99], [0.0, 2.0], [2.0, 10.0], [0.0, 1.0], [100.0, 1000.0], [3.0, 8.0], [0.0, 1.0], [0.0, 1.0], [0.0, 1.0]], "X": [[271.0, 13.0, 5.60368745191023e-07, 0.07868130740742395, 1.0, 1.0, 0.973379790035513, 1.0, 2.0, 1.0, 547.6653180586843, 4.0, 1.0, 1.0, 1.0], [677.0, 13.0, 7.560821786559292e-07, 0.013615747684838508, 1.0, 1.0, 0.9150137281216666, 2.0, 6.0, 0.0, 277.31891498315815, 7.0, 0.0, 0.0, 0.0], [938.0, 9.0, 2.0155471952189532e-07, 0.05505936684768389, 1.0, 2.0, 0.9673638749116286, 0.0, 8.0, 0.0, 383.086221169069, 4.0, 1.0, 0.0, 1.0], [505.0, 17.0, 2.9391436090730967e-07, 0.09212607349196934, 2.0, 0.0, 0.9275516858129766, 1.0, 4.0, 1.0, 912.5845474456005, 5.0, 1.0, 0.0, 0.0], [454.0, 8.0, 6.031084012756379e-07, 0.06056859803229832, 0.0, 1.0, 0.9708852117897216, 0.0, 7.0, 1.0, 129.17853972511045, 4.0, 0.0, 0.0, 0.0]], "y": [9133.042176421272, 11291.01551799989, 18180.75025344421, 6865.176466908466, 12086.865540434663], "counter": 5, "min_y": 6865.176466908466, "min_X": [505.0, 17.0, 2.9391436090730967e-07, 0.09212607349196934, 2.0, 0.0, 0.9275516858129766, 1.0, 4.0, 1.0, 912.5845474456005, 5.0, 1.0, 0.0, 0.0], "min_mean_X": [505.0, 17.0, 2.9391436090730967e-07, 0.09212607349196934, 2.0, 0.0, 0.9275516858129766, 1.0, 4.0, 1.0, 912.5845474456005, 5.0, 1.0, 0.0, 0.0], "min_mean_y": 6865.176466908466, "mean_X": [[271.0, 13.0, 5.60368745191023e-07, 0.07868130740742395, 1.0, 1.0, 0.973379790035513, 1.0, 2.0, 1.0, 547.6653180586843, 4.0, 1.0, 1.0, 1.0], [677.0, 13.0, 7.560821786559292e-07, 0.013615747684838508, 1.0, 1.0, 0.9150137281216666, 2.0, 6.0, 0.0, 277.31891498315815, 7.0, 0.0, 0.0, 0.0], [938.0, 9.0, 2.0155471952189532e-07, 0.05505936684768389, 1.0, 2.0, 0.9673638749116286, 0.0, 8.0, 0.0, 383.086221169069, 4.0, 1.0, 0.0, 1.0], [505.0, 17.0, 2.9391436090730967e-07, 0.09212607349196934, 2.0, 0.0, 0.9275516858129766, 1.0, 4.0, 1.0, 912.5845474456005, 5.0, 1.0, 0.0, 0.0], [454.0, 8.0, 6.031084012756379e-07, 0.06056859803229832, 0.0, 1.0, 0.9708852117897216, 0.0, 7.0, 1.0, 129.17853972511045, 4.0, 0.0, 0.0, 0.0]], "mean_y": [9133.042176421272, 11291.01551799989, 18180.75025344421, 6865.176466908466, 12086.865540434663], "var_y": [NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713469014.4519129", "result": "Results for 000_1713469014.4519129: Finally, the best value is 186.8522365994297 at [ 0.          0.36930575 -0.         11.        ].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LogisticRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "Phishing", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, 0.0, -10.0, -4.0, 6.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 1250, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_21-36-24", "target_column": "y", "target_type": "bool", "task": "Binary Classification", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.0, 0.1, 10.0, 0.0, 12.0], "var_name": ["optimizer", "loss", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["factor", "factor", "float", "float", "int", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"optimizer": {"levels": ["SGD"], "type": "factor", "default": "SGD", "transform": "None", "class_name": "river.optim", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "loss": {"levels": ["Log"], "type": "factor", "default": "Log", "transform": "None", "class_name": "river.optim.losses", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.1}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -10.0, "upper": 10.0}, "intercept_lr": {"type": "int", "default": -2, "transform": "transform_power_10", "lower": -4, "upper": 0}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 6, "upper": 12}}, "core_model_hyper_dict_default": {"optimizer": {"levels": ["SGD"], "type": "factor", "default": "SGD", "transform": "None", "class_name": "river.optim", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "loss": {"levels": ["Log"], "type": "factor", "default": "Log", "transform": "None", "class_name": "river.optim.losses", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.1}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -10.0, "upper": 10.0}, "intercept_lr": {"type": "int", "default": -2, "transform": "transform_power_10", "lower": -4, "upper": 0}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 6, "upper": 12}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "int", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -10.0, -4.0, 6.0], "k": 4, "upper": [0.1, 10.0, 0.0, 12.0], "var_type": ["float", "float", "int", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, 0.0, -10.0, -4.0, 6.0], "all_upper": [0.0, 0.0, 0.1, 10.0, 0.0, 12.0], "ident": [true, true, false, false, false, false], "red_dim": 1, "all_var_type": ["factor", "factor", "float", "float", "int", "int"], "all_var_name": ["optimizer", "loss", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.1], [-10.0, 10.0], [-4.0, 0.0], [6.0, 12.0]], "X": [[0.04635296273503714, -2.2152840752088903, -0.0, 11.0], [0.036481881978299394, 2.7516219733769063, -3.0, 7.0], [0.0036049087681399583, -1.5595707724447436, -4.0, 12.0], [0.08351516807805177, -6.855051853500382, -2.0, 8.0], [0.06145185482949666, 9.072367245574323, -1.0, 9.0], [0.04338884863914692, 1.0091635602114124, -0.0, 11.0], [0.04152867338165386, 2.240623428233253, -0.0, 11.0], [0.04258620299615467, 2.0862423412908164, -0.0, 11.0], [0.052836003499507844, 1.791534311330128, -0.0, 11.0], [0.0, 0.04512022175383561, -0.0, 11.0], [0.007820825709854273, 0.3101275819835399, -0.0, 11.0], [0.0, 0.3693057519630786, -0.0, 11.0], [0.0, 0.5766147741285881, -0.0, 11.0], [0.0, 0.8286945791919228, -0.0, 11.0], [0.0, 0.7443933936482889, -0.0, 11.0], [0.0, 0.7063134034099254, -0.0, 11.0], [0.0, 0.6863072084107188, -0.0, 11.0], [0.0, 0.6761051472515813, -0.0, 11.0], [0.0, 0.6714727585824352, -0.0, 11.0], [0.0, 0.6696676994576952, -0.0, 11.0], [0.0, 0.6700249074588495, -0.0, 11.0], [0.00021343486910121306, 0.5449132650007793, -0.0, 11.0], [0.0, 0.6326634468711428, -0.0, 11.0], [0.0, 0.6356422060899642, -0.0, 11.0], [0.0, 0.637146705548731, -0.0, 11.0], [0.0, 0.6395374018492183, -0.0, 11.0], [0.0, 0.6418052760283585, -0.0, 11.0], [0.0, 0.6446682971426383, -0.0, 11.0], [0.0, 0.6479156758850745, -0.0, 11.0], [0.0, 0.6462236033837891, -0.0, 11.0]], "y": [200.0107428709785, 505.27391183386663, 357.9054808403323, 481.5897032944848, 307.9054896252802, 197.37923953018623, 197.3791447396413, 197.37910633744113, 205.27377006126727, 189.4837846191402, 194.74748007444987, 186.8522365994297, 186.8522439272981, 189.48380471466652, 189.48381266192968, 189.48380579895598, 189.48381726166653, 189.48381211158758, 189.48382864656125, 189.4838219843244, 189.4838272419823, 186.85277505031826, 189.4838100237981, 189.48382011587705, 189.48382692837706, 189.48381249537704, 189.48382494156127, 189.48382964556126, 189.48383263890335, 189.48380786366653], "counter": 30, "min_y": 186.8522365994297, "min_X": [0.0, 0.3693057519630786, -0.0, 11.0], "min_mean_X": [0.0, 0.3693057519630786, -0.0, 11.0], "min_mean_y": 186.8522365994297, "mean_X": [[0.04635296273503714, -2.2152840752088903, -0.0, 11.0], [0.036481881978299394, 2.7516219733769063, -3.0, 7.0], [0.0036049087681399583, -1.5595707724447436, -4.0, 12.0], [0.08351516807805177, -6.855051853500382, -2.0, 8.0], [0.06145185482949666, 9.072367245574323, -1.0, 9.0], [0.04338884863914692, 1.0091635602114124, -0.0, 11.0], [0.04152867338165386, 2.240623428233253, -0.0, 11.0], [0.04258620299615467, 2.0862423412908164, -0.0, 11.0], [0.052836003499507844, 1.791534311330128, -0.0, 11.0], [0.0, 0.04512022175383561, -0.0, 11.0], [0.007820825709854273, 0.3101275819835399, -0.0, 11.0], [0.0, 0.3693057519630786, -0.0, 11.0], [0.0, 0.5766147741285881, -0.0, 11.0], [0.0, 0.8286945791919228, -0.0, 11.0], [0.0, 0.7443933936482889, -0.0, 11.0], [0.0, 0.7063134034099254, -0.0, 11.0], [0.0, 0.6863072084107188, -0.0, 11.0], [0.0, 0.6761051472515813, -0.0, 11.0], [0.0, 0.6714727585824352, -0.0, 11.0], [0.0, 0.6696676994576952, -0.0, 11.0], [0.0, 0.6700249074588495, -0.0, 11.0], [0.00021343486910121306, 0.5449132650007793, -0.0, 11.0], [0.0, 0.6326634468711428, -0.0, 11.0], [0.0, 0.6356422060899642, -0.0, 11.0], [0.0, 0.637146705548731, -0.0, 11.0], [0.0, 0.6395374018492183, -0.0, 11.0], [0.0, 0.6418052760283585, -0.0, 11.0], [0.0, 0.6446682971426383, -0.0, 11.0], [0.0, 0.6479156758850745, -0.0, 11.0], [0.0, 0.6462236033837891, -0.0, 11.0]], "mean_y": [200.0107428709785, 505.27391183386663, 357.9054808403323, 481.5897032944848, 307.9054896252802, 197.37923953018623, 197.3791447396413, 197.37910633744113, 205.27377006126727, 189.4837846191402, 194.74748007444987, 186.8522365994297, 186.8522439272981, 189.48380471466652, 189.48381266192968, 189.48380579895598, 189.48381726166653, 189.48381211158758, 189.48382864656125, 189.4838219843244, 189.4838272419823, 186.85277505031826, 189.4838100237981, 189.48382011587705, 189.48382692837706, 189.48381249537704, 189.48382494156127, 189.48382964556126, 189.48383263890335, 189.48380786366653], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "00012_1713469813.50812", "result": "Results for 00012_1713469813.50812: Finally, the best value is 197.37907960874583 at [ 0.04288546  2.0384333  -0.         11.        ].", "fun_control": {"PREFIX": "00012", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LogisticRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "Phishing", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, 0.0, -10.0, -4.0, 6.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 1250, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/00012_bartz10_2024-04-18_21-49-37", "target_column": "y", "target_type": "bool", "task": "Binary Classification", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.0, 0.1, 10.0, 0.0, 12.0], "var_name": ["optimizer", "loss", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["factor", "factor", "float", "float", "int", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"optimizer": {"levels": ["SGD"], "type": "factor", "default": "SGD", "transform": "None", "class_name": "river.optim", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "loss": {"levels": ["Log"], "type": "factor", "default": "Log", "transform": "None", "class_name": "river.optim.losses", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.1}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -10.0, "upper": 10.0}, "intercept_lr": {"type": "int", "default": -2, "transform": "transform_power_10", "lower": -4, "upper": 0}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 6, "upper": 12}}, "core_model_hyper_dict_default": {"optimizer": {"levels": ["SGD"], "type": "factor", "default": "SGD", "transform": "None", "class_name": "river.optim", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "loss": {"levels": ["Log"], "type": "factor", "default": "Log", "transform": "None", "class_name": "river.optim.losses", "core_model_parameter_type": "instance()", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.1}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -10.0, "upper": 10.0}, "intercept_lr": {"type": "int", "default": -2, "transform": "transform_power_10", "lower": -4, "upper": 0}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 6, "upper": 12}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "int", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -10.0, -4.0, 6.0], "k": 4, "upper": [0.1, 10.0, 0.0, 12.0], "var_type": ["float", "float", "int", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, 0.0, -10.0, -4.0, 6.0], "all_upper": [0.0, 0.0, 0.1, 10.0, 0.0, 12.0], "ident": [true, true, false, false, false, false], "red_dim": 1, "all_var_type": ["factor", "factor", "float", "float", "int", "int"], "all_var_name": ["optimizer", "loss", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.1], [-10.0, 10.0], [-4.0, 0.0], [6.0, 12.0]], "X": [[0.04635296273503714, -2.2152840752088903, -0.0, 11.0], [0.036481881978299394, 2.7516219733769063, -3.0, 7.0], [0.0036049087681399583, -1.5595707724447436, -4.0, 12.0], [0.08351516807805177, -6.855051853500382, -2.0, 8.0], [0.06145185482949666, 9.072367245574323, -1.0, 9.0], [0.043362749571113426, 1.0093190708363777, -0.0, 11.0], [0.041477414629200814, 2.2406679270082854, -0.0, 11.0], [0.04257694338166584, 2.086298819356734, -0.0, 11.0], [0.042885462501425727, 2.038433299988179, -0.0, 11.0], [0.04306190515639821, 2.0115177322689846, -0.0, 11.0], [0.04322493282315215, 1.9936368620579932, -0.0, 11.0], [0.04328697247976311, 1.980679522421945, -0.0, 11.0], [0.04334382611225342, 1.9705940934742927, -0.0, 11.0], [0.04340451415357052, 1.9629085041680538, -0.0, 11.0], [0.04312586372194723, 1.9564754774522433, -0.0, 11.0], [0.0434913373179596, 1.9511953151093455, -0.0, 11.0], [0.04354111953555947, 1.946783437004417, -0.0, 11.0], [0.0435493031915261, 1.9429154548701493, -0.0, 11.0], [0.043548024968968584, 1.9395965401548567, -0.0, 11.0], [0.04378348324149629, 1.9366358706183378, -0.0, 11.0], [0.04358965480755239, 1.9341025498389302, -0.0, 11.0], [0.04367026211440459, 1.9319445229701924, -0.0, 11.0], [0.04360355769412968, 1.9297583809607084, -0.0, 11.0], [0.04364749139642246, 1.9279190213729935, -0.0, 11.0], [0.04366810451512546, 1.9262734738064689, -0.0, 11.0], [0.04364547011885072, 1.9246853276043283, -0.0, 11.0], [0.04362587762876863, 1.9232293957878914, -0.0, 11.0], [0.04366376009583077, 1.9220662353659574, -0.0, 11.0], [0.043662350262839246, 1.9208835540040905, -0.0, 11.0], [0.043725038458611906, 1.91844318852677, -0.0, 11.0]], "y": [200.01083220642587, 505.2739365598403, 357.90553434033234, 481.58974980106376, 307.9055263216749, 197.37923614629148, 197.37916724115772, 197.37908783898266, 197.37907960874583, 197.37910064608792, 197.37912248369318, 197.3791302272195, 197.37922646290372, 197.37915911758793, 197.37911549898266, 197.37912040043003, 197.37911784882476, 197.37912225019318, 197.37912226327214, 197.37911692235107, 197.37912560216688, 197.3791177765616, 197.37912635877214, 197.37911470848266, 197.37911273598266, 197.37912335208793, 197.37910499358793, 197.37917477979846, 197.37911394532478, 197.37911222279845], "counter": 30, "min_y": 197.37907960874583, "min_X": [0.042885462501425727, 2.038433299988179, -0.0, 11.0], "min_mean_X": [0.042885462501425727, 2.038433299988179, -0.0, 11.0], "min_mean_y": 197.37907960874583, "mean_X": [[0.04635296273503714, -2.2152840752088903, -0.0, 11.0], [0.036481881978299394, 2.7516219733769063, -3.0, 7.0], [0.0036049087681399583, -1.5595707724447436, -4.0, 12.0], [0.08351516807805177, -6.855051853500382, -2.0, 8.0], [0.06145185482949666, 9.072367245574323, -1.0, 9.0], [0.043362749571113426, 1.0093190708363777, -0.0, 11.0], [0.041477414629200814, 2.2406679270082854, -0.0, 11.0], [0.04257694338166584, 2.086298819356734, -0.0, 11.0], [0.042885462501425727, 2.038433299988179, -0.0, 11.0], [0.04306190515639821, 2.0115177322689846, -0.0, 11.0], [0.04322493282315215, 1.9936368620579932, -0.0, 11.0], [0.04328697247976311, 1.980679522421945, -0.0, 11.0], [0.04334382611225342, 1.9705940934742927, -0.0, 11.0], [0.04340451415357052, 1.9629085041680538, -0.0, 11.0], [0.04312586372194723, 1.9564754774522433, -0.0, 11.0], [0.0434913373179596, 1.9511953151093455, -0.0, 11.0], [0.04354111953555947, 1.946783437004417, -0.0, 11.0], [0.0435493031915261, 1.9429154548701493, -0.0, 11.0], [0.043548024968968584, 1.9395965401548567, -0.0, 11.0], [0.04378348324149629, 1.9366358706183378, -0.0, 11.0], [0.04358965480755239, 1.9341025498389302, -0.0, 11.0], [0.04367026211440459, 1.9319445229701924, -0.0, 11.0], [0.04360355769412968, 1.9297583809607084, -0.0, 11.0], [0.04364749139642246, 1.9279190213729935, -0.0, 11.0], [0.04366810451512546, 1.9262734738064689, -0.0, 11.0], [0.04364547011885072, 1.9246853276043283, -0.0, 11.0], [0.04362587762876863, 1.9232293957878914, -0.0, 11.0], [0.04366376009583077, 1.9220662353659574, -0.0, 11.0], [0.043662350262839246, 1.9208835540040905, -0.0, 11.0], [0.043725038458611906, 1.91844318852677, -0.0, 11.0]], "mean_y": [200.01083220642587, 505.2739365598403, 357.90553434033234, 481.58974980106376, 307.9055263216749, 197.37923614629148, 197.37916724115772, 197.37908783898266, 197.37907960874583, 197.37910064608792, 197.37912248369318, 197.3791302272195, 197.37922646290372, 197.37915911758793, 197.37911549898266, 197.37912040043003, 197.37911784882476, 197.37912225019318, 197.37912226327214, 197.37911692235107, 197.37912560216688, 197.3791177765616, 197.37912635877214, 197.37911470848266, 197.37911273598266, 197.37912335208793, 197.37910499358793, 197.37917477979846, 197.37911394532478, 197.37911222279845], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713473528.6051059", "result": "Results for 000_1713473528.6051059: Finally, the best value is 475598.027092055 at [9.07429843e-03 9.06841911e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_22-52-01", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145661494013283, 0.907236718877838, 0.013162667499175565, 12.0], [0.006129061414450295, 0.90724244103414, 0.01547836145018752, 12.0], [0.007729652851161041, 0.9072393646684052, 0.014188374644020035, 12.0], [0.0073423411982307335, -0.26305183901903595, 0.02, 13.0], [0.00745279244360387, 0.9072430189556357, 0.014209323046895046, 12.0], [0.0024150316336011162, -0.24471595154093473, 0.02, 13.0], [0.006701257589711842, -0.24511650039986962, 0.02, 13.0], [0.000191128682961689, -0.244951902401147, 0.019276213545435187, 13.0], [0.01, -0.24494615080525997, 0.02, 13.0], [0.006931738975301204, -0.24466138629333986, 0.02, 13.0], [0.0017763393558212948, -0.2444121271923697, 0.011294466903728623, 13.0], [0.006919648241827286, 0.9072597867122164, 0.013415851108815928, 12.0], [0.006919676573949693, 0.9072415562383671, 0.013416019433648575, 12.0], [0.0069196742273375375, 0.9072428319149449, 0.013416119211317922, 12.0], [0.0069196737062991315, 0.9072428053111482, 0.013416222037236102, 12.0], [0.006919672596154976, 0.9072428060441141, 0.01341632487324996, 12.0], [0.0069196728536420945, 0.9072428057696265, 0.013416428536880062, 12.0], [0.006919672030383588, 0.9072428062987339, 0.013416532849275157, 12.0], [0.006919671485040645, 0.9072428056463088, 0.013416638739405509, 12.0], [0.0088634361719844, 0.9072428736032068, 0.015490618632826, 12.0], [0.006206553672460012, 0.9072409017036367, 0.013089847592953912, 12.0], [0.006919836383531367, 0.9072487515605051, 0.013417895690745219, 12.0], [0.009131416243305874, 0.9072411745202108, 0.01677726485377951, 12.0], [0.006452258217575044, 0.9072195422717569, 0.02, 12.0], [0.00907429842613455, 0.9068419109566946, 0.02, 12.0]], "y": [495715.30302949616, 1028781.885308199, 1195926.3482198115, 791704.129625198, 650349.5120037223, 650370.889114965, 581291.253732256, 618198.7101778053, 478498.42040932295, 617580.0469469524, 478647.36947380577, 478480.1464839736, 493554.9640536321, 478350.29025078384, 478470.0002859946, 720336.0372922813, 642179.4564052083, 642174.1432295728, 642170.9541899076, 642167.672164995, 642164.3897685845, 642161.0809038035, 642157.7514282184, 642154.3716023241, 580849.795793916, 652746.5737736713, 642114.227492796, 547302.0547031246, 475699.9995164631, 475598.027092055], "counter": 30, "min_y": 475598.027092055, "min_X": [0.00907429842613455, 0.9068419109566946, 0.02, 12.0], "min_mean_X": [0.00907429842613455, 0.9068419109566946, 0.02, 12.0], "min_mean_y": 475598.027092055, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006145661494013283, 0.907236718877838, 0.013162667499175565, 12.0], [0.006129061414450295, 0.90724244103414, 0.01547836145018752, 12.0], [0.007729652851161041, 0.9072393646684052, 0.014188374644020035, 12.0], [0.0073423411982307335, -0.26305183901903595, 0.02, 13.0], [0.00745279244360387, 0.9072430189556357, 0.014209323046895046, 12.0], [0.0024150316336011162, -0.24471595154093473, 0.02, 13.0], [0.006701257589711842, -0.24511650039986962, 0.02, 13.0], [0.000191128682961689, -0.244951902401147, 0.019276213545435187, 13.0], [0.01, -0.24494615080525997, 0.02, 13.0], [0.006931738975301204, -0.24466138629333986, 0.02, 13.0], [0.0017763393558212948, -0.2444121271923697, 0.011294466903728623, 13.0], [0.006919648241827286, 0.9072597867122164, 0.013415851108815928, 12.0], [0.006919676573949693, 0.9072415562383671, 0.013416019433648575, 12.0], [0.0069196742273375375, 0.9072428319149449, 0.013416119211317922, 12.0], [0.0069196737062991315, 0.9072428053111482, 0.013416222037236102, 12.0], [0.006919672596154976, 0.9072428060441141, 0.01341632487324996, 12.0], [0.0069196728536420945, 0.9072428057696265, 0.013416428536880062, 12.0], [0.006919672030383588, 0.9072428062987339, 0.013416532849275157, 12.0], [0.006919671485040645, 0.9072428056463088, 0.013416638739405509, 12.0], [0.0088634361719844, 0.9072428736032068, 0.015490618632826, 12.0], [0.006206553672460012, 0.9072409017036367, 0.013089847592953912, 12.0], [0.006919836383531367, 0.9072487515605051, 0.013417895690745219, 12.0], [0.009131416243305874, 0.9072411745202108, 0.01677726485377951, 12.0], [0.006452258217575044, 0.9072195422717569, 0.02, 12.0], [0.00907429842613455, 0.9068419109566946, 0.02, 12.0]], "mean_y": [495715.30302949616, 1028781.885308199, 1195926.3482198115, 791704.129625198, 650349.5120037223, 650370.889114965, 581291.253732256, 618198.7101778053, 478498.42040932295, 617580.0469469524, 478647.36947380577, 478480.1464839736, 493554.9640536321, 478350.29025078384, 478470.0002859946, 720336.0372922813, 642179.4564052083, 642174.1432295728, 642170.9541899076, 642167.672164995, 642164.3897685845, 642161.0809038035, 642157.7514282184, 642154.3716023241, 580849.795793916, 652746.5737736713, 642114.227492796, 547302.0547031246, 475699.9995164631, 475598.027092055], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713473542.492955", "result": "Results for 000_1713473542.492955: Finally, the best value is 475480.1880837982 at [9.27616564e-03 9.52242682e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_22-52-15", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061444408248602376, 0.9072366949244571, 0.013162737279342923, 12.0], [0.006144032258702795, 0.9072368930436269, 0.01547514343112806, 12.0], [0.00772986381690095, 0.9072368995922464, 0.014186663205327665, 12.0], [0.007342311268639411, -0.2630514252410119, 0.02, 13.0], [0.008150033117549733, 0.9072449443407115, 0.014286253693932865, 12.0], [0.0024217291987013202, -0.244717928869119, 0.02, 13.0], [0.008921485076425126, 0.9072844547210438, 0.02, 12.0], [0.01, -0.25107984351563983, 0.02, 13.0], [0.0034763667897663116, -0.24969299308573392, 0.02, 13.0], [0.0020963764917986166, -0.24874802977564617, 0.02, 13.0], [0.01, -0.2480592786019476, 0.02, 13.0], [0.0020684515899424705, -0.24753437228459138, 0.01731063121180828, 13.0], [0.005686418837741717, 0.9082747266679201, 0.01931389043907351, 12.0], [0.0032210210023201585, 0.9210127654161062, 0.02, 12.0], [0.006142193333654452, 0.959878376487618, 0.02, 12.0], [0.004427527546317497, 0.9529939362147779, 0.02, 12.0], [0.00927616564068443, 0.9522426823353023, 0.02, 12.0], [0.0024996870215936466, 0.9516433147328686, 0.02, 12.0], [0.004271138664424581, 0.9511175756941898, 0.02, 12.0], [0.0063252340352537625, 0.9506499273391881, 0.02, 12.0], [0.00446130389729424, 0.9502825467867748, 0.019693976898270626, 12.0], [0.009212020557544295, 0.9499212656549548, 0.02, 12.0], [0.007119045153264635, 0.9495635860515662, 0.02, 12.0], [0.005378853163267859, 0.9492376688396412, 0.02, 12.0], [0.0086706296767377, 0.9489408106991288, 0.02, 12.0]], "y": [495715.3028911534, 1028781.8852824374, 1195926.3482240585, 791704.1296178144, 650349.5119812408, 650368.6642564018, 581378.610456764, 618250.1773071032, 478498.4205493525, 615249.7722654185, 478647.1114343123, 475602.95194313, 478365.14291019144, 478617.77419722517, 478669.6372364134, 478357.8286471255, 537725.3328121831, 489670.1557808291, 475793.3963930461, 475584.6761060347, 475668.62580395717, 475480.1880837982, 475747.5426067296, 475679.3051659468, 475599.83635508927, 481812.0803621117, 475488.3253808469, 475571.3179886125, 475640.3907297063, 475511.9428352611], "counter": 30, "min_y": 475480.1880837982, "min_X": [0.00927616564068443, 0.9522426823353023, 0.02, 12.0], "min_mean_X": [0.00927616564068443, 0.9522426823353023, 0.02, 12.0], "min_mean_y": 475480.1880837982, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061444408248602376, 0.9072366949244571, 0.013162737279342923, 12.0], [0.006144032258702795, 0.9072368930436269, 0.01547514343112806, 12.0], [0.00772986381690095, 0.9072368995922464, 0.014186663205327665, 12.0], [0.007342311268639411, -0.2630514252410119, 0.02, 13.0], [0.008150033117549733, 0.9072449443407115, 0.014286253693932865, 12.0], [0.0024217291987013202, -0.244717928869119, 0.02, 13.0], [0.008921485076425126, 0.9072844547210438, 0.02, 12.0], [0.01, -0.25107984351563983, 0.02, 13.0], [0.0034763667897663116, -0.24969299308573392, 0.02, 13.0], [0.0020963764917986166, -0.24874802977564617, 0.02, 13.0], [0.01, -0.2480592786019476, 0.02, 13.0], [0.0020684515899424705, -0.24753437228459138, 0.01731063121180828, 13.0], [0.005686418837741717, 0.9082747266679201, 0.01931389043907351, 12.0], [0.0032210210023201585, 0.9210127654161062, 0.02, 12.0], [0.006142193333654452, 0.959878376487618, 0.02, 12.0], [0.004427527546317497, 0.9529939362147779, 0.02, 12.0], [0.00927616564068443, 0.9522426823353023, 0.02, 12.0], [0.0024996870215936466, 0.9516433147328686, 0.02, 12.0], [0.004271138664424581, 0.9511175756941898, 0.02, 12.0], [0.0063252340352537625, 0.9506499273391881, 0.02, 12.0], [0.00446130389729424, 0.9502825467867748, 0.019693976898270626, 12.0], [0.009212020557544295, 0.9499212656549548, 0.02, 12.0], [0.007119045153264635, 0.9495635860515662, 0.02, 12.0], [0.005378853163267859, 0.9492376688396412, 0.02, 12.0], [0.0086706296767377, 0.9489408106991288, 0.02, 12.0]], "mean_y": [495715.3028911534, 1028781.8852824374, 1195926.3482240585, 791704.1296178144, 650349.5119812408, 650368.6642564018, 581378.610456764, 618250.1773071032, 478498.4205493525, 615249.7722654185, 478647.1114343123, 475602.95194313, 478365.14291019144, 478617.77419722517, 478669.6372364134, 478357.8286471255, 537725.3328121831, 489670.1557808291, 475793.3963930461, 475584.6761060347, 475668.62580395717, 475480.1880837982, 475747.5426067296, 475679.3051659468, 475599.83635508927, 481812.0803621117, 475488.3253808469, 475571.3179886125, 475640.3907297063, 475511.9428352611], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713474191.7077792", "result": "Results for 000_1713474191.7077792: Finally, the best value is 475449.85092438187 at [1.00000000e-02 9.53041708e-01 2.00000000e-02 1.20000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "AdaptiveStandardScaler", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_23-03-04", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061448345579317165, 0.9072367202573203, 0.013162738164729576, 12.0], [0.0061443862912875, 0.9072368845087407, 0.015477038244800347, 12.0], [0.00772988884929568, 0.9072369010166127, 0.014187689578402477, 12.0], [0.007342318992897419, -0.2630516654290681, 0.02, 13.0], [0.008136421149376374, 0.9072448884649325, 0.014287389698075076, 12.0], [0.0024145960116732836, -0.24473004690894629, 0.02, 13.0], [0.008921461180607217, 0.9072834458098797, 0.02, 12.0], [0.01, -0.25107881826278067, 0.02, 13.0], [0.003006919384436036, -0.24969244664086784, 0.012558432784121356, 13.0], [0.006560337846991146, 0.9075208999572247, 0.02, 12.0], [0.006061042859246181, 0.9087817211486187, 0.02, 12.0], [0.01, 0.9145702776210437, 0.02, 12.0], [0.01, 0.9341866918887054, 0.02, 12.0], [0.0026480811756634925, 0.9503264047081856, 0.02, 12.0], [0.0007605970307966506, 0.9528273936875233, 0.02, 12.0], [0.005837195734053306, 0.9531765159703689, 0.02, 12.0], [0.01, 0.9530417084882785, 0.02, 12.0], [0.0023019948064251275, 0.952744180419597, 0.02, 12.0], [0.004889717273663603, 0.9523625902291806, 0.02, 12.0], [0.01, 0.9519660575511333, 0.02, 12.0], [0.00928945798346674, 0.95157402417731, 0.02, 12.0], [0.006529811869460334, 0.9511851713009577, 0.02, 12.0], [0.01, 0.9508040316162094, 0.02, 12.0], [0.007459128957440954, 0.950439743890962, 0.02, 12.0], [0.009326426580560798, 0.950087788169527, 0.02, 12.0]], "y": [495715.30302739644, 1028781.8853171874, 1195926.3482395269, 791704.1296443669, 650349.5119949052, 650368.6200221636, 581326.8230193292, 618219.3098211427, 478498.4208594738, 615216.3931141556, 478647.4207065049, 475602.95530618326, 478365.1404764186, 674686.0373190275, 475695.0289631554, 475711.5683433217, 475542.99250851537, 475495.5000297491, 475744.908061869, 475812.9163319395, 475612.8695516271, 475449.85092438187, 475752.6346263072, 475652.01838572946, 475452.4551407435, 475481.28543343587, 475590.51303936413, 475455.26847702794, 475555.8521211523, 475483.4330219458], "counter": 30, "min_y": 475449.85092438187, "min_X": [0.01, 0.9530417084882785, 0.02, 12.0], "min_mean_X": [0.01, 0.9530417084882785, 0.02, 12.0], "min_mean_y": 475449.85092438187, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.0061448345579317165, 0.9072367202573203, 0.013162738164729576, 12.0], [0.0061443862912875, 0.9072368845087407, 0.015477038244800347, 12.0], [0.00772988884929568, 0.9072369010166127, 0.014187689578402477, 12.0], [0.007342318992897419, -0.2630516654290681, 0.02, 13.0], [0.008136421149376374, 0.9072448884649325, 0.014287389698075076, 12.0], [0.0024145960116732836, -0.24473004690894629, 0.02, 13.0], [0.008921461180607217, 0.9072834458098797, 0.02, 12.0], [0.01, -0.25107881826278067, 0.02, 13.0], [0.003006919384436036, -0.24969244664086784, 0.012558432784121356, 13.0], [0.006560337846991146, 0.9075208999572247, 0.02, 12.0], [0.006061042859246181, 0.9087817211486187, 0.02, 12.0], [0.01, 0.9145702776210437, 0.02, 12.0], [0.01, 0.9341866918887054, 0.02, 12.0], [0.0026480811756634925, 0.9503264047081856, 0.02, 12.0], [0.0007605970307966506, 0.9528273936875233, 0.02, 12.0], [0.005837195734053306, 0.9531765159703689, 0.02, 12.0], [0.01, 0.9530417084882785, 0.02, 12.0], [0.0023019948064251275, 0.952744180419597, 0.02, 12.0], [0.004889717273663603, 0.9523625902291806, 0.02, 12.0], [0.01, 0.9519660575511333, 0.02, 12.0], [0.00928945798346674, 0.95157402417731, 0.02, 12.0], [0.006529811869460334, 0.9511851713009577, 0.02, 12.0], [0.01, 0.9508040316162094, 0.02, 12.0], [0.007459128957440954, 0.950439743890962, 0.02, 12.0], [0.009326426580560798, 0.950087788169527, 0.02, 12.0]], "mean_y": [495715.30302739644, 1028781.8853171874, 1195926.3482395269, 791704.1296443669, 650349.5119949052, 650368.6200221636, 581326.8230193292, 618219.3098211427, 478498.4208594738, 615216.3931141556, 478647.4207065049, 475602.95530618326, 478365.1404764186, 674686.0373190275, 475695.0289631554, 475711.5683433217, 475542.99250851537, 475495.5000297491, 475744.908061869, 475812.9163319395, 475612.8695516271, 475449.85092438187, 475752.6346263072, 475652.01838572946, 475452.4551407435, 475481.28543343587, 475590.51303936413, 475455.26847702794, 475555.8521211523, 475483.4330219458], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713474507.747884", "result": "Results for 000_1713474507.747884: Finally, the best value is 3725.7464818617013 at [0.0e+00 1.0e+00 1.0e-03 1.3e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 9, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "Bikes", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 182470, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": false, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_23-05-44", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006138129897864835, 0.1119628795350841, 0.011548545274294136, 12.0], [0.006876397876545734, 0.11224723660794945, 0.01143371705168818, 12.0], [0.006875968669062261, 0.1124646652253057, 0.011434082306384123, 12.0], [0.0, 1.0, 0.001, 13.0]], "y": [54219.846900493954, 3780.8431173010395, 3728.5707960555387, 3824.731080759532, 3795.74414129673, 3800.073827792184, 3807.2442614112992, 3807.2916673663417, 3725.7464818617013], "counter": 9, "min_y": 3725.7464818617013, "min_X": [0.0, 1.0, 0.001, 13.0], "min_mean_X": [0.0, 1.0, 0.001, 13.0], "min_mean_y": 3725.7464818617013, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.006138129897864835, 0.1119628795350841, 0.011548545274294136, 12.0], [0.006876397876545734, 0.11224723660794945, 0.01143371705168818, 12.0], [0.006875968669062261, 0.1124646652253057, 0.011434082306384123, 12.0], [0.0, 1.0, 0.001, 13.0]], "mean_y": [54219.846900493954, 3780.8431173010395, 3728.5707960555387, 3824.731080759532, 3795.74414129673, 3800.073827792184, 3807.2442614112992, 3807.2916673663417, 3725.7464818617013], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
+{"data": {"id": "000_1713474669.259705", "result": "Results for 000_1713474669.259705: Finally, the best value is 30339.775171102374 at [ 4.63529627e-03 -2.21528408e-01  1.91626325e-02  1.30000000e+01].", "fun_control": {"PREFIX": "000", "CHECKPOINT_PATH": "runs/saved_models/", "DATASET_PATH": "data/", "RESULTS_PATH": "results/", "TENSORBOARD_PATH": "runs/", "_L_in": null, "_L_out": null, "_torchmetric": null, "accelerator": "auto", "converters": null, "core_model_name": "linear_model.LinearRegression", "counter": 30, "data": null, "data_dir": "./data", "data_module": null, "data_set": null, "data_set_name": "ChickWeights", "db_dict_name": "spotRiver_db.json", "design": null, "device": null, "devices": 1, "enable_progress_bar": false, "eval": null, "fun_evals": 30, "fun_repeats": 1, "horizon": 10, "infill_criterion": "y", "k_folds": 3, "log_graph": false, "log_level": 50, "loss_function": null, "lower": [0.0, 0.0, -1.0, 0.001, 11.0], "max_time": 1.0, "max_surrogate_points": 30, "metric_sklearn_name": "mean_absolute_error", "metric_params": {}, "model_dict": {}, "noise": true, "n_points": 1, "n_samples": 578, "n_total": null, "num_workers": 0, "ocba_delta": 0, "oml_grace_period": null, "optimizer": null, "path": null, "prep_model_name": "prep_generic_num_cat.py", "progress_file": "progress.txt", "save_model": false, "seed": 123, "show_batch_interval": 1000000, "show_models": false, "show_progress": true, "shuffle": true, "sigma": 0.0, "spot_tensorboard_path": "runs/spot_logs/000_bartz10_2024-04-18_23-11-00", "target_column": "y", "target_type": "int", "task": "Regression", "test_seed": 1234, "test_size": 0.3, "tolerance_x": 1.4901161193847656e-08, "upper": [0.0, 0.01, 1.0, 0.02, 13.0], "var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "var_type": ["int", "float", "float", "float", "int"], "verbosity": 1, "weights": [1000.0, 1.0, 1.0], "weight_coeff": 0.0, "weights_entry": "1000, 1, 1", "core_model_hyper_dict": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}, "core_model_hyper_dict_default": {"l2": {"type": "int", "default": 0, "transform": "None", "lower": 0, "upper": 0}, "l1": {"type": "float", "default": 0.0, "transform": "None", "lower": 0.0, "upper": 0.01}, "intercept_init": {"type": "float", "default": 0.0, "transform": "None", "lower": -1.0, "upper": 1.0}, "intercept_lr": {"type": "float", "default": 0.01, "transform": "None", "lower": 0.001, "upper": 0.02}, "clip_gradient": {"type": "int", "default": 12, "transform": "transform_power_10", "lower": 11, "upper": 13}}}, "design_control": {"init_size": 5, "repeats": 1}, "surrogate_control": {"log_level": 50, "noise": true, "model_fun_evals": 10000, "min_theta": -3.0, "max_theta": 2.0, "n_theta": 4, "p_val": 2.0, "n_p": 1, "optim_p": false, "min_Lambda": 0.001, "max_Lambda": 100.0, "seed": 124, "theta_init_zero": true, "var_type": ["float", "float", "float", "int"], "metric_factorial": "canberra"}, "optimizer_control": {"max_iter": 1000, "seed": 125}, "spot_tuner_control": {"eps": 1.4901161193847656e-08, "lower": [0.0, -1.0, 0.001, 11.0], "k": 4, "upper": [0.01, 1.0, 0.02, 13.0], "var_type": ["float", "float", "float", "int"], "var_name": ["l1", "intercept_init", "intercept_lr", "clip_gradient"], "all_lower": [0.0, 0.0, -1.0, 0.001, 11.0], "all_upper": [0.0, 0.01, 1.0, 0.02, 13.0], "ident": [true, false, false, false, false], "red_dim": 1, "all_var_type": ["int", "float", "float", "float", "int"], "all_var_name": ["l2", "l1", "intercept_init", "intercept_lr", "clip_gradient"], "fun_evals": 30, "fun_repeats": 1, "max_time": 1.0, "noise": true, "tolerance_x": 1.4901161193847656e-08, "ocba_delta": 0, "log_level": 50, "show_models": false, "show_progress": true, "infill_criterion": "y", "n_points": 1, "max_surrogate_points": 30, "progress_file": "progress.txt", "de_bounds": [[0.0, 0.01], [-1.0, 1.0], [0.001, 0.02], [11.0, 13.0]], "X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.009215002940123796, 0.9072367385454355, 0.013163336841261822, 12.0], [0.007816296396526354, 0.5927909068803928, 0.0059377360747771306, 12.0], [0.007729663011780999, 0.9072401996238824, 0.01370567453862569, 12.0], [0.0042510844942311825, 0.9073205751707294, 0.02, 12.0], [0.00012452508805700486, -0.2666777110273018, 0.011255636024496618, 13.0], [0.0, 0.9100479807712517, 0.02, 12.0], [0.004356319351320429, 0.9471286410713721, 0.02, 12.0], [0.005421715779835936, -0.2365679737156669, 0.02, 13.0], [0.0053470647192488, -0.2362547739441391, 0.01978794898003259, 13.0], [0.0, 0.9364499863439537, 0.02, 12.0], [0.0, 0.9367157097021114, 0.02, 12.0], [0.007403475093454809, -0.23529350100502927, 0.02, 13.0], [0.006457484856152526, -0.23490049019803763, 0.017601385681178153, 13.0], [0.0, 0.9364012285487366, 0.02, 12.0], [0.0, 0.9364189160355617, 0.02, 12.0], [0.0, 0.9363993352446174, 0.02, 12.0], [0.0, 0.9363663749039527, 0.02, 12.0], [0.0, 0.9363285434578908, 0.02, 12.0], [0.0, 0.9362893937232766, 0.02, 12.0], [0.0, 0.9362504024052074, 0.02, 12.0], [0.0, 0.9362122730331552, 0.02, 12.0], [0.0, 0.9361752045632754, 0.02, 12.0], [0.0, 0.9361392833730814, 0.02, 12.0], [0.003929822448923514, 0.9280390700677732, 0.02, 12.0], [0.0, 0.928544213896714, 0.02, 12.0]], "y": [30339.775171102374, 55110.84765588269, 75160.72569918972, 38973.344969951104, 33591.380469082294, 33592.926435604386, 50129.247727996495, 33130.57785277065, 30479.750798266883, 35979.829168951925, 30479.59626901737, 30477.2905844106, 30540.14530366303, 30592.538652029056, 30477.88287791439, 30477.813880326856, 30539.742821656942, 31190.562045888735, 30477.69866160409, 30477.66206542799, 30477.63065492615, 30477.60285603845, 30477.577657467347, 30477.554740829044, 30477.53378643214, 30477.51445377948, 30477.496586297897, 30477.480021085226, 30477.679451571446, 30477.85107845937], "counter": 30, "min_y": 30339.775171102374, "min_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_X": [0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], "min_mean_y": 30339.775171102374, "mean_X": [[0.004635296273503713, -0.22152840752088898, 0.019162632483464077, 13.0], [0.003648188197829939, 0.27516219733769054, 0.005091289007497186, 11.0], [0.00036049087681399585, -0.15595707724447438, 0.0028507122701277787, 13.0], [0.008351516807805177, -0.6855051853500382, 0.009582425201508104, 12.0], [0.0061451854829496656, 0.9072367245574324, 0.013163324511243687, 12.0], [0.009215002940123796, 0.9072367385454355, 0.013163336841261822, 12.0], [0.007816296396526354, 0.5927909068803928, 0.0059377360747771306, 12.0], [0.007729663011780999, 0.9072401996238824, 0.01370567453862569, 12.0], [0.0042510844942311825, 0.9073205751707294, 0.02, 12.0], [0.00012452508805700486, -0.2666777110273018, 0.011255636024496618, 13.0], [0.0, 0.9100479807712517, 0.02, 12.0], [0.004356319351320429, 0.9471286410713721, 0.02, 12.0], [0.005421715779835936, -0.2365679737156669, 0.02, 13.0], [0.0053470647192488, -0.2362547739441391, 0.01978794898003259, 13.0], [0.0, 0.9364499863439537, 0.02, 12.0], [0.0, 0.9367157097021114, 0.02, 12.0], [0.007403475093454809, -0.23529350100502927, 0.02, 13.0], [0.006457484856152526, -0.23490049019803763, 0.017601385681178153, 13.0], [0.0, 0.9364012285487366, 0.02, 12.0], [0.0, 0.9364189160355617, 0.02, 12.0], [0.0, 0.9363993352446174, 0.02, 12.0], [0.0, 0.9363663749039527, 0.02, 12.0], [0.0, 0.9363285434578908, 0.02, 12.0], [0.0, 0.9362893937232766, 0.02, 12.0], [0.0, 0.9362504024052074, 0.02, 12.0], [0.0, 0.9362122730331552, 0.02, 12.0], [0.0, 0.9361752045632754, 0.02, 12.0], [0.0, 0.9361392833730814, 0.02, 12.0], [0.003929822448923514, 0.9280390700677732, 0.02, 12.0], [0.0, 0.928544213896714, 0.02, 12.0]], "mean_y": [30339.775171102374, 55110.84765588269, 75160.72569918972, 38973.344969951104, 33591.380469082294, 33592.926435604386, 50129.247727996495, 33130.57785277065, 30479.750798266883, 35979.829168951925, 30479.59626901737, 30477.2905844106, 30540.14530366303, 30592.538652029056, 30477.88287791439, 30477.813880326856, 30539.742821656942, 31190.562045888735, 30477.69866160409, 30477.66206542799, 30477.63065492615, 30477.60285603845, 30477.577657467347, 30477.554740829044, 30477.53378643214, 30477.51445377948, 30477.496586297897, 30477.480021085226, 30477.679451571446, 30477.85107845937], "var_y": [NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN, NaN], "min_var_y": NaN}}}
```

### Comparing `spotgui-0.5.1/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle` & `spotgui-0.5.2/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle` & `spotgui-0.5.2/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/demos/spot_demo_00_experiment.pickle` & `spotgui-0.5.2/spotRiverGUI/demos/spot_demo_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle` & `spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle` & `spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/images/spotlogo.png` & `spotgui-0.5.2/src/spotGUI/ctk/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/spotRiverGUI.py` & `spotgui-0.5.2/spotRiverGUI/spotRiverGUI.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,295 +1,56 @@
-from concurrent.futures import ThreadPoolExecutor
-# from threading import Thread
 import tkinter as tk
-import time
-import json
-import threading
 import customtkinter
 import pprint
 import webbrowser
 import os
 import numpy as np
 import copy
-import sys
-from PIL import Image
 from spotPython.utils.init import fun_control_init, design_control_init, surrogate_control_init, optimizer_control_init
-from spotGUI.ctk.CTk import CTkApp
+from spotGUI.ctk.CTk import CTkApp, SelectOptionMenuFrame
 
 from spotRiver.data.river_hyper_dict import RiverHyperDict
 from spotGUI.tuner.spotRun import (
     run_spot_python_experiment,
-    contour_plot,
-    parallel_plot,
-    importance_plot,
-    progress_plot,
-    actual_vs_prediction,
-    compare_tuned_default,
-    all_compare_tuned_default,
-    plot_confusion_matrices,
-    plot_rocs,
-    destroy_entries,
+    actual_vs_prediction_river,
+    compare_river_tuned_default,
+    plot_confusion_matrices_river,
+    plot_rocs_river,
     load_file_dialog,
-    get_report_file_name,
-    get_result,
     get_core_model_from_name,
     get_n_total,
     get_fun_evals,
     get_lambda_min_max,
     get_oml_grace_period,
-    get_prep_model,
     get_metric_sklearn,
     get_weights,
     get_kriging_noise,
     get_task_dict,
-    show_data,
     show_y_hist,
 )
 from spotRiver.data.selector import get_river_dataset_from_name
-from spotPython.utils.convert import map_to_True_False, check_type
+from spotPython.utils.convert import map_to_True_False, set_dataset_target_type, check_type
 from spotRiver.utils.data_conversion import split_df
-from spotPython.utils.numpy2json import NumpyEncoder
 from spotPython.hyperparameters.values import (
     add_core_model_to_fun_control,
-    set_control_hyperparameter_value,
     update_fun_control_with_hyper_num_cat_dicts,
 )
-from spotPython.utils.eda import gen_design_table
 from spotRiver.fun.hyperriver import HyperRiver
 from spotPython.utils.file import load_experiment as load_experiment_spot
-from spotPython.utils.file import get_experiment_filename
-
-customtkinter.set_default_color_theme("blue")  # Themes: "blue" (standard), "green", "dark-blue"
-
-
-class SelectScrollableComboBoxFrame(customtkinter.CTkScrollableFrame):
-    def __init__(self, master, item_list, item_default, command=None, **kwargs):
-        super().__init__(master, **kwargs)
-
-        self.combobox_var = customtkinter.StringVar(value=item_default)
-        combobox = customtkinter.CTkComboBox(
-            self, values=item_list, command=self.combobox_callback, variable=self.combobox_var
-        )
-        combobox.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="ew")
-        self.combobox_var.set(item_default)
-
-    def combobox_callback(self, choice):
-        print("combobox dropdown selected:", choice)
-
-    def get_selected_item(self):
-        return self.combobox_var.get()
-
-
-class SelectOptionMenuFrame(customtkinter.CTkFrame):
-    def __init__(self, master, title, item_list, item_default, command=None, **kwargs):
-        super().__init__(master, **kwargs)
-        self.title = title
-        self.title_label = customtkinter.CTkLabel(self, text=self.title, corner_radius=6)
-        self.title_label.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="ew")
-        print(f"item_list: {item_list}")
-
-        if item_default is None:
-            item_default = item_list[0]
-        self.optionmenu_var = customtkinter.StringVar(value=item_default)
-        optionmenu = customtkinter.CTkOptionMenu(self, values=item_list, command=command, variable=self.optionmenu_var)
-        optionmenu.grid(row=1, column=0, padx=10, pady=(10, 0), sticky="ew")
-        self.optionmenu_var.set(item_default)
-
-    def get_selected_optionmenu_item(self):
-        return self.optionmenu_var.get()
-
-    def set_selected_optionmenu_item(self, item):
-        self.optionmenu_var.set(item)
-
-
-class NumHyperparameterFrame(customtkinter.CTkFrame):
-    def __init__(self, master, command=None, entry_width=120, **kwargs):
-        super().__init__(master, **kwargs)
-        self.grid_columnconfigure(0, weight=1)
-        self.entry_width = entry_width
-
-        self.command = command
-        self.hp_list = []
-        self.default_list = []
-        self.lower_list = []
-        self.upper_list = []
-        self.transform_list = []
-        self.level_list = []
-
-    def add_header(self):
-        header_hp = customtkinter.CTkLabel(self, text="Hyperparameter", corner_radius=6)
-        header_hp.grid(row=0, column=0, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Default", corner_radius=6)
-        header_hp.grid(row=0, column=1, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Lower", corner_radius=6)
-        header_hp.grid(row=0, column=2, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Upper", corner_radius=6)
-        header_hp.grid(row=0, column=3, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Transform", corner_radius=6)
-        header_hp.grid(row=0, column=4, padx=0, pady=(10, 0), sticky="w")
-
-    def add_num_item(self, hp, default, lower, upper, transform):
-        self.hp_col = customtkinter.CTkLabel(self, text=hp, compound="left", padx=5, anchor="w")
-        self.default_col = customtkinter.CTkLabel(self, text=default, compound="left", padx=5, anchor="w")
-        self.lower_col = customtkinter.CTkEntry(self, width=self.entry_width)
-        self.lower_col.insert(0, str(lower))
-        self.upper_col = customtkinter.CTkEntry(self, width=self.entry_width)
-        self.upper_col.insert(0, str(upper))
-        self.transform_col = customtkinter.CTkLabel(self, text=transform, compound="left", padx=5, anchor="w")
-
-        self.hp_col.grid(row=1 + len(self.hp_list), column=0, pady=(0, 10), sticky="w")
-        self.default_col.grid(row=1 + len(self.default_list), column=1, pady=(0, 10), sticky="w")
-        self.lower_col.grid(row=1 + len(self.lower_list), column=2, pady=(0, 10), sticky="w")
-        self.upper_col.grid(row=1 + len(self.upper_list), column=3, pady=(0, 10), sticky="w")
-        self.transform_col.grid(row=1 + len(self.transform_list), column=4, pady=(0, 10), padx=5, sticky="w")
-        self.hp_list.append(self.hp_col)
-        self.default_list.append(self.default_col)
-        self.lower_list.append(self.lower_col)
-        self.upper_list.append(self.upper_col)
-        self.transform_list.append(self.transform_col)
-
-    def get_num_item(self) -> dict:
-        """
-        Get the values from self.hp_list, self.default_list, self.lower_list, self.upper_list,
-        and self.transform_list and put lower and upper in a dictionary with the corresponding
-        hyperparameter (hp) as key.
-
-        Note:
-            Method is designed for numerical parameters.
-
-        Args:
-            None
-
-        Returns:
-            num_hp_dict (dict): dictionary with hyperparameter as key and values
-            as dictionary with lower and upper values.
-        """
-        num_hp_dict = {}
-        for label, default, lower, upper, transform in zip(
-            self.hp_list, self.default_list, self.lower_list, self.upper_list, self.transform_list
-        ):
-            num_hp_dict[label.cget("text")] = dict(
-                lower=lower.get(),
-                upper=upper.get(),
-            )
-        return num_hp_dict
-
-    def remove_num_item(self, item):
-        for label, default, lower, upper, transform in zip(
-            self.hp_list, self.default_list, self.lower_list, self.upper_list, self.transform_list
-        ):
-            if item == label.cget("text"):
-                label.destroy()
-                default.destroy()
-                lower.destroy()
-                upper.destroy()
-                transform.destroy()
-                self.hp_list.remove(label)
-                self.default_list.remove(default)
-                self.lower_list.remove(lower)
-                self.upper_list.remove(upper)
-                self.transform_list.remove(transform)
-                return
-
-
-class CatHyperparameterFrame(customtkinter.CTkFrame):
-    def __init__(self, master, command=None, **kwargs):
-        super().__init__(master, **kwargs)
-        self.grid_columnconfigure(0, weight=1)
-
-        self.command = command
-        self.hp_list = []
-        self.default_list = []
-        self.lower_list = []
-        self.upper_list = []
-        self.transform_list = []
-        self.levels_list = []
-
-    def add_header(self):
-        header_hp = customtkinter.CTkLabel(self, text="Hyperparameter", corner_radius=6)
-        header_hp.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="ew")
-        header_hp = customtkinter.CTkLabel(self, text="Default", corner_radius=6)
-        header_hp.grid(row=0, column=1, padx=10, pady=(10, 0), sticky="ew")
-        header_hp = customtkinter.CTkLabel(self, text="Levels", corner_radius=6)
-        header_hp.grid(row=0, column=2, padx=10, pady=(10, 0), sticky="ew")
-
-    def add_cat_item(self, hp, default, levels, transform):
-        self.hp_col = customtkinter.CTkLabel(self, text=hp, compound="left", padx=5, anchor="w")
-        self.default_col = customtkinter.CTkLabel(self, text=default, compound="left", padx=5, anchor="w")
-        self.levels_col = customtkinter.CTkTextbox(self, width=400, height=1)
-        string_items = " ".join(levels)
-        self.levels_col.insert("0.0", string_items)
-
-        self.hp_col.grid(row=1 + len(self.hp_list), column=0, pady=(0, 10), sticky="w")
-        self.default_col.grid(row=1 + len(self.default_list), column=1, pady=(0, 10), sticky="w")
-        self.levels_col.grid(row=1 + len(self.levels_list), column=2, pady=(0, 10), sticky="w")
-        self.hp_list.append(self.hp_col)
-        self.default_list.append(self.default_col)
-        self.levels_list.append(self.levels_col)
-
-    def get_cat_item(self):
-        """
-        Get the values self.hp_list, self.default_list, self.levels_list,
-        and put lower and upper in a dictionary with the corresponding
-        hyperparameter (hp) as key.
-
-        Note:
-            Method is designed for categorical parameters.
-
-        Args:
-            None
-
-        Returns:
-            num_hp_dict (dict): dictionary with hyperparameter as key and values
-            as dictionary with lower and upper values.
-        """
-        cat_hp_dict = {}
-        for label, default, levels in zip(self.hp_list, self.default_list, self.levels_list):
-            cat_hp_dict[label.cget("text")] = dict(
-                levels=levels.get("0.0", "end-1c"),
-            )
-        return cat_hp_dict
-
-    def remove_cat_item(self, item):
-        for (
-            label,
-            default,
-            levels,
-        ) in zip(self.hp_list, self.default_list, self.level_list):
-            if item == label.cget("text"):
-                label.destroy()
-                default.destroy()
-                levels.destroy()
-                self.hp_list.remove(label)
-                self.default_list.remove(default)
-                self.lower_list.remove(levels)
-                return
 
 
 class RiverApp(CTkApp):
     def __init__(self):
         super().__init__()
 
         self.title("spotRiver GUI")
         self.geometry(f"{1600}x{900}")
         self.grid_columnconfigure((0, 1, 2, 3, 4), weight=1)
         self.grid_rowconfigure((0, 1), weight=1)
         self.entry_width = 80
-        # dictionary name for the database
-        # similar for all spotRiver experiments
-        self.db_dict_name = "spotRiver_db.json"
-        # name of the progress file
-        # self.progress_file = "progress.txt"
-        # if the progress file exists, delete it
-        # if os.path.exists(self.progress_file):
-        #    os.remove(self.progress_file)
-
-        current_path = os.path.dirname(os.path.abspath(__file__))
-        image_path = os.path.join(current_path, "images")
-        self.logo_image = customtkinter.CTkImage(Image.open(os.path.join(image_path, "spotlogo.png")), size=(85, 37))
 
         self.rhd = RiverHyperDict()
         self.task_name = "regression_tab"
         self.task_dict = get_task_dict()
         pprint.pprint(self.task_dict)
         self.core_model_name = self.task_dict[self.task_name]["core_model_names"][0]
         # Uncomment to get user defined core models (not useful for spotRiver):
@@ -801,20 +562,20 @@
             self.analysis_comparison_frame,
             text="Comparisons",
             font=customtkinter.CTkFont(weight="bold"),
             corner_radius=6,
         )
         self.analysis_comparison_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
         # create tuned default button
-        self.compare_tuned_default_button = customtkinter.CTkButton(
+        self.compare_river_tuned_default_button = customtkinter.CTkButton(
             master=self.analysis_comparison_frame,
             text="Tuned vs. default",
             command=self.plot_tuned_default_button_event,
         )
-        self.compare_tuned_default_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
+        self.compare_river_tuned_default_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
         #
         # create actual prediction button
         self.compare_actual_prediction_button = customtkinter.CTkButton(
             master=self.analysis_comparison_frame,
             text="Actual vs. prediction",
             command=self.plot_actual_prediction_button_event,
         )
@@ -886,180 +647,30 @@
         # update_thread.start()
         # e = ThreadPoolExecutor(max_workers=1)
         # e.submit(self.update_text)
         # e.shutdown(wait=False)
 
         # ---------------------------------------------------------------------- #
 
-    def print_tuned_design(self):
-        text = gen_design_table(self.fun_control)
-        self.textbox.delete("1.0", tk.END)
-        self.textbox.insert(tk.END, text)
-
-    def update_text(self):
-        # This method runs in a separate thread to update the text area
-        while True:  # Infinite loop to continuously update the textbox
-            try:
-                with open("progress.txt", "r") as file:
-                    lines = file.readlines()
-                    last_line = lines[-1] if lines else ""
-                    # Get the last line or an empty string if file is empty
-                    # text = file.read()  # Read the entire file
-                    self.textbox.delete("1.0", tk.END)
-                    self.textbox.insert(tk.END, last_line)
-            except FileNotFoundError:
-                # text = "File not found."
-                # self.textbox.insert(tk.END, text)
-                pass
-            time.sleep(1)  # Wait for 1 second before the next update
-
-    def plot_progress_button_event(self):
-        if self.spot_tuner is not None:
-            progress_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
-
+    # -------------- River specific plots ----------------- #
     def plot_tuned_default_button_event(self):
         if self.spot_tuner is not None:
-            compare_tuned_default(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
+            compare_river_tuned_default(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
     def plot_actual_prediction_button_event(self):
         if self.spot_tuner is not None:
-            actual_vs_prediction(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
-
-    def plot_contour_button_event(self):
-        if self.spot_tuner is not None:
-            contour_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
-
-    def plot_importance_button_event(self):
-        if self.spot_tuner is not None:
-            importance_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+            actual_vs_prediction_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
 
     def plot_confusion_button_event(self):
         if self.spot_tuner is not None:
-            plot_confusion_matrices(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
+            plot_confusion_matrices_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
     def plot_roc_button_event(self):
         if self.spot_tuner is not None:
-            plot_rocs(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
-
-    def label_button_frame_event(self, item):
-        print(f"label button frame clicked: {item}")
-
-    def select_data_frame_event(self, new_data: str):
-        print(f"Data modified: {new_data}")
-        print(f"Data Selection modified: {self.select_data_frame.get_selected_optionmenu_item()}")
-
-    def create_num_hp_frame(self, dict=None):
-        # create new num_hp_frame
-        self.num_hp_frame = NumHyperparameterFrame(
-            master=self.hp_main_frame, width=640, command=self.label_button_frame_event, entry_width=self.entry_width
-        )
-
-        self.num_hp_frame.grid(row=1, column=0, padx=0, pady=0, sticky="nsew")
-        self.num_hp_frame.add_header()
-        print(f"self.core_model_name: {self.core_model_name}")
-        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
-        if dict is None:
-            dict = self.rhd.hyper_dict[coremodel]
-        for i, (key, value) in enumerate(dict.items()):
-            if (
-                dict[key]["type"] == "int"
-                or dict[key]["type"] == "float"
-                or dict[key]["core_model_parameter_type"] == "bool"
-            ):
-                self.num_hp_frame.add_num_item(
-                    hp=key,
-                    default=value["default"],
-                    lower=value["lower"],
-                    upper=value["upper"],
-                    transform=value["transform"],
-                )
-
-    def create_cat_hp_frame(self, dict=None):
-        self.cat_hp_frame = CatHyperparameterFrame(master=self.hp_main_frame, command=self.label_button_frame_event)
-        self.cat_hp_frame.grid(row=2, column=0, padx=0, pady=0, sticky="nsew")
-        print(f"self.core_model_name: {self.core_model_name}")
-        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
-        if dict is None:
-            dict = self.rhd.hyper_dict[coremodel]
-        empty = True
-        for i, (key, value) in enumerate(dict.items()):
-            if dict[key]["type"] == "factor" and dict[key]["core_model_parameter_type"] != "bool":
-                if empty:
-                    self.cat_hp_frame.add_header()
-                    empty = False
-                self.cat_hp_frame.add_cat_item(
-                    hp=key, default=value["default"], levels=value["levels"], transform=value["transform"]
-                )
-
-    def create_core_model_frame(self, row, column):
-        # create new core model frame
-        self.select_core_model_frame = SelectOptionMenuFrame(
-            master=self.sidebar_frame,
-            command=self.select_core_model_frame_event,
-            item_list=self.task_dict[self.task_name]["core_model_names"],
-            item_default=None,
-            title="Select Core Model",
-        )
-        self.select_core_model_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nsew")
-        self.select_core_model_frame.configure(width=500)
-        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-
-    def create_select_data_frame(self, row, column):
-        data_set_values = copy.deepcopy(self.task_dict[self.task_name]["datasets"])
-        data_set_values.extend([f for f in os.listdir("userData") if f.endswith(".csv") or f.endswith(".pkl")])
-        self.select_data_frame = SelectOptionMenuFrame(
-            master=self.sidebar_frame,
-            command=self.select_data_frame_event,
-            item_list=data_set_values,
-            item_default=None,
-            title="Select Data",
-        )
-        self.select_data_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nswe")
-        self.select_data_frame.configure(width=500)
-        self.data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-
-    def select_core_model_frame_event(self, new_core_model: str):
-        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-        self.num_hp_frame.destroy()
-        self.create_num_hp_frame()
-        self.cat_hp_frame.destroy()
-        self.create_cat_hp_frame()
-
-    def select_prep_model_frame_event(self, new_prep_model: str):
-        print(f"Prep Model modified: {self.select_prep_model_frame.get_selected_optionmenu_item()}")
-
-    def select_metric_sklearn_levels_frame_event(self, new_metric_sklearn_levels: str):
-        print(f"Metric sklearn modified: {self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()}")
-        self.metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
-
-    def change_task_event(self, new_task: str):
-        print(f"Task changed to: {new_task}")
-        if new_task == "Binary Classification":
-            self.task_name = "classification_tab"
-        elif new_task == "Regression":
-            self.task_name = "regression_tab"
-        else:
-            print("Error: Task not found")
-        self.select_core_model_frame.destroy()
-        self.create_core_model_frame(row=2, column=0)
-        self.num_hp_frame.destroy()
-        self.create_num_hp_frame()
-        self.cat_hp_frame.destroy()
-        self.create_cat_hp_frame()
-        self.select_data_frame.destroy()
-        self.create_select_data_frame(row=4, column=0)
-
-    def run_button_event(self):
-        self.save_only = False
-        self.run_experiment()
-        # self.print_tuned_design()
-
-    def save_button_event(self):
-        self.save_only = True
-        self.run_experiment()
+            plot_rocs_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
     def load_button_event(self):
         filename = load_file_dialog()
         if filename:
             (
                 self.spot_tuner,
                 self.fun_control,
@@ -1154,132 +765,119 @@
             self.loaded_label.configure(text=self.experiment_name)
             self.experiment_name_entry.delete(0, "end")
             self.experiment_name_entry.insert(0, self.experiment_name)
             #
             # self.print_tuned_design()
 
     def plot_data_button_event(self):
-        self.seed = int(self.seed_var.get())
-        self.test_size = float(self.test_size_var.get())
-        self.shuffle = map_to_True_False(self.shuffle_var.get())
-        self.prepare_data()
-        show_y_hist(train=self.train, test=self.test, target_column="y")
+        train, test, n_samples, target_type = self.prepare_data()
+        show_y_hist(train=train, test=test, target_column="y")
         # TODO: show_data
         # show_data(train=self.train,
         #           test=self.test,
         #           target_column=self.target_column,
         #           n_samples=1000)
         print("\nData shown. No result saved.")
 
-    def get_dataset(self):
-        self.data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-        self.dataset, self.n_samples = get_river_dataset_from_name(
-            data_set_name=self.data_set_name,
+    def prepare_data(self):
+        seed = int(self.seed_var.get())
+        test_size = float(self.test_size_var.get())
+        shuffle = map_to_True_False(self.shuffle_var.get())
+        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
+        dataset, n_samples = get_river_dataset_from_name(
+            data_set_name=data_set_name,
             n_total=get_n_total(self.n_total_var.get()),
             river_datasets=self.task_dict[self.task_name]["datasets"],
         )
-
-    def set_dataset_y_type(self):
-        val = copy.deepcopy(self.dataset.iloc[0, -1])
-        self.target_type = check_type(val)
-        if self.target_type == "bool" or self.target_type == "str":
-            # convert the target column to 0 and 1
-            self.dataset["y"] = self.dataset["y"].astype(int)
-
-    def prepare_data(self):
-        self.get_dataset()
-        self.set_dataset_y_type()
-        self.train, self.test, self.n_samples = split_df(
-            dataset=self.dataset,
-            test_size=self.test_size,
-            target_type=self.target_type,
-            seed=self.seed,
-            shuffle=self.shuffle,
+        val = copy.deepcopy(dataset.iloc[0, -1])
+        target_type = check_type(val)
+        dataset = set_dataset_target_type(dataset=dataset, target="y")
+        train, test, n_samples = split_df(
+            dataset=dataset,
+            test_size=test_size,
+            target_type=target_type,
+            seed=seed,
+            shuffle=shuffle,
             stratify=None,
         )
+        return train, test, n_samples, target_type
 
     def run_experiment(self):
         task_name = self.task_frame.get_selected_optionmenu_item()
-        #
         core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-        #
         prep_model_name = self.select_prep_model_frame.get_selected_optionmenu_item()
         prepmodel = self.check_user_prep_model(prep_model_name=prep_model_name)
-        #
-        self.seed = int(self.seed_var.get())
-        self.test_size = float(self.test_size_var.get())
-        self.shuffle = map_to_True_False(self.shuffle_var.get())
-        self.prepare_data()
+
+        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
+
+        seed = int(self.seed_var.get())
+        test_size = float(self.test_size_var.get())
+        shuffle = map_to_True_False(self.shuffle_var.get())
         metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
         metric_sklearn = get_metric_sklearn(self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item())
-        #
+
         n_total = get_n_total(self.n_total_var.get())
-        #
-        # test_size = float(self.test_size_var.get())
-        #
-        # shuffle = map_to_True_False(self.shuffle_var.get())
-        #
         max_time = float(self.max_time_var.get())
-        #
         fun_evals = get_fun_evals(self.fun_evals_var.get())
-        #
         init_size = int(self.init_size_var.get())
         #
         lbd_min, lbd_max = get_lambda_min_max(self.lambda_min_max_var.get())
         kriging_noise = get_kriging_noise(lbd_min, lbd_max)
-        #
         max_surrogate_points = int(self.max_sp_var.get())
         #
-        # seed = int(self.seed_var.get())
-        #
+
         noise = map_to_True_False(self.noise_var.get())
         #
+        TENSORBOARD_CLEAN = map_to_True_False(self.tb_clean_var.get())
+        tensorboard_start = map_to_True_False(self.tb_start_var.get())
+        tensorboard_stop = map_to_True_False(self.tb_stop_var.get())
+        PREFIX = self.experiment_name_entry.get()
+
+        # ----------------- River specific ----------------- #
+        # dictionary name for the database
+        # similar for all spotRiver experiments
+        db_dict_name = "spotRiver_db.json"
+        train, test, n_samples, target_type = self.prepare_data()
         weights_entry = self.weights_var.get()
         weights = get_weights(
             self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item(), self.weights_var.get()
         )
-        #
         horizon = int(self.horizon_var.get())
-        #
         oml_grace_period = get_oml_grace_period(self.oml_grace_period_var.get())
-        #
-        TENSORBOARD_CLEAN = map_to_True_False(self.tb_clean_var.get())
-        tensorboard_start = map_to_True_False(self.tb_start_var.get())
-        tensorboard_stop = map_to_True_False(self.tb_stop_var.get())
-        PREFIX = self.experiment_name_entry.get()
-        #
+
+        # ----------------- fun_control ----------------- #
         fun_control = fun_control_init(
             PREFIX=PREFIX,
             TENSORBOARD_CLEAN=TENSORBOARD_CLEAN,
             core_model_name=core_model_name,
-            data_set_name=self.data_set_name,
-            db_dict_name=self.db_dict_name,
+            data_set_name=data_set_name,
+            db_dict_name=db_dict_name,
             fun_evals=fun_evals,
             fun_repeats=1,
             horizon=horizon,
             max_surrogate_points=max_surrogate_points,
             max_time=max_time,
             metric_sklearn=metric_sklearn,
             metric_sklearn_name=metric_sklearn_name,
             noise=noise,
-            n_samples=self.n_samples,
+            n_samples=n_samples,
             n_total=n_total,
             ocba_delta=0,
             oml_grace_period=oml_grace_period,
             prep_model=prepmodel,
             prep_model_name=prep_model_name,
             progress_file=self.progress_file,
-            seed=self.seed,
-            shuffle=self.shuffle,
+            seed=seed,
+            shuffle=shuffle,
             task=task_name,
             target_column="y",
-            target_type=self.target_type,
-            test=self.test,
-            test_size=self.test_size,
-            train=self.train,
+            target_type=target_type,
+            test=test,
+            test_size=test_size,
+            train=train,
             tolerance_x=np.sqrt(np.spacing(1)),
             verbosity=1,
             weights=weights,
             weights_entry=weights_entry,
             log_level=50,
         )
         coremodel, core_model_instance = get_core_model_from_name(core_model_name)
@@ -1289,32 +887,36 @@
             hyper_dict=RiverHyperDict,
             filename=None,
         )
         dict = self.rhd.hyper_dict[coremodel]
         num_dict = self.num_hp_frame.get_num_item()
         cat_dict = self.cat_hp_frame.get_cat_item()
         update_fun_control_with_hyper_num_cat_dicts(fun_control, num_dict, cat_dict, dict)
-        pprint.pprint(fun_control["core_model_hyper_dict"])
+
+        # ----------------- design_control ----------------- #
         design_control = design_control_init(
             init_size=init_size,
             repeats=1,
         )
+
+        # ----------------- surrogate_control ----------------- #
         surrogate_control = surrogate_control_init(
             # If lambda is set to 0, no noise will be used in the surrogate
             # Otherwise use noise in the surrogate:
             noise=kriging_noise,
             n_theta=2,
             min_Lambda=lbd_min,
             max_Lambda=lbd_max,
             log_level=50,
         )
-        print("surrogate_control in run_experiment():")
-        pprint.pprint(surrogate_control)
+
+        # ----------------- optimizer_control ----------------- #
         optimizer_control = optimizer_control_init()
-        # call spot:
+
+        # ----------------- Run experiment ----------------- #
         run_spot_python_experiment(
             save_only=self.save_only,
             fun_control=fun_control,
             design_control=design_control,
             surrogate_control=surrogate_control,
             optimizer_control=optimizer_control,
             fun=HyperRiver(log_level=fun_control["log_level"]).fun_oml_horizon,
@@ -1324,33 +926,21 @@
         if self.save_only:
             print("\nExperiment saved.")
         elif not self.save_only:
             print("\nExperiment started.")
         else:
             print("\nExperiment failed. No result saved.")
 
-    def check_user_prep_model(self, prep_model_name):
-        if prep_model_name.endswith(".py"):
-            print(f"prep_model_name = {prep_model_name}")
-            sys.path.insert(0, "./userPrepModel")
-            # remove the file extension from the prep_model_name
-            prep_model_name = prep_model_name[:-3]
-            print(f"prep_model_name = {prep_model_name}")
-            __import__(prep_model_name)
-            prepmodel = sys.modules[prep_model_name].set_prep_model()
-        else:
-            prepmodel = get_prep_model(prep_model_name)
-        return prepmodel
-
 
 # TODO:
 # Check the handling of l1/l2 in LogisticRegression. A note (from the River documentation):
 # > For now, only one type of penalty can be used. The joint use of L1 and L2 is not explicitly supported.
 # Therefore, we set l1 bounds to 0.0:
 # modify_hyper_parameter_bounds(fun_control, "l1", bounds=[0.0, 0.0])
 # set_control_hyperparameter_value(fun_control, "l1", [0.0, 0.0])
 # modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
 
 if __name__ == "__main__":
     customtkinter.set_appearance_mode("light")
+    customtkinter.set_default_color_theme("blue")  # Themes: "blue" (standard), "green", "dark-blue"
     app = RiverApp()
     app.mainloop()
```

### Comparing `spotgui-0.5.1/spotRiverGUI/spotRiverGUI_v01.py` & `spotgui-0.5.2/spotRiverGUI/spotRiverGUI_v01.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/PhishingData.csv` & `spotgui-0.5.2/spotRiverGUI/userData/PhishingData.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand.csv` & `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_lagged.csv` & `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_lagged.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv` & `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/phishingRiver.csv` & `spotgui-0.5.2/spotRiverGUI/userData/phishingRiver.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userData/user_data.csv` & `spotgui-0.5.2/spotRiverGUI/userData/user_data.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc` & `spotgui-0.5.2/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -62,15 +62,15 @@
      7          84 PUSH_NULL
                 86 LOAD_NAME               12 (print)
                 88 LOAD_CONST               6 ('Prep model for bike sharing demand prediction')
                 90 PRECALL                  1
                 94 CALL                     1
                104 POP_TOP
    
-    37         106 LOAD_CONST               7 (<code object set_prep_model, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py", line 37>)
+    37         106 LOAD_CONST               7 (<code object set_prep_model, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py", line 37>)
                108 MAKE_FUNCTION            0
                110 STORE_NAME              13 (set_prep_model)
                112 LOAD_CONST               1 (None)
                114 RETURN_VALUE
    consts
       0
       None
@@ -134,19 +134,19 @@
             'x9'
             'x10'
             'x12'
          names      ('compose', 'Select', 'preprocessing', 'StandardScaler', 'SelectType', 'str', 'OneHotEncoder')
          varnames   ('num', 'cat', 'prepmodel')
          freevars   ()
          cellvars   ()
-         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py'
+         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py'
          name       'set_prep_model'
          firstlineno 37
          lnotab 0x020156015a010a01
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'river', 'compose', 'preprocessing', 'feature_extraction', 'stats', 'numbers', 'print', 'set_prep_model')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py'
+   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020126010c010c010c010802161e
```

### Comparing `spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_Bikes_river.py` & `spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_Bikes_river.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py` & `spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/src/spotGUI/eda/pairplot.py` & `spotgui-0.5.2/src/spotGUI/eda/pairplot.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/src/spotGUI/tuner/images/spotlogo.png` & `spotgui-0.5.2/src/spotGUI/tuner/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/src/spotGUI/tuner/plot.png` & `spotgui-0.5.2/src/spotGUI/tuner/plot.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/src/spotGUI/tuner/spotRun.py` & `spotgui-0.5.2/src/spotGUI/tuner/spotRun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from threading import Thread
-
-# from concurrent.futures import ThreadPoolExecutor
 import copy
 import matplotlib.pyplot as plt
 import sklearn.metrics
 import pylab
 import pprint
 import numpy as np
 import os
@@ -26,15 +23,14 @@
 
 from spotRiver.evaluation.eval_bml import eval_oml_horizon
 from spotRiver.evaluation.eval_bml import plot_bml_oml_horizon_metrics, plot_bml_oml_horizon_predictions
 from spotPython.plot.validation import plot_roc_from_dataframes
 from spotPython.plot.validation import plot_confusion_matrix
 from spotPython.hyperparameters.values import get_one_core_model_from_X
 from spotPython.hyperparameters.values import get_default_hyperparameters_as_array
-from spotGUI.eda.pairplot import generate_pairplot
 from spotPython.utils.file import get_experiment_filename
 
 
 def get_classification_core_model_names():
     classification_core_model_names = [
         "linear_model.LogisticRegression",
         "forest.AMFClassifier",
@@ -295,15 +291,17 @@
     # train_sample = test_sample = False
     # if train_size > n_samples:
     #     train = train.sample(n=n_samples)
     #     train_sample = True
     # if test_size > n_samples:
     #     test = test.sample(n=n_samples)
     #     test_sample = True
-    # generate_pairplot(data=train, target_column=target_column, title="Train Data", sample=train_sample, size=train_size)
+    # generate_pairplot(data=train,
+    #                   target_column=target_column,
+    #                   title="Train Data", sample=train_sample, size=train_size)
     # generate_pairplot(data=test, target_column=target_column, title="Test Data", sample=test_sample, size=test_size)
     plt.show()
 
 
 def run_spot_python_experiment(
     save_only,
     fun_control,
@@ -440,15 +438,15 @@
 
 def progress_plot(spot_tuner, fun_control):
     spot_tuner.plot_progress(show=False)
     plt.title(fun_control["PREFIX"])
     plt.show()
 
 
-def plot_confusion_matrices(spot_tuner, fun_control, show=False) -> None:
+def plot_confusion_matrices_river(spot_tuner, fun_control, show=False) -> None:
     X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1, -1))
     print(f"X = {X}")
     core_model_spot = get_one_core_model_from_X(X, fun_control)
     if fun_control["prep_model"] is None:
         model_spot = core_model_spot
     else:
         model_spot = compose.Pipeline(fun_control["prep_model"], core_model_spot)
@@ -500,15 +498,15 @@
     )
     # add a title to the figure
     fig.suptitle(fun_control["PREFIX"])
     if show:
         plt.show()
 
 
-def plot_rocs(spot_tuner, fun_control, show=False) -> None:
+def plot_rocs_river(spot_tuner, fun_control, show=False) -> None:
     X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1, -1))
     print(f"X = {X}")
     core_model_spot = get_one_core_model_from_X(X, fun_control)
     if fun_control["prep_model"] is None:
         model_spot = core_model_spot
     else:
         model_spot = compose.Pipeline(fun_control["prep_model"], core_model_spot)
@@ -541,15 +539,15 @@
         model_names=["default", "spot"],
         target_column=fun_control["target_column"],
         show=show,
         title=fun_control["PREFIX"],
     )
 
 
-def compare_tuned_default(spot_tuner, fun_control, show=False) -> None:
+def compare_river_tuned_default(spot_tuner, fun_control, show=False) -> None:
     print(vars(spot_tuner))
     X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1, -1))
     print(f"X = {X}")
     core_model_spot = get_one_core_model_from_X(X, fun_control)
     if fun_control["prep_model"] is None:
         model_spot = core_model_spot
     else:
@@ -588,15 +586,15 @@
         metric=fun_control["metric_sklearn"],
         filename=None,
         show=show,
         title=fun_control["PREFIX"],
     )
 
 
-def actual_vs_prediction(spot_tuner, fun_control, show=False, length=50) -> None:
+def actual_vs_prediction_river(spot_tuner, fun_control, show=False, length=50) -> None:
     m = fun_control["test"].shape[0]
     a = int(m / 2) - length
     b = int(m / 2)
     print(vars(spot_tuner))
     X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1, -1))
     print(f"X = {X}")
     core_model_spot = get_one_core_model_from_X(X, fun_control)
```

### Comparing `spotgui-0.5.1/src/spotGUI/tuner/spot_00experiment.pickle` & `spotgui-0.5.2/src/spotGUI/tuner/spot_00experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.1/src/spotgui.egg-info/PKG-INFO` & `spotgui-0.5.2/src/spotgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotgui
-Version: 0.5.1
+Version: 0.5.2
 Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotgui-0.5.1/src/spotgui.egg-info/SOURCES.txt` & `spotgui-0.5.2/src/spotgui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
 spotRiverGUI/db_dicts/spotRiver_db.json
 spotRiverGUI/db_dicts/spotRiver_db_default.json
 spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
 spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
 spotRiverGUI/demos/spot_demo_00_experiment.pickle
 spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
 spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
-spotRiverGUI/images/spotlogo.png
 spotRiverGUI/userData/PhishingData.csv
 spotRiverGUI/userData/PhishingData_license.txt
 spotRiverGUI/userData/bike_sharing_demand.csv
 spotRiverGUI/userData/bike_sharing_demand_lagged.csv
 spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
 spotRiverGUI/userData/phishingRiver.csv
 spotRiverGUI/userData/user_data.csv
 spotRiverGUI/userModel/__init__.py
 spotRiverGUI/userPrepModel/__init__.py
 spotRiverGUI/userPrepModel/prep_Bikes_river.py
 spotRiverGUI/userPrepModel/prep_generic_num_cat.py
 spotRiverGUI/userPrepModel/prep_test.py
 src/spotGUI/ctk/CTk.py
+src/spotGUI/ctk/images/spotlogo.png
 src/spotGUI/eda/pairplot.py
 src/spotGUI/tuner/plot.png
 src/spotGUI/tuner/spotRun.py
 src/spotGUI/tuner/spot_00experiment.pickle
 src/spotGUI/tuner/images/spotlogo.png
 src/spotgui.egg-info/PKG-INFO
 src/spotgui.egg-info/SOURCES.txt
```

### Comparing `spotgui-0.5.1/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc` & `spotgui-0.5.2/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -76,15 +76,15 @@
      7         108 LOAD_CONST               0 (0)
                110 LOAD_CONST               7 (('spot',))
                112 IMPORT_NAME             20 (spotPython.spot)
                114 IMPORT_FROM             21 (spot)
                116 STORE_NAME              21 (spot)
                118 POP_TOP
    
-    10         120 LOAD_CONST               8 (<code object test_run_spot_python_experiment_save_only, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py", line 10>)
+    10         120 LOAD_CONST               8 (<code object test_run_spot_python_experiment_save_only, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.2/test/test_spotRun.py", line 10>)
                122 MAKE_FUNCTION            0
                124 STORE_NAME              22 (test_run_spot_python_experiment_save_only)
                126 LOAD_CONST               1 (None)
                128 RETURN_VALUE
    consts
       0
       None
@@ -209,21 +209,21 @@
             ('PREFIX',)
             ('fun_control', 'core_model', 'hyper_dict')
             'run_spot_python_experiment(save_only) raised an exception: '
          names      ('fun_control_init', 'design_control_init', 'surrogate_control_init', 'optimizer_control_init', 'add_core_model_to_fun_control', 'NetLightRegression', 'LightHyperDict', 'run_spot_python_experiment', 'Exception', 'pytest', 'fail')
          varnames   ('save_only', 'fun_control', 'design_control', 'surrogate_control', 'optimizer_control', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py'
+         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.2/test/test_spotRun.py'
          name       'test_run_spot_python_experiment_save_only'
          firstlineno 10
          lnotab
             0x0202040120011c011c011c02380302010c01020102010201020102fb16
             07120142ff
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'spotGUI.tuner.spotRun', 'run_spot_python_experiment', 'spotPython.utils.init', 'fun_control_init', 'design_control_init', 'surrogate_control_init', 'optimizer_control_init', 'spotPython.light.regression.netlightregression', 'NetLightRegression', 'spotPython.hyperdict.light_hyper_dict', 'LightHyperDict', 'spotPython.hyperparameters.values', 'add_core_model_to_fun_control', 'spotPython.spot', 'spot', 'test_run_spot_python_experiment_save_only')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py'
+   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.2/test/test_spotRun.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020122010c0118010c010c010c010c03
```

### Comparing `spotgui-0.5.1/test/test_spotRun.py` & `spotgui-0.5.2/test/test_spotRun.py`

 * *Files identical despite different names*

