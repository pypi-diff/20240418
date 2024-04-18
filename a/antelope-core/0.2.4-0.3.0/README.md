# Comparing `tmp/antelope_core-0.2.4.tar.gz` & `tmp/antelope_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_core-0.2.4.tar", last modified: Thu Apr 18 21:32:50 2024, max compression
+gzip compressed data, was "antelope_core-0.3.0.tar", last modified: Thu Mar 21 22:37:35 2024, max compression
```

## Comparing `antelope_core-0.2.4.tar` & `antelope_core-0.3.0.tar`

### file list

```diff
@@ -1,190 +1,192 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.2.4/LICENSE
--rw-r--r--   0 b          (500) b          (506)      335 2023-07-21 21:37:06.000000 antelope_core-0.2.4/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)    14539 2024-04-18 21:32:50.692230 antelope_core-0.2.4/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)    13586 2023-07-21 21:50:10.000000 antelope_core-0.2.4/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/
--rw-r--r--   0 b          (500) b          (506)     3177 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/archives/
--rw-r--r--   0 b          (500) b          (506)     4638 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/archives/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2364 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/archive_index.py
--rw-r--r--   0 b          (500) b          (506)    19334 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/basic_archive.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/archives/data/
--rw-r--r--   0 b          (500) b          (506)    27863 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/data/elcd_reference_quantities.json
--rw-r--r--   0 b          (500) b          (506)    28771 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/entity_store.py
--rw-r--r--   0 b          (500) b          (506)     6288 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/lc_archive.py
--rw-r--r--   0 b          (500) b          (506)     6588 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)    42938 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/term_manager.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/archives/tests/
--rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/archives/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_base.py
--rw-r--r--   0 b          (500) b          (506)     3557 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_basic_archive.py
--rw-r--r--   0 b          (500) b          (506)     1802 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_entity_store.py
--rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_json.json
--rw-r--r--   0 b          (500) b          (506)     2287 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_qdb.py
--rw-r--r--   0 b          (500) b          (506)     3044 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)     2286 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_quantity_relation.py
--rw-r--r--   0 b          (500) b          (506)     3013 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/archives/tests/test_term_manager.py
--rw-r--r--   0 b          (500) b          (506)     4101 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/autorange.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/catalog/
--rw-r--r--   0 b          (500) b          (506)       70 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/catalog/__init__.py
--rw-r--r--   0 b          (500) b          (506)    18441 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/catalog/catalog.py
--rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.2.4/antelope_core/catalog/catalog_root.py
--rw-r--r--   0 b          (500) b          (506)     6104 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/catalog/configurator.py
--rw-r--r--   0 b          (500) b          (506)    21860 2024-04-18 04:32:42.000000 antelope_core-0.2.4/antelope_core/catalog/lc_catalog.py
--rw-r--r--   0 b          (500) b          (506)     8782 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/catalog/lc_resolver.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/catalog/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/catalog/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     5139 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/catalog/tests/test_catalogs.py
--rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/catalog/tests/test_process_ref.py
--rw-r--r--   0 b          (500) b          (506)     1624 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/catalog/tests/test_quantity_refs.py
--rw-r--r--   0 b          (500) b          (506)    13015 2024-04-17 22:51:41.000000 antelope_core-0.2.4/antelope_core/catalog_query.py
--rw-r--r--   0 b          (500) b          (506)    10710 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/characterizations.py
--rw-r--r--   0 b          (500) b          (506)    17778 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/contexts.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.685563 antelope_core-0.2.4/antelope_core/data_sources/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.4/antelope_core/data_sources/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3851 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/data_source.py
--rw-r--r--   0 b          (500) b          (506)     7497 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     1741 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)     1303 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/gwp_ipcc_2007.py
--rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.2.4/antelope_core/data_sources/local.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/data_sources/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4159 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_aa_local.py
--rw-r--r--   0 b          (500) b          (506)     1541 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_ecoinvent_lci.py
--rw-r--r--   0 b          (500) b          (506)      815 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_ipcc2007.py
--rw-r--r--   0 b          (500) b          (506)     1999 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_traci.py
--rw-r--r--   0 b          (500) b          (506)     7401 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/data_sources/tests/test_uslci.py
--rw-r--r--   0 b          (500) b          (506)     2438 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/data_sources/traci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/data_sources/uslci/
--rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.2.4/antelope_core/data_sources/uslci/__init__.py
--rw-r--r--   0 b          (500) b          (506)     6853 2024-03-21 02:23:41.000000 antelope_core-0.2.4/antelope_core/data_sources/uslci/uslci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/entities/
--rw-r--r--   0 b          (500) b          (506)      181 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/entities/__init__.py
--rw-r--r--   0 b          (500) b          (506)    11425 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/entities/entities.py
--rw-r--r--   0 b          (500) b          (506)     4408 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/entities/flows.py
--rw-r--r--   0 b          (500) b          (506)    25036 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/entities/processes.py
--rw-r--r--   0 b          (500) b          (506)     7804 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/entities/quantities.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/entities/tests/
--rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/entities/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.2.4/antelope_core/entities/tests/base_testclass.py
--rw-r--r--   0 b          (500) b          (506)    99142 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_archive.json
--rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_entities.py
--rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_entity_refs.py
--rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_processes.py
--rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.2.4/antelope_core/entities/tests/test_quantities.py
--rw-r--r--   0 b          (500) b          (506)    18234 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/entities/xlsx_editor.py
--rw-r--r--   0 b          (500) b          (506)    22640 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/exchanges.py
--rw-r--r--   0 b          (500) b          (506)     6756 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/file_accessor.py
--rw-r--r--   0 b          (500) b          (506)     1137 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/from_json.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/implementations/
--rw-r--r--   0 b          (500) b          (506)      333 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/implementations/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8804 2024-04-17 22:51:41.000000 antelope_core-0.2.4/antelope_core/implementations/background.py
--rw-r--r--   0 b          (500) b          (506)     5843 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/implementations/basic.py
--rw-r--r--   0 b          (500) b          (506)    10035 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/implementations/configure.py
--rw-r--r--   0 b          (500) b          (506)     2812 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/implementations/exchange.py
--rw-r--r--   0 b          (500) b          (506)     6048 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/implementations/index.py
--rw-r--r--   0 b          (500) b          (506)    32761 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/implementations/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/implementations/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.2.4/antelope_core/implementations/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/implementations/tests/test_quantity.py
--rw-r--r--   0 b          (500) b          (506)    16689 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/lc_resource.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/lcia_engine/
--rw-r--r--   0 b          (500) b          (506)     5632 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/lcia_engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8163 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/lcia_engine/clookup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/lcia_engine/data/
--rw-r--r--   0 b          (500) b          (506)     8420 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/lcia_engine/data/contexts.json
--rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/lcia_engine/data/flowables.json
--rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.2.4/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
--rw-r--r--   0 b          (500) b          (506)    18298 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/lcia_engine/lcia_engine.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/lcia_engine/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/lcia_engine/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1645 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_biogenic_co2.py
--rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_clookup.py
--rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_ipcc.py
--rw-r--r--   0 b          (500) b          (506)     2981 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_lcia_engine.py
--rw-r--r--   0 b          (500) b          (506)    44192 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/lcia_results.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/providers/
--rw-r--r--   0 b          (500) b          (506)     4610 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/providers/data/
--rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/data/__init__.py
--rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
--rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
--rw-r--r--   0 b          (500) b          (506)     9551 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)    11083 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/ecospold.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.688896 antelope_core-0.2.4/antelope_core/providers/ecospold2/
--rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/ecospold2/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24560 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/ecospold2/ecospold2.py
--rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.2.4/antelope_core/providers/ecospold2/ecospold2_index.py
--rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/providers/ecospold2/master_data.py
--rw-r--r--   0 b          (500) b          (506)    10917 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/file_store.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/ilcd/
--rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/__init__.py
--rw-r--r--   0 b          (500) b          (506)    17683 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd.py
--rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd_flowables.py
--rw-r--r--   0 b          (500) b          (506)     5806 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd_lcia.py
--rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/index.py
--rw-r--r--   0 b          (500) b          (506)     3177 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.682229 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.682229 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.682229 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
--rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
--rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
--rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
--rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
--rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
--rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
--rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.2.4/antelope_core/providers/ilcd/tests/test_ilcd.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/openlca/
--rw-r--r--   0 b          (500) b          (506)       49 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/openlca/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24980 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/providers/openlca/openlca_jsonld.py
--rw-r--r--   0 b          (500) b          (506)      775 2024-03-20 22:20:51.000000 antelope_core-0.2.4/antelope_core/providers/openlca/schema_mapping.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/openlca/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2024-01-05 07:24:59.000000 antelope_core-0.2.4/antelope_core/providers/openlca/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)       83 2024-01-05 07:57:07.000000 antelope_core-0.2.4/antelope_core/providers/openlca/tests/test_olca_ref.py
--rw-r--r--   0 b          (500) b          (506)      729 2023-07-21 21:37:06.000000 antelope_core-0.2.4/antelope_core/providers/parse_math.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.2.4/antelope_core/providers/tests/test_ecospold.py
--rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/tests/test_xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/traci/
--rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/providers/traci/__init__.py
--rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.2.4/antelope_core/providers/traci/index.py
--rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.2.4/antelope_core/providers/traci/q_info.py
--rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.2.4/antelope_core/providers/traci/quantity.py
--rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/providers/traci/test_traci.py
--rw-r--r--   0 b          (500) b          (506)     6687 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/traci/traci_2_1_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/providers/xdb_client/
--rw-r--r--   0 b          (500) b          (506)       67 2023-08-19 07:49:00.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/__init__.py
--rw-r--r--   0 b          (500) b          (506)    16378 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/implementation.py
--rw-r--r--   0 b          (500) b          (506)     4007 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/requester.py
--rw-r--r--   0 b          (500) b          (506)     7171 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/rest_client.py
--rw-r--r--   0 b          (500) b          (506)     6317 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/xdb_client.py
--rw-r--r--   0 b          (500) b          (506)     3093 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/providers/xdb_client/xdb_entities.py
--rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/providers/xl_dict.py
--rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.2.4/antelope_core/providers/xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.4/antelope_core/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1007 2023-07-21 21:50:10.000000 antelope_core-0.2.4/antelope_core/tests/test_autorange.py
--rw-r--r--   0 b          (500) b          (506)    13194 2024-04-17 22:48:31.000000 antelope_core-0.2.4/antelope_core/tests/test_contexts.py
--rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.2.4/antelope_core/tests/test_exchanges.py
--rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.2.4/antelope_core/tests/test_lcia_results.py
--rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.2.4/antelope_core/tests/test_resources.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:32:50.692230 antelope_core-0.2.4/antelope_core.egg-info/
--rw-r--r--   0 b          (500) b          (506)    14539 2024-04-18 21:32:50.000000 antelope_core-0.2.4/antelope_core.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     6986 2024-04-18 21:32:50.000000 antelope_core-0.2.4/antelope_core.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 21:32:50.000000 antelope_core-0.2.4/antelope_core.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)      169 2024-04-18 21:32:50.000000 antelope_core-0.2.4/antelope_core.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       14 2024-04-18 21:32:50.000000 antelope_core-0.2.4/antelope_core.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 21:32:50.692230 antelope_core-0.2.4/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     3824 2024-04-17 22:51:41.000000 antelope_core-0.2.4/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.3.0/LICENSE
+-rw-r--r--   0 b          (500) b          (506)      335 2023-07-21 21:37:06.000000 antelope_core-0.3.0/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)    14232 2024-03-21 22:37:35.467665 antelope_core-0.3.0/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)    13586 2023-07-21 21:50:10.000000 antelope_core-0.3.0/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/
+-rw-r--r--   0 b          (500) b          (506)     3264 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/archives/
+-rw-r--r--   0 b          (500) b          (506)     4638 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/archives/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2364 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/archives/archive_index.py
+-rw-r--r--   0 b          (500) b          (506)    19543 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/basic_archive.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/archives/data/
+-rw-r--r--   0 b          (500) b          (506)    27954 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/data/elcd_reference_quantities.json
+-rw-r--r--   0 b          (500) b          (506)    28771 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     6288 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/lc_archive.py
+-rw-r--r--   0 b          (500) b          (506)     6744 2024-03-21 02:23:41.000000 antelope_core-0.3.0/antelope_core/archives/quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)    43106 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/term_manager.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/archives/tests/
+-rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/archives/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_base.py
+-rw-r--r--   0 b          (500) b          (506)     3557 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_basic_archive.py
+-rw-r--r--   0 b          (500) b          (506)     1802 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_json.json
+-rw-r--r--   0 b          (500) b          (506)     2442 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_qdb.py
+-rw-r--r--   0 b          (500) b          (506)     3044 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)     2286 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_relation.py
+-rw-r--r--   0 b          (500) b          (506)     3013 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/archives/tests/test_term_manager.py
+-rw-r--r--   0 b          (500) b          (506)     4101 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/autorange.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/catalog/
+-rw-r--r--   0 b          (500) b          (506)       70 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/catalog/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    18519 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/catalog/catalog.py
+-rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.3.0/antelope_core/catalog/catalog_root.py
+-rw-r--r--   0 b          (500) b          (506)     6104 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/configurator.py
+-rw-r--r--   0 b          (500) b          (506)    22430 2024-03-21 19:57:40.000000 antelope_core-0.3.0/antelope_core/catalog/lc_catalog.py
+-rw-r--r--   0 b          (500) b          (506)     8782 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/lc_resolver.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/catalog/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/catalog/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     5139 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_catalogs.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     1624 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/catalog/tests/test_quantity_refs.py
+-rw-r--r--   0 b          (500) b          (506)    18075 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/catalog_query.py
+-rw-r--r--   0 b          (500) b          (506)    10746 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/characterizations.py
+-rw-r--r--   0 b          (500) b          (506)    17778 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/contexts.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/data_sources/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.0/antelope_core/data_sources/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     3851 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/data_source.py
+-rw-r--r--   0 b          (500) b          (506)     7497 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     1741 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)     1303 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/gwp_ipcc_2007.py
+-rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.3.0/antelope_core/data_sources/local.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.454331 antelope_core-0.3.0/antelope_core/data_sources/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4159 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_aa_local.py
+-rw-r--r--   0 b          (500) b          (506)     1541 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py
+-rw-r--r--   0 b          (500) b          (506)      815 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_ipcc2007.py
+-rw-r--r--   0 b          (500) b          (506)     1999 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_traci.py
+-rw-r--r--   0 b          (500) b          (506)     7401 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/data_sources/tests/test_uslci.py
+-rw-r--r--   0 b          (500) b          (506)     2438 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/data_sources/traci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/data_sources/uslci/
+-rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/data_sources/uslci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     6853 2024-03-21 02:23:41.000000 antelope_core-0.3.0/antelope_core/data_sources/uslci/uslci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/entities/
+-rw-r--r--   0 b          (500) b          (506)      181 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    11763 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/entities.py
+-rw-r--r--   0 b          (500) b          (506)     4408 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/flows.py
+-rw-r--r--   0 b          (500) b          (506)    25036 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/entities/processes.py
+-rw-r--r--   0 b          (500) b          (506)     7969 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/quantities.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/entities/tests/
+-rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/entities/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.3.0/antelope_core/entities/tests/base_testclass.py
+-rw-r--r--   0 b          (500) b          (506)    99145 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_archive.json
+-rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_entities.py
+-rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_entity_refs.py
+-rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_processes.py
+-rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.3.0/antelope_core/entities/tests/test_quantities.py
+-rw-r--r--   0 b          (500) b          (506)    18234 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/entities/xlsx_editor.py
+-rw-r--r--   0 b          (500) b          (506)    22640 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/exchanges.py
+-rw-r--r--   0 b          (500) b          (506)     6756 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/file_accessor.py
+-rw-r--r--   0 b          (500) b          (506)     1137 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/from_json.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/implementations/
+-rw-r--r--   0 b          (500) b          (506)      333 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/implementations/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8735 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/background.py
+-rw-r--r--   0 b          (500) b          (506)     6114 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/basic.py
+-rw-r--r--   0 b          (500) b          (506)    10035 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/implementations/configure.py
+-rw-r--r--   0 b          (500) b          (506)     2812 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/implementations/exchange.py
+-rw-r--r--   0 b          (500) b          (506)     6800 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/index.py
+-rw-r--r--   0 b          (500) b          (506)    32892 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/implementations/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.457665 antelope_core-0.3.0/antelope_core/implementations/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.3.0/antelope_core/implementations/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/implementations/tests/test_quantity.py
+-rw-r--r--   0 b          (500) b          (506)    16915 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lc_resource.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/
+-rw-r--r--   0 b          (500) b          (506)     5682 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8163 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/lcia_engine/clookup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/data/
+-rw-r--r--   0 b          (500) b          (506)     8401 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/contexts.json
+-rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/flowables.json
+-rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
+-rw-r--r--   0 b          (500) b          (506)    18280 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_engine/lcia_engine.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/lcia_engine/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1645 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py
+-rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_clookup.py
+-rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_ipcc.py
+-rw-r--r--   0 b          (500) b          (506)     2981 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_lcia_engine.py
+-rw-r--r--   0 b          (500) b          (506)    45982 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/lcia_results.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/providers/
+-rw-r--r--   0 b          (500) b          (506)     4643 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.460998 antelope_core-0.3.0/antelope_core/providers/data/
+-rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/data/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
+-rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
+-rw-r--r--   0 b          (500) b          (506)     9551 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)    11083 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecospold.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ecospold2/
+-rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24560 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2.py
+-rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2_index.py
+-rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/ecospold2/master_data.py
+-rw-r--r--   0 b          (500) b          (506)    10917 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/file_store.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/
+-rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    17683 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd.py
+-rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_flowables.py
+-rw-r--r--   0 b          (500) b          (506)     5806 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_lcia.py
+-rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/index.py
+-rw-r--r--   0 b          (500) b          (506)     3177 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
+-rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
+-rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
+-rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
+-rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
+-rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
+-rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
+-rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.3.0/antelope_core/providers/ilcd/tests/test_ilcd.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/openlca/
+-rw-r--r--   0 b          (500) b          (506)       91 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4887 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/olca_accessor.py
+-rw-r--r--   0 b          (500) b          (506)    12011 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/openlca/olca_ref_data.py
+-rw-r--r--   0 b          (500) b          (506)    24980 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/providers/openlca/openlca_jsonld.py
+-rw-r--r--   0 b          (500) b          (506)      775 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/providers/openlca/schema_mapping.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.464331 antelope_core-0.3.0/antelope_core/providers/openlca/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2024-01-05 07:24:59.000000 antelope_core-0.3.0/antelope_core/providers/openlca/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)       83 2024-01-05 07:57:07.000000 antelope_core-0.3.0/antelope_core/providers/openlca/tests/test_olca_ref.py
+-rw-r--r--   0 b          (500) b          (506)      729 2023-07-21 21:37:06.000000 antelope_core-0.3.0/antelope_core/providers/parse_math.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/tests/test_ecospold.py
+-rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/tests/test_xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/traci/
+-rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/providers/traci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/traci/index.py
+-rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.3.0/antelope_core/providers/traci/q_info.py
+-rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.3.0/antelope_core/providers/traci/quantity.py
+-rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/traci/test_traci.py
+-rw-r--r--   0 b          (500) b          (506)     6687 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/providers/xdb_client/
+-rw-r--r--   0 b          (500) b          (506)       67 2023-08-19 07:49:00.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    16888 2024-03-21 05:35:17.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/implementation.py
+-rw-r--r--   0 b          (500) b          (506)     4447 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/requester.py
+-rw-r--r--   0 b          (500) b          (506)     7202 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/rest_client.py
+-rw-r--r--   0 b          (500) b          (506)     7616 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_client.py
+-rw-r--r--   0 b          (500) b          (506)     3971 2024-03-21 02:23:39.000000 antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_entities.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/providers/xl_dict.py
+-rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.3.0/antelope_core/providers/xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.467665 antelope_core-0.3.0/antelope_core/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.3.0/antelope_core/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1007 2023-07-21 21:50:10.000000 antelope_core-0.3.0/antelope_core/tests/test_autorange.py
+-rw-r--r--   0 b          (500) b          (506)    13194 2024-03-20 22:20:51.000000 antelope_core-0.3.0/antelope_core/tests/test_contexts.py
+-rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/tests/test_exchanges.py
+-rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.3.0/antelope_core/tests/test_lcia_results.py
+-rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.3.0/antelope_core/tests/test_resources.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:37:35.450998 antelope_core-0.3.0/antelope_core.egg-info/
+-rw-r--r--   0 b          (500) b          (506)    14232 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     7084 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)      169 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       14 2024-03-21 22:37:35.000000 antelope_core-0.3.0/antelope_core.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2024-03-21 22:37:35.467665 antelope_core-0.3.0/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     3723 2024-03-21 02:23:39.000000 antelope_core-0.3.0/setup.py
```

### Comparing `antelope_core-0.2.4/LICENSE` & `antelope_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/PKG-INFO` & `antelope_core-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 Metadata-Version: 2.1
 Name: antelope_core
-Version: 0.2.4
+Version: 0.3.0
 Home-page: https://github.com/AntelopeLCA/core
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: XML
+Provides-Extra: write_to_excel
 License-File: LICENSE
-Requires-Dist: synonym_dict>=0.2.4
-Requires-Dist: antelope_interface>=0.2.4
-Requires-Dist: xlstools>=0.1.3
-Requires-Dist: python-magic>=0.4.18
-Requires-Dist: requests>=2.25
-Requires-Dist: pydantic>=2.5.0
-Provides-Extra: xml
-Requires-Dist: lxml>=1.2.0; extra == "xml"
-Provides-Extra: write-to-excel
-Requires-Dist: xlsxwriter>=1.3.7; extra == "write-to-excel"
 
 ![](https://travis-ci.com/AntelopeLCA/core.svg?branch=master&status=passed) ![](https://coveralls.io/repos/github/AntelopeLCA/core/badge.svg?branch=master)
 
 # core
 Antelope Catalog - reference implementation.
 
 This repository provides code that enables access to different forms of life cycle
```

### Comparing `antelope_core-0.2.4/README.md` & `antelope_core-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/__init__.py` & `antelope_core-0.3.0/antelope_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 from antelope import antelope_herd
 
 import importlib
 
 from .from_json import from_json, to_json
 from .archives import archive_factory, ArchiveError
 
+
+class AntelopeMeta:
+    version: str = '0.3'
+
+
 FOUND_PROVIDERS = LowerDict()
+FOUND_PROVIDERS['_dev'] = AntelopeMeta
 
 
 def _find_providers():
     for ant in [__name__] + antelope_herd:
         found = []
 
         def _add_found_providers(_found, _the):
@@ -46,15 +52,15 @@
         print('%s:%s' % (v.__name__, k))
 
 
 def herd_factory(ds_type):
     try:
         return archive_factory(ds_type)
     except ArchiveError:
-        if len(FOUND_PROVIDERS) == 0:
+        if len(FOUND_PROVIDERS) <= 1:
             _find_providers()
         if ds_type in FOUND_PROVIDERS:
             prov = FOUND_PROVIDERS[ds_type]
             try:
                 return getattr(prov, ds_type)
             except AttributeError:
                 dsl = ds_type.lower()
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/__init__.py` & `antelope_core-0.3.0/antelope_core/archives/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/archive_index.py` & `antelope_core-0.3.0/antelope_core/archives/archive_index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/basic_archive.py` & `antelope_core-0.3.0/antelope_core/archives/basic_archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,17 +476,21 @@
         j['@context'] = LD_CONTEXT
 
         j['flows'] = sorted([f.serialize(domesticate=domesticate, drop_fields=self._drop_fields['flow'])
                              for f in self.entities_by_type('flow')],
                             key=lambda x: x['externalId'])
         if characterizations:
             j['termManager'], qqs, rqs = self.tm.serialize(self.ref, values=values)
+            # we need to add all the quantities that are mentioned in our characterizations
             for q in qqs:
                 if self[q] is None:
                     self.add(self.tm.get_canonical(q))
+            for q in rqs:
+                if self[q] is None:
+                    self.add(self.tm.get_canonical(q))
 
         j['quantities'] = self._serialize_quantities(domesticate=domesticate)
 
         return j
 
     def export_quantities(self, filename, *quantities, domesticate=True, values=True, gzip=False):
         """
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/data/elcd_reference_quantities.json` & `antelope_core-0.3.0/antelope_core/archives/data/elcd_reference_quantities.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999103601077285%*

 * *Differences: {"'quantities'": "{0: {'UnitConversion': {'Unit': 1.0, 'unit': 1.0, 'Units': 1.0, 'units': 1.0}}, "*

 * *                 "7: {'UnitConversion': {'kwh': 1.0}}, 12: {'InverseUnitConversion': {'kWh': "*

 * *                 '3.6}}}'}*

```diff
@@ -192,17 +192,21 @@
             "Comment": "Reference Flow Property Data Set of the International Reference Life Cycle Data System (ILCD).",
             "Name": "Number of items",
             "UnitConversion": {
                 "Count": 1.0,
                 "Dozen(s)": 0.08333333333333333,
                 "Item(s)": 1.0,
                 "Items": 1.0,
+                "Unit": 1.0,
+                "Units": 1.0,
                 "count": 1.0,
                 "item": 1.0,
-                "items": 1.0
+                "items": 1.0,
+                "unit": 1.0,
+                "units": 1.0
             },
             "entityId": "01846770-4cfe-4a25-8ad9-919d8d378345",
             "entityType": "quantity",
             "externalId": "01846770-4cfe-4a25-8ad9-919d8d378345",
             "origin": "elcd.3.2",
             "referenceUnit": "Item(s)",
             "synonyms": [
@@ -371,15 +375,16 @@
                 "EcoSpold Quantity kWh",
                 "Electricity"
             ],
             "UnitConversion": {
                 "GWh": 1e-06,
                 "KJ": 3600.0,
                 "MJ": 3.6,
-                "MWh": 0.001
+                "MWh": 0.001,
+                "kwh": 1.0
             },
             "entityId": "77ae64fa-7e74-4252-9c3b-889c1cd20bfc",
             "entityType": "quantity",
             "externalId": "77ae64fa-7e74-4252-9c3b-889c1cd20bfc",
             "origin": "local.ecoinvent.3.2.cutoff",
             "referenceUnit": "kWh"
         },
@@ -513,15 +518,15 @@
                 "TJ": 1000000.0,
                 "TOE": 41867.28072011723,
                 "TWh": 3599971200.230398,
                 "cal": 4.186728072011723e-06,
                 "eV": 1.6022046335758002e-25,
                 "erg": 1e-13,
                 "kJ": 0.001,
-                "kWh": 3.5999712002303976,
+                "kWh": 3.6,
                 "kpm": 9.806805923310778e-06
             },
             "Name": "Energy from renewable raw materials (net cal. value)",
             "entityId": "8695e049-7a18-4b83-b3bd-035747039652",
             "entityType": "quantity",
             "externalId": "8695e049-7a18-4b83-b3bd-035747039652",
             "origin": "elcd.3.2",
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/entity_store.py` & `antelope_core-0.3.0/antelope_core/archives/entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/lc_archive.py` & `antelope_core-0.3.0/antelope_core/archives/lc_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/quantity_manager.py` & `antelope_core-0.3.0/antelope_core/archives/quantity_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,18 @@
         if unit == self.unit:
             return
         if self._quantity is not None:
             try:
                 cv = convert(self._quantity, from_unit=unit, to=self.unit)
                 if cv == 1.0:
                     return
+                print('Unit conversion mismatch %s->%s = %g' % (unit, self.unit, cv))
             except ConversionError:
-                pass
+                print('%s: Unit conversion KeyError on %s' % (self._quantity.name, unit))
+
         raise QuantityUnitMismatch('incoming %s (set %s)' % (unit, self.unit))
 
     @classmethod
     def new(cls, quantity):
         return cls(quantity.name, quantity=quantity)
 
     def _validate_quantity(self, quantity):
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/term_manager.py` & `antelope_core-0.3.0/antelope_core/archives/term_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,24 +876,24 @@
         generator was already returned before iterating.
 
         contexts are searched first, then quantities, then flowables
         :param term:
         :return:
         """
         try:
-            obj = self._cm[term]
-            it = self._cm.synonyms(obj)
+            obj = self._cm[term]  # we need this to trip the KeyError if it's not found
+            it = self._cm.synonyms(term)
         except KeyError:
             try:
-                obj = self._qm[term]
-                it = self._qm.synonyms(obj)
+                obj = self._qm[term]  # we need this to trip the KeyError if it's not found
+                it = self._qm.synonyms(term)
             except KeyError:
                 try:
-                    obj = self._fm[term]
-                    it = self._fm.synonyms(obj)
+                    obj = self._fm[term]  # we need this to trip the KeyError if it's not found
+                    it = self._fm.synonyms(term)
                 except KeyError:
                     it = ()
         for k in it:
             yield k
 
     def contexts(self, search=None, origin=None):
         for cx in self._cm.objects:
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_base.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_basic_archive.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_basic_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_entity_store.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_json.json` & `antelope_core-0.3.0/antelope_core/archives/tests/test_json.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_qdb.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_qdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,13 +52,14 @@
             if k.external_ref in ('f6811440-ee37-11de-8a39-0800200c9a66', 'e288b5d2-9fcc-4a10-b13c-440786090f43'):
                 # 'energy' (unspecified) and 'emissive coolness' respectively
                 with self.assertRaises(EntityNotFound):
                     self._qdb.query.get_canonical(k.external_ref)
                 self._qdb.add_entity_and_children(k)  # we commented out as foolhardy the code that auto-adds quantities in get_canonical
                 self.assertIs(self._qdb.query.get_canonical(k.external_ref), k)
             else:
-                qc = self._qdb.query.get_canonical(k)
-                self.assertEqual(qc.origin, 'local.qdb')
+                self.assertTrue(self._qdb.query.get_canonical(k))
+                # this is no longer desired behavior--- masqueraded entities read like their natural origin
+                # this test simply becomes an assertion that the canonical lookup completes
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_quantity_manager.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_quantity_relation.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_quantity_relation.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/archives/tests/test_term_manager.py` & `antelope_core-0.3.0/antelope_core/archives/tests/test_term_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/autorange.py` & `antelope_core-0.3.0/antelope_core/autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/catalog.py` & `antelope_core-0.3.0/antelope_core/catalog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,26 +443,28 @@
             pass
         else:
             raise InvalidQuery(origin)
         if cache:
             self._queries[origin] = query
         return query
 
-    def lookup(self, catalog_ref, keep_properties=False):
+    def lookup(self, catalog_ref):
         """
         Attempts to return a valid grounded reference matching the one supplied.
         :param catalog_ref:
-        :param keep_properties: [False] if True, apply incoming ref's properties to grounded ref, probably with a
+        :deprecated keep_properties: [False] if True, apply incoming ref's properties to grounded ref, probably with a
         prefix or something.
         :return:
         """
         ref = self.query(catalog_ref.origin).get(catalog_ref.external_ref)
+        '''
         if keep_properties:
             for k in catalog_ref.properties():
                 ref[k] = catalog_ref[k]
+        '''
         return ref
 
     '''
     def lookup(self, origin, external_ref=None):
         """
         Attempts to secure an entity
         :param origin:
@@ -480,14 +482,16 @@
         raise EntityNotFound('%s/%s' % (origin, external_ref))
     '''
 
     def fetch(self, link):
         origin, external_ref = link.split('/', maxsplit=1)
         return self.query(origin).get(external_ref)
 
+    '''
+    # why is this here? I don't think we even want this.
     def catalog_ref(self, origin, external_ref, entity_type=None, **kwargs):
         """
         TODO: make foreground-generated CatalogRefs lazy-loading. This mainly requires removing the expectation of a
         locally-defined reference entity, and properly implementing and using a reference-retrieval process in the
         basic interface.
         :param origin:
         :param external_ref:
@@ -501,8 +505,8 @@
             ref = CatalogRef(origin, external_ref, entity_type=entity_type, **kwargs)
             print('Ungrounded catalog ref %s' % ref.link)
             self._bad_origins[origin].add(ref)
             return ref
         return q.get(external_ref)
         # except EntityNotFound:  why would we catch this?
         #     return CatalogRef.from_query(external_ref, q, entity_type=entity_type, **kwargs)
-
+    '''
```

### Comparing `antelope_core-0.2.4/antelope_core/catalog/catalog_root.py` & `antelope_core-0.3.0/antelope_core/catalog/catalog_root.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/configurator.py` & `antelope_core-0.3.0/antelope_core/catalog/configurator.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/lc_catalog.py` & `antelope_core-0.3.0/antelope_core/catalog/lc_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,23 +161,25 @@
         :return:
         """
         self._resolver.add_resource(resource, store=store)
 
     def purge_resource_archive(self, resource: LcResource):
         """
         - find all cached queries that could return the resource
-        - check their cached interfaces to see if they use our archive
+        - check their cached ifaces to see if they use our archive
         - delete those entries from the cache
         :param resource:
         :return:
         """
         # TODO: though this corrects our catalog queries, the entities are not connected to the catalog queries
         for org, q in self._queries.items():
             if resource.origin.startswith(org):
+                print('Purging %s' % q)
                 q.purge_cache_with(resource.archive)
+        print('Removing archive from %s' % resource)
         resource.remove_archive()
 
     def delete_resource(self, resource, delete_source=None, delete_cache=True):
         """
         Removes the resource from the resolver and also removes the serialization of the resource. Also deletes the
         resource's source (as well as all files in the same directory that start with the same name) under the following
         circumstances:
@@ -259,27 +261,34 @@
             except HTTPError:
                 client.close()
                 raise
         else:
             client = RestClient(blackbook_url, token=token, auth_route='auth/token', **kwargs)
         self._blackbook_client = client
 
-    def get_blackbook_resources(self, origin, store=False):
+    @property
+    def blackbook_origins(self):
+        if self._blackbook_client is not None:
+            for org in sorted(self._blackbook_client.get_raw('origins')):
+                yield org
+
+    def get_blackbook_resources(self, origin, store=False, **kwargs):
         """
         Use a blackbook server to obtain resources for a given origin.
         :param origin:
         :param store: whether to save resources. by default we don't, assuming the tokens are short-lived.
+        :param kwargs: init args to add to returned resources, such as 'verify' certificate paths
         :return:
         """
         res = list(self.resources(origin))
         if len(res) > 0:
             return self.refresh_xdb_tokens(origin)
         else:
             resource_dict = self._blackbook_client.get_one(dict, 'origins', origin, 'resource')
-            return self._configure_blackbook_resources(resource_dict, store=store)
+            return self._configure_blackbook_resources(resource_dict, store=store, **kwargs)
 
     '''
     def get_blackbook_resources_by_client(self, bb_client, username, origin, store=False):
         """
         this uses the local maintenance client rather than the REST client
         :param bb_client:
         :param username:
@@ -287,15 +296,15 @@
         :param store:
         :return:
         """
         resource_dict = bb_client.retrieve_resource(username, origin)
         return self._finish_get_blackbook_resources(resource_dict, store=store)
     '''
 
-    def _configure_blackbook_resources(self, resource_dict, store=False):
+    def _configure_blackbook_resources(self, resource_dict, store=False, **kwargs):
         """
         Emerging issue here in the xdb/oryx context-- we need to be able to replace resources even if they are
         serialized and already initialized.
 
         response: this is easy- the XdbClient provider (and subclasses) has refresh_token and refresh_auth methods
         already.
 
@@ -315,31 +324,34 @@
         for recv_origin, res_list in resource_dict.items():
             # self._resolver.delete_origin(recv_origin)
             for res in res_list:
                 if not isinstance(res, ResourceSpec):
                     res = ResourceSpec(**res)
                 try:
                     exis = next(x for x in self.resources(recv_origin) if x.ds_type == res.ds_type)
+                    exis.init_args.update(kwargs)
                     exis.check(self)
                     # one exists-- update it
                     exis.init_args.update(res.options)
                     if exis.source == res.source:
                         exis.archive.refresh_token(res.options['token'])
                     else:
                         exis.source = res.source
                         exis.archive.refresh_auth(res.source, res.options['token'])
                     for i in res.interfaces:
                         if i not in exis.interfaces:
                             exis.add_interface(i)
                     for i in exis.interfaces:
                         if i not in res.interfaces:
                             exis.remove_interface(i)
+                    if store:
+                        exis.write_to_file(self.resource_dir)
                     rtn.append(exis)
                 except StopIteration:
-                    r = LcResource(**res.dict())
+                    r = LcResource(**res.model_dump(), **kwargs)
                     self.add_resource(r, store=store)
                     rtn.append(r)
         return rtn
 
     def refresh_xdb_tokens(self, origin):
         """
         requires an active blackbook client (try blackbook_authenticate() if it has expired)
```

### Comparing `antelope_core-0.2.4/antelope_core/catalog/lc_resolver.py` & `antelope_core-0.3.0/antelope_core/catalog/lc_resolver.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/tests/test_catalogs.py` & `antelope_core-0.3.0/antelope_core/catalog/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/tests/test_process_ref.py` & `antelope_core-0.3.0/antelope_core/catalog/tests/test_process_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog/tests/test_quantity_refs.py` & `antelope_core-0.3.0/antelope_core/catalog/tests/test_quantity_refs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/catalog_query.py` & `antelope_core-0.3.0/antelope_core/catalog_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """
 Query Interface -- used to operate catalog refs
 """
 
-from antelope import (BasicInterface, IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface,
-                      EntityNotFound, UnknownOrigin)
+from antelope import (IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface, EntityNotFound,
+                      UnknownOrigin,
+                      ExchangeRef, comp_dir, BaseEntity)
 #                      ForegroundInterface,
 #                      IndexRequired, PropertyExists,
 #                      )
 from antelope.refs.exchange_ref import RxRef
 
+from antelope.models import LciaResult as LciaResultModel, Characterization as CharacterizationModel
+
+from .lcia_results import LciaResult
+from .characterizations import QRResult, Characterization
+from .contexts import NullContext
+
+from synonym_dict import InconsistentLineage
+
 INTERFACE_TYPES = ('basic', 'index', 'exchange', 'background', 'quantity', 'foreground')
 READONLY_INTERFACE_TYPES = {'basic', 'index', 'exchange', 'background', 'quantity'}
 
 
 def zap_inventory(interface, warn=False):
     if interface == 'inventory':
         if warn:
@@ -30,15 +39,15 @@
     pass
 
 
 class BadInterfaceSpec(Exception):
     pass
 
 
-class CatalogQuery(BasicInterface, IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface):
+class CatalogQuery(IndexInterface, BackgroundInterface, ExchangeInterface, QuantityInterface):
     """
     A CatalogQuery is a class that performs any supported query against a supplied catalog.
     Supported queries are defined in the lcatools.interfaces, which are all abstract.
     Implementations also subclass the abstract classes.
 
     This reduces code duplication (all the catalog needs to do is provide interfaces) and ensures consistent signatures.
 
@@ -107,23 +116,24 @@
         return self._tm[context.fullname].elementary
     '''
 
     def cascade(self, origin):
         """
         Generate a new query for the specified origin.
         Enables the query to follow the origins of foreign objects found locally.
+        If not found locally, the current query is used instead
         :param origin:
         :return:
         """
         return self._grounded_query(origin)
 
     def _grounded_query(self, origin):
         if origin is None or origin == self._origin:
             return self
-        return self._catalog.query(origin)
+        return self._catalog.query(origin, cache=False)
 
     '''
     def __str__(self):
         return '%s for %s (catalog: %s)' % (self.__class__.__name__, self.origin, self._catalog.root)
     '''
     def _setup_background(self, bi):
         self._debug('Setting up background interface')
@@ -156,16 +166,19 @@
         try:
             for iface in self._iface(itype, strict=strict):
                 try:
                     self._debug('Attempting %s query on iface %s' % (attrname, iface))
                     result = getattr(iface, attrname)(*args, **kwargs)
                     message = '(%s) %s' % (itype, attrname)  # implementation found
                 except exc:  # allow nonimplementations to pass silently
+                    message = '(%s) %s except %s' % (itype, attrname, exc.__name__)
                     continue
-                if result is not None:  # successful query must return something
+                if result is None:  # successful query must return something
+                    message = '(%s) %s null' % (itype, attrname)
+                else:
                     return result
         except NotImplementedError:
             pass
 
         raise exc('%s: %s | %s' % (self.origin, message, args))
 
     def resolve(self, itype=INTERFACE_TYPES, strict=False):
@@ -212,19 +225,21 @@
 
     '''
     LCIA Support
     get_canonical(quantity)
     catch get_canonical calls to return the query from the local Qdb; fetch if absent and load its characterizations
     (using super ==> _perform_query)
     '''
+    '''
     def get_context(self, term, **kwargs):
         cx = super(CatalogQuery, self).get_context(term, **kwargs)
         return self._tm[cx]
+    '''
 
-    def get_canonical(self, quantity, **kwargs):
+    def get_canonical(self, quantity: str | BaseEntity, **kwargs):
         try:
             # print('Gone canonical')
             q_can = self._tm.get_canonical(quantity)
         except EntityNotFound:
             if hasattr(quantity, 'entity_type') and quantity.entity_type == 'quantity':
                 print('Missing canonical quantity-- adding to LciaDb')
                 self._catalog.register_entity_ref(quantity)
@@ -265,15 +280,15 @@
         :param location:
         :param kwargs:
         :return:
         """
         rq = self.get_canonical(ref_quantity)
         qq = self.get_canonical(query_quantity)
         origin = kwargs.pop('origin', self.origin)
-        print('@@@ going characterization-commando')
+        # print('@@@ going characterization-commando')
         return self._tm.add_characterization(flowable, rq, qq, value, context=context, location=location,
                                              origin=origin, **kwargs)
 
     def clear_seen_characterizations(self, quantity):
         """
         An ugly hack to deal with the absolutely terrible way we are working around our slow-ass Qdb implementation
         the proper solution is for qdb lookup to be local,  fast and correct, so as to not require caching at all.
@@ -300,14 +315,25 @@
             try:
                 e_ref = entity.make_ref(self._grounded_query(entity.origin))
             except UnknownOrigin:
                 e_ref = entity.make_ref(self)
         else:
             e_ref = entity  # already a ref
         if entity.entity_type == 'quantity':
+
+            '''# question of whether to put this test before or after the get_canonical() attempts
+            if before- we allow non-canonical "mass" to accumulate in the workspace
+            if after- we catch 'mass' and 'freight' (and any LCIA methods we already know locally)
+            and only return shit we don't recognize, but lose connection to remote sources
+            
+            prefer before: we may want to query core quantities like "net calorific value" for flow characterizations
+            '''
+            if entity.has_lcia_engine():  # we don't need a canonical version if it runs itself
+                return e_ref
+
             ''' # astonishingly, we don't want this - register but not return
             # print('Going canonical')
             # astonishing because it's not true. 
             Well. not exactly true.
             
             CatalogQueries should return canonical quantities. that is the point of the catalog.  The reason we didn't
             want this was because we were using the catalog to access origin-specific data to re-serve it.  On the
@@ -317,16 +343,113 @@
             
             True, the data won't match the source.  but we will still RECOGNIZE the source because we will register the 
             quantity terms with the term manager.  Which we WEREN"T doing before.
             
             A corollary of this is that CatalogQuery.get() should get_canonical FIRST
             '''
             try:
-                _ = self._tm.get_canonical(entity)
+                return self._tm.get_canonical(entity.link)
             except EntityNotFound:
-                self._catalog.register_entity_ref(e_ref)
-                return self._tm.get_canonical(entity)
-            # print('@@@ Canonical quantity missing link-- adding direct to qm')  # I predict this never occurs
-            # in fact, it occurred several times immediately
-            return self._tm.add_quantity(entity)  # this will be identical to _ unless there is a unit conflict
+                try:
+                    _ = self._tm.get_canonical(entity)
+                except EntityNotFound:
+                    self._catalog.register_entity_ref(e_ref)
+                    return self._tm.get_canonical(entity)
+                # print('@@@ Canonical quantity missing link-- adding direct to qm')  # I predict this never occurs
+                # in fact, it occurred several times immediately
+                return self._tm.add_quantity(entity)  # this will be identical to _ unless there is a unit conflict
         else:
             return e_ref
+
+    '''
+    de-reference Characterization factor models
+    '''
+
+    def _resolve_cf(self, cf: CharacterizationModel) -> Characterization:
+        """
+
+        :param cf:
+        :return:
+        """
+        rq = self.get_canonical(cf.ref_quantity)
+        qq = self.get_canonical(cf.query_quantity)
+        try:
+            cx = self._tm[tuple(cf.context)]
+        except InconsistentLineage:
+            cx = NullContext
+        c = Characterization(cf.flowable, rq, qq, cx, origin=cf.origin)
+        for k, v in cf.value.items():
+            c[k] = v
+        return c
+
+    def factors(self, quantity, flowable=None, context=None, **kwargs):
+        for cf in super(CatalogQuery, self).factors(quantity, flowable=flowable, context=context, **kwargs):
+            if isinstance(cf, CharacterizationModel):
+                yield self._resolve_cf(cf)
+            else:
+                yield cf
+
+    '''
+    de-reference LciaResult models
+    '''
+
+    def _result_from_model(self, process_ref, quantity, res_m: LciaResultModel):
+        """
+        Constructs a Detailed LCIA result from a background LCIA query, when we don't have a list of exchanges
+        :param process_ref:
+        :param quantity:
+        :param res_m:
+        :return:
+        """
+        res = LciaResult(quantity, scenario=res_m.scenario, scale=res_m.scale)
+        process = self.get(process_ref)
+        for c in res_m.components:
+            for d in c.details:
+                value = d.result / d.factor.value
+                cx = self._tm[tuple(d.factor.context)]
+                try:
+                    flow_ref = self.cascade(d.exchange.origin).get(d.exchange.external_ref)
+                except UnknownOrigin:
+                    flow_ref = self.get(d.exchange.external_ref, origin=d.exchange.origin)
+                ex_dir = comp_dir(cx.sense)
+                if ex_dir is None:
+                    print('Bad context: %s' % list(cx))
+                    print('using "Output" direction')
+                    ex_dir = 'Output'
+                ex = ExchangeRef(process, flow_ref,
+                                 ex_dir,
+                                 termination=cx, value=value)
+                rq = self.get_canonical(d.exchange.quantity_ref)
+                cf = QRResult(d.factor.flowable, rq, quantity, cx,
+                              d.factor.locale, d.factor.origin, d.factor.value)
+                res.add_score(c.component, ex, cf)
+        for s in res_m.summaries:
+            res.add_summary(s.component, s.component, s.node_weight, s.unit_score)
+        return res
+
+    def _cycle_through_ress(self, ress, process, query_qty):
+        if isinstance(ress, list):
+            conv = []
+            for res in ress:
+                if isinstance(res, LciaResultModel):
+                    conv.append(self._result_from_model(process_ref=process, quantity=query_qty, res_m=res))
+                else:
+                    conv.append(res)
+            return conv
+        else:
+            if isinstance(ress, LciaResultModel):
+                return self._result_from_model(process_ref=process, quantity=query_qty, res_m=ress)
+            else:
+                return ress
+
+    def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
+        """
+        Reimplement this to detect pydantic LciaResult models and de-reference them
+        :param process:
+        :param query_qty:
+        :param observed:
+        :param ref_flow:
+        :param kwargs:
+        :return:
+        """
+        ress = super(CatalogQuery, self).bg_lcia(process, query_qty, observed=observed, ref_flow=ref_flow, **kwargs)
+        return self._cycle_through_ress(ress, process, query_qty)
```

### Comparing `antelope_core-0.2.4/antelope_core/characterizations.py` & `antelope_core-0.3.0/antelope_core/characterizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         :param value: passed to add_value if present
         :param location: 'GLO' passed to add_value if present
         :param origin: of data, if applicable
         :return:
         """
         assert ref_quantity.entity_type == 'quantity', "'ref_quantity' must be an LcQuantity"
         assert query_quantity.entity_type == 'quantity', "'query_quantity' must be an LcQuantity"
-        assert ref_quantity.is_lcia_method is False, "'ref_quantity' cannot be an LCIA method"
+        assert ref_quantity.is_lcia_method is False, "'ref_quantity' %s cannot be an LCIA method" % ref_quantity
 
         self.flowable = str(flow_name)
         self.quantity = query_quantity
         self._ref_q = ref_quantity
         if context is None:
             raise MissingContext('%s, %s, %s' % (flow_name, ref_quantity, query_quantity))
         self._context = context
@@ -194,16 +194,16 @@
             elif isclose(self._locations[key], value, rel_tol=1e-6):
                 print('%e %e' % (self._locations[key], value))
                 return
             if isinstance(self._locations[key], str):
                 pval = '%s (incoming: %s)' % (self._locations[key], value)
             else:
                 pval = '%g (incoming: %s)' % (self._locations[key], value)
-            raise DuplicateCharacterizationError('%s: Characterization value already present! %s = %s\n%s' %
-                                                 (self.quantity, key, pval, self.flowable))
+            raise DuplicateCharacterizationError('%s: Characterization value already present! %s = %s\n%s\n%s' %
+                                                 (self.quantity, key, pval, self.flowable, self.context))
         self._locations[key] = value
 
     def update_values(self, **kwargs):
         self._locations.update(kwargs)
 
     def add_value(self, value=None, location=None, overwrite=False):
         if location is None:
```

### Comparing `antelope_core-0.2.4/antelope_core/contexts.py` & `antelope_core-0.3.0/antelope_core/contexts.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/data_source.py` & `antelope_core-0.3.0/antelope_core/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/ecoinvent.py` & `antelope_core-0.3.0/antelope_core/data_sources/ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/ecoinvent_lcia.py` & `antelope_core-0.3.0/antelope_core/data_sources/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/gwp_ipcc_2007.py` & `antelope_core-0.3.0/antelope_core/data_sources/gwp_ipcc_2007.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/local.py` & `antelope_core-0.3.0/antelope_core/data_sources/local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_aa_local.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_aa_local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_ecoinvent.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_ecoinvent_lci.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_ipcc2007.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_ipcc2007.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_traci.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/tests/test_uslci.py` & `antelope_core-0.3.0/antelope_core/data_sources/tests/test_uslci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/traci.py` & `antelope_core-0.3.0/antelope_core/data_sources/traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/data_sources/uslci/uslci.py` & `antelope_core-0.3.0/antelope_core/data_sources/uslci/uslci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/entities.py` & `antelope_core-0.3.0/antelope_core/entities/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         if self._query_ref is None:
             d = dict()
             for k in self.signature_fields():
                 if k == self._ref_field:
                     continue
                 if k in self._d:
                     d[k] = self._d[k]
+            # this is a potential DWR--
+            # if the query does not match the entity, we want the ref to have the authentic origin
+            # we're expecting this to only occur from within CatalogQuery._grounded_query() -> UnknownOrigin
+            if query.origin != self.origin:
+                d['masquerade'] = self.origin
             self._query_ref = CatalogRef.from_query(self.external_ref, query, self.entity_type,
                                                     uuid=self.uuid, **d)
         return self._query_ref
 
     @property
     def entity_type(self):
         return self._entity_type
```

### Comparing `antelope_core-0.2.4/antelope_core/entities/flows.py` & `antelope_core-0.3.0/antelope_core/entities/flows.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/processes.py` & `antelope_core-0.3.0/antelope_core/entities/processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/quantities.py` & `antelope_core-0.3.0/antelope_core/entities/quantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,19 @@
 
     def _set_reference(self, ref_entity):
         if isinstance(ref_entity, str):
             ref_entity = LcUnit(ref_entity)
         super(LcQuantity, self)._set_reference(ref_entity)
 
     def quantity_terms(self):
-        yield self['Name']
-        yield self.name
-        yield str(self)  # this is the same as above for entities, but includes origin for refs
-        yield self.external_ref  # do we definitely want this?  will squash versions together
+        if not self.is_lcia_method:
+            yield self['Name']
+            yield self.name
+            yield str(self)  # this is the same as above for entities, but includes origin for refs
+        yield self.external_ref  # do we definitely want this?  version-less name will return earliest version
         if self.uuid is not None:
             yield self.uuid
         if self.origin is not None:
             yield self.link
         if self.has_property('Synonyms'):
             syns = self['Synonyms']
             if isinstance(syns, str):
@@ -108,14 +109,16 @@
 
     """
     Quantity Interface Methods
     Quantity entities use the quantity interface provided by the parent archive; this emulates the operation of 
     quantity refs, which have access to the catalog.
     """
     def has_lcia_engine(self):
+        if self._qi is None:
+            return False
         return self._qi.is_lcia_engine()
 
     def canonical(self):
         return self._qi.get_canonical(self)
 
     def cf(self, flow, locale='GLO', **kwargs):
         """
@@ -165,15 +168,16 @@
     def reset_unitstring(self, ustring):
         self.reference_entity.reset_unitstring(ustring)
 
     @property
     def _name(self):
         n = '%s [%s]' % (self._d['Name'].replace('\n', '|'), self.reference_entity.unitstring)
         if self.is_lcia_method:
-            return '%s [LCIA]' % n
+            m = self.get('Method', 'LCIA')
+            return '%s [%s]' % (n, m)
         return n
 
     @property
     def name(self):
         return self._name
 
     def __str__(self):
```

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/base_testclass.py` & `antelope_core-0.3.0/antelope_core/entities/tests/base_testclass.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/test_archive.json` & `antelope_core-0.3.0/antelope_core/entities/tests/test_archive.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'catalogNames'": "{replace: OrderedDict([('local.uslci.olca', "*

 * *                   "['/data/GitHub/lca-tools/lcatools/entities/tests/test_archive.json'])])}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "@context": "https://bkuczenski.github.io/lca-tools-datafiles/context.jsonld",
     "catalogNames": {
-        "test.entities": [
+        "local.uslci.olca": [
             "/data/GitHub/lca-tools/lcatools/entities/tests/test_archive.json"
         ]
     },
     "dataSource": "/data/GitHub/lca-tools/lcatools/entities/tests/test_archive.json",
     "dataSourceType": "LcArchive",
     "flows": [
         {
```

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/test_entities.py` & `antelope_core-0.3.0/antelope_core/entities/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/test_entity_refs.py` & `antelope_core-0.3.0/antelope_core/entities/tests/test_entity_refs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/test_processes.py` & `antelope_core-0.3.0/antelope_core/entities/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/tests/test_quantities.py` & `antelope_core-0.3.0/antelope_core/entities/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/entities/xlsx_editor.py` & `antelope_core-0.3.0/antelope_core/entities/xlsx_editor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/exchanges.py` & `antelope_core-0.3.0/antelope_core/exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/file_accessor.py` & `antelope_core-0.3.0/antelope_core/file_accessor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/from_json.py` & `antelope_core-0.3.0/antelope_core/from_json.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/implementations/background.py` & `antelope_core-0.3.0/antelope_core/implementations/background.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from itertools import chain
 
 from .basic import BasicImplementation
-from antelope import BackgroundInterface, EntityNotFound, comp_dir  # , ProductFlow
-from antelope.models import ExteriorFlow
+from antelope import BackgroundInterface, ExteriorFlow, EntityNotFound, comp_dir  # , ProductFlow
 from antelope_core.contexts import Context
 
 
 class NonStaticBackground(Exception):
     pass
 
 
@@ -32,25 +31,25 @@
     def check_bg(self, **kwargs):
         self.setup_bm(**kwargs)
         return bool(self._index is not None)
 
     def setup_bm(self, index=None):
         """
         Requires an index interface or catalog query <-- preferred
-        HOLD UP- catalog query limits access to interfaces named in the resource, which may not include index.
-        It also returns entity references, which may be inadequate to the task of generating results (e.g. it is
-        an error for the same LOCAL implementation to provide both 'exchange' and 'background' as they will be the
-        same).  So routes that require exchange access, e.g. to fake up lci, should access the archive directly
+        This must provide .get() and .get_context() (so really it should maybe be 'basic'
+        The trivial implementation uses .flows() and .targets() to mock up an exterior flows method
         :param index:
         :return:
         """
         if self._index is None:
             if index is None:
+                print('%%%%%% Setting up Background Impl for %s from archive %s' % (self.origin, self._archive))
                 self._index = self._archive.make_interface('index')
             else:
+                print('%%%%%% Setting up Background Impl for %s from index %s' % (self.origin, index))
                 self._index = index
 
     def _ensure_ref_flow(self, ref_flow):
         if ref_flow is not None:
             if isinstance(ref_flow, str) or isinstance(ref_flow, int):
                 ref_flow = self._archive.retrieve_or_fetch_entity(ref_flow)
         return ref_flow
@@ -101,15 +100,15 @@
                 dirn = comp_dir(cx.sense)  # this is already w.r.t. interior
                 '''
                 if self.is_elementary(f):
                     yield ExteriorFlow(self._archive.ref, f, 'Output', f['Compartment'])
                 else:
                     yield ExteriorFlow(self._archive.ref, f, 'Output', None)
                 '''
-                yield ExteriorFlow.from_background(f, dirn, cx)
+                yield ExteriorFlow(self._archive.ref, f, dirn, cx)
 
     def consumers(self, process, ref_flow=None, **kwargs):
         """
         Not supported for trivial backgrounds
         :param process:
         :param ref_flow:
         :param kwargs:
```

### Comparing `antelope_core-0.2.4/antelope_core/implementations/basic.py` & `antelope_core-0.3.0/antelope_core/implementations/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,19 @@
     def __str__(self):
         return '%s for %s (%s)' % (self.__class__.__name__, self.origin, self._archive.source)
 
     def __getitem__(self, item):
         return self._archive[item]
 
     def _dereference_entity(self, external_ref):
+        """
+        returns a real local entity (non ref) for which is_entity is True
+        :param external_ref:
+        :return:
+        """
         if hasattr(external_ref, 'external_ref'):
             eref = external_ref
             external_ref = eref.external_ref
         else:
             eref = None
         entity = self.get(external_ref)
         # if entity:
@@ -70,15 +75,18 @@
         same, throws an error.
         :param external_ref:
         :param item:
         :return:
         """
         entity = self._dereference_entity(external_ref)
         if entity.has_property(item):
-            return entity[item]
+            obj = entity[item]
+            if obj is None:
+                raise KeyError
+            return obj
         raise KeyError('%s: %s [%s]' % (self.origin, external_ref, item))
         # raise EntityNotFound(external_ref)
 
     def get_reference(self, key):
         entity = self._dereference_entity(key)
         if entity is None:
             return None
@@ -86,18 +94,20 @@
             # need to get actual references with exchange values-- not the reference_entity
             return [x for x in entity.references()]
         if entity.reference_entity is None:
             return NullEntity(self.origin)
         return entity.reference_entity
 
     def get_uuid(self, external_ref):
-        u = self._archive.get_uuid(external_ref)
+        u = self._fetch(external_ref)
         if u is None:
             return False
-        return u
+        if u.uuid is None:
+            return False
+        return u.uuid
 
     def _fetch(self, external_ref, **kwargs):
         if external_ref is None:
             return None
         if self._archive.static:
             return self._archive[external_ref]
         try:
```

### Comparing `antelope_core-0.2.4/antelope_core/implementations/configure.py` & `antelope_core-0.3.0/antelope_core/implementations/configure.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/implementations/exchange.py` & `antelope_core-0.3.0/antelope_core/implementations/exchange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/implementations/index.py` & `antelope_core-0.3.0/antelope_core/implementations/index.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 
 from antelope import IndexInterface, comp_dir, CONTEXT_STATUS_
 from .basic import BasicImplementation
 from ..contexts import NullContext
+from ..entities import MetaQuantityUnit
 
 
 class IndexImplementation(BasicImplementation, IndexInterface):
     """
     A CatalogInterface provides basic-level semantic data about entities
 
     Only requires the abstract ArchiveImplementation
@@ -36,15 +37,15 @@
         This should only be run if the archive is local
         :param cutoffs: [False] if true, terminations include all cutoff [null-termination] exchanges, not just
           references
          :NOTE: until context refactor there is no consistent usage of terminations, so we will skip this
         :return:
         """
         for p in self._archive.entities_by_type('process'):
-            if cutoffs and CONTEXT_STATUS_ == 'new':
+            if cutoffs and CONTEXT_STATUS_ != 'compat':
                 for x in p.exchanges():
                     if x.termination is None:
                         self._terminations[x.flow.external_ref].add((x.direction, p))
             else:
                 for rx in p.reference_entity:
                     self._terminations[rx.flow.external_ref].add((rx.direction, p))
     """
@@ -66,16 +67,33 @@
         for q in self._archive.search('quantity', **kwargs):
             if unit is not None:
                 if q.unit != unit:
                     continue
             yield q
 
     def lcia_methods(self, **kwargs):
-        for q in self._archive.search('quantity', **kwargs):
-            if q.is_lcia_method:
+        """
+        Generate LCIA Methods-- which are quantities that have defined indicators
+        :param kwargs:
+        :return:
+        """
+        indicator = kwargs.pop('Indicator', '')
+        for i in filter(lambda x: x.has_property('Indicator'), self.quantities(Indicator=indicator, **kwargs)):
+            yield i
+
+    def lcia(self, **kwargs):
+        """
+        Generate LCIA Methodologies or method collections- these are specified by having the singleton MetaQuantityUnit
+        (and/or the unitstring '0') as a unit. They should *not* have indicators.
+        They have a property 'impactCategories' which is a list of included lcia_methods
+        :param kwargs:
+        :return:
+        """
+        for q in self.quantities():
+            if q.reference_entity is MetaQuantityUnit:
                 yield q
 
     def targets(self, flow_ref, direction=None, **kwargs):
         """
         Generate processes in the archive that terminate a given exchange i.e. - have the same flow and a complementary
         direction.  If refs_only is specified, only report processes that terminate the exchange with a reference
         exchange.
```

### Comparing `antelope_core-0.2.4/antelope_core/implementations/quantity.py` & `antelope_core-0.3.0/antelope_core/implementations/quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @classmethod
     def copy(cls, conv):
         return cls(*conv.results, query=conv.query, context=conv.context)
 
     def __init__(self, *args, query=None, context=NullContext):
         self._query = query  # this is just a stub to give ref conversion machinery something to grab hold of
-        self._context = context
+        self._context = context  # this is the canonical context that was used to generate the QR Results
         self._results = []
         for arg in args:
             self.add_result(arg)
 
     def __hash__(self):
         return hash((self.flowable, self.ref, self.query, self.context, self.locale))
 
@@ -120,19 +120,23 @@
     def flowable(self):
         if len(self._results) == 0:
             return None
         return self._results[0].flowable
 
     @property
     def context(self):
+        """
+        We want to return the canonical context if at all possible
+        :return:
+        """
+        if self._context is not None:
+            return self._context
         for qrr in reversed(self._results):
             if qrr.context is not None:
                 return qrr.context
-        if self._context is not None:
-            return self._context
         return NullContext
 
     @property
     def locale(self):
         locs = []
         for res in self._results:
             if res.locale not in locs:
@@ -396,65 +400,65 @@
         if qq.origin != self._archive.ref:
             self._archive.add_entity_and_children(qq)  # catches EntityExists
         if origin is None:
             origin = self.origin
         return self._archive.tm.add_characterization(flowable, rq, qq, value, context=context, location=location,
                                                      origin=origin, **kwargs)
 
-    def _ref_qty_conversion(self, target_quantity, flowable, compartment, conv, locale, _reverse=True):
+    def _ref_qty_conversion(self, target_quantity, fb, cx, conv, locale, _reverse=True):
         """
         Transforms a CF into a quantity conversion with the proper ref quantity. Does it recursively! watch with terror.
-        :param target_quantity: conversion target
-        :param flowable:
-        :param compartment:
+        :param target_quantity: conversion target (canonical)
+        :param fb: flowable (canonical)
+        :param cx: context (canonical)
         :param conv: An existing QuantityConversion chain, whose ref we must turn into target_quantity
         :param locale:
         :return: the incoming conv, augmented
         """
         if target_quantity is None:
             raise ConversionReferenceMismatch('Cannot convert to None')
         found_quantity = self.get_canonical(conv.ref)  # this is still necessary because CFs are stored with native ref quantities
         if found_quantity != target_quantity:
             # zero look for conversions
             try:
-                qr_result = try_convert(flowable, target_quantity, found_quantity, compartment, locale)
+                qr_result = try_convert(fb, target_quantity, found_quantity, cx, locale)
                 conv.add_result(qr_result)
                 return conv
             except NoConversion:
                 pass
 
             # first look for forward matches
-            cfs_fwd = [cf for cf in self._archive.tm.factors_for_flowable(flowable, quantity=found_quantity,
-                                                                          context=compartment, dist=3)
+            cfs_fwd = [cf for cf in self._archive.tm.factors_for_flowable(fb, quantity=found_quantity,
+                                                                          context=cx, dist=3)
                        if not conv.seen(cf.ref_quantity)]
             for cf in cfs_fwd:
                 new_conv = QuantityConversion.copy(conv)
                 new_conv.add_result(cf.query(locale))
                 try:
-                    return self._ref_qty_conversion(target_quantity, flowable, compartment, new_conv, locale,
+                    return self._ref_qty_conversion(target_quantity, fb, cx, new_conv, locale,
                                                     _reverse=_reverse)
                 except ConversionReferenceMismatch:
                     continue
 
             # then look for reverse matches... but... only once
             if _reverse:
                 new_conv = QuantityConversion.copy(conv)
                 try:
-                    rev_conv = self._ref_qty_conversion(found_quantity, flowable, compartment,
-                                                        QuantityConversion(query=target_quantity), locale,
+                    rev_conv = self._ref_qty_conversion(found_quantity, fb, cx,
+                                                        QuantityConversion(query=target_quantity, context=cx), locale,
                                                         _reverse=False)
 
                     for res in rev_conv.invert().results:
                         new_conv.add_result(res)
                     if new_conv.ref == target_quantity:
                         return new_conv
                 except QuantityRequired:  # if we don't have a reverse qty interface, we can't look for reverse cfs
                     pass
 
-            raise ConversionReferenceMismatch('Flow %s\nfrom %s\nto %s' % (flowable,
+            raise ConversionReferenceMismatch('Flow %s\nfrom %s\nto %s' % (fb,
                                                                            conv.ref,
                                                                            target_quantity))
         return conv
 
     def _quantity_engine(self, fb, rq, qq, cx, locale='GLO',
                          **kwargs):
         """
@@ -674,15 +678,15 @@
     def quantity_relation(self, flowable, ref_quantity, query_quantity, context, locale='GLO',
                           strategy=None, allow_proxy=True, **kwargs):
 
         fb, rq, cx = self._get_flowable_info(flowable, ref_quantity, context)  # call only for exception handling
         qq = self.get_canonical(query_quantity)
 
         if qq == rq:  # is?
-            return QRResult(flowable, rq, qq, context or NullContext, locale, qq.origin, 1.0)
+            return QRResult(flowable, rq, qq, cx, locale, qq.origin, 1.0)
 
         result, mismatch = self._quantity_relation(fb, rq, qq, cx, locale=locale,
                                                    strategy=strategy, allow_proxy=allow_proxy, **kwargs)
         if result is None:
             if len(mismatch) > 0:
                 '''
                 for k in mismatch:
```

### Comparing `antelope_core-0.2.4/antelope_core/implementations/tests/test_quantity.py` & `antelope_core-0.3.0/antelope_core/implementations/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lc_resource.py` & `antelope_core-0.3.0/antelope_core/lc_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,24 +177,26 @@
         print('Created archive of %s containing:' % self._archive)
         self._archive.check_counter()
 
     def make_interface(self, iface):
         return self._archive.make_interface(iface)
 
     def apply_config(self, catalog=None):
-        if len(self._config) == 0:
-            return
+        # if len(self._config) == 0:  # NOW we don't even need to alter blackbook!!!
+        #    return
         print('Applying stored configuration')
-        if catalog is not None:
-            if 'hints' in self._config:
-                catalog.lcia_engine.apply_hints(self._archive.catalog_names, self._config['hints'])
         try:
             self._archive.make_interface('configure').apply_config(self._config)
         except InterfaceError:
             pass
+        # we are moving this below apply_config to allow the archive to add/edit hints, which it can do because
+        # it receives the authentic config dict as an argument
+        if catalog is not None:
+            if 'hints' in self._config:
+                catalog.lcia_engine.apply_hints(self._archive.catalog_names, self._config['hints'])
 
     def remove_interface(self, iface):
         iface = zap_inventory(iface)  # don't warn when interpreting resource specifications
         if iface in self._interfaces:
             self._interfaces.remove(iface)
 
     def add_interface(self, iface):
```

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/__init__.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,19 +101,20 @@
                                          Name=entity['Name'], Indicator=ind)
 
             for k in entity.properties():  # local only for ref
                 q_masq[k] = entity[k]
 
             # print('LciaDb: Adding masquerade %s' % q_masq)
             self.tm.add_quantity(q_masq)
-            assert self.tm.get_canonical(q_masq) is q_masq, 'impostor:%s\noriginal:%s' % (self.tm.get_canonical(q_masq),
-                                                                                          q_masq)
+            cnncl = self.tm.get_canonical(q_masq)
+            # assert self.tm.get_canonical(q_masq) is q_masq, 'impostor:%s\noriginal:%s' % (self.tm.get_canonical(q_masq),
+            #                                                                               q_masq)
             self.tm.add_quantity(entity)  # should turn up as a child
-            assert self.tm.get_canonical(entity) is q_masq, 'child:%s\n masq:%s[%s]' % (self.tm.get_canonical(entity),
-                                                                                        q_masq, q_masq.link)
+            assert self.tm.get_canonical(entity) is cnncl, 'child:%s\n masq:%s[%s]' % (self.tm.get_canonical(entity),
+                                                                                       cnncl, cnncl.link)
 
             if not entity.is_entity:  # not local -- local ones were already imported
                 # print('LciaDb: Importing factors')
                 self.tm.save_for_later(entity)
 
         elif isinstance(entity, FlowInterface):
             self.tm.add_flow(entity, merge_strategy=merge_strategy)
```

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/clookup.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/data/contexts.json` & `antelope_core-0.3.0/antelope_core/lcia_engine/data/contexts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997184684684685%*

 * *Differences: {"'Compartments'": "{35: {'synonyms': {delete: [1]}}}"}*

```diff
@@ -317,15 +317,14 @@
             ]
         },
         {
             "name": "fossil",
             "parent": "from ground",
             "synonyms": [
                 "Fossil fuels",
-                "fossil-",
                 "Non-renewable energy resources from ground",
                 "Crude oil (resource)",
                 "Hard coal (resource)",
                 "Lignite (resource)",
                 "Natural gas (resource)",
                 "Peat (resource)"
             ]
```

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/data/flowables.json` & `antelope_core-0.3.0/antelope_core/lcia_engine/data/flowables.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/data/ipcc_2007_gwp.json` & `antelope_core-0.3.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/lcia_engine.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/lcia_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,16 @@
                 try:
                     self._qm.add_synonym(canonical, term)
                 except TermExists:
                     c = self._qm[canonical]
                     t = self._qm[term]
                     if c is not t:
                         print('!X!X!X!X!X!X!X! conflict when applying hint %s->%s' % (term, canonical))
-                        print('                canonical: %s = ' % c.quantity.link)
-                        print('                extisting: %s = ' % t.quantity.link)
+                        print('                canonical: %s = ' % c.link)
+                        print('                collision: %s = ' % t.link)
                     # assert self._qm[canonical] is self._qm[term]
             elif hint_type == 'flowable':
                 print('Applying flowable hint %s -> %s' % (term, canonical))
                 try:
                     self._fm.add_synonym(canonical, term)
                 except TermExists:
                     assert self._fm[canonical] == self._fm[term]
```

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_biogenic_co2.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_clookup.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_ipcc.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_engine/tests/test_lcia_engine.py` & `antelope_core-0.3.0/antelope_core/lcia_engine/tests/test_lcia_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/lcia_results.py` & `antelope_core-0.3.0/antelope_core/lcia_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from antelope import comp_dir  # , CatalogRef, ExchangeRef
 from .exchanges import ExchangeValue, DissipationExchange
 from .autorange import AutoRange
 from numbers import Number
 from math import isclose
 from collections import defaultdict
 
-#from .models import DetailedLciaResult as DetailedLciaResultModel
+from antelope.models import SummaryLciaScore, DisaggregatedLciaScore, LciaDetail
 # from lcatools.interfaces import to_uuid
 
 
 class InconsistentQuantity(Exception):
     pass
 
 
@@ -47,14 +47,16 @@
     def __init__(self, lc_result, exchange, qrresult):
         """
 
         :param lc_result:
         :param exchange:
         :param qrresult: meets the QRResult spec: has properties 'flowable', 'ref', 'query', 'context', 'locale',
         'origin', 'value'
+        'ref' has to have property 'unit'
+        'context' has to *be* a context (with 'sense')
         """
         if exchange.flow.unit != qrresult.ref.unit and qrresult.value != 0.0:
             print('%s: Inconsistent qty\nexch: %s\nqrr:  %s' % (self.__class__.__name__, exchange.flow.reference_entity, qrresult))
             #  raise InconsistentQuantity('%s\n%s' % (exchange.flow.reference_entity, qrresult))
         self._exchange = exchange
         self._qr = qrresult
         self._lc = lc_result
@@ -144,32 +146,26 @@
                                                   number(self.result * self._lc.autorange),
                                                   cf,
                                                   number(self.value),
                                                   self._qr.locale,
                                                   self.flowable,
                                                   self.context)
 
-    def serialize(self, detailed=False):
-        flowname = self.flow.name
-        if self.exchange.termination is not None:
-            flowname = ', '.join([flowname, self.exchange.termination.name])
-        return {
-            'flow': self.flowable,
-            'context': self.context,
-            'exchange': self.value,
-            'factor': self._qr.value,
-            'result': self.result,
-            'locale': self._qr.locale
-        }
+    def serialize(self):
+        return LciaDetail.from_detailed_lcia_result(self)
 
 
 class SummaryLciaResult(object):
     """
-    like a DetailedLciaResult except omitting the exchange and factor information.  This makes them totally static.
-    The unit_score can itself _be_ an LciaResult, making the datatype recursive.
+    A container for a separately computed Lcia result, *especially* for the results of a fragment LCIA.
+    Includes a node weight and a unit score-- its cumulative result is the product of these.
+    If the unit score is a number, the summary is static.
+
+    However, the unit_score can itself _be_ an LciaResult, making the datatype recursive.
+
     This has __add__ functionality, for merging repeated instances of the same fragment during traversal
     """
     def __init__(self, lc_result, entity, node_weight, unit_score):
         """
         :param lc_result: who "owns" you. scale report by their scale.
         entity_id must either have get_uuid() or be hashable
         :param entity: a hashable identifier
@@ -206,16 +202,25 @@
     def id(self):
         try:
             return self.entity.fragment.external_ref
         except AttributeError:
             try:
                 return self.entity.external_ref
             except AttributeError:
-                return None
+                return str(self.entity)
 
+    @property
+    def origin(self):
+        try:
+            return self.entity.fragment.origin
+        except AttributeError:
+            try:
+                return self.entity.origin
+            except AttributeError:
+                return 'None'
 
     @property
     def static(self):
         return self._static_value is not None
 
     @property
     def is_null(self):
@@ -268,31 +273,23 @@
     def __eq__(self, other):
         if not isinstance(other, SummaryLciaResult):
             return False
         return self.entity == other.entity
 
     def __str__(self):
         return 'S%s = %-s x %-s | %s' % (number(self.cumulative_result * self._lc.autorange), number(self.node_weight),
-                                        number(self.unit_score * self._lc.autorange),
-                                        self.entity)
+                                         number(self.unit_score * self._lc.autorange),
+                                         self.entity)
 
     def show(self):
         if self.static:
             print('%s' % self)
         else:
             self._internal_result.show()
 
-    def details(self):
-        if self.static:
-            yield self
-        else:
-            for k in self._internal_result.keys():
-                for d in self._internal_result[k].details():
-                    yield d
-
     def show_detailed_result(self):
         if self.static:
             self.show()
         else:
             self._internal_result.show_components()
 
     def flatten(self):
@@ -368,50 +365,62 @@
         else:
             print('\n%s' % self)
             print(other)
             raise InconsistentSummaries('At least one not static, and unit scores do not match')
         return SummaryLciaResult(self._lc, self.entity, _node_weight, unit_score)
 
     def serialize(self, detailed=False):
-        j = {
-            'node_weight': self.node_weight,
-            'unit_score': self.unit_score,
-            'result': self.cumulative_result,
-            'component': self.name,
-        }
-        if self.id is not None:
-            j['entity_id'] = self.id
-
+        """
+        If detailed is True, this should return DisaggregatedLciaScores
+        If detailed is False, this should return SummaryLciaScores
+        :param detailed:
+        :return:
+        """
         if detailed:
             if not self.static:
                 f = self.flatten()  # will yield a list of aggregate lcia scores with one component each
-                j['details'] = [d.serialize() for p in f.components() for d in p.details()]
-        return j
+                details = [d.serialize() for p in f.components() for d in p.details()]
+                return DisaggregatedLciaScore(component=self.name, result=self.cumulative_result,
+                                              node_weight=self.node_weight, unit_score=self.unit_score,
+                                              origin=self.origin, entity_id=self.id,
+                                              details=details)
+        return SummaryLciaScore(component=self.name, result=self.cumulative_result,
+                                node_weight=self.node_weight, unit_score=self.unit_score,
+                                origin=self.origin, entity_id=self.id)
 
 
 class SummaryLciaMissing(SummaryLciaResult):
     @property
     def name(self):
         return 'Missing %s' % self.entity
 
     is_null = False
 
     def __str__(self):
         return '%s = %-s x (MISSING)  | %s' % (
             number(self.cumulative_result * self._lc.autorange), number(self.node_weight),
             self.entity)
 
+    def serialize(self, detailed=False):
+        print('serialize SummaryLciaMissing - suspected broken')
+        if detailed:
+            return DisaggregatedLciaScore(component=self.name, result=self.cumulative_result,
+                                          node_weight=self.node_weight, unit_score=self.unit_score,
+                                          origin=self.origin, entity_id=self.id,
+                                          details=[])
+        return SummaryLciaScore(component=self.name, result=self.cumulative_result,
+                                node_weight=self.node_weight, unit_score=self.unit_score,
+                                origin=self.origin, entity_id=self.id)
+
 
-class AggregateLciaScore(object):
+class AggregateLciaResult(object):
     """
-    contains an entityId which should be either a process or a fragment (fragment stages show up as fragments??)
-    The Aggregate score is constructed either from individual LCIA Details (exchange value x characterization factor)
-    or from summary results
+    contains an entityId which could be a process or a fragment (but presents as a process, i.e. with exchanges)
+    The Aggregate score is constructed from individual LCIA Details (exchange value x characterization factor)
     """
-    static = True
 
     def __init__(self, lc_result, entity):
         self.entity = entity
         self._lc = lc_result
         self.LciaDetails = []  # what exactly was having unique membership protecting us from??
 
     def update_parent(self, lc_result):
@@ -484,26 +493,38 @@
         # print('=' * 60)
         # print('             Total score: %g ' % self.cumulative_result)
 
     def __str__(self):
         return 'A%s  %s' % (number(self.cumulative_result * self._lc.autorange), self.entity)
 
     def serialize(self, detailed=False):
+        """
+        If detailed is True, this should return DisaggregatedLciaScores
+        If detailed is False, this should return SummaryLciaScores
+        :param detailed:
+        :return:
+        """
         j = {
             'result': self.cumulative_result,
             'component': self.name
         }
         if hasattr(self.entity, 'external_ref'):
             j['entity_id'] = self.entity.external_ref
+            j['origin'] = self.entity.origin
+        else:
+            j['origin'] = 'None'
+            j['entity_id'] = str(self.entity)
 
         if detailed:
-            if self.static:
-                j['details'] = []
-            j['details'] = [p.serialize(detailed=False) for p in self.LciaDetails]
-        return j
+            j['details'] = [p.serialize() for p in self.LciaDetails]
+            return DisaggregatedLciaScore(**j)
+
+        j['node_weight'] = 1.0
+        j['unit_score'] = j['result']
+        return SummaryLciaScore(**j)
 
 
 def show_lcia(lcia_results):
     """
     Takes in a dict of uuids to lcia results, and summarizes them in a neat table
     :param lcia_results:
     :return:
@@ -519,15 +540,15 @@
     """
     pass
 
 
 class LciaResult(object):
     """
     An LCIA result object contains a collection of LCIA results for a related set of entities, called components.  Each
-     component is an AggregateLciaScore, which itself is a collection of either detailed LCIA results or summary scores.
+     component is an AggregateLciaResult, which itself is a collection of either detailed LCIA results or summary scores.
 
     Each component which is a FragmentFlow represents a specific traversal scenario and is thus static.
 
     Each component which is a process will contain actual exchanges and factors, which are scenario-sensitive, and
      so is (theoretically) dynamic. This is not yet useful in practice.  LCIA Results are in sharp need of testing /
      refactoring.
     """
@@ -638,15 +659,15 @@
         if isinstance(item, int):
             return
     '''
 
     def aggregate(self, key=lambda x: x.fragment['StageName'], entity_id=None):
         """
         returns a new LciaResult object in which the components of the original LciaResult object are aggregated into
-        static values according to a key.  The key is a lambda expression that is applied to each AggregateLciaScore
+        static values according to a key.  The key is a lambda expression that is applied to each AggregateLciaResult
         component's entity property (components where the lambda fails will all be grouped together).
 
         The special key '*' will aggregate all components together.  'entity_id' argument is required in this case to
         provide a distinguishing key for the result (falls back to "aggregated result").
 
         :param key: default: lambda x: x.fragment['StageName'] -- assuming the payload is a FragmentFlow
         :param entity_id: a descriptive string for the entity, to allow the aggregation to be distinguished in
@@ -759,27 +780,27 @@
     def add_component(self, key, entity=None):
         if any(isinstance(c, SummaryLciaResult) for c in self._LciaScores.values()):
             self.show_components()
             raise MixedComponents(key, entity)
         if entity is None:
             entity = key
         if key not in self._LciaScores.keys():
-            self._LciaScores[key] = AggregateLciaScore(self, entity)
+            self._LciaScores[key] = AggregateLciaResult(self, entity)
 
     def add_score(self, key, exchange, qrresult):
         if qrresult.query != self.quantity:
             raise InconsistentQuantity('%s\nqrresult.quantity: %s\nself.quantity: %s' % (qrresult,
                                                                                          qrresult.query,
                                                                                          self.quantity))
         if key not in self._LciaScores.keys():
             self.add_component(key)
         self._LciaScores[key].add_detailed_result(exchange, qrresult)
 
     def add_summary(self, key, entity, node_weight, unit_score):
-        if any(isinstance(c, AggregateLciaScore) for c in self._LciaScores.values()):
+        if any(isinstance(c, AggregateLciaResult) for c in self._LciaScores.values()):
             self.show_components()
             raise MixedComponents
         summary = SummaryLciaResult(self, entity, node_weight, unit_score)
         if key in self._LciaScores.keys():
             # raise DuplicateResult('Key %s is already present' % key)
             '''
             tgt = self._LciaScores[key]
@@ -791,15 +812,15 @@
                                                                                  tgt.entity,
                                                                                  tgt.node_weight, tgt.unit_score,
                                                                                  entity,
                                                                                  node_weight, uss))
             '''
             try:
                 self._LciaScores[key] += summary
-            except TypeError:  # AggregateLciaScore doesn't know how to add-- summary takes over
+            except TypeError:  # AggregateLciaResult doesn't know how to add-- summary takes over
                 summary += self._LciaScores[key]
                 self._LciaScores[key] = summary
             except InconsistentSummaries:
                 self._failed.append(summary)
         else:
             self._LciaScores[key] = summary
 
@@ -1013,28 +1034,28 @@
         """
         '''
         Further explanation:
          we are dis-aggregating our own internal score and re-aggregating it by terminal nodes.  aggs is a dictionary
          that maps the terminal node to the component, and scores maps the terminal node to the cumulative *weight* of 
          the terminal node.  Why we called it 'scores' is unclear.
          Procedure: we go through our components and for each:
-          - If it is an AggregateLciaScore (i.e. a true LCIA computation), then it becomes a terminal node
+          - If it is an AggregateLciaResult (i.e. a true LCIA computation), then it becomes a terminal node
           - If it is a static Summary, then we can't disaggregate and it also becomes a terminal node
           - If it is a dynamic summary, we recurse on it, and we take its terminal nodes and parse them out.
         For this to work, each terminal node must have the same unit score. 
         
         If we find non-matching scores for the same terminal node, we suffix the name and make a new component.
         This could happen if: two different fragments use the same process, but one is derived from an lci() and the 
         other is from a sys_lci() with a subtracted flow.  So naturally their scores are different.. No easy way to
         deal with that.... we just incrementally create new keys ("hunt for a distinct name...")
         '''
         aggs = dict()
         scores = defaultdict(float)
         for c in self.components():
-            if isinstance(c, AggregateLciaScore):
+            if isinstance(c, AggregateLciaResult):
                 # base case
                 if c.entity in aggs:
                     if aggs[c.entity].cumulative_result != c.cumulative_result:
                         raise KeyError(c)
                 else:
                     aggs[c.entity] = c
                 scores[c.entity] += weight
@@ -1141,8 +1162,15 @@
         if bal_idx is not None:
             results[bal_idx] = balance
             return results, 0.0
         else:
             return results, balance
 
     def serialize_components(self, detailed=False):
-        return [c.serialize(detailed=detailed) for c in sorted(self.components(), key=lambda x: x.result, reverse=True)]
+        """
+        If detailed is True, this should return DisaggregatedLciaScores
+        If detailed is False, this should return SummaryLciaScores
+        :param detailed:
+        :return:
+        """
+        return [c.serialize(detailed=detailed) for c in sorted(self.components(), key=lambda x: x.cumulative_result,
+                                                               reverse=True)]
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/__init__.py` & `antelope_core-0.3.0/antelope_core/providers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     from .ecospold import EcospoldV1Archive
 
     _prov = ['IlcdArchive', 'IlcdLcia', 'EcospoldV2Archive', 'EcospoldV1Archive']
 except ImportError:
     _prov = []
 
 from .ecoinvent_lcia import EcoinventLcia
-from .openlca import OpenLcaJsonLdArchive
+from .openlca import OpenLcaRefData,OpenLcaJsonLdArchive
 from .traci import Traci21Factors
 from .xdb_client import XdbClient
 
-PROVIDERS = _prov + ['EcoinventLcia', 'OpenLcaJsonLdArchive', 'Traci21Factors', 'XdbClient']
+PROVIDERS = _prov + ['EcoinventLcia', 'OpenLcaJsonLdArchive', 'Traci21Factors', 'XdbClient', 'OpenLcaRefData']
 
 ''' # this has all been folded into archive.__init__
 class ArchiveError(Exception):
     pass
 
 
 def create_archive(source, ds_type, catalog=None, **kwargs):
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx` & `antelope_core-0.3.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx` & `antelope_core-0.3.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ecoinvent_lcia.py` & `antelope_core-0.3.0/antelope_core/providers/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ecospold.py` & `antelope_core-0.3.0/antelope_core/providers/ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ecospold2/ecospold2.py` & `antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ecospold2/ecospold2_index.py` & `antelope_core-0.3.0/antelope_core/providers/ecospold2/ecospold2_index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ecospold2/master_data.py` & `antelope_core-0.3.0/antelope_core/providers/ecospold2/master_data.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/file_store.py` & `antelope_core-0.3.0/antelope_core/providers/file_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd.py` & `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd_flowables.py` & `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_flowables.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/ilcd_lcia.py` & `antelope_core-0.3.0/antelope_core/providers/ilcd/ilcd_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/quantity.py` & `antelope_core-0.3.0/antelope_core/providers/ilcd/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/ilcd/tests/test_ilcd.py` & `antelope_core-0.3.0/antelope_core/providers/ilcd/tests/test_ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/openlca/openlca_jsonld.py` & `antelope_core-0.3.0/antelope_core/providers/openlca/openlca_jsonld.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/openlca/schema_mapping.py` & `antelope_core-0.3.0/antelope_core/providers/openlca/schema_mapping.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/parse_math.py` & `antelope_core-0.3.0/antelope_core/providers/parse_math.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/tests/test_ecospold.py` & `antelope_core-0.3.0/antelope_core/providers/tests/test_ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/tests/test_xml_widgets.py` & `antelope_core-0.3.0/antelope_core/providers/tests/test_xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/traci/index.py` & `antelope_core-0.3.0/antelope_core/providers/traci/index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/traci/q_info.py` & `antelope_core-0.3.0/antelope_core/providers/traci/q_info.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/traci/quantity.py` & `antelope_core-0.3.0/antelope_core/providers/traci/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/traci/test_traci.py` & `antelope_core-0.3.0/antelope_core/providers/traci/test_traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/traci/traci_2_1_spreadsheet.py` & `antelope_core-0.3.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/xdb_client/implementation.py` & `antelope_core-0.3.0/antelope_core/providers/xdb_client/implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # from collections import defaultdict
 import json
-from antelope import IndexInterface, ExchangeInterface, QuantityInterface, BackgroundInterface
-from antelope import ExchangeRef, RxRef, EntityNotFound, comp_dir
+from antelope import IndexInterface, ExchangeInterface, QuantityInterface, BackgroundInterface, NoFactorsFound
+from antelope import RxRef, EntityNotFound
 from antelope.models import (OriginCount, Entity, FlowEntity, Exchange, ReferenceExchange, UnallocatedExchange,
-                             LciaResult as LciaResultModel, AllocatedExchange, Characterization as CharacterizationModel,
-                             ExchangeValues, DirectedFlow)
+                             LciaResult as LciaResultModel, AllocatedExchange,
+                             Characterization as CharacterizationModel,
+                             ExchangeValues, DirectedFlow, FlowFactors)
 
-from antelope_core.implementations import BasicImplementation
+from antelope_core.implementations import BasicImplementation, ConfigureImplementation
 from antelope_core.lcia_results import LciaResult
-from antelope_core.characterizations import Characterization, QRResult
+from antelope_core.characterizations import QRResult
+from .xdb_entities import XdbReferenceRequired
+
 
 from requests.exceptions import HTTPError
 
 
 class BadClientRequest(Exception):
     pass
 
 
+class XdbConfigureImplementation(ConfigureImplementation):
+    def apply_config(self, config, **kwargs):
+        r_config = self._archive.r.get_raw('config')
+        # no other config needs to be run for now
+        config.update(r_config)
+        super(XdbConfigureImplementation, self).apply_config(config, **kwargs)
+
+
 class RemoteExchange(Exchange):
     @property
     def is_reference(self):
         return self.type == 'reference'
 
 
 class RemoteExchangeValues(ExchangeValues):
@@ -48,28 +59,40 @@
 class XdbImplementation(BasicImplementation, IndexInterface, ExchangeInterface, QuantityInterface, BackgroundInterface):
     """
     The implementation is very thin, so pile everything into one class
     """
     def setup_bm(self, query):
         return True
 
+    def get(self, external_ref, origin=None, **kwargs):
+        return self._archive.retrieve_or_fetch_entity(external_ref, origin=origin, **kwargs)
+
     def get_reference(self, key):
         p = self.get(key)
         if p.entity_type == 'process':
-            rs = self._archive.r.get_many(ReferenceExchange, _ref(key), 'references')
-            return [RxRef(p, self.get(r.flow.external_ref), r.direction, comment=r.comment) for r in rs]
+            try:
+                rs = p.ref.get(p.ref.reference_field)
+            except XdbReferenceRequired:
+                rs = None
+            if rs is None:
+                rs = self._archive.r.get_many(ReferenceExchange, _ref(key), 'references')
+            return [RxRef(p, self._archive.get_or_make(r.flow), r.direction, comment=r.comment) for r in rs]
         elif p.entity_type == 'flow':
             return self._archive.r.get_one(Entity, _ref(key), 'reference')
         elif p.entity_type == 'quantity':
             return self._archive.r.get_one(str, _ref(key), 'reference')
         else:
             raise TypeError(p.entity_type)
 
     def properties(self, external_ref, **kwargs):
-        return self._archive.r.get_many(str, _ref(external_ref), 'properties')
+        the_ref = self.get(external_ref, **kwargs)
+        props = self._archive.r.get_one(dict, _ref(external_ref), 'properties')
+        for k, v in props.items():
+            the_ref[k] = v
+            yield k
 
     def get_item(self, external_ref, item):
         try:
             return self._archive.r.get_raw(_ref(external_ref), 'doc', item)
         except HTTPError as e:
             if e.args[0] == 404:
                 raise KeyError(external_ref, item)
@@ -94,23 +117,31 @@
         :param kwargs:
         :return:
         """
         return sum(k.count[entity_type] for k in self._archive.r.get_many(OriginCount, 'count'))
 
     def processes(self, **kwargs):
         llargs = {k.lower(): v for k, v in kwargs.items()}
-        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'process', **llargs)]
+        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'processes', **llargs)]
 
     def flows(self, **kwargs):
         llargs = {k.lower(): v for k, v in kwargs.items()}
-        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(FlowEntity, 'flow', **llargs)]
+        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(FlowEntity, 'flows', **llargs)]
 
     def quantities(self, **kwargs):
         llargs = {k.lower(): v for k, v in kwargs.items()}
-        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'quantity', **llargs)]
+        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'quantities', **llargs)]
+
+    def lcia(self, **kwargs):
+        llargs = {k.lower(): v for k, v in kwargs.items()}
+        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'lcia', **llargs)]
+
+    def lcia_methods(self, **kwargs):
+        llargs = {k.lower(): v for k, v in kwargs.items()}
+        return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, 'lcia_methods', **llargs)]
 
     def contexts(self, **kwargs):
         return self._archive.tm.contexts(**kwargs)
 
     def get_context(self, term, **kwargs):
         if isinstance(term, list) or isinstance(term, tuple):
             return self._archive.tm.get_context(term[-1])
@@ -119,27 +150,27 @@
     def targets(self, flow, direction=None, **kwargs):
         return [self._archive.get_or_make(k) for k in self._archive.r.get_many(Entity, _ref(flow), 'targets')]
 
     '''
     Exchange routes
     '''
     def _resolve_ex(self, ex):
-        self.get_canonical(ex.flow.quantity_ref)
+        # self.get_canonical(ex.flow.quantity_ref)  # wtf was this for
         ex.flow = self._archive.get_or_make(FlowEntity.from_exchange_model(ex))  # must get turned into a ref with make_ref
 
         if ex.type == 'context':
             ex.termination = self.get_context(ex.context)
         elif ex.type == 'cutoff':
             ex.termination = None
         return ex
 
     def _resolve_exv(self, exv: ExchangeValues):
         exv = self._resolve_ex(exv)
-        if 'null' in exv.values:
-            exv.values[None] = exv.values.pop('null')
+        if 'None' in exv.values:
+            exv.values[None] = exv.values.pop('None')
         return exv
 
     def exchanges(self, process, **kwargs):
         """
         Client code (process_ref.ProcessRef) already turns them into ExchangeRefs
         :param process:
         :param kwargs:
@@ -231,52 +262,29 @@
         dmd = [UnallocatedExchange.from_inv(x).dict() for x in demand]
         return list(self._resolve_ex(ex)  # DWR! THESE ARE NOT OPERATIONAL EXCHANGES YET!!!
                     for ex in self._archive.r.post_return_many(dmd, UnallocatedExchange, 'sys_lci', **kwargs))
 
     '''
     qdb routes
     '''
-    def get_canonical(self, quantity, **kwargs):
-        """
-
-        :param quantity:
-        :param kwargs:
-        :return:
-        """
-        return self._archive.retrieve_or_fetch_entity(quantity, **kwargs)
-
-    def _resolve_cf(self, cf: CharacterizationModel) -> Characterization:
-        """
-
-        :param cf:
-        :return:
-        """
-        rq = self.get_canonical(cf.ref_quantity)
-        qq = self.get_canonical(cf.query_quantity)
-        cx = self.get_context(cf.context)
-        c = Characterization(cf.flowable, rq, qq, cx, origin=cf.origin)
-        for k, v in cf.value.items():
-            c[k] = v
-        return c
-
     def factors(self, quantity, flowable=None, context=None, **kwargs):
         """
         We need to construct operable characterizations with quantities that are recognized by the LciaEngine- in other
         words, with refs from our archive
         :param quantity:
         :param flowable:
         :param context: not implemented at the API
         :param kwargs:
         :return:
         """
         if flowable:
             facs = self._archive.r.get_many(CharacterizationModel, quantity, 'factors', flowable)
         else:
             facs = self._archive.r.get_many(CharacterizationModel, quantity, 'factors')
-        return list(self._resolve_cf(cf) for cf in facs)
+        return list(facs)
 
     def cf(self, flow, quantity, ref_quantity=None, context=None, locale='GLO', **kwargs):
         """
         We still want to retain the ability to ask the remote server for CFs, even if we may prefer to get that
         info locally for local flows
         :param flow:
         :param quantity:
@@ -287,83 +295,89 @@
         :return:
         """
         try:
             return self._archive.r.get_one(float, _ref(flow), 'cf', _ref(quantity), context=context, locale=locale)
         except HTTPError:
             return 0.0
 
+    def quantity_relation(self, flowable, ref_quantity, query_quantity, context, locale='GLO', **kwargs):
+        """
+        not yet implemented
+        :param flowable:
+        :param ref_quantity:
+        :param query_quantity:
+        :param context:
+        :param locale:
+        :param kwargs:
+        :return:
+        """
+        print('quantity_relation not implemented! %s, %s, %s' % (flowable, _ref(ref_quantity), _ref(query_quantity)))
+        raise NoFactorsFound
+
     @staticmethod
     def _result_from_exchanges(quantity, exch_map, res_m: LciaResultModel):
         """
         Constructs a detailed LCIA result using details provided by the backend server, populated with exchanges
         that we provided via POST.
 
         :param quantity:
         :param exch_map:
         :param res_m:
         :return:
         """
         res = LciaResult(quantity, scenario=res_m.scenario, scale=res_m.scale)
-        nodes = set(v.process for v in exch_map.values())
         for c in res_m.components:
-            try:
-                node = next(v for v in nodes if v.external_ref == c.entity_id)
-            except StopIteration:
-                node = c.entity_id
             for d in c.details:
                 key = (d.exchange.external_ref, tuple(d.exchange.context))
-                ex = exch_map[key]
+                try:
+                    ex = exch_map[key]
+                except KeyError:
+                    print('missing key %s,%s' % key)
+                    continue
                 val = d.result / d.factor.value
                 if val != ex.value:
                     print('%s: value mismatch %g vs %g' % (key, val, ex.value))
                 cf = QRResult(d.factor.flowable, ex.flow.reference_entity, quantity, ex.termination,
                               d.factor.locale, d.factor.origin, d.factor.value)
                 res.add_score(c.component, ex, cf)
-            for s in c.summaries:
-                res.add_summary(c.component, node, s.node_weight, s.unit_score)
+        if len(res_m.summaries) > 0:
+            print('Ignoring spurious summaries:')
+            for s in res_m.summaries:
+                print(s)
+        # the results here shouldn't have any summaries
+        # for s in res_m.summaries:
+        #     res.add_summary(s.component, node, s.node_weight, s.unit_score)
         return res
 
-    def _result_from_model(self, process_ref, quantity, res_m: LciaResultModel):
+    def get_factors(self, quantity, flow_specs, **kwargs):
+    #def _result_from_model(self, process_ref, quantity, res_m: LciaResultModel):
         """
-        Constructs a Detailed LCIA result from a background LCIA query, when we don't have a list of exchanges
-        :param process_ref:
+
         :param quantity:
-        :param res_m:
+        :param flow_specs:
+        :param kwargs:
         :return:
         """
-        res = LciaResult(quantity, scenario=res_m.scenario, scale=res_m.scale)
-        process = self.get(process_ref)
-        res.add_component(process_ref, entity=process)
-        for c in res_m.components:
-            for d in c.details:
-                value = d.result / d.factor.value
-                cx = self.get_context(d.exchange.context)
-                ex = ExchangeRef(process, self.get(d.exchange.external_ref), comp_dir(cx.sense),
-                                 termination=cx, value=value)
-                rq = self.get_canonical(d.exchange.quantity_ref)
-                cf = QRResult(d.factor.flowable, rq, quantity, cx,
-                              d.factor.locale, d.factor.origin, d.factor.value)
-                res.add_score(c.component, ex, cf)
-            for s in c.summaries:
-                res.add_summary(c.component, process, s.node_weight, s.unit_score)
-        return res
+        specs = [fs.dict() for fs in flow_specs]
+        return self._archive.r.origin_post_return_many('qdb', specs, FlowFactors,
+                                                       _ref(quantity), 'flow_specs')
 
     def do_lcia(self, quantity, inventory, locale='GLO', **kwargs):
         """
 
         :param quantity:
         :param inventory:
         :param locale:
         :param kwargs:
         :return:
         """
         exchanges = [UnallocatedExchange.from_inv(x).dict() for x in inventory]
         exch_map = {(x.flow.external_ref, x.term_ref): x for x in inventory}
 
-        ress = self._archive.r.qdb_post_return_many(exchanges, LciaResultModel, _ref(quantity), 'do_lcia')
+        ress = self._archive.r.origin_post_return_many('qdb', exchanges, LciaResultModel, _ref(quantity), 'do_lcia')
         return [self._result_from_exchanges(quantity, exch_map, res) for res in ress]
 
     def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
         """
         We want to override the interface implementation and send a simple request to the backend
         :param process:
         :param query_qty:
@@ -392,8 +406,8 @@
                                                     'lcia', _ref(query_qty), **kwargs)
         except HTTPError as e:
             if e.args[0] == 404:
                 content = json.loads(e.args[1])
                 raise EntityNotFound(content['detail'])
             else:
                 raise
-        return [self._result_from_model(process, query_qty, res) for res in ress]
+        return ress  # [self._result_from_model(process, query_qty, res) for res in ress]
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/xdb_client/requester.py` & `antelope_core-0.3.0/antelope_core/providers/xdb_client/requester.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from antelope.models import ResponseModel, OriginMeta
 from .rest_client import RestClient
 
 
 class XdbRequester(RestClient):
     """
-    A RestClient that encapsulates translating the HTTP responses to Pydantic models
+    A RestClient that encapsulates translating the HTTP responses to Pydantic models.  A token is structurally required
+    but is still None default (will just give 401 unauthorized).  On initialization, queries API_root/origins to
+    determine the set of origins the query knows.
+
+    ref is optional and if supplied, the origin will be automatically prefixed to every query. Escape this behavior
+    by using origin_x routes to supply origin explicitly.
+    (if None, a client will be expected to specify origin in every query
+
+    {{What *is* the difference between .origin and .ref? anyway? why the absurd machinations around catalog_names?
+       ans: something (perhaps superstitious) about provenance- it's about mapping the ref to a 'physical' source }}
+
+    pydantic operations
+    use specified ref as origin
      -get_one
      -get_many
-     -qdb_get_one
-     -qdb_get_many
      -post_return_one
      -post_return_many
+    user supplies origin as a positional parameter
+     -origin_get_one
+     -origin_get_many
+     -origin_post_return_one
+     -origin_post_return_many
     """
     def __init__(self, api_root, ref=None, token=None, quiet=False, **kwargs):
         super(XdbRequester, self).__init__(api_root, token=token, quiet=quiet, **kwargs)
-
-        if ref:
-            # we make a list of all the endpoint's origins that match our ref
-            self._org = ref  # '/'.join([api_root, origin])  # we prepend the API_ROOT now in the parent class
-            self._origins = sorted((OriginMeta(**k) for k in self._get_endpoint(self._org)),
-                                   key=lambda x: len(x.origin))
-        else:
-            # we make a list of all the endpoint's origins- user just has to supply origin as an argument
-            self._org = ''
-            self._origins = sorted((OriginMeta(**k) for origin in self._get_endpoint(api_root, 'origins')
-                                    for k in self._get_endpoint(api_root, origin)),
-                                   key=lambda x: x.origin)
-
-        self._qdb = 'qdb'  # '/'.join([api_root, 'qdb'])  # we prepend the API_ROOT now in the parent class
+        # retrieve origins authorized by this token
+        self._origins = sorted((OriginMeta(**k) for k in self._get_endpoint('origins')),
+                               key=lambda x: x.origin)
+        self._org = ref  # '/'.join([api_root, origin])  # we prepend the API_ROOT now in the parent class
 
     @property
     def origin(self):
         return self._org
 
     @property
     def origins(self):
         """
-        This generates OriginMeta cached from the server for origins granted by our token
+        generates OriginMeta objects obtained by the server when the token was first authenticated
         Returns OriginMeta data-- this should probably include config information !
         :return:
         """
         for org in self._origins:
             yield org
 
     @property
@@ -58,39 +63,42 @@
 
     def get_many(self, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
             return [model(**k) for k in self._get_endpoint(self._org, *args, **kwargs)]
         else:
             return [model(k) for k in self._get_endpoint(self._org, *args, **kwargs)]
 
-    def qdb_get_one(self, model, *args, **kwargs):
-        return model(**self._get_endpoint(self._qdb, *args, **kwargs))
-
-    def qdb_get_many(self, model, *args, **kwargs):
-        return [model(**k) for k in self._get_endpoint(self._qdb, *args, **kwargs)]
+    def origin_get_one(self, model, *args, **kwargs):
+        if issubclass(model, ResponseModel):
+            return model(**self._get_endpoint(*args, **kwargs))
+        else:
+            return model(self._get_endpoint(*args, **kwargs))
 
-    def _post_qdb(self, postdata, *args, **params):
-        return self._post(postdata, self._qdb, *args, **params)
+    def origin_get_many(self, model, *args, **kwargs):
+        if issubclass(model, ResponseModel):
+            return [model(**k) for k in self._get_endpoint(*args, **kwargs)]
+        else:
+            return [model(k) for k in self._get_endpoint(*args, **kwargs)]
 
     def post_return_one(self, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
             return model(**self._post(postdata, self._org, *args, **kwargs))
         else:
             return model(self._post(postdata, self._org, *args, **kwargs))
 
-    def qdb_post_return_one(self, postdata, model, *args, **kwargs):
+    def origin_post_return_one(self, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
-            return model(**self._post_qdb(postdata, *args, **kwargs))
+            return model(**self._post(postdata, *args, **kwargs))
         else:
-            return model(self._post_qdb(postdata, *args, **kwargs))
+            return model(self._post(postdata, *args, **kwargs))
 
     def post_return_many(self, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
             return [model(**k) for k in self._post(postdata, self._org, *args, **kwargs)]
         else:
             return [model(k) for k in self._post(postdata, self._org, *args, **kwargs)]
 
-    def qdb_post_return_many(self, postdata, model, *args, **kwargs):
+    def origin_post_return_many(self, origin, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
-            return [model(**k) for k in self._post_qdb(postdata, *args, **kwargs)]
+            return [model(**k) for k in self._post(postdata, origin, *args, **kwargs)]
         else:
-            return [model(k) for k in self._post_qdb(postdata, *args, **kwargs)]
+            return [model(k) for k in self._post(postdata, origin, *args, **kwargs)]
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/xdb_client/rest_client.py` & `antelope_core-0.3.0/antelope_core/providers/xdb_client/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             if len(toks) == 1:
                 self._token = OAuthToken(token_type='bearer', access_token=token)
             elif len(toks) == 2:
                 self._token = OAuthToken(token_type=toks[0], access_token=toks[1])
             else:
                 raise ValueError('invalid token specification')
         else:
-            raise ValueError('Invalid token type')
+            raise ValueError('Invalid token type %s' % type(token))
         self._s.headers['Authorization'] = self._token.auth
 
     def _upd_save(self, save_credentials):
         """
         Updates the flag indicating whether we are saving credentials. None = do nothing. clears the cache if false.
         :param save_credentials:
         :return:
@@ -165,15 +165,15 @@
         el = time() - t
         self._print('%d [%.2f sec]' % (resp.status_code, el))
         if resp.status_code >= 400:
             raise HTTPError(resp.status_code, resp.content)
         return json.loads(resp.content)
 
     def _get_endpoint(self, route, *args, **params):
-        url = '/'.join(map(str, [route, *args]))
+        url = '/'.join(map(str, filter(None, [route, *args])))
         return self._request('GET', url, params=params)
 
     def get_raw(self, *args, **kwargs):
         return self._get_endpoint(*args, **kwargs)
 
     def get_one(self, model, *args, **kwargs):
         if issubclass(model, BaseModel):
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/xdb_client/xdb_client.py` & `antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from antelope.models import Context as ContextModel, Entity
 from antelope_core.archives import LcArchive, InterfaceError
 from antelope_core.catalog_query import READONLY_INTERFACE_TYPES
 from antelope_core.contexts import ContextManager, NullContext
 
 from .requester import XdbRequester
-from .implementation import XdbImplementation, _ref
+from .implementation import XdbImplementation, XdbConfigureImplementation, _ref
 from .xdb_entities import XdbEntity
 
 from requests.exceptions import HTTPError
 
 
 class XdbTermManager(object):
     def __init__(self, requester: XdbRequester):
@@ -134,47 +134,80 @@
     An XdbClient accesses xdb at a named URL using an access token.
     """
 
     _base_type = XdbEntity
 
     def __init__(self, source, ref=None, token=None, **requester_args):
         self._requester_args = requester_args
-        self._requester = XdbRequester(source, ref, token=token, **self._requester_args)
+        try:
+            self._requester = XdbRequester(source, ref, token=token, **self._requester_args)
+        except HTTPError as e:
+            raise InterfaceError('HTTP Request failed %s, %s' % (e.args[0], e.args[1]))
         if ref is None:
             ref = 'qdb'
         super(XdbClient, self).__init__(source, ref=ref, term_manager=XdbTermManager(self._requester))
 
     def refresh_token(self, new_token):
         self._requester.set_token(new_token)
 
     def refresh_auth(self, new_source, new_token):
-        self._requester = XdbRequester(new_source, new_token, **self._requester_args)
+        self._requester = XdbRequester(new_source, self.ref, token=new_token, **self._requester_args)
         self.tm.update_requester(self._requester)
 
     @property
     def r(self):
         return self._requester
 
     def make_interface(self, iface):
         if iface in READONLY_INTERFACE_TYPES:
             return XdbImplementation(self)
+        elif iface == 'configure':
+            return XdbConfigureImplementation(self)
         raise InterfaceError(iface)
 
+    def _model_to_entity(self, model):
+        entity = self._base_type(model)
+        self._entities[model.link] = entity
+        return entity
+
     def get_or_make(self, model):
         """
         Retrieve or create an entity, when we have already received its model data from the server
         :param model:
         :return:
         """
-        key = model.entity_id
+        key = model.link
         if key in self._entities:
             return self._entities[key]
-        entity = self._base_type(model)
-        self._entities[key] = entity
-        return entity
+        return self._model_to_entity(model)
 
-    def _fetch(self, key, **kwargs):
-        if key in self._entities:
-            return self._entities[key]
-        entity = self._base_type(self._requester.get_one(Entity, _ref(key)))
-        self._entities[key] = entity
-        return entity
+    def __getitem__(self, item):
+        """
+        For cursed reasons, our EntityStore __getitem__ method must return None instead of raising a KeyError
+        :param item:
+        :return:
+        """
+        try:
+            if hasattr(item, 'link'):
+                return self._entities[item.link]
+            return self._entities[item]
+        except KeyError:
+            return None
+
+    def _fetch(self, key, origin=None, **kwargs):
+        # I'm just reimplementing _ref_to_key except in situ  ## EntityStore is whack legacy
+        if hasattr(key, 'link'):
+            link = key.link
+            origin = origin or key.origin
+            key = key.external_ref
+        else:  # anything that has "external_ref" would have "link", right?
+            if origin:
+                link = '/'.join([origin, str(key)])
+            else:
+                link = '/'.join([self.ref, str(key)])
+        if link in self._entities:
+            return self._entities[link]
+        if origin:
+            model = self._requester.origin_get_one(Entity, origin, _ref(key))
+        else:
+            model = self._requester.get_one(Entity, _ref(key))
+        return self._model_to_entity(model)
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/xdb_client/xdb_entities.py` & `antelope_core-0.3.0/antelope_core/providers/xdb_client/xdb_entities.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,21 +26,26 @@
 
         The return objects are immediately used as arguments for BasicQuery.make_ref() or CatalogQuery.make_ref(),
         either of which calls this class's make_ref() with the query as argument.  Then the make_ref() is responsible
         for constructing the fully-featured reference object that is stored in the local archive.
 
         Must supply the pydantic model that comes out of the query, and also the archive that stores the ref
         :param model:
-        :param local:
         """
         assert issubclass(type(model), Entity), 'model is not a Pydantic Entity (%s)' % type(model)
         self._model = model
         self._ref = None
 
     @property
+    def ref(self):
+        if self._ref is None:
+            raise XdbReferenceRequired
+        return self._ref
+
+    @property
     def reference_entity(self):
         raise XdbReferenceRequired
 
     @property
     def entity_type(self):
         return self._model.entity_type
 
@@ -52,33 +57,58 @@
     def external_ref(self):
         return self._model.entity_id
 
     def properties(self):
         for k in self._model.properties:
             yield k
 
+    def __setitem__(self, key, value):
+        if self._ref:
+            self._ref[key] = value
+        self._model.properties[key] = value
+
+    def __getitem__(self, item):
+        if self._ref:
+            return self._ref[item]
+        return self._model.properties[item]
+
     def make_ref(self, query):
         if self._ref is not None:
             return self._ref
 
         args = {k: v for k, v in self._model.properties.items()}
-        if self.entity_type == 'quantity' and 'referenceUnit' in args:
-            args['reference_entity'] = args.pop('referenceUnit')
+        if self.entity_type == 'quantity' and 'unit' in args:
+            args['reference_entity'] = args.pop('unit')
         elif self.entity_type == 'flow':
             if 'referenceQuantity' in args:
                 args['reference_entity'] = query.get(args.pop('referenceQuantity'))
             if isinstance(self._model, FlowEntity):
                 args['context'] = self._model.context
                 args['locale'] = self._model.locale
+                # query._tm.add_context(self._model.context, origin=self._model.origin)  # this is somewhat cursed
         elif self.entity_type == 'process':
             if 'referenceExchange' in args:
                 # we cannot synthesize RxRefs prior to the existence of the ProcessRef. sorry.
-                args['referenceExchange'] = [ReferenceExchange(**k) for k in args.pop('referenceExchange')]
+                rxs = args.pop('referenceExchange')
+                try:
+                    args['referenceExchange'] = [ReferenceExchange(**k) for k in rxs]
+                except TypeError:
+                    print(self.link)
+                    print(rxs)
+                    raise
+
+        if self.origin != query.origin:
+            args['masquerade'] = self.origin
 
         ref = CatalogRef.from_query(self.external_ref, query, self.entity_type, **args)
         if ref.entity_type == 'flow':
             if any(bool(re.search('carbon.dioxide', k, flags=re.I)) for k in ref.synonyms):
                 print('%s ***** CO2' % ref.link)
                 ref.is_co2 = True
 
         self._ref = ref
         return ref
+
+    def has_lcia_engine(self):
+        if self._ref is not None:
+            return self._ref.has_lcia_engine()
+        return False
```

### Comparing `antelope_core-0.2.4/antelope_core/providers/xl_dict.py` & `antelope_core-0.3.0/antelope_core/providers/xl_dict.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/providers/xml_widgets.py` & `antelope_core-0.3.0/antelope_core/providers/xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/tests/test_autorange.py` & `antelope_core-0.3.0/antelope_core/tests/test_autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/tests/test_contexts.py` & `antelope_core-0.3.0/antelope_core/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/tests/test_exchanges.py` & `antelope_core-0.3.0/antelope_core/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core/tests/test_resources.py` & `antelope_core-0.3.0/antelope_core/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.4/antelope_core.egg-info/PKG-INFO` & `antelope_core-0.3.0/antelope_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 Metadata-Version: 2.1
-Name: antelope_core
-Version: 0.2.4
+Name: antelope-core
+Version: 0.3.0
 Home-page: https://github.com/AntelopeLCA/core
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: XML
+Provides-Extra: write_to_excel
 License-File: LICENSE
-Requires-Dist: synonym_dict>=0.2.4
-Requires-Dist: antelope_interface>=0.2.4
-Requires-Dist: xlstools>=0.1.3
-Requires-Dist: python-magic>=0.4.18
-Requires-Dist: requests>=2.25
-Requires-Dist: pydantic>=2.5.0
-Provides-Extra: xml
-Requires-Dist: lxml>=1.2.0; extra == "xml"
-Provides-Extra: write-to-excel
-Requires-Dist: xlsxwriter>=1.3.7; extra == "write-to-excel"
 
 ![](https://travis-ci.com/AntelopeLCA/core.svg?branch=master&status=passed) ![](https://coveralls.io/repos/github/AntelopeLCA/core/badge.svg?branch=master)
 
 # core
 Antelope Catalog - reference implementation.
 
 This repository provides code that enables access to different forms of life cycle
```

### Comparing `antelope_core-0.2.4/antelope_core.egg-info/SOURCES.txt` & `antelope_core-0.3.0/antelope_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
 antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
 antelope_core/providers/openlca/__init__.py
+antelope_core/providers/openlca/olca_accessor.py
+antelope_core/providers/openlca/olca_ref_data.py
 antelope_core/providers/openlca/openlca_jsonld.py
 antelope_core/providers/openlca/schema_mapping.py
 antelope_core/providers/openlca/tests/__init__.py
 antelope_core/providers/openlca/tests/test_olca_ref.py
 antelope_core/providers/tests/__init__.py
 antelope_core/providers/tests/test_ecospold.py
 antelope_core/providers/tests/test_xml_widgets.py
```

### Comparing `antelope_core-0.2.4/setup.py` & `antelope_core-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.3.0'
 
 requires = [
     "synonym_dict>=0.2.4",
-    "antelope_interface>=0.2.4",
+    "antelope_interface>=0.2.3",
     "xlstools>=0.1.3",
     "python-magic>=0.4.18",
     "requests>=2.25",
     "pydantic>=2.5.0"
 ]
 
 # optional: pylzma
 """
 Version History
-0.2.4   2024-04-17 - Remove antelope.ExteriorFlow in favor of antelope.models.ExteriorFlow
 
-0.2.3   2024-03-21 - compatibility release for antelope_interface upgrades and terminology changes
-                     OpenLCA v2 schema handled
-                     lots of cloud work 
+0.3.0   2024-01-05 - 0.3-branch development version, supporting end-user access to vault.lc resources 
+
+# ^ 0.3.* 0.3-branch fork   
+# v 0.2.* main / master for legacy projects
 
 0.2.1   2023-04-10 - xdb passes benchmarks
                      pydantic models moved into interface
                      sys_lci and bg_lcia operational, both locally and remotely
 
 0.2.0   2023-04-07 - "release" virtualize branch. 
                    - Add pydantic models for everything
```

