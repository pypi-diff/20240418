# Comparing `tmp/oedisi-2.tar.gz` & `tmp/oedisi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oedisi-2.tar", last modified: Fri Apr 12 17:37:19 2024, max compression
+gzip compressed data, was "oedisi-2.0.1.tar", last modified: Wed Apr 17 22:58:05 2024, max compression
```

## Comparing `oedisi-2.tar` & `oedisi-2.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.524960 oedisi-2/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-2/LICENSE.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-12 17:37:19.523977 oedisi-2/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1433 2023-11-14 18:52:46.000000 oedisi-2/README.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2396 2024-04-12 17:36:29.000000 oedisi-2/pyproject.toml
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2024-04-12 17:37:19.525177 oedisi-2/setup.cfg
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.456334 oedisi-2/src/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.459841 oedisi-2/src/oedisi/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/__init__.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.470725 oedisi-2/src/oedisi/componentframework/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/componentframework/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3694 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/componentframework/basic_component.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4413 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/componentframework/mock_component.py
--rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/componentframework/mock_component.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9766 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/componentframework/system_configuration.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3976 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/componentframework/wiring_diagram_utils.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.477165 oedisi-2/src/oedisi/tools/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/tools/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/tools/api.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      951 2024-02-16 20:51:42.000000 oedisi-2/src/oedisi/tools/broker_utils.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    19042 2024-04-11 14:59:42.000000 oedisi-2/src/oedisi/tools/cli_tools.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5124 2024-03-01 22:51:51.000000 oedisi-2/src/oedisi/tools/metrics.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1090 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/tools/pausing_broker.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2018 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/tools/testing_broker.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.480519 oedisi-2/src/oedisi/types/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/types/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      681 2024-04-11 14:59:42.000000 oedisi-2/src/oedisi/types/common.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7493 2024-04-11 14:59:37.000000 oedisi-2/src/oedisi/types/data_types.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/types/generate_schema.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.518616 oedisi-2/src/oedisi/types/schemas/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/AdmittanceMatrix.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/AdmittanceSparse.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CapacitorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Command.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/types/schemas/CommandList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CostArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Injection.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3833 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/InverterControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4270 2024-01-31 18:05:05.000000 oedisi-2/src/oedisi/types/schemas/InverterControlList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/MeasurementArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/OperationalCosts.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/ReactiveCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/ReactiveWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RealCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RealWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RegulatorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/SolarIrradiances.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/StateArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/StatesOfCharge.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/SwitchStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Temperatures.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22562 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Topology.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1540 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VVControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      680 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VWControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/WindSpeeds.json
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.519780 oedisi-2/src/oedisi.egg-info/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2556 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/SOURCES.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/dependency_links.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/entry_points.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      294 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/requires.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/top_level.txt
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.807054 oedisi-2.0.1/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-2.0.1/LICENSE.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-17 22:58:05.804030 oedisi-2.0.1/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1433 2023-11-14 18:52:46.000000 oedisi-2.0.1/README.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2396 2024-04-17 22:57:42.000000 oedisi-2.0.1/pyproject.toml
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2024-04-17 22:58:05.807624 oedisi-2.0.1/setup.cfg
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.693204 oedisi-2.0.1/src/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.696641 oedisi-2.0.1/src/oedisi/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-17 22:57:42.000000 oedisi-2.0.1/src/oedisi/__init__.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.724559 oedisi-2.0.1/src/oedisi/componentframework/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-17 22:57:42.000000 oedisi-2.0.1/src/oedisi/componentframework/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3694 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/componentframework/basic_component.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4413 2024-01-31 22:17:06.000000 oedisi-2.0.1/src/oedisi/componentframework/mock_component.py
+-rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2024-01-31 15:23:02.000000 oedisi-2.0.1/src/oedisi/componentframework/mock_component.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9766 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/componentframework/system_configuration.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3976 2024-01-31 22:17:06.000000 oedisi-2.0.1/src/oedisi/componentframework/wiring_diagram_utils.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.731436 oedisi-2.0.1/src/oedisi/tools/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2024-04-17 22:57:42.000000 oedisi-2.0.1/src/oedisi/tools/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-01-31 15:23:02.000000 oedisi-2.0.1/src/oedisi/tools/api.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      951 2024-02-16 20:51:42.000000 oedisi-2.0.1/src/oedisi/tools/broker_utils.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    19042 2024-04-11 14:59:42.000000 oedisi-2.0.1/src/oedisi/tools/cli_tools.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5124 2024-03-01 22:51:51.000000 oedisi-2.0.1/src/oedisi/tools/metrics.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1090 2024-01-31 15:23:02.000000 oedisi-2.0.1/src/oedisi/tools/pausing_broker.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2018 2024-01-31 22:17:06.000000 oedisi-2.0.1/src/oedisi/tools/testing_broker.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.737490 oedisi-2.0.1/src/oedisi/types/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-17 22:57:42.000000 oedisi-2.0.1/src/oedisi/types/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      705 2024-04-17 22:57:06.000000 oedisi-2.0.1/src/oedisi/types/common.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7493 2024-04-11 14:59:37.000000 oedisi-2.0.1/src/oedisi/types/data_types.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2024-01-31 15:23:02.000000 oedisi-2.0.1/src/oedisi/types/generate_schema.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.795474 oedisi-2.0.1/src/oedisi/types/schemas/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/AdmittanceMatrix.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/AdmittanceSparse.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CapacitorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/Command.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2024-01-31 15:23:02.000000 oedisi-2.0.1/src/oedisi/types/schemas/CommandList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CostArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CurrentsAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CurrentsImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CurrentsMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/CurrentsReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/Injection.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3833 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/InverterControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4270 2024-01-31 18:05:05.000000 oedisi-2.0.1/src/oedisi/types/schemas/InverterControlList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/MeasurementArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/OperationalCosts.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/PowersAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/PowersImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/PowersMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/PowersReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/ReactiveCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/ReactiveWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/RealCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/RealWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/RegulatorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/SolarIrradiances.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/StateArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/StatesOfCharge.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/SwitchStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/Temperatures.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22562 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/Topology.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1540 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VVControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      680 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VWControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VoltagesAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VoltagesImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VoltagesMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/VoltagesReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2.0.1/src/oedisi/types/schemas/WindSpeeds.json
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-17 22:58:05.797405 oedisi-2.0.1/src/oedisi.egg-info/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2556 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/SOURCES.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/dependency_links.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/entry_points.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      294 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/requires.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2024-04-17 22:58:05.000000 oedisi-2.0.1/src/oedisi.egg-info/top_level.txt
```

### Comparing `oedisi-2/LICENSE.md` & `oedisi-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oedisi-2/PKG-INFO` & `oedisi-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 2.0.0
+Version: 2.0.1
 Summary: Orchestration interface for HELICS power simulations
 Author-email: Joseph McKinsey <joseph.mckinsey@nrel.gov>
 License: BSD 3-Clause
 Keywords: oedisi,gadal,helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `oedisi-2/README.md` & `oedisi-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oedisi-2/pyproject.toml` & `oedisi-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oedisi"
-version = "2.0.0"
+version = "2.0.1"
 description = "Orchestration interface for HELICS power simulations"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["oedisi", "gadal", "helics"]
 authors = [{ name = "Joseph McKinsey", email = "joseph.mckinsey@nrel.gov" }]
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `oedisi-2/src/oedisi/componentframework/basic_component.py` & `oedisi-2.0.1/src/oedisi/componentframework/basic_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/componentframework/mock_component.py` & `oedisi-2.0.1/src/oedisi/componentframework/mock_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/componentframework/system_configuration.py` & `oedisi-2.0.1/src/oedisi/componentframework/system_configuration.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/componentframework/wiring_diagram_utils.py` & `oedisi-2.0.1/src/oedisi/componentframework/wiring_diagram_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/tools/broker_utils.py` & `oedisi-2.0.1/src/oedisi/tools/broker_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/tools/cli_tools.py` & `oedisi-2.0.1/src/oedisi/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/tools/metrics.py` & `oedisi-2.0.1/src/oedisi/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/tools/pausing_broker.py` & `oedisi-2.0.1/src/oedisi/tools/pausing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/tools/testing_broker.py` & `oedisi-2.0.1/src/oedisi/tools/testing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/common.py` & `oedisi-2.0.1/src/oedisi/types/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     INPUT_MAPPING = "input_mapping.json"
     STATIC_INPUTS = "static_inputs.json"
 
 class BrokerConfig(BaseModel):
     broker_port: int = 23404
     broker_ip: str = "10.5.0.2"
     api_port: int = 12345
-    feeder_host: str
-    feeder_port: int
-    
+    feeder_host: str | None = None
+    feeder_port: int | None = None
+
 
 class HeathCheck(BaseModel):
     hostname: str
     host_ip: str
 
 
 class ServerReply(BaseModel):
```

### Comparing `oedisi-2/src/oedisi/types/data_types.py` & `oedisi-2.0.1/src/oedisi/types/data_types.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/generate_schema.py` & `oedisi-2.0.1/src/oedisi/types/generate_schema.py`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/AdmittanceMatrix.json` & `oedisi-2.0.1/src/oedisi/types/schemas/AdmittanceMatrix.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/AdmittanceSparse.json` & `oedisi-2.0.1/src/oedisi/types/schemas/AdmittanceSparse.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CapacitorStates.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CapacitorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/Command.json` & `oedisi-2.0.1/src/oedisi/types/schemas/Command.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CommandList.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CommandList.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CostArray.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CostArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CurrentsAngle.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CurrentsAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CurrentsImaginary.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CurrentsImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CurrentsMagnitude.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CurrentsMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/CurrentsReal.json` & `oedisi-2.0.1/src/oedisi/types/schemas/CurrentsReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/Injection.json` & `oedisi-2.0.1/src/oedisi/types/schemas/Injection.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/InverterControl.json` & `oedisi-2.0.1/src/oedisi/types/schemas/InverterControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/InverterControlList.json` & `oedisi-2.0.1/src/oedisi/types/schemas/InverterControlList.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/MeasurementArray.json` & `oedisi-2.0.1/src/oedisi/types/schemas/MeasurementArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/OperationalCosts.json` & `oedisi-2.0.1/src/oedisi/types/schemas/OperationalCosts.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/PowersAngle.json` & `oedisi-2.0.1/src/oedisi/types/schemas/PowersAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/PowersImaginary.json` & `oedisi-2.0.1/src/oedisi/types/schemas/PowersImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/PowersMagnitude.json` & `oedisi-2.0.1/src/oedisi/types/schemas/PowersMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/PowersReal.json` & `oedisi-2.0.1/src/oedisi/types/schemas/PowersReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/ReactiveCostFunctions.json` & `oedisi-2.0.1/src/oedisi/types/schemas/ReactiveCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/ReactiveWholesalePrices.json` & `oedisi-2.0.1/src/oedisi/types/schemas/ReactiveWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/RealCostFunctions.json` & `oedisi-2.0.1/src/oedisi/types/schemas/RealCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/RealWholesalePrices.json` & `oedisi-2.0.1/src/oedisi/types/schemas/RealWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/RegulatorStates.json` & `oedisi-2.0.1/src/oedisi/types/schemas/RegulatorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/SolarIrradiances.json` & `oedisi-2.0.1/src/oedisi/types/schemas/SolarIrradiances.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/StateArray.json` & `oedisi-2.0.1/src/oedisi/types/schemas/StateArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/StatesOfCharge.json` & `oedisi-2.0.1/src/oedisi/types/schemas/StatesOfCharge.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/SwitchStates.json` & `oedisi-2.0.1/src/oedisi/types/schemas/SwitchStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/Temperatures.json` & `oedisi-2.0.1/src/oedisi/types/schemas/Temperatures.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/Topology.json` & `oedisi-2.0.1/src/oedisi/types/schemas/Topology.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VVControl.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VVControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VWControl.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VWControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VoltagesAngle.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VoltagesAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VoltagesImaginary.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VoltagesImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VoltagesMagnitude.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VoltagesMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/VoltagesReal.json` & `oedisi-2.0.1/src/oedisi/types/schemas/VoltagesReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi/types/schemas/WindSpeeds.json` & `oedisi-2.0.1/src/oedisi/types/schemas/WindSpeeds.json`

 * *Files identical despite different names*

### Comparing `oedisi-2/src/oedisi.egg-info/PKG-INFO` & `oedisi-2.0.1/src/oedisi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 2.0.0
+Version: 2.0.1
 Summary: Orchestration interface for HELICS power simulations
 Author-email: Joseph McKinsey <joseph.mckinsey@nrel.gov>
 License: BSD 3-Clause
 Keywords: oedisi,gadal,helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `oedisi-2/src/oedisi.egg-info/SOURCES.txt` & `oedisi-2.0.1/src/oedisi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

