# Comparing `tmp/quicfire-tools-0.7.1.tar.gz` & `tmp/quicfire_tools-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicfire-tools-0.7.1.tar", last modified: Fri Apr 12 23:40:38 2024, max compression
+gzip compressed data, was "quicfire_tools-0.7.2.tar", last modified: Thu Apr 18 16:32:51 2024, max compression
```

## Comparing `quicfire-tools-0.7.1.tar` & `quicfire_tools-0.7.2.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.732594 quicfire-tools-0.7.1/quicfire_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.732594 quicfire-tools-0.7.1/quicfire_tools/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.736594 quicfire-tools-0.7.1/quicfire_tools/data/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/IgnitionType.json
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Advanced_User_Inputs.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Bldg_Advanced_User_Inputs.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Plume_Advanced_User_Inputs.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QP_buildout.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QUIC_fire.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_TopoInputs.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_buildings.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_fileoptions.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_metparams.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_movingcoords.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_simparams.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/Runtime_Advanced_User_Inputs.inp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/TopoType.json
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/gridlist.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/rasterorigin.txt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/documentation/sensor1.inp.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.732594 quicfire-tools-0.7.1/quicfire_tools/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.740594 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      812 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Bldg_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Plume_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QP_buildout.inp
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QUIC_fire.inp
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_TopoInputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_buildings.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_fileoptions.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_landuse.inp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_metparams.inp
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_movingcoords.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1567 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_simparams.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/Runtime_Advanced_User_Inputs.inp
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/gridlist
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/rasterorigin.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/sensor.inp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      812 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Bldg_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Plume_Advanced_User_Inputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QP_buildout.inp
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QUIC_fire.inp
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_TopoInputs.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_buildings.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_fileoptions.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_landuse.inp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_metparams.inp
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_movingcoords.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1567 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_simparams.inp
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/Runtime_Advanced_User_Inputs.inp
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/gridlist
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/rasterorigin.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/sensor.inp
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/ignitions.py
--rw-r--r--   0 runner    (1001) docker     (127)   124673 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37375 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/topography.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/quicfire_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/quicfire_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 23:40:38.000000 quicfire-tools-0.7.1/quicfire_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-12 23:40:38.000000 quicfire-tools-0.7.1/quicfire_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:40:38.000000 quicfire-tools-0.7.1/quicfire_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 23:40:38.000000 quicfire-tools-0.7.1/quicfire_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 23:40:38.000000 quicfire-tools-0.7.1/quicfire_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-12 23:40:29.000000 quicfire-tools-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:40:38.744594 quicfire-tools-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   111955 2024-04-12 23:40:30.000000 quicfire-tools-0.7.1/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38916 2024-04-12 23:40:30.000000 quicfire-tools-0.7.1/tests/test_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.540026 quicfire_tools-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-18 16:32:51.540026 quicfire_tools-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.528026 quicfire_tools-0.7.2/quicfire_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.528026 quicfire_tools-0.7.2/quicfire_tools/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.532026 quicfire_tools-0.7.2/quicfire_tools/data/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/IgnitionType.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Advanced_User_Inputs.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Bldg_Advanced_User_Inputs.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Plume_Advanced_User_Inputs.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QP_buildout.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QUIC_fire.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_TopoInputs.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_buildings.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_fileoptions.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_metparams.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_movingcoords.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_simparams.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/Runtime_Advanced_User_Inputs.inp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/TopoType.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/gridlist.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/rasterorigin.txt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/documentation/sensor1.inp.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.532026 quicfire_tools-0.7.2/quicfire_tools/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/outputs/outputs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.528026 quicfire_tools-0.7.2/quicfire_tools/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.532026 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      812 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Bldg_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Plume_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QP_buildout.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QUIC_fire.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_TopoInputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_buildings.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_fileoptions.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_landuse.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_metparams.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_movingcoords.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1567 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_simparams.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/Runtime_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/gridlist
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/rasterorigin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/sensor.inp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.536026 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      812 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Bldg_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1459 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Plume_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QP_buildout.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QUIC_fire.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_TopoInputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_buildings.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_fileoptions.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_landuse.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_metparams.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_movingcoords.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1567 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_simparams.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/Runtime_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/gridlist
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/rasterorigin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/sensor.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/ignitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124673 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37375 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/topography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/quicfire_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.540026 quicfire_tools-0.7.2/quicfire_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-18 16:32:51.000000 quicfire_tools-0.7.2/quicfire_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-18 16:32:51.000000 quicfire_tools-0.7.2/quicfire_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:32:51.000000 quicfire_tools-0.7.2/quicfire_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 16:32:51.000000 quicfire_tools-0.7.2/quicfire_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 16:32:51.000000 quicfire_tools-0.7.2/quicfire_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:32:51.540026 quicfire_tools-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 16:32:42.000000 quicfire_tools-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:32:51.536026 quicfire_tools-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   111955 2024-04-18 16:32:43.000000 quicfire_tools-0.7.2/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38916 2024-04-18 16:32:43.000000 quicfire_tools-0.7.2/tests/test_outputs.py
```

### Comparing `quicfire-tools-0.7.1/LICENSE` & `quicfire_tools-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/PKG-INFO` & `quicfire_tools-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.7.1/README.md` & `quicfire_tools-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/IgnitionType.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/IgnitionType.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Advanced_User_Inputs.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Advanced_User_Inputs.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Bldg_Advanced_User_Inputs.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Bldg_Advanced_User_Inputs.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QFire_Plume_Advanced_User_Inputs.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QFire_Plume_Advanced_User_Inputs.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QUIC_fire.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QUIC_fire.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_TopoInputs.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_TopoInputs.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_buildings.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_buildings.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_fileoptions.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_fileoptions.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/QU_simparams.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/QU_simparams.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/TopoType.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/TopoType.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/gridlist.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/gridlist.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/documentation/sensor1.inp.json` & `quicfire_tools-0.7.2/quicfire_tools/data/documentation/sensor1.inp.json`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Bldg_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Bldg_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QFire_Plume_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QFire_Plume_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QUIC_fire.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QUIC_fire.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_TopoInputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_TopoInputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v5/QU_simparams.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v5/QU_simparams.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Bldg_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Bldg_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QFire_Plume_Advanced_User_Inputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QFire_Plume_Advanced_User_Inputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QUIC_fire.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QUIC_fire.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_TopoInputs.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_TopoInputs.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/data/templates/v6/QU_simparams.inp` & `quicfire_tools-0.7.2/quicfire_tools/data/templates/v6/QU_simparams.inp`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/ignitions.py` & `quicfire_tools-0.7.2/quicfire_tools/ignitions.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/inputs.py` & `quicfire_tools-0.7.2/quicfire_tools/inputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/outputs.py` & `quicfire_tools-0.7.2/quicfire_tools/outputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/topography.py` & `quicfire_tools-0.7.2/quicfire_tools/topography.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools/utils.py` & `quicfire_tools-0.7.2/quicfire_tools/utils.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/quicfire_tools.egg-info/PKG-INFO` & `quicfire_tools-0.7.2/quicfire_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.7.1/quicfire_tools.egg-info/SOURCES.txt` & `quicfire_tools-0.7.2/quicfire_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ./quicfire_tools/data/documentation/QU_movingcoords.inp.json
 ./quicfire_tools/data/documentation/QU_simparams.inp.json
 ./quicfire_tools/data/documentation/Runtime_Advanced_User_Inputs.inp.json
 ./quicfire_tools/data/documentation/TopoType.json
 ./quicfire_tools/data/documentation/gridlist.json
 ./quicfire_tools/data/documentation/rasterorigin.txt.json
 ./quicfire_tools/data/documentation/sensor1.inp.json
+./quicfire_tools/data/outputs/outputs.json
 ./quicfire_tools/data/templates/v5/QFire_Advanced_User_Inputs.inp
 ./quicfire_tools/data/templates/v5/QFire_Bldg_Advanced_User_Inputs.inp
 ./quicfire_tools/data/templates/v5/QFire_Plume_Advanced_User_Inputs.inp
 ./quicfire_tools/data/templates/v5/QP_buildout.inp
 ./quicfire_tools/data/templates/v5/QUIC_fire.inp
 ./quicfire_tools/data/templates/v5/QU_TopoInputs.inp
 ./quicfire_tools/data/templates/v5/QU_buildings.inp
```

### Comparing `quicfire-tools-0.7.1/setup.py` & `quicfire_tools-0.7.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,12 +55,18 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
     ],
     package_dir={"": "."},
     packages=find_packages(exclude=["docs", "tests"]),
-    package_data={"quicfire_tools": ["data/templates/*/*", "data/documentation/*"]},
+    package_data={
+        "quicfire_tools": [
+            "data/templates/*/*",
+            "data/documentation/*",
+            "data/outputs/*",
+        ]
+    },
     include_package_data=True,
     install_requires=REQUIREMENTS,
     python_requires=">=3.8",
 )
```

### Comparing `quicfire-tools-0.7.1/tests/test_inputs.py` & `quicfire_tools-0.7.2/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.7.1/tests/test_outputs.py` & `quicfire_tools-0.7.2/tests/test_outputs.py`

 * *Files identical despite different names*

