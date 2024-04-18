# Comparing `tmp/ak_sap-0.0.2.tar.gz` & `tmp/ak_sap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_sap-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ak_sap-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ak_sap-0.0.2.tar` & `ak_sap-0.0.3.tar`

### file list

```diff
@@ -1,77 +1,79 @@
--rw-r--r--   0        0        0      881 2024-03-07 18:56:04.266769 ak_sap-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1988 2023-11-20 19:23:32.080492 ak_sap-0.0.2/.gitignore
--rw-r--r--   0        0        0     1739 2024-02-14 19:20:22.960381 ak_sap-0.0.2/.streamlit/config.toml
--rw-r--r--   0        0        0       42 2024-02-07 18:34:29.862192 ak_sap-0.0.2/.streamlit/credentials.toml
--rw-r--r--   0        0        0    17098 2024-02-13 21:14:56.961859 ak_sap-0.0.2/LICENSE
--rw-r--r--   0        0        0     5219 2024-03-07 18:53:01.281779 ak_sap-0.0.2/README.md
--rw-r--r--   0        0        0     2118 2024-02-07 19:24:13.794642 ak_sap-0.0.2/Start_Here.py
--rw-r--r--   0        0        0    13443 2024-03-08 20:57:47.682004 ak_sap-0.0.2/documentation/Layout.md
--rw-r--r--   0        0        0    17654 2024-03-08 20:56:47.097361 ak_sap-0.0.2/documentation/Usage.ipynb
--rw-r--r--   0        0        0     2202 2024-02-28 17:16:04.962731 ak_sap-0.0.2/documentation/Usage/GUI.md
--rw-r--r--   0        0        0    43825 2024-02-20 19:52:50.398151 ak_sap-0.0.2/documentation/assets/GUI-streamlit-Export-Hilti.png
--rw-r--r--   0        0        0     9227 2024-02-20 19:51:12.684479 ak_sap-0.0.2/documentation/assets/GUI-streamlit-Export.png
--rw-r--r--   0        0        0    19460 2024-02-07 18:34:29.888009 ak_sap-0.0.2/documentation/assets/GUI-streamlit-Models.png
--rw-r--r--   0        0        0    14763 2024-02-07 18:34:29.956970 ak_sap-0.0.2/documentation/assets/GUI-streamlit-Start_Here.png
--rw-r--r--   0        0        0    38466 2024-02-07 18:34:29.968605 ak_sap-0.0.2/documentation/assets/GUI-streamlit-Tables.png
--rw-r--r--   0        0        0    39069 2023-11-22 03:59:44.546855 ak_sap-0.0.2/documentation/assets/mindmap.png
--rw-r--r--   0        0        0     8492 2024-02-21 00:59:09.016858 ak_sap-0.0.2/documentation/assets/mindmap.svg
--rw-r--r--   0        0        0      657 2024-02-07 18:34:29.977576 ak_sap-0.0.2/pages/1_Model.py
--rw-r--r--   0        0        0      542 2024-02-07 18:34:29.984569 ak_sap-0.0.2/pages/2_Tables.py
--rw-r--r--   0        0        0     1040 2024-02-20 19:38:44.442471 ak_sap-0.0.2/pages/3_Export.py
--rw-r--r--   0        0        0        0 2024-02-14 21:14:40.882233 ak_sap-0.0.2/pages/Export/__init__.py
--rw-r--r--   0        0        0     5157 2024-03-07 19:10:00.255464 ak_sap-0.0.2/pages/Export/hilti_export.py
--rw-r--r--   0        0        0      875 2024-03-07 18:55:20.770265 ak_sap-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      218 2024-02-22 16:53:43.441167 ak_sap-0.0.2/scripts/freshvenv-windows.bat
--rwxr-xr-x   0        0        0      899 2024-02-22 16:53:43.443167 ak_sap-0.0.2/scripts/install.bat
--rwxr-xr-x   0        0        0      696 2024-02-28 17:15:50.969191 ak_sap-0.0.2/scripts/run.bat
--rw-r--r--   0        0        0       25 2024-03-08 18:13:25.620941 ak_sap-0.0.2/src/ak_sap/Analyze/__init__.py
--rw-r--r--   0        0        0     4172 2024-03-08 18:57:56.435699 ak_sap-0.0.2/src/ak_sap/Analyze/main.py
--rw-r--r--   0        0        0       25 2023-11-21 04:45:16.171618 ak_sap-0.0.2/src/ak_sap/Database/__init__.py
--rw-r--r--   0        0        0      274 2023-11-22 03:36:24.000848 ak_sap-0.0.2/src/ak_sap/Database/table_constants.py
--rw-r--r--   0        0        0      354 2023-11-22 03:36:31.503903 ak_sap-0.0.2/src/ak_sap/Database/table_structured_data.py
--rw-r--r--   0        0        0     8191 2024-02-28 17:15:50.971190 ak_sap-0.0.2/src/ak_sap/Database/tables.py
--rw-r--r--   0        0        0     2976 2024-03-08 00:18:27.053163 ak_sap-0.0.2/src/ak_sap/Loads/LoadCases.py
--rw-r--r--   0        0        0      548 2024-03-08 00:18:09.142859 ak_sap-0.0.2/src/ak_sap/Loads/LoadCombos.py
--rw-r--r--   0        0        0     2494 2024-03-08 00:18:42.674010 ak_sap-0.0.2/src/ak_sap/Loads/LoadPatterns.py
--rw-r--r--   0        0        0     3873 2024-02-07 18:34:30.021566 ak_sap-0.0.2/src/ak_sap/Loads/Modal/Eigen/main.py
--rw-r--r--   0        0        0     2880 2024-02-07 18:34:30.022565 ak_sap-0.0.2/src/ak_sap/Loads/Modal/Ritz/main.py
--rw-r--r--   0        0        0       25 2024-02-07 18:34:30.024546 ak_sap-0.0.2/src/ak_sap/Loads/Modal/__init__.py
--rw-r--r--   0        0        0      430 2024-02-07 18:34:30.025573 ak_sap-0.0.2/src/ak_sap/Loads/Modal/main.py
--rw-r--r--   0        0        0       22 2024-02-07 18:34:30.030573 ak_sap-0.0.2/src/ak_sap/Loads/__init__.py
--rw-r--r--   0        0        0     1472 2024-02-07 18:34:30.031572 ak_sap-0.0.2/src/ak_sap/Loads/constants.py
--rw-r--r--   0        0        0      460 2024-02-14 19:29:45.844985 ak_sap-0.0.2/src/ak_sap/Loads/main.py
--rw-r--r--   0        0        0     1496 2024-02-21 01:02:26.172525 ak_sap-0.0.2/src/ak_sap/Material/Materials/rebar.py
--rw-r--r--   0        0        0      277 2024-02-21 00:02:43.002785 ak_sap-0.0.2/src/ak_sap/Material/constants.py
--rw-r--r--   0        0        0     3020 2024-03-08 00:19:46.497618 ak_sap-0.0.2/src/ak_sap/Material/material.py
--rw-r--r--   0        0        0      170 2024-02-20 22:43:17.007430 ak_sap-0.0.2/src/ak_sap/Material/types.py
--rw-r--r--   0        0        0       38 2023-11-20 23:56:07.347644 ak_sap-0.0.2/src/ak_sap/Model/__init__.py
--rw-r--r--   0        0        0      667 2023-11-20 23:13:05.386626 ak_sap-0.0.2/src/ak_sap/Model/constants.py
--rw-r--r--   0        0        0     5336 2024-02-20 22:49:16.315040 ak_sap-0.0.2/src/ak_sap/Model/model.py
--rw-r--r--   0        0        0       23 2024-03-07 19:08:25.983983 ak_sap-0.0.2/src/ak_sap/Object/__init__.py
--rw-r--r--   0        0        0     3981 2024-03-08 00:14:10.842185 ak_sap-0.0.2/src/ak_sap/Object/frame.py
--rw-r--r--   0        0        0     2182 2024-03-08 00:13:26.606890 ak_sap-0.0.2/src/ak_sap/Object/helper.py
--rw-r--r--   0        0        0     1766 2024-03-08 00:46:39.014872 ak_sap-0.0.2/src/ak_sap/Object/obj.py
--rw-r--r--   0        0        0     3082 2024-03-08 00:42:38.180696 ak_sap-0.0.2/src/ak_sap/Object/point.py
--rw-r--r--   0        0        0     1704 2024-03-08 00:20:35.913498 ak_sap-0.0.2/src/ak_sap/Results/Setup.py
--rw-r--r--   0        0        0       25 2024-02-13 20:34:34.184319 ak_sap-0.0.2/src/ak_sap/Results/__init__.py
--rw-r--r--   0        0        0     7067 2024-03-08 19:42:57.834370 ak_sap-0.0.2/src/ak_sap/Results/main.py
--rw-r--r--   0        0        0       24 2024-03-08 19:44:32.049009 ak_sap-0.0.2/src/ak_sap/Select/__init__.py
--rw-r--r--   0        0        0     4184 2024-03-08 20:54:38.768719 ak_sap-0.0.2/src/ak_sap/Select/main.py
--rw-r--r--   0        0        0      541 2024-03-08 21:13:08.780021 ak_sap-0.0.2/src/ak_sap/__init__.py
--rw-r--r--   0        0        0      401 2024-02-07 18:34:30.043565 ak_sap-0.0.2/src/ak_sap/gui/cli_app.py
--rw-r--r--   0        0        0       33 2024-02-07 18:34:30.045565 ak_sap-0.0.2/src/ak_sap/gui/streamlit/__init__.py
--rw-r--r--   0        0        0      935 2024-02-07 19:22:48.185881 ak_sap-0.0.2/src/ak_sap/gui/streamlit/config.py
--rw-r--r--   0        0        0       30 2024-03-08 00:29:06.162329 ak_sap-0.0.2/src/ak_sap/misc/__init__.py
--rw-r--r--   0        0        0      191 2024-03-08 00:33:40.563722 ak_sap-0.0.2/src/ak_sap/misc/coordinates.py
--rw-r--r--   0        0        0      708 2024-02-07 19:19:05.002402 ak_sap-0.0.2/src/ak_sap/utils/__init__.py
--rw-r--r--   0        0        0      385 2024-02-07 19:17:08.530490 ak_sap-0.0.2/src/ak_sap/utils/credentials.py
--rw-r--r--   0        0        0      944 2024-02-13 20:46:18.236147 ak_sap-0.0.2/src/ak_sap/utils/decorators.py
--rw-r--r--   0        0        0     2567 2024-02-07 18:34:30.055559 ak_sap-0.0.2/src/ak_sap/utils/logger.py
--rw-r--r--   0        0        0     6159 2024-03-08 19:45:15.381332 ak_sap-0.0.2/src/ak_sap/wrapper.py
--rw-r--r--   0        0        0     1688 2024-03-08 18:47:39.502088 ak_sap-0.0.2/src/tests/Analyze/test_Analyze_main.py
--rw-r--r--   0        0        0     3402 2024-02-28 17:15:50.975187 ak_sap-0.0.2/src/tests/Database/test_tables.py
--rw-r--r--   0        0        0     2694 2024-03-08 19:39:50.790317 ak_sap-0.0.2/src/tests/Results/test_Results_main.py
--rw-r--r--   0        0        0      553 2024-03-08 20:04:31.595926 ak_sap-0.0.2/src/tests/Select/test_Select_main.py
--rw-r--r--   0        0        0        0 2023-11-20 19:23:32.090731 ak_sap-0.0.2/src/tests/__init__.py
--rw-r--r--   0        0        0     1326 2024-03-07 19:52:12.054917 ak_sap-0.0.2/src/tests/utils/test_decorators.py
--rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 ak_sap-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      881 2024-03-07 18:56:04.266769 ak_sap-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1988 2023-11-20 19:23:32.080492 ak_sap-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1739 2024-02-14 19:20:22.960381 ak_sap-0.0.3/.streamlit/config.toml
+-rw-r--r--   0        0        0       42 2024-02-07 18:34:29.862192 ak_sap-0.0.3/.streamlit/credentials.toml
+-rw-r--r--   0        0        0    17098 2024-02-13 21:14:56.961859 ak_sap-0.0.3/LICENSE
+-rw-r--r--   0        0        0    18680 2024-04-18 19:21:07.567745 ak_sap-0.0.3/README.md
+-rw-r--r--   0        0        0     2118 2024-02-07 19:24:13.794642 ak_sap-0.0.3/Start_Here.py
+-rw-r--r--   0        0        0    13937 2024-04-05 19:11:23.194258 ak_sap-0.0.3/documentation/Layout.md
+-rw-r--r--   0        0        0    18320 2024-04-05 19:11:20.207500 ak_sap-0.0.3/documentation/Usage.ipynb
+-rw-r--r--   0        0        0     2195 2024-04-05 18:45:56.173139 ak_sap-0.0.3/documentation/Usage/GUI.md
+-rw-r--r--   0        0        0    43825 2024-02-20 19:52:50.398151 ak_sap-0.0.3/documentation/assets/GUI-streamlit-Export-Hilti.png
+-rw-r--r--   0        0        0     9227 2024-02-20 19:51:12.684479 ak_sap-0.0.3/documentation/assets/GUI-streamlit-Export.png
+-rw-r--r--   0        0        0    19460 2024-02-07 18:34:29.888009 ak_sap-0.0.3/documentation/assets/GUI-streamlit-Models.png
+-rw-r--r--   0        0        0    14763 2024-02-07 18:34:29.956970 ak_sap-0.0.3/documentation/assets/GUI-streamlit-Start_Here.png
+-rw-r--r--   0        0        0    38466 2024-02-07 18:34:29.968605 ak_sap-0.0.3/documentation/assets/GUI-streamlit-Tables.png
+-rw-r--r--   0        0        0    39069 2023-11-22 03:59:44.546855 ak_sap-0.0.3/documentation/assets/mindmap.png
+-rw-r--r--   0        0        0    44635 2024-04-05 18:11:07.370578 ak_sap-0.0.3/documentation/assets/mindmap.svg
+-rw-r--r--   0        0        0      657 2024-02-07 18:34:29.977576 ak_sap-0.0.3/pages/1_Model.py
+-rw-r--r--   0        0        0      542 2024-02-07 18:34:29.984569 ak_sap-0.0.3/pages/2_Tables.py
+-rw-r--r--   0        0        0     1040 2024-02-20 19:38:44.442471 ak_sap-0.0.3/pages/3_Export.py
+-rw-r--r--   0        0        0        0 2024-02-14 21:14:40.882233 ak_sap-0.0.3/pages/Export/__init__.py
+-rw-r--r--   0        0        0     5157 2024-03-07 19:10:00.255464 ak_sap-0.0.3/pages/Export/hilti_export.py
+-rw-r--r--   0        0        0      928 2024-04-05 18:41:39.778434 ak_sap-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      218 2024-02-22 16:53:43.441167 ak_sap-0.0.3/scripts/freshvenv-windows.bat
+-rwxr-xr-x   0        0        0      899 2024-02-22 16:53:43.443167 ak_sap-0.0.3/scripts/install.bat
+-rwxr-xr-x   0        0        0      696 2024-02-28 17:15:50.969191 ak_sap-0.0.3/scripts/run.bat
+-rw-r--r--   0        0        0       25 2024-03-08 18:13:25.620941 ak_sap-0.0.3/src/ak_sap/Analyze/__init__.py
+-rw-r--r--   0        0        0     4217 2024-04-05 19:14:46.147108 ak_sap-0.0.3/src/ak_sap/Analyze/main.py
+-rw-r--r--   0        0        0       25 2023-11-21 04:45:16.171618 ak_sap-0.0.3/src/ak_sap/Database/__init__.py
+-rw-r--r--   0        0        0      274 2023-11-22 03:36:24.000848 ak_sap-0.0.3/src/ak_sap/Database/table_constants.py
+-rw-r--r--   0        0        0      354 2023-11-22 03:36:31.503903 ak_sap-0.0.3/src/ak_sap/Database/table_structured_data.py
+-rw-r--r--   0        0        0     8191 2024-02-28 17:15:50.971190 ak_sap-0.0.3/src/ak_sap/Database/tables.py
+-rw-r--r--   0        0        0     2976 2024-03-08 00:18:27.053163 ak_sap-0.0.3/src/ak_sap/Loads/LoadCases.py
+-rw-r--r--   0        0        0      548 2024-03-08 00:18:09.142859 ak_sap-0.0.3/src/ak_sap/Loads/LoadCombos.py
+-rw-r--r--   0        0        0     2494 2024-03-08 00:18:42.674010 ak_sap-0.0.3/src/ak_sap/Loads/LoadPatterns.py
+-rw-r--r--   0        0        0     3915 2024-04-05 19:15:53.843560 ak_sap-0.0.3/src/ak_sap/Loads/Modal/Eigen/main.py
+-rw-r--r--   0        0        0     2922 2024-04-05 19:16:07.026468 ak_sap-0.0.3/src/ak_sap/Loads/Modal/Ritz/main.py
+-rw-r--r--   0        0        0       25 2024-02-07 18:34:30.024546 ak_sap-0.0.3/src/ak_sap/Loads/Modal/__init__.py
+-rw-r--r--   0        0        0      430 2024-02-07 18:34:30.025573 ak_sap-0.0.3/src/ak_sap/Loads/Modal/main.py
+-rw-r--r--   0        0        0       22 2024-02-07 18:34:30.030573 ak_sap-0.0.3/src/ak_sap/Loads/__init__.py
+-rw-r--r--   0        0        0     1472 2024-02-07 18:34:30.031572 ak_sap-0.0.3/src/ak_sap/Loads/constants.py
+-rw-r--r--   0        0        0      460 2024-02-14 19:29:45.844985 ak_sap-0.0.3/src/ak_sap/Loads/main.py
+-rw-r--r--   0        0        0     1496 2024-02-21 01:02:26.172525 ak_sap-0.0.3/src/ak_sap/Material/Materials/rebar.py
+-rw-r--r--   0        0        0      277 2024-02-21 00:02:43.002785 ak_sap-0.0.3/src/ak_sap/Material/constants.py
+-rw-r--r--   0        0        0     3020 2024-03-08 00:19:46.497618 ak_sap-0.0.3/src/ak_sap/Material/material.py
+-rw-r--r--   0        0        0      170 2024-02-20 22:43:17.007430 ak_sap-0.0.3/src/ak_sap/Material/types.py
+-rw-r--r--   0        0        0       38 2023-11-20 23:56:07.347644 ak_sap-0.0.3/src/ak_sap/Model/__init__.py
+-rw-r--r--   0        0        0      667 2023-11-20 23:13:05.386626 ak_sap-0.0.3/src/ak_sap/Model/constants.py
+-rw-r--r--   0        0        0     5336 2024-02-20 22:49:16.315040 ak_sap-0.0.3/src/ak_sap/Model/model.py
+-rw-r--r--   0        0        0       23 2024-03-07 19:08:25.983983 ak_sap-0.0.3/src/ak_sap/Object/__init__.py
+-rw-r--r--   0        0        0     5172 2024-04-05 19:13:30.255997 ak_sap-0.0.3/src/ak_sap/Object/frame.py
+-rw-r--r--   0        0        0     2182 2024-03-08 00:13:26.606890 ak_sap-0.0.3/src/ak_sap/Object/helper.py
+-rw-r--r--   0        0        0     1773 2024-04-05 19:13:50.933855 ak_sap-0.0.3/src/ak_sap/Object/obj.py
+-rw-r--r--   0        0        0     4025 2024-04-05 19:12:18.943139 ak_sap-0.0.3/src/ak_sap/Object/point.py
+-rw-r--r--   0        0        0     1704 2024-03-08 00:20:35.913498 ak_sap-0.0.3/src/ak_sap/Results/Setup.py
+-rw-r--r--   0        0        0       25 2024-02-13 20:34:34.184319 ak_sap-0.0.3/src/ak_sap/Results/__init__.py
+-rw-r--r--   0        0        0     7142 2024-04-05 19:17:38.593240 ak_sap-0.0.3/src/ak_sap/Results/main.py
+-rw-r--r--   0        0        0       24 2024-03-08 19:44:32.049009 ak_sap-0.0.3/src/ak_sap/Select/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-05 19:17:52.011553 ak_sap-0.0.3/src/ak_sap/Select/main.py
+-rw-r--r--   0        0        0      525 2024-04-18 19:21:55.508710 ak_sap-0.0.3/src/ak_sap/__init__.py
+-rw-r--r--   0        0        0      395 2024-04-05 18:21:51.114651 ak_sap-0.0.3/src/ak_sap/cli/cli_app.py
+-rw-r--r--   0        0        0     1340 2024-04-05 18:28:19.095817 ak_sap-0.0.3/src/ak_sap/cli/update_doc.py
+-rw-r--r--   0        0        0      313 2024-04-05 18:43:36.856629 ak_sap-0.0.3/src/ak_sap/gui/gui_app.py
+-rw-r--r--   0        0        0       33 2024-02-07 18:34:30.045565 ak_sap-0.0.3/src/ak_sap/gui/streamlit/__init__.py
+-rw-r--r--   0        0        0      935 2024-02-07 19:22:48.185881 ak_sap-0.0.3/src/ak_sap/gui/streamlit/config.py
+-rw-r--r--   0        0        0       30 2024-03-08 00:29:06.162329 ak_sap-0.0.3/src/ak_sap/misc/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-05 19:16:44.595170 ak_sap-0.0.3/src/ak_sap/misc/coordinates.py
+-rw-r--r--   0        0        0      708 2024-02-07 19:19:05.002402 ak_sap-0.0.3/src/ak_sap/utils/__init__.py
+-rw-r--r--   0        0        0      385 2024-02-07 19:17:08.530490 ak_sap-0.0.3/src/ak_sap/utils/credentials.py
+-rw-r--r--   0        0        0      944 2024-02-13 20:46:18.236147 ak_sap-0.0.3/src/ak_sap/utils/decorators.py
+-rw-r--r--   0        0        0     2612 2024-04-05 19:18:15.242085 ak_sap-0.0.3/src/ak_sap/utils/logger.py
+-rw-r--r--   0        0        0     6231 2024-04-05 18:16:24.335551 ak_sap-0.0.3/src/ak_sap/wrapper.py
+-rw-r--r--   0        0        0     1688 2024-03-08 18:47:39.502088 ak_sap-0.0.3/src/tests/Analyze/test_Analyze_main.py
+-rw-r--r--   0        0        0     3402 2024-02-28 17:15:50.975187 ak_sap-0.0.3/src/tests/Database/test_tables.py
+-rw-r--r--   0        0        0     2694 2024-03-08 19:39:50.790317 ak_sap-0.0.3/src/tests/Results/test_Results_main.py
+-rw-r--r--   0        0        0      553 2024-03-08 20:04:31.595926 ak_sap-0.0.3/src/tests/Select/test_Select_main.py
+-rw-r--r--   0        0        0        0 2023-11-20 19:23:32.090731 ak_sap-0.0.3/src/tests/__init__.py
+-rw-r--r--   0        0        0     1326 2024-03-07 19:52:12.054917 ak_sap-0.0.3/src/tests/utils/test_decorators.py
+-rw-r--r--   0        0        0    19051 1970-01-01 00:00:00.000000 ak_sap-0.0.3/PKG-INFO
```

### Comparing `ak_sap-0.0.2/.github/workflows/test.yml` & `ak_sap-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/.gitignore` & `ak_sap-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/.streamlit/config.toml` & `ak_sap-0.0.3/.streamlit/config.toml`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/LICENSE` & `ak_sap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/Start_Here.py` & `ak_sap-0.0.3/Start_Here.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/Layout.md` & `ak_sap-0.0.3/documentation/Layout.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 - [Parent Level](#parent-level)
 - [Sub-Modules](#sub-modules)
   - [Model](#model)
   - [Element](#element)
     - [Point](#point)
     - [Frame](#frame)
   - [Database](#database)
+  - [Select](#select)
   - [Loads](#loads)
     - [Load Patterns](#load-patterns)
     - [Load Cases](#load-cases)
     - [Modal](#modal)
       - [Eigen](#eigen)
       - [Ritz](#ritz)
   - [Analyze](#analyze)
@@ -45,14 +46,15 @@
 
 ```python
 sap.hide()                                  #Hide the SAP2000 window
 sap.unhide()                                #Unhides SAP2000 window
 sap.ishidden                                #Check if window is hidden
 sap.version                                 #Returns SAP2000 version number
 sap.api_version                             #Returns Sap0API version number
+sap.exit(save=False)                        #Exit the application
 
 sap.save(r'\Path\to\save\file.sdb')
 ```
 
 # Sub-Modules
 ## Model
 
@@ -119,14 +121,21 @@
 
 #Manipilate
 points.deselect_all()                       #Deselect all points
 points.select(name='1')                     #Select a single point
 points.align(axis='Z', ordinate = 100)      #Align selected points
 points.deselect(name='1')                   #Deselect a single point
 
+# Extrude point to frame
+points.extrude(
+    point_name='3',
+    property_name='FSec1',
+    dx=0, dy=144, dz=0,
+    num_frames=3
+)
 points.merge(tolerance=2)                   #Merge points that are within tol
 points.change_coord(name='1', x=0, y=0, z=0)#Change point coordinate
 ```
 
 ### Frame
 
 Manipulate Frame Elements
@@ -149,14 +158,23 @@
 frames.divide_by_distance(name='1',
     dist=0.5,Iend=True)                     #Divide frame by distance
 frames.divide_by_intersection(name='2')   #Divide at selected intersections
 frames.divide_by_ratio(name='3',ratio=0.3)#Divide at selected ratio
 frames.join('2','3')                  #Join Colinear frames
 frames.change_points(name='1', point1='1', point2='3')  #Change connected points of frame
 
+# Extrude frames to area
+frames.extrude(
+    frame_name='8',
+    property_name='Default',
+    dx=0, dy=144, dz=0,
+    num_areas=3,
+    del_frame=True
+)
+
 # Get frame properties
 frames.Prop.rename(old_name="FSEC1", new_name="MySection")  #Rename frame property
 frames.Prop.total()                         #Total # of defined frame properties
 ```
 
 ## Database
 
@@ -174,38 +192,44 @@
 
 # Update Table
 df.iloc[0,0] = 'New Value'
 tables.update(TableKey='Material Properties 01 - General', data=df, apply=True)
 ```
 
 ## Select
-elect = sap.Select
 
-select.all()                    #Select all objects
-select.clear()                  #Deselect all objects
+Usage Examples:
 
-select.constraint(name='Diaph1')#Select points in constraint
+```python
+select = sap.Select
+
+select.all()                                    #Select all objects
+select.clear()                                  #Deselect all objects
+
+select.constraint(name='Diaph1')                #Select points in constraint
 select.constraint(name='Diaph1', reverse=True)  #Deselect points in constraint
 
 select.invert()                 #Invert selections
 select.selected                 #Returns list of selected objects
 select.previous()               #restores the previous selection
 
 #Selection based on plane
-select.in_plane(pointname='1', plane='XY')  #Select in XY plane
+select.in_plane(pointname='1', plane='XY')                  #Select in XY plane
 select.in_plane(pointname='2', plane='YZ', reverse=False)   #Deselect
 
 #Select by property
 select.property(type='Area', name='ASEC1')
 select.property(type='Cable', name='CAB1', reverse=True)
 select.property(type='Frame', name='FSEC1')
 select.property(type='Link', name='GAP1', reverse=True)
 select.property(type='Material', name='A992Fy50')
 select.property(type='Solid', name='SOLID1', reverse=True)
 select.property(type='Tendon', name='TEN1')
+```
+
 ## Loads
 
 Control the definition and assignments of loads.
 ### Load Patterns
 
 Usage Examples:
 
@@ -293,15 +317,15 @@
 Usage Examples:
 
 ```python
 analyze = sap.Analyze
 analyze.create_model()                      #Create analysis model
 analyze.run()                               #Runs the analysis
 analyze.case_status()                       #retrieves the status for all load cases.
-analyze.get_run_status()                    #retrieves the run flags for all cases
+analyze.get_run_flag()                      #retrieves the run flags for all cases
 analyze.set_run_flag(case='MODAL', status=True) # Set case to run
 analyze.get_solver()                        #Get solver info
 
 #Set solver options
 analyze.set_solver(
     SolverType='Standard',
     SolverProcessType='Auto',
```

### Comparing `ak_sap-0.0.2/documentation/Usage.ipynb` & `ak_sap-0.0.3/documentation/Usage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974621296905859%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(5, 'sap.exit(save=False)                        #Exit the "*

 * *            "application\\n')]}}, 10: {'source': {insert: [(16, '# Extrude point to frame\\n'), "*

 * *            '(17, \'points.extrude(\\n\'), (18, "    point_name=\'3\',\\n"), (19, "    '*

 * *            'property_name=\'FSec1\',\\n"), (20, \'    dx=0, dy=144, dz=0,\\n\'), (21, \'    '*

 * *            "num_frames=3\\n'), (22, ')\\n')]}}, 12: {'source': {insert: [(18, '\\n'), (19, '# "*

 * *            'Extrude frames to are […]*

```diff
@@ -37,14 +37,15 @@
             "outputs": [],
             "source": [
                 "sap.hide()                                  #Hide the SAP2000 window\n",
                 "sap.unhide()                                #Unhides SAP2000 window\n",
                 "sap.ishidden                                #Check if window is hidden\n",
                 "sap.version                                 #Returns SAP2000 version number\n",
                 "sap.api_version                             #Returns Sap0API version number\n",
+                "sap.exit(save=False)                        #Exit the application\n",
                 "\n",
                 "sap.save(r'\\Path\\to\\save\\file.sdb')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -141,14 +142,21 @@
                 "\n",
                 "#Manipilate\n",
                 "points.deselect_all()                       #Deselect all points\n",
                 "points.select(name='1')                     #Select a single point\n",
                 "points.align(axis='Z', ordinate = 100)      #Align selected points\n",
                 "points.deselect(name='1')                   #Deselect a single point\n",
                 "\n",
+                "# Extrude point to frame\n",
+                "points.extrude(\n",
+                "    point_name='3',\n",
+                "    property_name='FSec1',\n",
+                "    dx=0, dy=144, dz=0,\n",
+                "    num_frames=3\n",
+                ")\n",
                 "points.merge(tolerance=2)                   #Merge points that are within tol\n",
                 "points.change_coord(name='1', x=0, y=0, z=0)#Change point coordinate"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -179,14 +187,23 @@
                 "frames.divide_by_distance(name='1',\n",
                 "    dist=0.5,Iend=True)                     #Divide frame by distance\n",
                 "frames.divide_by_intersection(name='2')   #Divide at selected intersections\n",
                 "frames.divide_by_ratio(name='3',ratio=0.3)#Divide at selected ratio\n",
                 "frames.join('2','3')                  #Join Colinear frames\n",
                 "frames.change_points(name='1', point1='1', point2='3')  #Change connected points of frame\n",
                 "\n",
+                "# Extrude frames to area\n",
+                "frames.extrude(\n",
+                "    frame_name='8',\n",
+                "    property_name='Default',\n",
+                "    dx=0, dy=144, dz=0,\n",
+                "    num_areas=3,\n",
+                "    del_frame=True\n",
+                ")\n",
+                "\n",
                 "# Get frame properties\n",
                 "frames.Prop.rename(old_name=\"FSEC1\", new_name=\"MySection\")  #Rename frame property\n",
                 "frames.Prop.total()                         #Total # of defined frame properties"
             ]
         },
         {
             "cell_type": "markdown",
@@ -219,31 +236,37 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Select"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "vscode": {
+                    "languageId": "plaintext"
+                }
+            },
+            "outputs": [],
             "source": [
                 "select = sap.Select\n",
                 "\n",
-                "select.all()                    #Select all objects\n",
-                "select.clear()                  #Deselect all objects\n",
+                "select.all()                                    #Select all objects\n",
+                "select.clear()                                  #Deselect all objects\n",
                 "\n",
-                "select.constraint(name='Diaph1')#Select points in constraint\n",
+                "select.constraint(name='Diaph1')                #Select points in constraint\n",
                 "select.constraint(name='Diaph1', reverse=True)  #Deselect points in constraint\n",
                 "\n",
                 "select.invert()                 #Invert selections\n",
                 "select.selected                 #Returns list of selected objects\n",
                 "select.previous()               #restores the previous selection\n",
                 "\n",
                 "#Selection based on plane\n",
-                "select.in_plane(pointname='1', plane='XY')  #Select in XY plane\n",
+                "select.in_plane(pointname='1', plane='XY')                  #Select in XY plane\n",
                 "select.in_plane(pointname='2', plane='YZ', reverse=False)   #Deselect\n",
                 "\n",
                 "#Select by property\n",
                 "select.property(type='Area', name='ASEC1')\n",
                 "select.property(type='Cable', name='CAB1', reverse=True)\n",
                 "select.property(type='Frame', name='FSEC1')\n",
                 "select.property(type='Link', name='GAP1', reverse=True)\n",
@@ -395,15 +418,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "analyze = sap.Analyze\n",
                 "analyze.create_model()                      #Create analysis model\n",
                 "analyze.run()                               #Runs the analysis\n",
                 "analyze.case_status()                       #retrieves the status for all load cases.\n",
-                "analyze.get_run_status()                    #retrieves the run flags for all cases\n",
+                "analyze.get_run_flag()                      #retrieves the run flags for all cases\n",
                 "analyze.set_run_flag(case='MODAL', status=True) # Set case to run\n",
                 "analyze.get_solver()                        #Get solver info\n",
                 "\n",
                 "#Set solver options\n",
                 "analyze.set_solver(\n",
                 "    SolverType='Standard',\n",
                 "    SolverProcessType='Auto',\n",
```

### Comparing `ak_sap-0.0.2/documentation/Usage/GUI.md` & `ak_sap-0.0.3/documentation/Usage/GUI.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     git clone https://github.com/rpakishore/ak_sap.git
     cd ak_sap
     ```
 
 - Install dependencies
 
     ```bash
-    pip install flit && flit install
+    pip install flit && flit install --extras gui
     ```
 
 - Launch the app run
 
     ```bash
-    python -m streamlit run Start_Here.py
+    gui
     ```
 
   - Alternatively, In windows launch by executing the script
 
     ```cmd
-    cd scripts
-    run.bat
+    python -m streamlit run Start_Here.py
     ```
 
 - Open up the SAP2000 model of your choice and click `Attach to Model`
 
 ## 1.1. Attach an Instance
 
 ![GUI-Streamlit-Start_Here.png](../assets/GUI-streamlit-Start_Here.png)
```

### Comparing `ak_sap-0.0.2/documentation/assets/GUI-streamlit-Export-Hilti.png` & `ak_sap-0.0.3/documentation/assets/GUI-streamlit-Export-Hilti.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/assets/GUI-streamlit-Export.png` & `ak_sap-0.0.3/documentation/assets/GUI-streamlit-Export.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/assets/GUI-streamlit-Models.png` & `ak_sap-0.0.3/documentation/assets/GUI-streamlit-Models.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/assets/GUI-streamlit-Start_Here.png` & `ak_sap-0.0.3/documentation/assets/GUI-streamlit-Start_Here.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/assets/GUI-streamlit-Tables.png` & `ak_sap-0.0.3/documentation/assets/GUI-streamlit-Tables.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/documentation/assets/mindmap.png` & `ak_sap-0.0.3/documentation/assets/mindmap.png`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/pages/1_Model.py` & `ak_sap-0.0.3/pages/1_Model.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/pages/2_Tables.py` & `ak_sap-0.0.3/pages/2_Tables.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/pages/3_Export.py` & `ak_sap-0.0.3/pages/3_Export.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/pages/Export/hilti_export.py` & `ak_sap-0.0.3/pages/Export/hilti_export.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/pyproject.toml` & `ak_sap-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)"]
 dynamic = ["version", "description"]
 dependencies = [
     "comtypes==1.2.0",
     "forallpeople==2.6.7",
-    "pandas==2.1.3",
-    "rich==13.7.0",
-    "typer[all]==0.9.0"
+    "pandas==2.1.3"
 ]
 
 [project.optional-dependencies]
 
 dev = [
     "ipykernel",
     "ipywidgets",
@@ -28,16 +26,22 @@
 ]
 
 gui = [
     "streamlit==1.31.0",
     "hilti_profis==0.0.3"
 ]
 
+cli = [
+    "rich==13.7.0",
+    "typer[all]==0.9.0"
+]
+
 test = [
     "pytest==7.4.3"
 ]
 
 [project.urls]
 Home = "https://github.com/rpakishore/ak_sap"
 
 [project.scripts]
-app="ak_sap.gui.cli_app:app"
+gui="ak_sap.gui.gui_app:app"
+update-doc="ak_sap.cli.update_doc:app"
```

### Comparing `ak_sap-0.0.2/scripts/install.bat` & `ak_sap-0.0.3/scripts/install.bat`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/scripts/run.bat` & `ak_sap-0.0.3/scripts/run.bat`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Analyze/main.py` & `ak_sap-0.0.3/src/ak_sap/Analyze/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     @smooth_sap_do
     def case_status(self) -> dict:
         """retrieves the status for all load cases.
 
         Returns:
             list[dict]: Cases and their current status.
         """
-        return case_status(ret=self.__Analyze.GetCaseStatus()), 0
+        return case_status(ret=self.__Analyze.GetCaseStatus()), 0 # type: ignore
 
     @smooth_sap_do
     def get_run_flag(self) -> dict:
         """retrieves the run flags for all analysis cases.
 
         Returns:
             dict: Loadcases and their run flags
         """
-        return get_run_flag(ret=self.__Analyze.GetRunCaseFlag()), 0
+        return get_run_flag(ret=self.__Analyze.GetRunCaseFlag()), 0 # type: ignore
 
     @smooth_sap_do
     def set_run_flag(self, case: str, status: bool):
         """sets the run flag for load cases
 
         Args:
             case (str): name of an existing load case
@@ -53,15 +53,15 @@
     @smooth_sap_do
     def get_solver(self) -> dict:
         """retrieves the model solver options
 
         Returns:
             dict: Solver Info
         """
-        return get_solver(ret = self.__Analyze.GetSolverOption_3()), 0
+        return get_solver(ret = self.__Analyze.GetSolverOption_3()), 0 # type: ignore
     
     @smooth_sap_do
     def set_solver(self, 
                     SolverType: Literal['Standard', 'Advanced', 'Multi-threaded'],
                     SolverProcessType: Literal['Auto', 'GUI', 'Separate'],
                     NumberParallelRuns: Literal[0,1,2,3,4,5,6,7,8],
                     StiffCase: str = ''
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Database/tables.py` & `ak_sap-0.0.3/src/ak_sap/Database/tables.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/LoadCases.py` & `ak_sap-0.0.3/src/ak_sap/Loads/LoadCases.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/LoadCombos.py` & `ak_sap-0.0.3/src/ak_sap/Loads/LoadCombos.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/LoadPatterns.py` & `ak_sap-0.0.3/src/ak_sap/Loads/LoadPatterns.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/Modal/Eigen/main.py` & `ak_sap-0.0.3/src/ak_sap/Loads/Modal/Eigen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ak_sap.utils.decorators import smooth_sap_do
 from ak_sap.utils import MasterClass
 
 class Eigen(MasterClass):
     def __init__(self, mySapObject) -> None:
         super().__init__(mySapObject=mySapObject)
+        assert self.SapModel is not None
         self.ModalEigen = self.SapModel.LoadCases.ModalEigen
     
     def __str__(self) -> str:
         return f'Instance of `Loads.Modal.{self.__class__.__name__}`. Holds collection of functions'
     
     @smooth_sap_do
     def get_initial_case(self, case_name: str) -> str:
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/Modal/Ritz/main.py` & `ak_sap-0.0.3/src/ak_sap/Loads/Modal/Ritz/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ak_sap.utils.decorators import smooth_sap_do
 from ak_sap.utils import MasterClass
 
 class Ritz(MasterClass):
     def __init__(self, mySapObject) -> None:
         super().__init__(mySapObject=mySapObject)
+        assert self.SapModel is not None
         self.ModalRitz = self.SapModel.LoadCases.ModalRitz
     
     def __str__(self) -> str:
         return f'Instance of `Loads.Modal.{self.__class__.__name__}`. Holds collection of functions'
     
     @smooth_sap_do
     def get_initial_case(self, case_name: str) -> str:
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Loads/constants.py` & `ak_sap-0.0.3/src/ak_sap/Loads/constants.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Material/Materials/rebar.py` & `ak_sap-0.0.3/src/ak_sap/Material/Materials/rebar.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Material/material.py` & `ak_sap-0.0.3/src/ak_sap/Material/material.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Model/constants.py` & `ak_sap-0.0.3/src/ak_sap/Model/constants.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Model/model.py` & `ak_sap-0.0.3/src/ak_sap/Model/model.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Object/frame.py` & `ak_sap-0.0.3/src/ak_sap/Object/frame.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from .helper import MasterObj
 
 class Frame(MasterObj):
     def __init__(self, mySapObject) -> None:
         super().__init__(mySapObject=mySapObject, ElemObj=mySapObject.SapModel.FrameObj)
         
         self.__EditFrame = mySapObject.SapModel.EditFrame
+        self.__EditGeneral = mySapObject.SapModel.EditGeneral
+        self.__FrameObj = mySapObject.SapModel.FrameObj
+        
         self.Prop = Prop(mySapObject=mySapObject)
     
     @smooth_sap_do
     def get_section(self, name: str) -> str:
         self.check_obj_legal(name=name)
-        _ret = self.ElemObj.GetSection(name)
+        _ret = self.__FrameObj.GetSection(name)
         return (_ret[0], _ret[-1]) # type: ignore
     
     @smooth_sap_do
     def get_points(self, name: str) -> tuple[str]:
         """retrieves the names of the point objects at each end of a specified frame object."""
         #self.check_obj_legal(name=name)
-        return self.ElemObj.GetPoints(name)
+        return self.__FrameObj.GetPoints(name)
     
     @smooth_sap_do
     def divide_by_distance(self, name: str, dist: float, Iend: bool=True) -> tuple[str]:
         """divides straight frame objects into two objects at a location defined by the Dist and IEnd items. 
         Curved frame objects are not divided.
         """
         return self.__EditFrame.DivideAtDistance(name, dist, Iend)
@@ -73,14 +76,32 @@
         Args:
             name (str): name of an existing frame object
             point1 (str): name of the point object at the I-End of the frame object.
             point2 (str): name of the point object at the J-End of the frame object.
         """
         return self.__EditFrame.ChangeConnectivity(name, point1, point2)
     
+    @smooth_sap_do
+    def extrude(self, frame_name: str, dx: float, dy: float, dz: float, num_areas: int, property_name: str|None = None, del_frame: bool=False) -> list[str]:
+        """Creates new area objects by linearly extruding a specified frame obj.
+
+        Args:
+            frame_name (str): Name of existing frame to extrude
+            dx (float): x offset.
+            dy (float): y offset.
+            dz (float): z offset.
+            num_areas (int): number of area objects to create
+            property_name (str | None, optional): Name of a defined area section property to be used for the new obj. Defaults to None.
+            del_frame(bool, optional): If this item is True, the straight frame object indicated by the Name item is deleted after the extrusion is complete. Defaults to False.
+
+        Returns:
+            list[str]: array of the name of each area object created
+        """
+        return self.__EditGeneral.ExtrudeFrameToAreaLinear(frame_name, property_name, dx, dy, dz, num_areas, del_frame)
+    
 class Prop:
     def __init__(self, mySapObject) -> None:
         self.__mySapObject=mySapObject.SapModel
     
     def __len__(self) -> int:
         return self.total()
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Object/helper.py` & `ak_sap-0.0.3/src/ak_sap/Object/helper.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Object/obj.py` & `ak_sap-0.0.3/src/ak_sap/Object/obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         """moves selected point, frame, cable, tendon, area, solid and link objects.
 
         Args:
             dx (float): x offsets
             dy (float): y offsets
             dz (float): z offsets
         """
-        self.__EditGeneral.Move(dx, dy, dz)
+        return self.__EditGeneral.Move(dx, dy, dz)
         
     @smooth_sap_do
     def copy(self, dx: float, dy: float, dz: float, num: int) -> tuple:
         """linearly replicates selected objects.
 
         Args:
             dx (float): x offset
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Object/point.py` & `ak_sap-0.0.3/src/ak_sap/Object/point.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from .helper import MasterObj
 
 class Point(MasterObj):
     def __init__(self, mySapObject) -> None:
         super().__init__(mySapObject=mySapObject, ElemObj=mySapObject.SapModel.PointObj)
         self.__EditPoint = mySapObject.SapModel.EditPoint
         self.__PointObj = mySapObject.SapModel.PointObj
+        self.__EditGeneral = mySapObject.SapModel.EditGeneral
     
     @smooth_sap_do
     def add_by_coord(self, point: tuple[float, float, float], name: str='', coord_sys: str = 'Global') -> str:
         """Adds point to the model
         Args:
             point (tuple[float, float, float]): x, y, z coordinates
             name (str, optional): Custom name for point. Defaults to ''.
             coord_sys (str, optional): Name of coordinate system. Defaults to 'Global'.
         """
-        return self.ElemObj.AddCartesian(*point, '', name, coord_sys)
+        return self.__PointObj.AddCartesian(*point, '', name, coord_sys)
 
     @smooth_sap_do
     def align(self, axis: Literal['X', 'Y', 'Z'], ordinate: float) -> tuple:
         """aligns selected point objects.
 
         Args:
             axis (Literal['X', 'Y', 'Z']): Align points to this ordinate in present coordinate system
@@ -69,8 +70,25 @@
             x (float): new x coordinate.
             y (float): new y coordinate.
             z (float): new z coordinate.
 
         Returns:
             bool: Success
         """
-        return self.__EditPoint.ChangeCoordinates_1(name, x, y, z)
+        return self.__EditPoint.ChangeCoordinates_1(name, x, y, z)
+    
+    @smooth_sap_do
+    def extrude(self, point_name: str, dx: float, dy: float, dz: float, num_frames: int, property_name: str|None = None) -> list[str]:
+        """Creates new frame objects by linearly extruding a specified point obj. into frame objects.
+
+        Args:
+            point_name (str): Name of existing point to extrude
+            dx (float): x offset.
+            dy (float): y offset.
+            dz (float): z offset.
+            num_frames (int): number of frame objects to create
+            property_name (str | None, optional): Name of a defined frame section property to be used for the new frame obj. Defaults to None.
+
+        Returns:
+            list[str]: array of the name of each frame object created
+        """
+        return self.__EditGeneral.ExtrudePointToFrameLinear(point_name, property_name, dx, dy, dz, num_frames)
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Results/Setup.py` & `ak_sap-0.0.3/src/ak_sap/Results/Setup.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/Results/main.py` & `ak_sap-0.0.3/src/ak_sap/Results/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,52 +14,52 @@
     @smooth_sap_do
     def delete(self, casename: str|Literal['All']) -> bool:
         """deletes results for load cases.
 
         Args:
             casename (str | Literal['All']): name of an existing load case that is to have its results deleted.
         """
-        return self.mySapObject.SapModel.Analyze.DeleteResykts(casename, casename.casefold() == 'all')
+        return self.mySapObject.SapModel.Analyze.DeleteResykts(casename, casename.casefold() == 'all') # type: ignore
     
     @smooth_sap_do
     def joint_reactions(self, jointname:str) -> list[dict]:
         """reports the joint reactions for the specified point elements
 
         Args:
             jointname (str): name of an existing point object
         """
-        return joint_reactions_parse(ret=self.__Results.JointReact(jointname, 1)), 0
+        return joint_reactions_parse(ret=self.__Results.JointReact(jointname, 1)), 0 # type: ignore
 
 
     @smooth_sap_do
     def joint_displacements(self, jointname:str) -> list[dict]:
         """reports the joint displacements for the specified point elements
 
         Args:
             jointname (str): name of an existing point object
         """
-        return joint_displacements_parse(ret=self.__Results.JointDispl(jointname, 1)), 0
+        return joint_displacements_parse(ret=self.__Results.JointDispl(jointname, 1)), 0 # type: ignore
     
     @smooth_sap_do
     def joint_accelerations(self, jointname:str) ->  list[dict]:
         """reports the joint accelerations for the specified point elements
 
         Args:
             jointname (str): name of an existing point object
         """
-        return joint_displacements_parse(ret=self.__Results.JointAcc(jointname, 1)), 0
+        return joint_displacements_parse(ret=self.__Results.JointAcc(jointname, 1)), 0 # type: ignore
             
     @smooth_sap_do
     def joint_velocities(self, jointname:str, format: Literal['Pandas', 'List']= 'List') ->  list[dict]:
         """reports the joint velocities for the specified point elements
 
         Args:
             jointname (str): name of an existing point object
         """
-        return joint_displacements_parse(ret=self.__Results.JointVel(jointname, 1)), 0
+        return joint_displacements_parse(ret=self.__Results.JointVel(jointname, 1)), 0 # type: ignore
             
 def joint_displacements_parse(ret: list) -> list[dict]:
     assert ret[-1] == 0
     displacements: list[dict] = []
     
     if ret[0] == 1:
         return [
```

### Comparing `ak_sap-0.0.2/src/ak_sap/Select/main.py` & `ak_sap-0.0.3/src/ak_sap/Select/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             name (str): name of an existing joint constraint
             reverse (bool): deselect
         """
         return self.__SelectObj.Constraint(name, reverse)
     
     @property
     def selected(self) -> list[dict]:
-        return selected_parse(ret=self.__SelectObj.GetSelected()), 0
+        return selected_parse(ret=self.__SelectObj.GetSelected()), 0 # type: ignore
     
     @smooth_sap_do
     def in_plane(self, pointname: str, plane: Literal['XY', 'YZ', 'XZ'], reverse: bool=False) -> bool:
         """selects or deselects all objects that are in the same plane as specified point object
 
         Args:
             pointname (str): point name
```

### Comparing `ak_sap-0.0.2/src/ak_sap/__init__.py` & `ak_sap-0.0.3/src/ak_sap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 "Python wrapper for SAP2000 API"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from ak_sap.utils.logger import log
 from ak_sap.wrapper import Sap2000Wrapper
 from ak_sap.misc import Coord
 
-#log = Log()
-
 def debug(status=False):
     """Import this in a new module and enable debug to use debug
     example:
     ```python
     from ak_sap import debug
     debug(True)
     ```
```

### Comparing `ak_sap-0.0.2/src/ak_sap/gui/streamlit/config.py` & `ak_sap-0.0.3/src/ak_sap/gui/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/utils/__init__.py` & `ak_sap-0.0.3/src/ak_sap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/utils/decorators.py` & `ak_sap-0.0.3/src/ak_sap/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/ak_sap/utils/logger.py` & `ak_sap-0.0.3/src/ak_sap/utils/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,30 +26,30 @@
         self.logger.debug(msg)
         
     def info(self, msg):
         self.logger.info(msg)
         
     def warning(self, msg):
         try:
-            suffix = f'Warning in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: '
+            suffix = f'Warning in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: ' # type: ignore
         except Exception:
             suffix = f'Warning in {Path(inspect.stack()[1].filename).name}: '
         self.logger.warning(suffix + msg)
         
     def error(self, msg):
         try:
-            suffix = f'Error in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: '
+            suffix = f'Error in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: ' # type: ignore
         except Exception:
             suffix = f'Error in {Path(inspect.stack()[1].filename).name}: '
         self.logger.error(suffix + str(msg))
         self.logger.exception(msg)
         
     def critical(self, msg):
         try:
-            suffix = f'Critical in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: '
+            suffix = f'Critical in {Path(inspect.stack()[1].filename).name} -> {inspect.currentframe().f_back.f_code.co_name}: ' # type: ignore
         except Exception:
             suffix = f'Error in {Path(inspect.stack()[1].filename).name}: '
         self.logger.critical(suffix + str(msg))
         self.logger.exception(msg)
         
     def log(self, level, msg):
         self.logger.log(level, msg)
```

### Comparing `ak_sap-0.0.2/src/ak_sap/wrapper.py` & `ak_sap-0.0.3/src/ak_sap/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,16 @@
     def __repr__(self) -> str:
         attach_to_exist = self.attach_to_exist
         return f'Sap2000Wrapper({attach_to_exist=})'
     
     def __del__(self) -> None:
         try:
             # assert self.mySapObject.ApplicationExit(False) == 0
-            # self.SapModel = None
-            # self.mySapObject = None
-            pass
+            self.SapModel = None
+            self.mySapObject = None
         except Exception as e:
             log.error(e.__str__())
     
     def save(self, savepath: str|Path|None = None) -> bool:
         """Saves SAP model to the `savepath`.
         If no save path is provided, saves to the default path
         """
@@ -95,14 +94,17 @@
     @property
     def ishidden(self) -> bool:
         return self.mySapObject.Visible()
     
     @property
     def version(self) -> str:
         return self.SapModel.GetVersion()[0]
+    
+    def exit(self, save: bool=False):
+        self.mySapObject.ApplicationExit(False)
         
 def model(attach_to_instance: bool, program_path: str|Path|None = None):
     """Returns SapObject.
     If `attach_to_instance` is True, returns the current opened model
     If `program_path` is NOT set, Creates a model from latest installed version of SAP2000
     `program_path`, allows lauch of older versions of SAP2000"""
     #create API helper object
```

### Comparing `ak_sap-0.0.2/src/tests/Analyze/test_Analyze_main.py` & `ak_sap-0.0.3/src/tests/Analyze/test_Analyze_main.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/tests/Database/test_tables.py` & `ak_sap-0.0.3/src/tests/Database/test_tables.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/tests/Results/test_Results_main.py` & `ak_sap-0.0.3/src/tests/Results/test_Results_main.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/tests/Select/test_Select_main.py` & `ak_sap-0.0.3/src/tests/Select/test_Select_main.py`

 * *Files identical despite different names*

### Comparing `ak_sap-0.0.2/src/tests/utils/test_decorators.py` & `ak_sap-0.0.3/src/tests/utils/test_decorators.py`

 * *Files identical despite different names*

