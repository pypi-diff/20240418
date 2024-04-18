# Comparing `tmp/pywbem-1.7.0.tar.gz` & `tmp/pywbem-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywbem-1.7.0.tar", last modified: Tue Apr 16 05:55:23 2024, max compression
+gzip compressed data, was "pywbem-1.7.1.tar", last modified: Thu Apr 18 09:04:09 2024, max compression
```

## Comparing `pywbem-1.7.0.tar` & `pywbem-1.7.1.tar`

### file list

```diff
@@ -1,1914 +1,1914 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.362347 pywbem-1.7.0/
--rw-r--r--   0 maiera     (501) staff       (20)      883 2024-04-07 12:36:21.000000 pywbem-1.7.0/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    26436 2022-03-09 17:32:21.000000 pywbem-1.7.0/LICENSE.txt
--rw-r--r--   0 maiera     (501) staff       (20)      527 2024-04-16 05:55:07.000000 pywbem-1.7.0/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     7338 2024-04-16 05:55:23.361720 pywbem-1.7.0/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     7476 2024-04-15 16:22:46.000000 pywbem-1.7.0/README.md
--rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-04-16 05:50:04.000000 pywbem-1.7.0/README_PYPI.md
--rwxr-xr-x   0 maiera     (501) staff       (20)     2881 2022-03-30 06:07:15.000000 pywbem-1.7.0/build_moftab.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    13849 2022-11-09 03:23:37.000000 pywbem-1.7.0/mof_compiler
--rw-r--r--   0 maiera     (501) staff       (20)      105 2022-03-09 17:32:21.000000 pywbem-1.7.0/mof_compiler.bat
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.431930 pywbem-1.7.0/pywbem/
--rw-r--r--   0 maiera     (501) staff       (20)     3441 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    10911 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cim_constants.py
--rw-r--r--   0 maiera     (501) staff       (20)    25269 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cim_http.py
--rw-r--r--   0 maiera     (501) staff       (20)   306789 2024-04-15 16:22:46.000000 pywbem-1.7.0/pywbem/_cim_obj.py
--rw-r--r--   0 maiera     (501) staff       (20)   446903 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cim_operations.py
--rw-r--r--   0 maiera     (501) staff       (20)    51216 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cim_types.py
--rw-r--r--   0 maiera     (501) staff       (20)    56118 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cim_xml.py
--rw-r--r--   0 maiera     (501) staff       (20)     1971 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_cliutils.py
--rw-r--r--   0 maiera     (501) staff       (20)    25906 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_exceptions.py
--rw-r--r--   0 maiera     (501) staff       (20)     1685 2022-03-30 06:07:16.000000 pywbem-1.7.0/pywbem/_features.py
--rw-r--r--   0 maiera     (501) staff       (20)    50659 2024-04-15 19:35:13.000000 pywbem-1.7.0/pywbem/_listener.py
--rw-r--r--   0 maiera     (501) staff       (20)    21597 2024-04-07 12:36:21.000000 pywbem-1.7.0/pywbem/_logging.py
--rw-r--r--   0 maiera     (501) staff       (20)   114330 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem/_mof_compiler.py
--rw-r--r--   0 maiera     (501) staff       (20)     2648 2024-04-16 05:55:07.000000 pywbem-1.7.0/pywbem/_moflextab.py
--rw-r--r--   0 maiera     (501) staff       (20)    70070 2024-04-16 05:55:07.000000 pywbem-1.7.0/pywbem/_mofparsetab.py
--rw-r--r--   0 maiera     (501) staff       (20)     3565 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem/_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)    44065 2024-04-15 16:22:46.000000 pywbem-1.7.0/pywbem/_recorder.py
--rw-r--r--   0 maiera     (501) staff       (20)    55199 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_server.py
--rw-r--r--   0 maiera     (501) staff       (20)    29927 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_statistics.py
--rw-r--r--   0 maiera     (501) staff       (20)    63708 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem/_subscription_manager.py
--rw-r--r--   0 maiera     (501) staff       (20)    91345 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_tupleparse.py
--rw-r--r--   0 maiera     (501) staff       (20)    19906 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_tupletree.py
--rw-r--r--   0 maiera     (501) staff       (20)    25988 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem/_units.py
--rw-r--r--   0 maiera     (501) staff       (20)    13309 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)    38042 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem/_valuemapping.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.387934 pywbem-1.7.0/pywbem/_vendor/
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.441364 pywbem-1.7.0/pywbem/_vendor/nocasedict/
--rw-r--r--   0 maiera     (501) staff       (20)    26526 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      294 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     2080 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/_hashable.py
--rw-r--r--   0 maiera     (501) staff       (20)     1432 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/_keyableby.py
--rw-r--r--   0 maiera     (501) staff       (20)    31357 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)     1083 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)      321 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocasedict/_version.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.443851 pywbem-1.7.0/pywbem/_vendor/nocaselist/
--rw-r--r--   0 maiera     (501) staff       (20)    11357 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocaselist/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      191 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocaselist/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    20968 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocaselist/_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      321 2024-04-16 05:55:09.000000 pywbem-1.7.0/pywbem/_vendor/nocaselist/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)     1192 2024-04-16 05:50:04.000000 pywbem-1.7.0/pywbem/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)     2916 2022-11-09 03:23:37.000000 pywbem-1.7.0/pywbem/_warnings.py
--rw-r--r--   0 maiera     (501) staff       (20)     5164 2022-11-09 03:23:37.000000 pywbem-1.7.0/pywbem/config.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.349075 pywbem-1.7.0/pywbem.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     7338 2024-04-16 05:55:21.000000 pywbem-1.7.0/pywbem.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)   111311 2024-04-16 05:55:21.000000 pywbem-1.7.0/pywbem.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-16 05:55:21.000000 pywbem-1.7.0/pywbem.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)     2021 2024-04-16 05:55:21.000000 pywbem-1.7.0/pywbem.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       19 2024-04-16 05:55:21.000000 pywbem-1.7.0/pywbem.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-15 19:37:14.000000 pywbem-1.7.0/pywbem.egg-info/zip-safe
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.456962 pywbem-1.7.0/pywbem_mock/
--rw-r--r--   0 maiera     (501) staff       (20)     2272 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    23345 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem_mock/_baseprovider.py
--rw-r--r--   0 maiera     (501) staff       (20)    13993 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_baserepository.py
--rw-r--r--   0 maiera     (501) staff       (20)    23108 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_dmtf_cim_schema.py
--rw-r--r--   0 maiera     (501) staff       (20)    12337 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem_mock/_inmemoryrepository.py
--rw-r--r--   0 maiera     (501) staff       (20)    38310 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_instancewriteprovider.py
--rw-r--r--   0 maiera     (501) staff       (20)   155063 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem_mock/_mainprovider.py
--rw-r--r--   0 maiera     (501) staff       (20)    10974 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_methodprovider.py
--rw-r--r--   0 maiera     (501) staff       (20)    15051 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_mockmofwbemconnection.py
--rw-r--r--   0 maiera     (501) staff       (20)    14604 2024-04-15 15:44:36.000000 pywbem-1.7.0/pywbem_mock/_namespaceprovider.py
--rw-r--r--   0 maiera     (501) staff       (20)     5969 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_providerdependentregistry.py
--rw-r--r--   0 maiera     (501) staff       (20)    31642 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_providerdispatcher.py
--rw-r--r--   0 maiera     (501) staff       (20)    18747 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_providerregistry.py
--rw-r--r--   0 maiera     (501) staff       (20)    22692 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_resolvermixin.py
--rw-r--r--   0 maiera     (501) staff       (20)    35926 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_subscriptionproviders.py
--rw-r--r--   0 maiera     (501) staff       (20)     2742 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)    83136 2024-04-15 13:04:34.000000 pywbem-1.7.0/pywbem_mock/_wbemconnection_mock.py
--rw-r--r--   0 maiera     (501) staff       (20)     4391 2022-03-30 06:07:16.000000 pywbem-1.7.0/pywbem_mock/config.py
--rw-r--r--   0 maiera     (501) staff       (20)     2405 2024-04-15 15:44:36.000000 pywbem-1.7.0/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2024-04-16 05:55:23.362467 pywbem-1.7.0/setup.cfg
--rw-r--r--   0 maiera     (501) staff       (20)    12189 2024-04-15 19:35:13.000000 pywbem-1.7.0/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     3919 2024-04-08 06:08:13.000000 pywbem-1.7.0/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.460060 pywbem-1.7.0/tests/
--rw-r--r--   0 maiera     (501) staff       (20)     6771 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/README
--rw-r--r--   0 maiera     (501) staff       (20)     1070 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.464160 pywbem-1.7.0/tests/dtd/
--rw-r--r--   0 maiera     (501) staff       (20)    13950 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/dtd/CIM_DTD_V22.dtd
--rw-r--r--   0 maiera     (501) staff       (20)    13093 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/dtd/DSP0203_2.2.0.dtd
--rw-r--r--   0 maiera     (501) staff       (20)    11595 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/dtd/DSP0203_2.3.1.dtd
--rw-r--r--   0 maiera     (501) staff       (20)    13558 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/dtd/DSP0203_2.4.0.dtd
--rw-r--r--   0 maiera     (501) staff       (20)      987 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/elapsed_timer.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.475546 pywbem-1.7.0/tests/end2endtest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/end2endtest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3996 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/es_schema.yml
--rw-r--r--   0 maiera     (501) staff       (20)     4786 2023-01-14 04:26:06.000000 pywbem-1.7.0/tests/end2endtest/es_server.yml
--rw-r--r--   0 maiera     (501) staff       (20)     2031 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/es_vault.yml
--rw-r--r--   0 maiera     (501) staff       (20)    23992 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/end2endtest/test_indications.py
--rw-r--r--   0 maiera     (501) staff       (20)     7212 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/end2endtest/test_operation_timeouts.py
--rw-r--r--   0 maiera     (501) staff       (20)     5095 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/test_profile_generic.py
--rw-r--r--   0 maiera     (501) staff       (20)    11759 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/test_profile_snia_server.py
--rw-r--r--   0 maiera     (501) staff       (20)     6150 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/test_profile_snia_smis.py
--rw-r--r--   0 maiera     (501) staff       (20)     6902 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/test_server.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.480922 pywbem-1.7.0/tests/end2endtest/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/end2endtest/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    34790 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/utils/assertions.py
--rw-r--r--   0 maiera     (501) staff       (20)    21916 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/end2endtest/utils/pytest_extensions.py
--rw-r--r--   0 maiera     (501) staff       (20)    18206 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/end2endtest/utils/utils.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.547051 pywbem-1.7.0/tests/functiontest/
--rw-r--r--   0 maiera     (501) staff       (20)    11990 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/README.md
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/functiontest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    32036 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/associatornames_classes.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    21661 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/associatornames_instances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    14347 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/associators_classes.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    28850 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/associators_instances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)      572 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/clienterror.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     4574 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/closeenumeration.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    48406 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/functiontest/conftest.py
--rw-r--r--   0 maiera     (501) staff       (20)    23888 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/createclass.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    37957 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/createinstance.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     7150 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/deleteclass.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    13606 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/deleteinstance.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     7265 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/deletequalifier.yaml
--rw-r--r--   0 maiera     (501) staff       (20)   145717 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/embeddedinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)   102560 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/embeddedobjectclasses.yaml
--rw-r--r--   0 maiera     (501) staff       (20)   147992 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/embeddedobjectinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    11867 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/enumerateclasses.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    18452 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/enumerateclassnames.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    47962 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/enumerateinstancenames.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    89223 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/enumerateinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    45436 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/enumeratequalifiers.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    28065 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/execquery.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    17687 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/exportindication.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    11027 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/getalltypes.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    36353 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/getclass.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    36600 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/getinstance.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    11665 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/getqualifier.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    23505 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/headers.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    26122 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/invalidexpresponseerror.yaml
--rw-r--r--   0 maiera     (501) staff       (20)   118735 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/invalidresponseerror.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    41218 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/invokemethod.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    25214 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/modifyclass.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    14752 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/modifyinstance.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     9716 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/networkerror.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    14388 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openassociatorinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    15343 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openasssociatorinstancepaths.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    42372 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openenumerateinstancepaths.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    68783 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openenumerateinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    17007 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openqueryinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    30740 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openreferenceinstancepaths.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    20487 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/openreferenceinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    25729 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/pullinstancepaths.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    26501 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/pullinstances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    30945 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/pullinstanceswithpath.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     8132 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/referencenames_classes.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    11530 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/referencenames_instances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     8891 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/functiontest/references_classes.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    26925 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/references_instances.yaml
--rw-r--r--   0 maiera     (501) staff       (20)     9642 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/functiontest/setqualifier.yaml
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.548485 pywbem-1.7.0/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    13097 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.558827 pywbem-1.7.0/tests/leaktest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     5417 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/leaktest/test_leaks_cim_obj.py
--rw-r--r--   0 maiera     (501) staff       (20)      936 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/test_leaks_cim_xml.py
--rw-r--r--   0 maiera     (501) staff       (20)     2218 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/test_leaks_dict.py
--rw-r--r--   0 maiera     (501) staff       (20)     1140 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/test_leaks_elementtree.py
--rw-r--r--   0 maiera     (501) staff       (20)     2482 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/test_leaks_minidom.py
--rw-r--r--   0 maiera     (501) staff       (20)      644 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/leaktest/test_leaks_statistics.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.573211 pywbem-1.7.0/tests/manualtest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/manualtest/__init__.py
--rwxr-xr-x   0 maiera     (501) staff       (20)   276186 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/manualtest/run_cim_operations.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    19059 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/manualtest/run_enum_performance.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    20227 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/manualtest/run_enum_performancesimple.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     1358 2022-03-09 17:42:38.000000 pywbem-1.7.0/tests/manualtest/run_mof_compiler_script.sh
--rwxr-xr-x   0 maiera     (501) staff       (20)    14094 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/manualtest/run_operationtimeouts.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    22302 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/manualtest/run_response_performance.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     7915 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/manualtest/run_uprint.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     1209 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/manualtest/test_uprint.bat
--rwxr-xr-x   0 maiera     (501) staff       (20)     1078 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/manualtest/test_uprint.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.575588 pywbem-1.7.0/tests/perftest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/perftest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     6643 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/perftest/test_indications.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.576668 pywbem-1.7.0/tests/profiles/
--rw-r--r--   0 maiera     (501) staff       (20)    30178 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/profiles/profiles.yml
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.582054 pywbem-1.7.0/tests/resourcetest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     4949 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/memory_utils.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    11084 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/random_objects.py
--rw-r--r--   0 maiera     (501) staff       (20)     1390 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/resource_measurement.py
--rw-r--r--   0 maiera     (501) staff       (20)     2032 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/test_enuminst.py
--rw-r--r--   0 maiera     (501) staff       (20)     3120 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/resourcetest/timers.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.583034 pywbem-1.7.0/tests/schema/
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.589932 pywbem-1.7.0/tests/schema/OpenPegasus/
--rw-r--r--   0 maiera     (501) staff       (20)      203 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/schema/OpenPegasus/PG_Namespace.mof
--rw-r--r--   0 maiera     (501) staff       (20)  1822991 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/schema/cim_schema_2.49.0Final-MOFs.zip
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.594439 pywbem-1.7.0/tests/schema/mofFinal2.49.0/
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.727505 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/
--rw-r--r--   0 maiera     (501) staff       (20)     1611 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_AGPSoftwareFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8097 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_Action.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2026 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ActionSequence.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12333 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1167 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4329 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDirectory.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1053 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemHierarchy.mof
--rw-r--r--   0 maiera     (501) staff       (20)      792 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemSoftwareFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12511 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ArchitectureCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)      741 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_AssociatedAppSystemOverviewStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2920 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2500 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      657 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeatureBIOSElements.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8769 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_Check.mof
--rw-r--r--   0 maiera     (501) staff       (20)      802 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareElements.mof
--rw-r--r--   0 maiera     (501) staff       (20)      804 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareFeatures.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1139 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CopyFileAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      329 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CreateDirectoryAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1361 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DiagnosticTestSoftware.mof
--rw-r--r--   0 maiera     (501) staff       (20)      546 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectoryAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)      629 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecificationFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1176 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DiskSpaceCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)      626 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ExecuteProgram.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1925 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FRUIncludesSoftwareFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      405 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FileAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2480 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FileSpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)      831 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectoryAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      827 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectorySpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2843 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProduct.mof
--rw-r--r--   0 maiera     (501) staff       (20)      794 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProductImage.mof
--rw-r--r--   0 maiera     (501) staff       (20)      695 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledSoftwareElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      303 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeAppClientModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      979 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplication.mof
--rw-r--r--   0 maiera     (501) staff       (20)      645 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationHostedOnServer.mof
--rw-r--r--   0 maiera     (501) staff       (20)      711 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      833 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionFactoryAvailableToJCAResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4411 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionPoolStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3225 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1319 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDeployedObject.mof
--rw-r--r--   0 maiera     (501) staff       (20)      755 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)      941 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJB.mof
--rw-r--r--   0 maiera     (501) staff       (20)      709 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBInModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      312 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      829 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      268 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBean.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1800 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBeanStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1255 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      674 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactoryManagedConnectionFactory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      699 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionPools.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1273 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAManagedConnectionFactory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      702 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCANonpooledConnections.mof
--rw-r--r--   0 maiera     (501) staff       (20)      257 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      326 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      705 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCConnectionPools.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1221 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      540 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSourceDriver.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDriver.mof
--rw-r--r--   0 maiera     (501) staff       (20)      708 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCNonpooledConnections.mof
--rw-r--r--   0 maiera     (501) staff       (20)      333 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      792 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResourceUsesDataSource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      329 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      704 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionSessions.mof
--rw-r--r--   0 maiera     (501) staff       (20)      646 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      561 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConsumerStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2416 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSEndpointStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      589 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSProducerStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      257 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      694 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionConsumers.mof
--rw-r--r--   0 maiera     (501) staff       (20)      694 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionProducers.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2509 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      699 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStatConnections.mof
--rw-r--r--   0 maiera     (501) staff       (20)      330 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      316 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJNDIResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      296 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      892 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2365 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVM.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1826 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVMStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      280 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      528 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5063 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObject.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3385 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObjectCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      283 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBean.mof
--rw-r--r--   0 maiera     (501) staff       (20)      539 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBeanStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      413 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      631 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModuleUsesJVM.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4053 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeNotification.mof
--rw-r--r--   0 maiera     (501) staff       (20)      281 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeRMI_IIOPResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1766 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      947 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      845 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterInModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      354 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      708 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceOnServer.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1097 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServer.mof
--rw-r--r--   0 maiera     (501) staff       (20)      743 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerInDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)      688 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerUsesJVM.mof
--rw-r--r--   0 maiera     (501) staff       (20)      870 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServlet.mof
--rw-r--r--   0 maiera     (501) staff       (20)      729 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletInModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1701 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      337 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBean.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBeanStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      303 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBean.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1114 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBeanStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      305 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatelessSessionBean.mof
--rw-r--r--   0 maiera     (501) staff       (20)      387 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatelessSessionBeanStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2828 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatistic.mof
--rw-r--r--   0 maiera     (501) staff       (20)      257 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      534 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLStats.mof
--rw-r--r--   0 maiera     (501) staff       (20)      308 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeWebModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1145 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_MemoryCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ModifySettingAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2296 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_OSVersionCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)      713 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_OperatingSystemSoftwareFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      608 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ProductSoftwareFeatures.mof
--rw-r--r--   0 maiera     (501) staff       (20)      309 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_RebootAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      592 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_RemoveDirectoryAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      338 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_RemoveFileAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SettingCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9693 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      593 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementActions.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1079 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementChecks.mof
--rw-r--r--   0 maiera     (501) staff       (20)      783 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2679 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementSAPImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2640 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementServiceImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5995 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementVersionCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2557 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      784 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1311 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSAPImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1270 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureServiceImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      726 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSoftwareElements.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3268 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_StatisticalRuntimeOverview.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1185 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SwapSpaceCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)      627 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SystemBIOS.mof
--rw-r--r--   0 maiera     (501) staff       (20)      839 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectoryAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      835 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectorySpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1120 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VersionCompatibilityCheck.mof
--rw-r--r--   0 maiera     (501) staff       (20)      962 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1999 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      710 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeatureVideoBIOSElements.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.937938 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/
--rw-r--r--   0 maiera     (501) staff       (20)     2433 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractBasedOn.mof
--rw-r--r--   0 maiera     (501) staff       (20)      722 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      855 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementAllocatedFromPool.mof
--rw-r--r--   0 maiera     (501) staff       (20)      685 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3394 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ActiveConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1133 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ActsAsSpare.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2310 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AdminDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)      529 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AllocatedLogicalElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5071 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AllocationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9787 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AssociatedPowerManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      943 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_BasedOn.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1080 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_BindsTo.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9889 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Capabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      658 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectedCollections.mof
--rw-r--r--   0 maiera     (501) staff       (20)      691 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectedMSEs.mof
--rw-r--r--   0 maiera     (501) staff       (20)      385 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Collection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2219 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionOfMSEs.mof
--rw-r--r--   0 maiera     (501) staff       (20)      585 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CompatibleProduct.mof
--rw-r--r--   0 maiera     (501) staff       (20)      673 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Component.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2761 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1525 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1099 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponentView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1696 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1834 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12938 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteJob.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2227 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Configuration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1655 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5550 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1277 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationForSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      701 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ContainedDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)      700 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ContainedLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      549 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DefaultSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      648 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Dependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1738 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DependencyContext.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceSAPImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1224 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceServiceImplementation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1663 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      643 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      668 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementAllocatedFromPool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2053 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)      903 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1582 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      586 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3015 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4161 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSoftwareIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1037 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1011 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementView.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13055 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3784 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8934 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EthernetPortAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      966 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ExtentRedundancyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ExtraCapacityGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2588 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_FRU.mof
--rw-r--r--   0 maiera     (501) staff       (20)      945 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_FRUIncludesProduct.mof
--rw-r--r--   0 maiera     (501) staff       (20)      495 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_FRUPhysicalElements.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1963 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_GroupSynchronized.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1045 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedAccessPoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      867 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      608 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)      777 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedResourcePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1165 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2622 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ImplementationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      802 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_InstalledSoftwareIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2106 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_IsSpare.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13830 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Job.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6288 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_JobCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      982 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13309 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10010 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5112 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LocalizationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1152 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Location.mof
--rw-r--r--   0 maiera     (501) staff       (20)    24725 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      545 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDeviceView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      405 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1981 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7549 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ManagedElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)    19314 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ManagedSystemElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      569 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_MemberOfCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3232 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_MethodParameters.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2609 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4565 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    21957 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2182 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2250 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1921 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedMemberOfCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      745 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OwningCollectionElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      848 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ParameterValueSources.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1436 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ParametersForMethod.mof
--rw-r--r--   0 maiera     (501) staff       (20)    59947 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalComputerSystemView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6729 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      673 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElementLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1318 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      675 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12080 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6878 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17336 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProcessorAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3844 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Product.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1906 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      650 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductElementComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      743 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductFRU.mof
--rw-r--r--   0 maiera     (501) staff       (20)      616 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductParentChild.mof
--rw-r--r--   0 maiera     (501) staff       (20)      695 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1162 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalElements.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1134 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductProductDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1484 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductServiceComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      679 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductSoftwareComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      724 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductSupport.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4183 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Profile.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13005 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9007 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      672 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2015 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesServiceToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      597 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RawMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      633 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Realizes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1234 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2355 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7942 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancySet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3348 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedElementCausingError.mof
--rw-r--r--   0 maiera     (501) staff       (20)      691 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      579 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1515 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RemotePort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4157 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RemoteServiceAccessPoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      710 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ReplaceableProductFRU.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2952 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ReplacementFRU.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15008 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourceAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8977 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2023 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11133 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      976 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPAvailableForElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      966 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPSAPDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1682 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      664 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      655 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1031 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1094 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedView.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10703 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Service.mof
--rw-r--r--   0 maiera     (501) staff       (20)      871 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessBySAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1545 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessPoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessURI.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6425 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1278 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElementWithQuota.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1229 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAvailableToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      634 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      827 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceSAPDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2746 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceServiceDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1646 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      636 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)    24294 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Setting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2154 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingContext.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8246 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      616 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingForSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7755 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1242 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineState.mof
--rw-r--r--   0 maiera     (501) staff       (20)    23368 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15494 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9537 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2915 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SpareGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      948 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Spared.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5458 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      920 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1239 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      583 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Statistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1217 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticsCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12473 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    23895 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3045 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancyGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1694 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancySet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1941 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SupportAccess.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13084 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Synchronized.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5109 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_System.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1665 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2351 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)      728 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      852 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemDeviceView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      800 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemPackaging.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1420 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSettingContext.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2992 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSpecificCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1289 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      629 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1804 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_TimeService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_View.mof
--rw-r--r--   0 maiera     (501) staff       (20)      635 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ViewOnSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2971 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualEthernetSwitchSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3501 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11315 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1428 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4322 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1960 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2287 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VisibleMemory.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:21.954937 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/
--rw-r--r--   0 maiera     (501) staff       (20)      652 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_AssociatedDatabaseSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4016 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabase.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1678 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1721 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      547 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1183 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseAdministrator.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseControlFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      923 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1666 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseParameter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1698 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseResourceStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3174 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegment.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3498 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegmentSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3203 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5293 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseServiceStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1045 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1424 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorageArea.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1458 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1154 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_SNMPDatabaseParameter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2372 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_ServiceAvailableToDatabase.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.377042 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/
--rw-r--r--   0 maiera     (501) staff       (20)     2337 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ADSLModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3809 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AGPVideoController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      467 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ATAInitiatorTargetLogicalUnitPath.mof
--rw-r--r--   0 maiera     (501) staff       (20)      579 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ATAPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2495 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AbstractProtocolControllerForDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      713 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AccessLabelReader.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1661 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AdapterActiveConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3153 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AdvancedStorageSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1778 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1247 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1017 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnAggregatePExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      997 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnPExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1053 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregateRedundancyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5600 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1875 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDeviceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2735 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2006 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1426 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolViewView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2008 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedResources.mof
--rw-r--r--   0 maiera     (501) staff       (20)      662 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedAlarm.mof
--rw-r--r--   0 maiera     (501) staff       (20)      775 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBattery.mof
--rw-r--r--   0 maiera     (501) staff       (20)      916 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBlockStatisticsManifestCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6670 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCacheMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1066 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedComponentExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      639 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCooling.mof
--rw-r--r--   0 maiera     (501) staff       (20)      638 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedDeviceMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1176 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedElementTier.mof
--rw-r--r--   0 maiera     (501) staff       (20)      740 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedIndicatorLED.mof
--rw-r--r--   0 maiera     (501) staff       (20)      613 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedInitiatorMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      712 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedLabelReader.mof
--rw-r--r--   0 maiera     (501) staff       (20)      683 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      658 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      669 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProcessorMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      896 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProtocolController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1100 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedRemainingExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      701 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedResourcePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)      675 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1430 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyCurrentSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1426 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyVoltageSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)      617 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedTargetMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2644 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AsymmetricAccessibility.mof
--rw-r--r--   0 maiera     (501) staff       (20)      814 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BIOSLoadedInNV.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1611 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BasedOnView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7658 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Battery.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1352 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BinarySensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5963 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16190 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1348 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifestCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15507 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10568 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStorageStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      300 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CDROMDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)      308 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CableModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5544 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CacheMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10184 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CallBasedModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1503 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ChangerDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      685 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CollectionOfSensors.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1075 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4386 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtentBasedOn.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1173 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1209 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemProcessor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5728 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ConfigurationReportingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1055 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ConnectionBasedModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2544 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ControlledBy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3114 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Controller.mof
--rw-r--r--   0 maiera     (501) staff       (20)    46492 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ControllerConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      459 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CoolingDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3539 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CurrentSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)      376 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DSLModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1213 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DVDDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DesktopMonitor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1804 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3840 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorCounts.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2073 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1396 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1364 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1794 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceServicesLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSharingCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2382 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSoftware.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1509 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiscreteSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2558 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9274 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskDriveView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      891 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5728 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      862 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionBasedOnVolume.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2994 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6604 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      306 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DisketteDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)      304 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Display.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3844 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DisplayController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2220 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Door.mof
--rw-r--r--   0 maiera     (501) staff       (20)      971 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      671 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToPhysicalElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      832 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DriveComponentViewView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      646 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DriveInDiskGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      251 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ESCONController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      878 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ElementStatisticalDataView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      649 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ElementStorageProtectionSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      705 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ErrorCountersForDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14648 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7180 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8707 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      829 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ExtentComponentView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      751 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ExtentInDiskGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCActiveConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5244 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCAdapterEventCounters.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14817 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2304 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2780 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortRateStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2343 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10378 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2310 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2010 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4377 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCTopologyView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      544 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FailoverStorageExtentsCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4093 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Fan.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16147 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibreChannelAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11617 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7332 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortActiveLogin.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4346 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortEventCounters.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1256 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortOnFCAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      504 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibreProtocolService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1978 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemGroupSynchronized.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15133 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    57887 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8796 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemSynchronized.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1723 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FlatPanel.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1661 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GPTDiskPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1572 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GenericDiskPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      724 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupInDiskGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6786 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13492 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      437 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HDSLModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2446 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HardwareThread.mof
--rw-r--r--   0 maiera     (501) staff       (20)      266 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HeatPipe.mof
--rw-r--r--   0 maiera     (501) staff       (20)      784 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)      803 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePoolView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1713 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IBSubnetManager.mof
--rw-r--r--   0 maiera     (501) staff       (20)      247 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IDEController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      322 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ISDNModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8447 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLED.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4813 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLEDCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      265 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InfraredController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2598 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorTargetLogicalUnitPath.mof
--rw-r--r--   0 maiera     (501) staff       (20)      810 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InstalledPartitionTable.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1669 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InterLibraryPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1072 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Keyboard.mof
--rw-r--r--   0 maiera     (501) staff       (20)    26624 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5396 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1776 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReader.mof
--rw-r--r--   0 maiera     (501) staff       (20)      780 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1848 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      982 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LibraryExchange.mof
--rw-r--r--   0 maiera     (501) staff       (20)      751 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LibraryPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2546 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LimitedAccessPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4298 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDisk.mof
--rw-r--r--   0 maiera     (501) staff       (20)      888 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1414 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      774 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolume.mof
--rw-r--r--   0 maiera     (501) staff       (20)      692 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolumeSet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2463 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2758 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)      878 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1429 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1651 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1191 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      318 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MagnetoOpticalDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)      337 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ManagementController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6859 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MappingProtocolControllerView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      904 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3258 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingExposedDeviceView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6469 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingView.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11413 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1831 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3236 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2885 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      906 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaPresent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      391 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaTransferDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8502 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Memory.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2896 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4590 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2000 2024-03-11 18:16:46.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3298 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6354 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryError.mof
--rw-r--r--   0 maiera     (501) staff       (20)      288 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Modem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ModulePort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2998 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MonitorResolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)      623 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MonitorSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      256 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MultiStateSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4282 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapterRedundancyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3953 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1891 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1455 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1222 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1404 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkVirtualAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2444 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NonVolatileStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17045 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NumericSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)      751 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1341 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      770 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5259 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1236 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifestCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2019 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2610 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9699 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1435 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OwningPrintQueue.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5177 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIBridge.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5367 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2709 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      641 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)      355 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIPortGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      598 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIeSwitch.mof
--rw-r--r--   0 maiera     (501) staff       (20)      252 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCMCIAController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCVideoController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1050 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PExtentRedundancyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5890 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_POTSModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1553 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PSExtentBasedOnPExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1098 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageAlarm.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1266 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageCooling.mof
--rw-r--r--   0 maiera     (501) staff       (20)      765 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1007 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageTempSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2120 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ParallelController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6669 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PassThroughModule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1934 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2667 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      521 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespace.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2446 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespaceSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4008 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PhysicalExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1570 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      819 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerForChanger.mof
--rw-r--r--   0 maiera     (501) staff       (20)      704 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerLabelReader.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1012 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2144 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1531 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PointingDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1035 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortActiveConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1480 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      921 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortImplementsEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      548 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortOnDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4896 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerAllocationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1386 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerSource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8530 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerSupply.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1281 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3227 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      614 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PoweredStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14294 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintInputTray.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10421 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintInterpreter.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16592 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintJob.mof
--rw-r--r--   0 maiera     (501) staff       (20)      618 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintJobFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11200 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintMarker.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9040 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintQueue.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1490 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9679 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13255 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintSupply.mof
--rw-r--r--   0 maiera     (501) staff       (20)    41074 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Printer.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5050 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      560 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingJob.mof
--rw-r--r--   0 maiera     (501) staff       (20)      661 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingQueue.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9362 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Processor.mof
--rw-r--r--   0 maiera     (501) staff       (20)      867 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2964 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCore.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2890 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedExtentBasedOn.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2407 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedSpaceExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      710 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2546 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerAccessesUnit.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2369 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      839 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2415 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnit.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnitView.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17354 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerMaskingCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4889 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueryStatisticsCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      850 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueueForPrintService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      670 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueueForwardsToPrintSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1288 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizedOnSide.mof
--rw-r--r--   0 maiera     (501) staff       (20)      993 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesAggregatePExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1178 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesDiskPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1276 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      969 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesPExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      704 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesTapePartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      276 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Refrigeration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RemoteReplicationCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RemoteResources.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16317 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPairView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      956 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPoolForStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4653 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationEntity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2638 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)   128552 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)   117170 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16588 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1584 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SASPHY.mof
--rw-r--r--   0 maiera     (501) staff       (20)      565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SASPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2022 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SBProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1704 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIArbitraryLogicalUnit.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2986 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3575 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInitiatorTargetLogicalUnitPath.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4807 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInterface.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10438 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5062 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7724 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIPathConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIProtocolController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7797 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSITargetPortGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      374 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SDSLModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      295 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SSAController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      262 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Scanner.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5533 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Sensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2532 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SerialController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1643 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SerialInterface.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4823 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SharedDeviceManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4182 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SharingDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2570 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Snapshot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1113 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SnapshotOfExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3688 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11151 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1329 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      590 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    22826 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    24631 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    53704 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      753 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageDefect.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7281 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17467 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementDriveDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1117 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1780 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      738 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1347 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageError.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5591 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibrary.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1135 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibraryCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17395 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePool.mof
--rw-r--r--   0 maiera     (501) staff       (20)      995 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      939 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2326 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12366 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2092 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProcessorAffinity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1792 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4582 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2649 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15541 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageRelocationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    18051 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageReplicationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1246 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageResourceLoadGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4497 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageServerAsymmetryCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    33857 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2923 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingWithHints.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1399 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsAssociatedToCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2117 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsGeneratedFromCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9144 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSynchronized.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3409 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageTier.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3371 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageTierCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7330 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageVolume.mof
--rw-r--r--   0 maiera     (501) staff       (20)      852 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SuppliesPower.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6097 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SynchronizationAspect.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1775 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SystemRegistrationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1054 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Tachometer.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapeDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)      470 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapeDriveResourceUsage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1287 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapePartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      790 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapePartitionOnSurface.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1368 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TargetMaskingGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1636 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TargetPortGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3459 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TemperatureSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4792 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13151 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6505 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6702 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15988 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5569 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6666 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      587 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1481 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBController.mof
--rw-r--r--   0 maiera     (501) staff       (20)      638 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBControllerHasHub.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9018 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      792 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBHub.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1913 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)      610 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBPortOnHub.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12242 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Unimodem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4697 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_UninterruptiblePowerSupply.mof
--rw-r--r--   0 maiera     (501) staff       (20)      586 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_UserDevice.mof
--rw-r--r--   0 maiera     (501) staff       (20)      384 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VDSLModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10011 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLResourceUsage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1485 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    24235 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2101 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTOCDiskPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6015 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoController.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4133 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoControllerResolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3298 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoHead.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3382 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoHeadResolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)      983 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      867 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ViewCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1157 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolatileStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3373 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VoltageSensor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2802 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1757 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSetBasedOnPSExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14567 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeView.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5249 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WBEMServerDeviceRegistrationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      298 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WORMDrive.mof
--rw-r--r--   0 maiera     (501) staff       (20)      726 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnModem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      743 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3818 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Watchdog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2654 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1237 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13391 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1383 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiRadio.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2436 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Zone.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2514 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1482 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneMembershipSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    19989 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1186 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneSet.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.405784 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/
--rw-r--r--   0 maiera     (501) staff       (20)    10175 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AbstractIndicationSubscription.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16025 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AlertIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1056 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AlertInstIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)      288 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassCreation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      286 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassDeletion.mof
--rw-r--r--   0 maiera     (501) staff       (20)      829 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)      722 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassModification.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2938 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      773 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollectionSubscription.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5261 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FormattedIndicationSubscription.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11244 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_Indication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9189 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationFilter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      825 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandler.mof
--rw-r--r--   0 maiera     (501) staff       (20)      827 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandlerCIMXML.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3418 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3119 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3689 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1222 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationSubscription.mof
--rw-r--r--   0 maiera     (501) staff       (20)      267 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstCreation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      273 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstDeletion.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1402 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2702 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstMethodCall.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1560 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstModification.mof
--rw-r--r--   0 maiera     (501) staff       (20)      277 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstRead.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4499 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestination.mof
--rw-r--r--   0 maiera     (501) staff       (20)      702 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationCIMXML.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4901 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationWSManagement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ProcessIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6625 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_SNMPTrapIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1575 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ThresholdIndication.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.430582 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/
--rw-r--r--   0 maiera     (501) staff       (20)     1705 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedProposal.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1976 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedTransform.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3506 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7502 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEProposal.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2021 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKERule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4332 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1227 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1356 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      526 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecProposal.mof
--rw-r--r--   0 maiera     (501) staff       (20)      378 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecRule.mof
--rw-r--r--   0 maiera     (501) staff       (20)      375 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTransportAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      874 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTunnelAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1040 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PacketConditionInSARule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForPreconfiguredTunnel.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForTunnel.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2884 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredSAAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      574 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTransportAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1065 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTunnelAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      690 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_RuleThatGeneratedSA.mof
--rw-r--r--   0 maiera     (501) staff       (20)      808 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3268 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SANegotiationAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1125 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAProposal.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1664 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SARule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1700 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAStaticAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2293 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_TransformOfPreconfiguredAction.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.463532 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/
--rw-r--r--   0 maiera     (501) staff       (20)     6105 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMOMStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      887 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5780 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCommunicationMechanism.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1230 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForManager.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1317 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForObjectManagerAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1043 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ElementConformsToProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)    19379 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Error.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4805 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_GenericOperationCapabilitiesStructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)      720 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_IdentificationOfManagedSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2785 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Message.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4764 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Namespace.mof
--rw-r--r--   0 maiera     (501) staff       (20)      879 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_NamespaceInManager.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3807 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManager.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3433 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7932 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerCommunicationMechanism.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2132 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ProtocolAdapter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3315 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_QueryCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      641 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      773 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedSpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15774 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6997 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSpecification.mof
--rw-r--r--   0 maiera     (501) staff       (20)      485 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSubProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1449 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SchemaInformationStructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)      980 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SubProfileRequiresProfile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3807 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SystemIdentification.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1836 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SystemInNamespace.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1959 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMProtocolServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2370 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServer.mof
--rw-r--r--   0 maiera     (501) staff       (20)      721 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3343 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerNamespace.mof
--rw-r--r--   0 maiera     (501) staff       (20)      565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      857 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WSManagementCapabilities.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.486258 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/
--rw-r--r--   0 maiera     (501) staff       (20)     2572 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricDefinition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1669 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricValue.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10859 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricDefinition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7001 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricValue.mof
--rw-r--r--   0 maiera     (501) staff       (20)      851 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementPerformsUoW.mof
--rw-r--r--   0 maiera     (501) staff       (20)      898 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementUnitOfWorkDef.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1706 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefForME.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefinition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      613 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricForME.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1089 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricInstance.mof
--rw-r--r--   0 maiera     (501) staff       (20)    28010 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6084 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      672 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_StartedUoW.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1458 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoW.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1181 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoWDef.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5035 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_TraceLevelType.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6450 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWork.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2998 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWorkDefinition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      916 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWDefTraceLevelType.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetric.mof
--rw-r--r--   0 maiera     (501) staff       (20)      948 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetricDefinition.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.772399 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/
--rw-r--r--   0 maiera     (501) staff       (20)     1150 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AFRelatedServices.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2601 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AFService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2037 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AHTransform.mof
--rw-r--r--   0 maiera     (501) staff       (20)      791 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ASBGPEndpoints.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1817 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ATAProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3752 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AdministrativeDistance.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2773 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AllocationSchedulingElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1403 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AreaOfConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)      914 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AssociatedNextHop.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5316 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AutonomousSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1326 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AverageRateMeterService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      862 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAdminDistance.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4460 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1915 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributesForRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1242 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPCluster.mof
--rw-r--r--   0 maiera     (501) staff       (20)      695 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPClustersInAS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3109 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPEndpointStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPIPRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6647 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPathAttributes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3872 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      657 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroupService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1067 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerUsesRouteMap.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9078 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4194 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMap.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1085 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMapsInRoutingPolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)      689 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRoutingPolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3063 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1213 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceAttributes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1096 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3677 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1111 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BindsToLANEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BoundedPrioritySchedulingElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3331 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BufferPool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4829 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5269 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1358 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculatedRoutes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1205 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculatesAmong.mof
--rw-r--r--   0 maiera     (501) staff       (20)      910 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculationBasedOnQueue.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1046 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculationServiceForDropper.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1613 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1734 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementInClassifierService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementUsesFilterList.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2324 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierFilterSet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1742 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      651 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CollectedBufferPool.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2208 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2352 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningServiceOnEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Confederation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1596 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1664 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityMembershipSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4706 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7366 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11421 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSGeneralSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3041 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3033 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1079 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DSCPMarkerService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2073 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DiffServService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2059 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DropThresholdCalculationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4437 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DropperService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2363 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DynamicForwardingEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1506 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EFService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1432 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EGPRouteCalcDependency.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4478 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ESPTransform.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1928 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EWMAMeterService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1489 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EgressConditioningServiceOnEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ElementInSchedulingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      742 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointForIPNetworkConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1150 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      597 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInArea.mof
--rw-r--r--   0 maiera     (501) staff       (20)      610 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInLink.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1382 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointOfNetworkPipe.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EntriesInFilterList.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1644 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ExtendedStaticIPAssignmentSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1473 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FailNextScheduler.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4085 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2477 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryBase.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1385 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3365 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterList.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1274 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterListInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      639 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterListsInBGPRouteMap.mof
--rw-r--r--   0 maiera     (501) staff       (20)      795 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterOfSecurityAssociation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      774 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilteredBGPAttributes.mof
--rw-r--r--   0 maiera     (501) staff       (20)      623 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FlowService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1024 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardedRoutes.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2643 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      753 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardsAmong.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4677 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021Filter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1490 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021PService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1265 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropQueueBinding.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1107 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropper.mof
--rw-r--r--   0 maiera     (501) staff       (20)      824 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedAdminDistance.mof
--rw-r--r--   0 maiera     (501) staff       (20)      752 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPAttributes.mof
--rw-r--r--   0 maiera     (501) staff       (20)      741 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPPeerGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      732 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPRouteMap.mof
--rw-r--r--   0 maiera     (501) staff       (20)      791 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterEntryBase.mof
--rw-r--r--   0 maiera     (501) staff       (20)      707 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterList.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedForwardingServices.mof
--rw-r--r--   0 maiera     (501) staff       (20)      765 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedNetworkPipe.mof
--rw-r--r--   0 maiera     (501) staff       (20)      688 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)      813 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingPolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingServices.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1397 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10938 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5622 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IKESAEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3009 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPAddressRange.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3995 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPAssignmentSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2042 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPCOMPTransform.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10047 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1406 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPConnectivitySubnet.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13624 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPHeadersFilter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2794 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPInterfaceSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      802 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPNetworkConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5400 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5504 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4511 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPSOFilterEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPSubnet.mof
--rw-r--r--   0 maiera     (501) staff       (20)      912 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPVersionSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      427 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPXConnectivityNetwork.mof
--rw-r--r--   0 maiera     (501) staff       (20)      723 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPXNetwork.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1009 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPXProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1613 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPsecSAEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      666 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InBGPPeerGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1201 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InLogicalNetwork.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1097 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InSegment.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3689 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InboundVLAN.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1315 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IngressConditioningServiceOnEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1772 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_KVMRedirectionSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1536 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANConnectivitySegment.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2912 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1915 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANSegment.mof
--rw-r--r--   0 maiera     (501) staff       (20)      941 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ListsInRoutingPolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3497 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetwork.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1228 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetworkService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1544 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MarkerService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4853 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2916 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3002 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MeterService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      833 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NamedAddressCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1625 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Network.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4950 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipe.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2873 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipeComposition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2272 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPortConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3131 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1288 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkServicesInAdminDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2295 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkVLAN.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1270 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworksInAdminDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopIPRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRoute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2315 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRouting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1332 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextScheduler.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1289 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterClassifierElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1911 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterMeter.mof
--rw-r--r--   0 maiera     (501) staff       (20)      538 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NonWorkConservingSchedulingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFArea.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4487 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFAreaConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1674 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFLink.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2668 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpointBase.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2453 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1013 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1597 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)      705 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFVirtualInterface.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1470 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OutboundVLAN.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2580 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PacketSchedulingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3071 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PeerIDPayloadFilterEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)      587 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PeerOfSAEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      840 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Phase1SAUsedForPhase2.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2399 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PreambleFilter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1963 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PreambleMarkerService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1557 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PrecedenceService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1076 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Priority8021QMarkerService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1589 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PrioritySchedulingElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1443 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ProtocolServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      980 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSConditioningSubService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2019 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1405 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSSubService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1260 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueAllocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1502 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueHierarchy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1260 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueToSchedule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1204 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueuingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4452 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_REDDropperService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1424 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RangeOfIPAddresses.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1330 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RangesOfConfiguration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3691 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      695 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      761 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorClientService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      760 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorNonClientService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      756 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      788 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RelatedSpanningTree.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1146 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RelatedTransparentBridgingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1433 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RemoteAccessAvailableToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1832 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteCalculationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1718 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteForwardedByService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      700 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteUsesEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2349 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInAS.mof
--rw-r--r--   0 maiera     (501) staff       (20)      853 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInBGPCluster.mof
--rw-r--r--   0 maiera     (501) staff       (20)      776 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutesBGP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5751 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingPolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)      866 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomain.mof
--rw-r--r--   0 maiera     (501) staff       (20)      649 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomainInAS.mof
--rw-r--r--   0 maiera     (501) staff       (20)      963 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointConnectionStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1327 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointRefreshSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3135 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SATransform.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3388 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SCSIProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2389 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPCommunityString.mof
--rw-r--r--   0 maiera     (501) staff       (20)      679 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1518 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPTrapTarget.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2316 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5116 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4891 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1497 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulerUsed.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3489 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingServiceToSchedule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2977 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SecurityAssociationEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)      982 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SourceRoutingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5559 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      862 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      656 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Specific802dot1QVLANService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2675 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_StaticForwardingEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2979 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_StaticIPAssignmentSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      589 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPort.mof
--rw-r--r--   0 maiera     (501) staff       (20)      645 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortDynamicForwarding.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1407 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortPair.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4063 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRouting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4190 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRoutingStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3169 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTree.mof
--rw-r--r--   0 maiera     (501) staff       (20)      618 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTreeStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      622 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStaticForwarding.mof
--rw-r--r--   0 maiera     (501) staff       (20)      934 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1479 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortTransparentBridgingStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2197 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      743 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSourceRouting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      738 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSpanningTree.mof
--rw-r--r--   0 maiera     (501) staff       (20)      764 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceTransparentBridging.mof
--rw-r--r--   0 maiera     (501) staff       (20)      892 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceVLAN.mof
--rw-r--r--   0 maiera     (501) staff       (20)      968 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Switchable.mof
--rw-r--r--   0 maiera     (501) staff       (20)      596 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchesAmong.mof
--rw-r--r--   0 maiera     (501) staff       (20)      834 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TCPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2297 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4910 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4595 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1865 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1492 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1107 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ToSMarkerService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2359 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TokenBucketMeterService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      740 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransformOfSecurityAssociation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      787 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingDynamicForwarding.mof
--rw-r--r--   0 maiera     (501) staff       (20)      827 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      764 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStaticForwarding.mof
--rw-r--r--   0 maiera     (501) staff       (20)      712 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      694 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TrapSourceForSNMPService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      752 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_UDPProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9603 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2218 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12184 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3326 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLAN.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9347 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1409 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2686 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      640 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANFor.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3076 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANNetwork.mof
--rw-r--r--   0 maiera     (501) staff       (20)      922 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2445 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WRRSchedulingElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2914 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WeightedREDDropperService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12092 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6116 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9101 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2407 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiNetworkDetectionSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2851 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_X509CredentialFilterEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4024 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSICapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1435 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9241 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5713 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6941 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnectionSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8132 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSILoginStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2564 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIProtocolEndpoint.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7534 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISession.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2836 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionFailures.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6343 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1954 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionStatistics.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.829407 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/
--rw-r--r--   0 maiera     (501) staff       (20)     1206 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_AdjacentSlots.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4011 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Card.mof
--rw-r--r--   0 maiera     (501) staff       (20)      721 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_CardInSlot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1481 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_CardOnCard.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7297 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Chassis.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1191 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ChassisInRack.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1048 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Chip.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6292 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConfigurationCapacity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      765 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectedTo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      763 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectorOnPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Container.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1023 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ContainerView.mof
--rw-r--r--   0 maiera     (501) staff       (20)      799 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Docked.mof
--rw-r--r--   0 maiera     (501) staff       (20)      867 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementCapacity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      729 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementInConnector.mof
--rw-r--r--   0 maiera     (501) staff       (20)      581 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementsLinked.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_HomeForMedia.mof
--rw-r--r--   0 maiera     (501) staff       (20)      730 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_LinkHasConnector.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2609 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Magazine.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1617 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3760 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2149 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryCapacity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      742 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryOnCard.mof
--rw-r--r--   0 maiera     (501) staff       (20)      673 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryWithMedia.mof
--rw-r--r--   0 maiera     (501) staff       (20)      756 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInChassis.mof
--rw-r--r--   0 maiera     (501) staff       (20)      994 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInConnector.mof
--rw-r--r--   0 maiera     (501) staff       (20)      847 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInSlot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1335 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1085 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackagedComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      567 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ParticipatesInSet.mof
--rw-r--r--   0 maiera     (501) staff       (20)      945 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalAssetCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1178 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalCapacity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3770 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9406 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalConnector.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3775 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalFrame.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2256 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalLink.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8561 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMedia.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1641 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMediaInLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5079 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMemory.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10134 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2212 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalTape.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1697 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Rack.mof
--rw-r--r--   0 maiera     (501) staff       (20)      761 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ReplacementSet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6799 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Slot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1933 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_SlotInSlot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5917 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_StorageMediaLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2680 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_SystemBusCard.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.887920 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/
--rw-r--r--   0 maiera     (501) staff       (20)     2227 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AcceptCredentialFrom.mof
--rw-r--r--   0 maiera     (501) staff       (20)      795 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AccountAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)      848 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1003 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationRule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1533 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_BiometricAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2358 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      868 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1565 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_DocumentAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1094 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ElementInPolicyRoleCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1219 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_FilterOfPacketCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      602 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_KerberosAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6693 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_MethodAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1769 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkPacketAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      833 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkingIDAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1869 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PacketFilterCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1551 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PhysicalCredentialAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1880 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_Policy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3893 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      844 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1790 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRepository.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1743 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2861 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionStructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)      800 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3814 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1127 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1829 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRepository.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1036 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2445 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionStructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)      836 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyContainerInPolicyContainer.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1327 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInPolicyGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      676 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1454 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      927 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepository.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepositoryInPolicyRepository.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3858 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      727 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollectionInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRule.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1151 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInPolicyGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      670 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1755 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleValidityPeriod.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySet.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1083 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetAppliesToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1835 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      830 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInRoleCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1477 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2410 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetValidityPeriod.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15588 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyTimePeriodCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      878 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PublicPrivateKeyAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3928 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_QueryCondition.mof
--rw-r--r--   0 maiera     (501) staff       (20)      789 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_RejectConnectionAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)      752 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicy.mof
--rw-r--r--   0 maiera     (501) staff       (20)      646 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicyContainer.mof
--rw-r--r--   0 maiera     (501) staff       (20)      872 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_SharedSecretAuthentication.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1651 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyAction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1695 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyCondition.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:22.946009 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/
--rw-r--r--   0 maiera     (501) staff       (20)     1737 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Activity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      483 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ActivityContact.mof
--rw-r--r--   0 maiera     (501) staff       (20)      530 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ActivityResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      556 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ActivityTransaction.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Address.mof
--rw-r--r--   0 maiera     (501) staff       (20)      482 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AddressLocation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      580 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdminAssociation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3197 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Administrative.mof
--rw-r--r--   0 maiera     (501) staff       (20)      558 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeContact.mof
--rw-r--r--   0 maiera     (501) staff       (20)      560 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeRevision.mof
--rw-r--r--   0 maiera     (501) staff       (20)      591 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Agreement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      506 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Attached.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2139 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Attachment.mof
--rw-r--r--   0 maiera     (501) staff       (20)      899 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Categorization.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1209 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Category.mof
--rw-r--r--   0 maiera     (501) staff       (20)      603 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_CategoryParentChild.mof
--rw-r--r--   0 maiera     (501) staff       (20)      419 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Contact.mof
--rw-r--r--   0 maiera     (501) staff       (20)      959 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactContactItem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      386 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactItem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      495 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactItemAddress.mof
--rw-r--r--   0 maiera     (501) staff       (20)      525 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactOrganization.mof
--rw-r--r--   0 maiera     (501) staff       (20)      501 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactPerson.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2339 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ExchangeElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      794 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Expression.mof
--rw-r--r--   0 maiera     (501) staff       (20)      403 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      735 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionLink.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1294 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Feature.mof
--rw-r--r--   0 maiera     (501) staff       (20)      590 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_FeatureResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      562 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Location.mof
--rw-r--r--   0 maiera     (501) staff       (20)      461 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Organization.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1074 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Person.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1099 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Problem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      745 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Product.mof
--rw-r--r--   0 maiera     (501) staff       (20)      654 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductAsset.mof
--rw-r--r--   0 maiera     (501) staff       (20)      677 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductParentChild.mof
--rw-r--r--   0 maiera     (501) staff       (20)      532 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Reference.mof
--rw-r--r--   0 maiera     (501) staff       (20)      937 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Resolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)      476 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ResolutionResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      817 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Resource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2295 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Revision.mof
--rw-r--r--   0 maiera     (501) staff       (20)      506 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_RevisionContact.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10185 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SISService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      548 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceActivity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      528 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceAgreement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3520 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceIncident.mof
--rw-r--r--   0 maiera     (501) staff       (20)      602 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProblem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      572 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProvider.mof
--rw-r--r--   0 maiera     (501) staff       (20)      766 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceRequester.mof
--rw-r--r--   0 maiera     (501) staff       (20)      685 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceResolutionSolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1797 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Solution.mof
--rw-r--r--   0 maiera     (501) staff       (20)      640 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionCategory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      760 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      626 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionExpression.mof
--rw-r--r--   0 maiera     (501) staff       (20)      918 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionHasElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      596 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionProblem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      617 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionReference.mof
--rw-r--r--   0 maiera     (501) staff       (20)      620 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionResolution.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4283 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Statement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      468 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_StatementFeature.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2115 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Transaction.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.149150 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/
--rw-r--r--   0 maiera     (501) staff       (20)     2097 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AffectedJobElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      873 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AllocatedDMA.mof
--rw-r--r--   0 maiera     (501) staff       (20)      628 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AllocatedResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      934 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AssociatedFileSystemStatisticsManifestCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)      685 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AssociatedJobMethodResult.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2010 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AvailableDiagnosticService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5015 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSAttribute.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1619 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSEnumeration.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1792 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSInteger.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2786 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSPassword.mof
--rw-r--r--   0 maiera     (501) staff       (20)    24356 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2363 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2335 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSString.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3632 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootConfigSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)      773 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootOSFromFS.mof
--rw-r--r--   0 maiera     (501) staff       (20)      258 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11057 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      571 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootServiceAccessBySAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6172 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1981 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3277 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootSourceSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5484 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CIFSSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      988 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CIFSShare.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2086 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Cluster.mof
--rw-r--r--   0 maiera     (501) staff       (20)      616 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ClusterServiceAccessBySAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)      280 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ClusteringSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1969 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ClusteringService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2168 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComponentCS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9819 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      669 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemDMA.mof
--rw-r--r--   0 maiera     (501) staff       (20)      652 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemIRQ.mof
--rw-r--r--   0 maiera     (501) staff       (20)      718 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemMappedIO.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1595 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemNodeCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      913 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)      680 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)      646 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingDataRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      636 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingsRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4549 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DMA.mof
--rw-r--r--   0 maiera     (501) staff       (20)      303 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DataFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      903 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DefaultElementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      626 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DeviceAccessedByFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      531 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DeviceFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2270 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticCompletionRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      643 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4800 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14007 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResult.mof
--rw-r--r--   0 maiera     (501) staff       (20)      802 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForMSE.mof
--rw-r--r--   0 maiera     (501) staff       (20)      813 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1151 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultInPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6099 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7866 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1896 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceJobCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3806 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)    21804 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16506 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      611 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingDataRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      958 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingForTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7268 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      774 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSubTestRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)    18382 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2858 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestForMSE.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1271 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestInPackage.mof
--rw-r--r--   0 maiera     (501) staff       (20)      897 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticsLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)      355 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Directory.mof
--rw-r--r--   0 maiera     (501) staff       (20)      649 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DirectoryContainsFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1966 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4538 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)      774 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Export.mof
--rw-r--r--   0 maiera     (501) staff       (20)     8651 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13000 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1301 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5961 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3776 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticTest.mof
--rw-r--r--   0 maiera     (501) staff       (20)      843 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FIFOPipeFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1461 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSDomainIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      479 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSIPInterfaceSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      494 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToPrincipal.mof
--rw-r--r--   0 maiera     (501) staff       (20)      741 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToTree.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3987 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6329 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaConfigEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2170 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaIndication.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12452 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5190 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaReportRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4426 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileExportCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    28439 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileExportService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      916 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7631 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2606 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    18483 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2607 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerSettings.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1050 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileShare.mof
--rw-r--r--   0 maiera     (501) staff       (20)      714 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileShareSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      688 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10207 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)    16452 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2548 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    33217 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)    17873 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1929 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15481 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticalData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2537 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    25622 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifest.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1400 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifestCollection.mof
--rw-r--r--   0 maiera     (501) staff       (20)    11333 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5670 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HelpService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1250 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HelpServiceAvailableToFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      911 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedBootSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)      764 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedBootService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      930 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)      916 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      752 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedFileSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      984 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedJobDestination.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1872 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedShare.mof
--rw-r--r--   0 maiera     (501) staff       (20)      626 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostingCS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3254 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_IRQ.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1230 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_InstalledOS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1554 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobDestination.mof
--rw-r--r--   0 maiera     (501) staff       (20)      619 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobDestinationJobs.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2877 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobQueue.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9492 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1702 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LastAppliedSnapshot.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocalAccessAvailableToFS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6206 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocalFileSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7236 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    19865 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemSetting.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3903 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Log.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4482 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogEntry.mof
--rw-r--r--   0 maiera     (501) staff       (20)      794 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInDataFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      894 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInDeviceFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1109 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInStorage.mof
--rw-r--r--   0 maiera     (501) staff       (20)      524 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogManagesRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2823 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      682 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogToLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4441 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogicalFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2029 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MemoryMappedIO.mof
--rw-r--r--   0 maiera     (501) staff       (20)      805 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MemoryResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)    26072 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MessageLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3802 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MethodResult.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1544 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Mount.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3230 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2151 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFSSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      839 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFSShare.mof
--rw-r--r--   0 maiera     (501) staff       (20)      723 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NISSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4911 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OOBAlertService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      714 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OSProcess.mof
--rw-r--r--   0 maiera     (501) staff       (20)    13462 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1567 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystemCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      784 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperationLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1067 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OwningJobElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2003 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ParticipatingCS.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6261 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2364 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogServiceCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      803 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PortResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6393 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Process.mof
--rw-r--r--   0 maiera     (501) staff       (20)      624 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessExecutable.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1101 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessOfJob.mof
--rw-r--r--   0 maiera     (501) staff       (20)      665 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessThread.mof
--rw-r--r--   0 maiera     (501) staff       (20)      786 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordAppliesToElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5139 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordForLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)      576 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordInLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2311 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1008 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordLogCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      751 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RemoteFileSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ReportRecord.mof
--rw-r--r--   0 maiera     (501) staff       (20)      814 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResidesOnExtent.mof
--rw-r--r--   0 maiera     (501) staff       (20)      711 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResourceAllocationFromPool.mof
--rw-r--r--   0 maiera     (501) staff       (20)      749 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResourceOfSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      858 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RunningOS.mof
--rw-r--r--   0 maiera     (501) staff       (20)      903 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SAPAvailableForFileShare.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2329 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ServiceProcess.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1462 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SettingAssociatedToCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2307 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Share.mof
--rw-r--r--   0 maiera     (501) staff       (20)      964 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SharedElement.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1059 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SnapshotOfVirtualSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3154 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SummaryDiagnostics.mof
--rw-r--r--   0 maiera     (501) staff       (20)      599 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SymbolicLink.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1540 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SystemPartition.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1235 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SystemResource.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3872 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Thread.mof
--rw-r--r--   0 maiera     (501) staff       (20)    10122 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_TimeZone.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4014 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnitaryComputerSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1477 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixDeviceFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)      736 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixDirectory.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5741 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixFile.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1602 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixLocalFileSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2943 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcess.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4607 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatisticalInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)      724 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatistics.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2630 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixThread.mof
--rw-r--r--   0 maiera     (501) staff       (20)      971 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UseOfLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)      674 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UseOfMessageLog.mof
--rw-r--r--   0 maiera     (501) staff       (20)      617 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualComputerSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5785 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemMigrationSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)    12628 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingDataComponent.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2350 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_WakeUpService.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.260389 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/
--rw-r--r--   0 maiera     (501) staff       (20)     5088 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccessControlInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14806 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Account.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1034 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5433 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7068 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1169 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountMapsToAccount.mof
--rw-r--r--   0 maiera     (501) staff       (20)      770 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountOnSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3473 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)      634 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AssignedIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)    14648 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AssociatedPrivilege.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1032 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticateForUse.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3321 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationRequirement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      731 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1405 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationTarget.mof
--rw-r--r--   0 maiera     (501) staff       (20)      394 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1159 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationSubject.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1311 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationTarget.mof
--rw-r--r--   0 maiera     (501) staff       (20)      863 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedPrivilege.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1253 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedSubject.mof
--rw-r--r--   0 maiera     (501) staff       (20)      657 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedTarget.mof
--rw-r--r--   0 maiera     (501) staff       (20)      930 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedUse.mof
--rw-r--r--   0 maiera     (501) staff       (20)      821 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CAHasPublicCertificate.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1348 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CASignsPublicKeyCertificate.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2650 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateAuthority.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4098 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    32809 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      763 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CollectionInOrganization.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1100 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CollectionInSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2489 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Credential.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3060 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialContext.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3946 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      413 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementSAP.mof
--rw-r--r--   0 maiera     (501) staff       (20)      334 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3012 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialStore.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1704 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ElementAsUser.mof
--rw-r--r--   0 maiera     (501) staff       (20)      681 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ElementSecuritySensitivity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1684 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_GatewayPathID.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2250 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Group.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1162 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_HostedACI.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1126 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_HostedAuthenticationRequirement.mof
--rw-r--r--   0 maiera     (501) staff       (20)      913 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IKESecretIsNamed.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2306 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IPNetworkIdentity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5014 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Identity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      817 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IdentityContext.mof
--rw-r--r--   0 maiera     (501) staff       (20)      311 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IdentityManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      863 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KDCIssuesKerberosTicket.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3363 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)      543 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosKeyDistributionCenter.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2702 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosTicket.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7759 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KeyBasedCredentialManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1532 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Keystore.mof
--rw-r--r--   0 maiera     (501) staff       (20)      404 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_LocalCredentialManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      950 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_LocallyManagedPublicKey.mof
--rw-r--r--   0 maiera     (501) staff       (20)      795 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagedCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)      606 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccount.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1132 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccountOnSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2291 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MemberPrincipal.mof
--rw-r--r--   0 maiera     (501) staff       (20)      649 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreGroupInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      662 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreOrgUnitInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      696 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreOrganizationInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      654 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MorePersonInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)      641 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreRoleInfo.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4052 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NamedCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3679 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NamedSharedIKESecret.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1903 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Notary.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1257 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NotaryVerifiesBiometric.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1249 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OpaqueManagementDataOwner.mof
--rw-r--r--   0 maiera     (501) staff       (20)      862 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OrgStructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2911 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OrgUnit.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3030 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Organization.mof
--rw-r--r--   0 maiera     (501) staff       (20)      344 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OrganizationalEntity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3293 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherGroupInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6126 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherOrgUnitInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7376 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherOrganizationInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15051 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherPersonInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6173 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherRoleInformation.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4031 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Person.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9572 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Privilege.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4145 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)    15814 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1940 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyCertificate.mof
--rw-r--r--   0 maiera     (501) staff       (20)      403 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2208 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PublicPrivateKeyPair.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1478 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RequireCredentialsFrom.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4260 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Role.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9766 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedAuthorizationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedManagementCapabilities.mof
--rw-r--r--   0 maiera     (501) staff       (20)      779 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleLimitedToTarget.mof
--rw-r--r--   0 maiera     (501) staff       (20)     6065 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecuritySensitivity.mof
--rw-r--r--   0 maiera     (501) staff       (20)      254 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecurityService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1077 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceForSystem.mof
--rw-r--r--   0 maiera     (501) staff       (20)      606 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceUsesAccount.mof
--rw-r--r--   0 maiera     (501) staff       (20)      800 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ServiceUsesSecurityService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3208 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2688 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecret.mof
--rw-r--r--   0 maiera     (501) staff       (20)      818 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretIsShared.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1030 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3698 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SignedCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3585 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageClientSettingData.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1267 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareID.mof
--rw-r--r--   0 maiera     (501) staff       (20)     9721 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareIDManagementService.mof
--rw-r--r--   0 maiera     (501) staff       (20)      663 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministrator.mof
--rw-r--r--   0 maiera     (501) staff       (20)      615 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorGroup.mof
--rw-r--r--   0 maiera     (501) staff       (20)      577 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorRole.mof
--rw-r--r--   0 maiera     (501) staff       (20)      788 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_TrustHierarchy.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2948 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UnsignedCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2715 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UnsignedPublicKey.mof
--rw-r--r--   0 maiera     (501) staff       (20)     3191 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UserContact.mof
--rw-r--r--   0 maiera     (501) staff       (20)      331 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UserEntity.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2822 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersAccess.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1030 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersAccount.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1122 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersCredential.mof
--rw-r--r--   0 maiera     (501) staff       (20)      463 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_VerificationService.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2745 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509CRL.mof
--rw-r--r--   0 maiera     (501) staff       (20)     7494 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509Certificate.mof
--rw-r--r--   0 maiera     (501) staff       (20)     4071 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509Infrastructure.mof
--rw-r--r--   0 maiera     (501) staff       (20)    92023 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/cim_schema_2.49.0.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5668 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/qualifiers.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1299 2024-03-11 18:16:47.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/qualifiers_optional.mof
--rw-r--r--   0 maiera     (501) staff       (20)      380 2024-03-11 18:11:15.000000 pywbem-1.7.0/tests/schema/mofFinal2.49.0/test_partial_schema.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.261919 pywbem-1.7.0/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.262901 pywbem-1.7.0/tests/unittest/end2endtest_utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/end2endtest_utils/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.263939 pywbem-1.7.0/tests/unittest/functiontest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/functiontest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     2251 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/functiontest/test_conftest.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.314866 pywbem-1.7.0/tests/unittest/pywbem/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)        0 2024-03-11 18:11:16.000000 pywbem-1.7.0/tests/unittest/pywbem/moflog.txt
--rw-r--r--   0 maiera     (501) staff       (20)        0 2024-03-11 18:11:16.000000 pywbem-1.7.0/tests/unittest/pywbem/moflog2.txt
--rw-r--r--   0 maiera     (501) staff       (20)     5002 2022-03-09 17:42:38.000000 pywbem-1.7.0/tests/unittest/pywbem/test.mof
--rwxr-xr-x   0 maiera     (501) staff       (20)    35002 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_cim_http.py
--rwxr-xr-x   0 maiera     (501) staff       (20)  1334024 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_cim_obj.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    46272 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_cim_operations.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    45416 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_cim_types.py
--rwxr-xr-x   0 maiera     (501) staff       (20)   130414 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_cim_xml.py
--rw-r--r--   0 maiera     (501) staff       (20)    14912 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_exceptions.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    38707 2024-04-15 19:35:13.000000 pywbem-1.7.0/tests/unittest/pywbem/test_indicationlistener.py
--rw-r--r--   0 maiera     (501) staff       (20)   103399 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_itermethods.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    19785 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_logging.py
--rwxr-xr-x   0 maiera     (501) staff       (20)   115625 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_mof_compiler.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     5335 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_nocasedict.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     5585 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_perf_equality.py
--rwxr-xr-x   0 maiera     (501) staff       (20)   112392 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/unittest/pywbem/test_recorder.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    23026 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_statistics.py
--rw-r--r--   0 maiera     (501) staff       (20)    86377 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_subscriptionmanager.py
--rwxr-xr-x   0 maiera     (501) staff       (20)   469334 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_tupleparse.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    30974 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/unittest/pywbem/test_tupletree.py
--rw-r--r--   0 maiera     (501) staff       (20)    24429 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_units.py
--rw-r--r--   0 maiera     (501) staff       (20)    21935 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)    37379 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_valuemapping.py
--rw-r--r--   0 maiera     (501) staff       (20)     4352 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_warnings.py
--rw-r--r--   0 maiera     (501) staff       (20)    16961 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem/test_wbemserverclass.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.324530 pywbem-1.7.0/tests/unittest/pywbem/testmofs/
--rw-r--r--   0 maiera     (501) staff       (20)     1372 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error01.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1349 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error02.mof
--rw-r--r--   0 maiera     (501) staff       (20)      889 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error03.mof
--rw-r--r--   0 maiera     (501) staff       (20)       76 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error04.mof
--rw-r--r--   0 maiera     (501) staff       (20)     5668 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/qualifiers.mof
--rw-r--r--   0 maiera     (501) staff       (20)     2431 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/test_instance.mof
--rw-r--r--   0 maiera     (501) staff       (20)     1338 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/test_refs.mof
--rw-r--r--   0 maiera     (501) staff       (20)      462 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem/testmofs/test_types.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.336710 pywbem-1.7.0/tests/unittest/pywbem_mock/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3065 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/conftest.py
--rw-r--r--   0 maiera     (501) staff       (20)    39127 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_complexassoc.py
--rw-r--r--   0 maiera     (501) staff       (20)    28707 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_inmemory_repository.py
--rw-r--r--   0 maiera     (501) staff       (20)    64912 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_multi_ns_assoc.py
--rw-r--r--   0 maiera     (501) staff       (20)    13646 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_providerdependentregistry.py
--rw-r--r--   0 maiera     (501) staff       (20)    13623 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_providerregistry.py
--rw-r--r--   0 maiera     (501) staff       (20)    19122 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_system_providers.py
--rw-r--r--   0 maiera     (501) staff       (20)   423818 2024-04-15 15:44:36.000000 pywbem-1.7.0/tests/unittest/pywbem_mock/test_wbemconnection_mock.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.340916 pywbem-1.7.0/tests/unittest/resourcetest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/unittest/resourcetest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     7498 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/resourcetest/test_memory_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)     2493 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/simple_mock_model.mof
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.342028 pywbem-1.7.0/tests/unittest/unittest_utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/unittest_utils/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-16 05:55:23.347590 pywbem-1.7.0/tests/unittest/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.0/tests/unittest/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3031 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/unittest/utils/dmtf_mof_schema_def.py
--rw-r--r--   0 maiera     (501) staff       (20)     9047 2024-04-07 12:36:21.000000 pywbem-1.7.0/tests/unittest/utils/pytest_extensions.py
--rw-r--r--   0 maiera     (501) staff       (20)     1886 2022-03-30 06:07:16.000000 pywbem-1.7.0/tests/unittest/utils/unichr2.py
--rw-r--r--   0 maiera     (501) staff       (20)    14313 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/unittest/utils/unittest_extensions.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     8737 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/unittest/utils/validate.py
--rw-r--r--   0 maiera     (501) staff       (20)    21400 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/unittest/utils/wbemserver_mock.py
--rw-r--r--   0 maiera     (501) staff       (20)    11719 2022-11-09 03:23:37.000000 pywbem-1.7.0/tests/utils.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.469457 pywbem-1.7.1/
+-rw-r--r--   0 maiera     (501) staff       (20)      883 2024-04-07 12:36:21.000000 pywbem-1.7.1/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    26436 2022-03-09 17:32:21.000000 pywbem-1.7.1/LICENSE.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      527 2024-04-18 09:03:54.000000 pywbem-1.7.1/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     7338 2024-04-18 09:04:09.468853 pywbem-1.7.1/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     7476 2024-04-18 06:23:07.000000 pywbem-1.7.1/README.md
+-rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-04-18 06:23:07.000000 pywbem-1.7.1/README_PYPI.md
+-rwxr-xr-x   0 maiera     (501) staff       (20)     2881 2024-04-18 06:23:07.000000 pywbem-1.7.1/build_moftab.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    13849 2022-11-09 03:23:37.000000 pywbem-1.7.1/mof_compiler
+-rw-r--r--   0 maiera     (501) staff       (20)      105 2022-03-09 17:32:21.000000 pywbem-1.7.1/mof_compiler.bat
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.701921 pywbem-1.7.1/pywbem/
+-rw-r--r--   0 maiera     (501) staff       (20)     3441 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    10911 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_constants.py
+-rw-r--r--   0 maiera     (501) staff       (20)    25269 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_http.py
+-rw-r--r--   0 maiera     (501) staff       (20)   306789 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_obj.py
+-rw-r--r--   0 maiera     (501) staff       (20)   446903 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_operations.py
+-rw-r--r--   0 maiera     (501) staff       (20)    51216 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_types.py
+-rw-r--r--   0 maiera     (501) staff       (20)    56118 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cim_xml.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1971 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_cliutils.py
+-rw-r--r--   0 maiera     (501) staff       (20)    25906 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_exceptions.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1685 2022-03-30 06:07:16.000000 pywbem-1.7.1/pywbem/_features.py
+-rw-r--r--   0 maiera     (501) staff       (20)    51339 2024-04-18 06:46:21.000000 pywbem-1.7.1/pywbem/_listener.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21597 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_logging.py
+-rw-r--r--   0 maiera     (501) staff       (20)   114330 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_mof_compiler.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2648 2024-04-18 09:03:53.000000 pywbem-1.7.1/pywbem/_moflextab.py
+-rw-r--r--   0 maiera     (501) staff       (20)    70070 2024-04-18 09:03:53.000000 pywbem-1.7.1/pywbem/_mofparsetab.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3565 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)    44065 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_recorder.py
+-rw-r--r--   0 maiera     (501) staff       (20)    55199 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_server.py
+-rw-r--r--   0 maiera     (501) staff       (20)    29927 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_statistics.py
+-rw-r--r--   0 maiera     (501) staff       (20)    63708 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_subscription_manager.py
+-rw-r--r--   0 maiera     (501) staff       (20)    91345 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_tupleparse.py
+-rw-r--r--   0 maiera     (501) staff       (20)    19906 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_tupletree.py
+-rw-r--r--   0 maiera     (501) staff       (20)    25988 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_units.py
+-rw-r--r--   0 maiera     (501) staff       (20)    13309 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)    38042 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_valuemapping.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.663540 pywbem-1.7.1/pywbem/_vendor/
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.710154 pywbem-1.7.1/pywbem/_vendor/nocasedict/
+-rw-r--r--   0 maiera     (501) staff       (20)    26526 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      294 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2080 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/_hashable.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1432 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/_keyableby.py
+-rw-r--r--   0 maiera     (501) staff       (20)    31357 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1083 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)      321 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocasedict/_version.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.712743 pywbem-1.7.1/pywbem/_vendor/nocaselist/
+-rw-r--r--   0 maiera     (501) staff       (20)    11357 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocaselist/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      191 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocaselist/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    20968 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocaselist/_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      321 2024-04-18 09:03:56.000000 pywbem-1.7.1/pywbem/_vendor/nocaselist/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1192 2024-04-18 09:03:30.000000 pywbem-1.7.1/pywbem/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2916 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem/_warnings.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5164 2022-11-09 03:23:37.000000 pywbem-1.7.1/pywbem/config.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.457098 pywbem-1.7.1/pywbem.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     7338 2024-04-18 09:04:07.000000 pywbem-1.7.1/pywbem.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)   111311 2024-04-18 09:04:07.000000 pywbem-1.7.1/pywbem.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-18 09:04:07.000000 pywbem-1.7.1/pywbem.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)     2021 2024-04-18 09:04:07.000000 pywbem-1.7.1/pywbem.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       19 2024-04-18 09:04:07.000000 pywbem-1.7.1/pywbem.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-18 06:48:17.000000 pywbem-1.7.1/pywbem.egg-info/zip-safe
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.725431 pywbem-1.7.1/pywbem_mock/
+-rw-r--r--   0 maiera     (501) staff       (20)     2272 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    23345 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_baseprovider.py
+-rw-r--r--   0 maiera     (501) staff       (20)    13993 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_baserepository.py
+-rw-r--r--   0 maiera     (501) staff       (20)    23108 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_dmtf_cim_schema.py
+-rw-r--r--   0 maiera     (501) staff       (20)    12337 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_inmemoryrepository.py
+-rw-r--r--   0 maiera     (501) staff       (20)    38310 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_instancewriteprovider.py
+-rw-r--r--   0 maiera     (501) staff       (20)   155063 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_mainprovider.py
+-rw-r--r--   0 maiera     (501) staff       (20)    10974 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_methodprovider.py
+-rw-r--r--   0 maiera     (501) staff       (20)    15051 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_mockmofwbemconnection.py
+-rw-r--r--   0 maiera     (501) staff       (20)    14604 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_namespaceprovider.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5969 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_providerdependentregistry.py
+-rw-r--r--   0 maiera     (501) staff       (20)    31642 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_providerdispatcher.py
+-rw-r--r--   0 maiera     (501) staff       (20)    18747 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_providerregistry.py
+-rw-r--r--   0 maiera     (501) staff       (20)    22692 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_resolvermixin.py
+-rw-r--r--   0 maiera     (501) staff       (20)    35926 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_subscriptionproviders.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2742 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)    83136 2024-04-18 06:23:07.000000 pywbem-1.7.1/pywbem_mock/_wbemconnection_mock.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4391 2022-03-30 06:07:16.000000 pywbem-1.7.1/pywbem_mock/config.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2405 2024-04-18 06:23:07.000000 pywbem-1.7.1/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2024-04-18 09:04:09.469572 pywbem-1.7.1/setup.cfg
+-rw-r--r--   0 maiera     (501) staff       (20)    12189 2024-04-18 06:23:07.000000 pywbem-1.7.1/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3919 2024-04-18 06:23:07.000000 pywbem-1.7.1/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.728907 pywbem-1.7.1/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)     6771 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/README
+-rw-r--r--   0 maiera     (501) staff       (20)     1070 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.733105 pywbem-1.7.1/tests/dtd/
+-rw-r--r--   0 maiera     (501) staff       (20)    13950 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/dtd/CIM_DTD_V22.dtd
+-rw-r--r--   0 maiera     (501) staff       (20)    13093 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/dtd/DSP0203_2.2.0.dtd
+-rw-r--r--   0 maiera     (501) staff       (20)    11595 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/dtd/DSP0203_2.3.1.dtd
+-rw-r--r--   0 maiera     (501) staff       (20)    13558 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/dtd/DSP0203_2.4.0.dtd
+-rw-r--r--   0 maiera     (501) staff       (20)      987 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/elapsed_timer.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.744017 pywbem-1.7.1/tests/end2endtest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/end2endtest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3996 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/end2endtest/es_schema.yml
+-rw-r--r--   0 maiera     (501) staff       (20)     4786 2023-01-14 04:26:06.000000 pywbem-1.7.1/tests/end2endtest/es_server.yml
+-rw-r--r--   0 maiera     (501) staff       (20)     2031 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/end2endtest/es_vault.yml
+-rw-r--r--   0 maiera     (501) staff       (20)    23992 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_indications.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7212 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_operation_timeouts.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5095 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_profile_generic.py
+-rw-r--r--   0 maiera     (501) staff       (20)    11759 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_profile_snia_server.py
+-rw-r--r--   0 maiera     (501) staff       (20)     6150 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_profile_snia_smis.py
+-rw-r--r--   0 maiera     (501) staff       (20)     6902 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/test_server.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.748457 pywbem-1.7.1/tests/end2endtest/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/end2endtest/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    34790 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/utils/assertions.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21916 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/utils/pytest_extensions.py
+-rw-r--r--   0 maiera     (501) staff       (20)    18206 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/end2endtest/utils/utils.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.815332 pywbem-1.7.1/tests/functiontest/
+-rw-r--r--   0 maiera     (501) staff       (20)    11990 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/README.md
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/functiontest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    32036 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/associatornames_classes.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    21661 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/associatornames_instances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    14347 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/associators_classes.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    28850 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/associators_instances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)      572 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/clienterror.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     4574 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/closeenumeration.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    48406 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/functiontest/conftest.py
+-rw-r--r--   0 maiera     (501) staff       (20)    23888 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/createclass.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    37957 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/createinstance.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     7150 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/deleteclass.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    13606 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/deleteinstance.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     7265 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/deletequalifier.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)   145717 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/embeddedinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)   102560 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/embeddedobjectclasses.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)   147992 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/embeddedobjectinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    11867 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/enumerateclasses.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    18452 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/enumerateclassnames.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    47962 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/enumerateinstancenames.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    89223 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/enumerateinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    45436 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/enumeratequalifiers.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    28065 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/execquery.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    17687 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/exportindication.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    11027 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/getalltypes.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    36353 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/getclass.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    36600 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/getinstance.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    11665 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/getqualifier.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    23505 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/headers.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    26122 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/invalidexpresponseerror.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)   118735 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/invalidresponseerror.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    41218 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/invokemethod.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    25214 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/modifyclass.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    14752 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/modifyinstance.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     9716 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/networkerror.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    14388 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openassociatorinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    15343 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openasssociatorinstancepaths.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    42372 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openenumerateinstancepaths.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    68783 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openenumerateinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    17007 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openqueryinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    30740 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openreferenceinstancepaths.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    20487 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/openreferenceinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    25729 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/pullinstancepaths.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    26501 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/pullinstances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    30945 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/pullinstanceswithpath.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     8132 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/referencenames_classes.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    11530 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/referencenames_instances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     8891 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/functiontest/references_classes.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)    26925 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/references_instances.yaml
+-rw-r--r--   0 maiera     (501) staff       (20)     9642 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/functiontest/setqualifier.yaml
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.816063 pywbem-1.7.1/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    13097 2024-04-07 12:36:21.000000 pywbem-1.7.1/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.822537 pywbem-1.7.1/tests/leaktest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/leaktest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5417 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_cim_obj.py
+-rw-r--r--   0 maiera     (501) staff       (20)      936 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_cim_xml.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2218 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_dict.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_elementtree.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2482 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_minidom.py
+-rw-r--r--   0 maiera     (501) staff       (20)      644 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/leaktest/test_leaks_statistics.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.834271 pywbem-1.7.1/tests/manualtest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/manualtest/__init__.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)   276186 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_cim_operations.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    19059 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_enum_performance.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    20227 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_enum_performancesimple.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     1358 2022-03-09 17:42:38.000000 pywbem-1.7.1/tests/manualtest/run_mof_compiler_script.sh
+-rwxr-xr-x   0 maiera     (501) staff       (20)    14094 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_operationtimeouts.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    22302 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_response_performance.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     7915 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/manualtest/run_uprint.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     1209 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/manualtest/test_uprint.bat
+-rwxr-xr-x   0 maiera     (501) staff       (20)     1078 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/manualtest/test_uprint.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.835564 pywbem-1.7.1/tests/perftest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/perftest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     6643 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/perftest/test_indications.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.836503 pywbem-1.7.1/tests/profiles/
+-rw-r--r--   0 maiera     (501) staff       (20)    30178 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/profiles/profiles.yml
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.842028 pywbem-1.7.1/tests/resourcetest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/resourcetest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4949 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/resourcetest/memory_utils.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    11084 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/resourcetest/random_objects.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1390 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/resourcetest/resource_measurement.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2032 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/resourcetest/test_enuminst.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3120 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/resourcetest/timers.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.842793 pywbem-1.7.1/tests/schema/
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.849054 pywbem-1.7.1/tests/schema/OpenPegasus/
+-rw-r--r--   0 maiera     (501) staff       (20)      203 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/schema/OpenPegasus/PG_Namespace.mof
+-rw-r--r--   0 maiera     (501) staff       (20)  1822991 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/schema/cim_schema_2.49.0Final-MOFs.zip
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.854414 pywbem-1.7.1/tests/schema/mofFinal2.49.0/
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:07.989715 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/
+-rw-r--r--   0 maiera     (501) staff       (20)     1611 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_AGPSoftwareFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8097 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_Action.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2026 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ActionSequence.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12333 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1167 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4329 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDirectory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1053 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemHierarchy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      792 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemSoftwareFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12511 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ArchitectureCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      741 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_AssociatedAppSystemOverviewStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2920 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2500 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      657 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeatureBIOSElements.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8769 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_Check.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      802 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareElements.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      804 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareFeatures.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1139 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CopyFileAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      329 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CreateDirectoryAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1361 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DiagnosticTestSoftware.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      546 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectoryAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      629 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecificationFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1176 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DiskSpaceCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      626 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ExecuteProgram.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1925 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FRUIncludesSoftwareFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      405 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FileAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2480 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FileSpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      831 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectoryAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      827 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectorySpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2843 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProduct.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      794 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProductImage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      695 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledSoftwareElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      303 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeAppClientModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      979 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      645 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationHostedOnServer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      711 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      833 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionFactoryAvailableToJCAResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4411 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionPoolStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3225 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1319 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDeployedObject.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      755 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      941 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJB.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      709 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBInModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      312 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      829 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      268 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBean.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1800 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBeanStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1255 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      674 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactoryManagedConnectionFactory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      699 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionPools.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1273 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAManagedConnectionFactory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      702 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCANonpooledConnections.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      257 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      326 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      705 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCConnectionPools.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1221 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      540 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSourceDriver.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDriver.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      708 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCNonpooledConnections.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      333 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      792 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResourceUsesDataSource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      329 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      704 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionSessions.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      646 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      561 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConsumerStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2416 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSEndpointStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      589 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSProducerStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      257 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      694 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionConsumers.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      694 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionProducers.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2509 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      699 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStatConnections.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      330 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      316 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJNDIResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      296 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      892 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2365 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVM.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1826 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVMStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      280 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      528 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5063 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObject.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3385 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObjectCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      283 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBean.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      539 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBeanStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      413 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      631 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModuleUsesJVM.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4053 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeNotification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      281 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeRMI_IIOPResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1766 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      947 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      845 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterInModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      354 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      708 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceOnServer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1097 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      743 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerInDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      688 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerUsesJVM.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      870 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServlet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      729 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletInModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1701 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      337 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBean.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBeanStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      303 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBean.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1114 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBeanStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      305 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatelessSessionBean.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      387 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatelessSessionBeanStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2828 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatistic.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      257 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      534 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLStats.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      308 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeWebModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1145 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_MemoryCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ModifySettingAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2296 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_OSVersionCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      713 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_OperatingSystemSoftwareFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      608 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ProductSoftwareFeatures.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      309 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_RebootAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      592 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_RemoveDirectoryAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      338 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_RemoveFileAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SettingCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9693 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      593 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementActions.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1079 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementChecks.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      783 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2679 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementSAPImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2640 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementServiceImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5995 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementVersionCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2557 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      784 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1311 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSAPImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1270 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureServiceImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      726 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSoftwareElements.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3268 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_StatisticalRuntimeOverview.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1185 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SwapSpaceCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      627 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SystemBIOS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      839 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectoryAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      835 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectorySpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1120 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VersionCompatibilityCheck.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      962 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1999 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      710 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeatureVideoBIOSElements.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.178521 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/
+-rw-r--r--   0 maiera     (501) staff       (20)     2433 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractBasedOn.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      722 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      855 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementAllocatedFromPool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      685 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3394 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ActiveConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1133 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ActsAsSpare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2310 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AdminDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      529 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AllocatedLogicalElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5071 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AllocationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9787 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AssociatedPowerManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      943 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_BasedOn.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1080 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_BindsTo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9889 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Capabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      658 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectedCollections.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      691 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectedMSEs.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      385 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Collection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2219 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionOfMSEs.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      585 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CompatibleProduct.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      673 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Component.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2761 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1525 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1099 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponentView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1696 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1834 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12938 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteJob.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2227 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Configuration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1655 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5550 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1277 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationForSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      701 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ContainedDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      700 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ContainedLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      549 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DefaultSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      648 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Dependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1738 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DependencyContext.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceSAPImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1224 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceServiceImplementation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1663 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      643 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      668 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementAllocatedFromPool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2053 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      903 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1582 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      586 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3015 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4161 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSoftwareIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1037 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1011 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13055 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3784 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8934 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EthernetPortAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      966 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ExtentRedundancyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ExtraCapacityGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2588 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_FRU.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      945 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_FRUIncludesProduct.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      495 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_FRUPhysicalElements.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1963 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_GroupSynchronized.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1045 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedAccessPoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      867 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      608 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      777 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedResourcePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1165 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2622 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ImplementationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      802 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_InstalledSoftwareIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2106 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_IsSpare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13830 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Job.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6288 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_JobCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      982 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13309 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10010 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5112 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LocalizationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1152 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Location.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    24725 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      545 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDeviceView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      405 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1981 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7549 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ManagedElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    19314 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ManagedSystemElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      569 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_MemberOfCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3232 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_MethodParameters.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2609 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4565 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    21957 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2182 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2250 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1921 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedMemberOfCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      745 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OwningCollectionElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      848 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ParameterValueSources.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1436 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ParametersForMethod.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    59947 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalComputerSystemView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6729 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      673 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElementLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1318 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      675 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12080 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6878 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17336 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProcessorAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3844 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Product.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1906 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      650 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductElementComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      743 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductFRU.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      616 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductParentChild.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      695 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1162 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalElements.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1134 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductProductDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1484 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductServiceComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      679 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductSoftwareComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      724 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductSupport.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4183 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Profile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13005 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9007 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      672 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2015 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesServiceToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      597 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RawMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      633 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Realizes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1234 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2355 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7942 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancySet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3348 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedElementCausingError.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      691 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      579 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1515 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RemotePort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4157 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RemoteServiceAccessPoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      710 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ReplaceableProductFRU.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2952 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ReplacementFRU.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15008 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourceAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8977 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2023 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11133 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      976 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPAvailableForElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      966 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPSAPDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1682 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      664 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      655 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1031 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1094 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10703 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Service.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      871 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessBySAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1545 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessPoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessURI.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6425 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1278 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElementWithQuota.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1229 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAvailableToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      634 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      827 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceSAPDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2746 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceServiceDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1646 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      636 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    24294 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Setting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2154 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingContext.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8246 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      616 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingForSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7755 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1242 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineState.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    23368 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15494 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9537 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2915 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SpareGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      948 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Spared.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5458 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      920 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1239 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      583 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Statistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1217 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticsCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12473 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    23895 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3045 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancyGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1694 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancySet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1941 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SupportAccess.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13084 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Synchronized.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5109 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_System.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1665 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2351 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      728 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      852 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemDeviceView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      800 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemPackaging.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1420 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSettingContext.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2992 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSpecificCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1289 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      629 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1804 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_TimeService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_View.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      635 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ViewOnSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2971 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualEthernetSwitchSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3501 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11315 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1428 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4322 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1960 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2287 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VisibleMemory.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.194501 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/
+-rw-r--r--   0 maiera     (501) staff       (20)      652 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_AssociatedDatabaseSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4016 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabase.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1678 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1721 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      547 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1183 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseAdministrator.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseControlFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      923 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1666 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseParameter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1698 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseResourceStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3174 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegment.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3498 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegmentSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3203 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5293 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseServiceStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1045 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1424 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorageArea.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1458 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1154 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_SNMPDatabaseParameter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2372 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_ServiceAvailableToDatabase.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.585979 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/
+-rw-r--r--   0 maiera     (501) staff       (20)     2337 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ADSLModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3809 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AGPVideoController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      467 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ATAInitiatorTargetLogicalUnitPath.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      579 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ATAPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2495 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AbstractProtocolControllerForDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      713 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AccessLabelReader.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1661 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AdapterActiveConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3153 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AdvancedStorageSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1778 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1247 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1017 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnAggregatePExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      997 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnPExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1053 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregateRedundancyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5600 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1875 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDeviceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2735 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2006 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1426 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolViewView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2008 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedResources.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      662 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedAlarm.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      775 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBattery.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      916 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBlockStatisticsManifestCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6670 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCacheMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1066 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedComponentExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      639 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCooling.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      638 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedDeviceMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1176 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedElementTier.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      740 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedIndicatorLED.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      613 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedInitiatorMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      712 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedLabelReader.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      683 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      658 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      669 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProcessorMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      896 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProtocolController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1100 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedRemainingExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      701 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedResourcePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      675 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1430 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyCurrentSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1426 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyVoltageSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      617 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedTargetMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2644 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AsymmetricAccessibility.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      814 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BIOSLoadedInNV.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1611 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BasedOnView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7658 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Battery.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1352 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BinarySensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5963 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16190 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1348 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifestCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15507 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10568 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStorageStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      300 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CDROMDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      308 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CableModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5544 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CacheMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10184 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CallBasedModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1503 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ChangerDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      685 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CollectionOfSensors.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1075 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4386 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtentBasedOn.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1173 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1209 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemProcessor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5728 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ConfigurationReportingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1055 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ConnectionBasedModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2544 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ControlledBy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3114 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Controller.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    46492 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ControllerConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      459 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CoolingDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3539 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CurrentSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      376 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DSLModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1213 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DVDDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DesktopMonitor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1804 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3840 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorCounts.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2073 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1396 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1364 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1794 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceServicesLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1218 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSharingCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2382 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSoftware.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1509 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiscreteSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2558 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9274 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskDriveView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      891 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5728 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      862 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionBasedOnVolume.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2994 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6604 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      306 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DisketteDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      304 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Display.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3844 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DisplayController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2220 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Door.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      971 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      671 2024-04-17 14:04:52.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToPhysicalElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      832 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DriveComponentViewView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      646 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DriveInDiskGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      251 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ESCONController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      878 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ElementStatisticalDataView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      649 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ElementStorageProtectionSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      705 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ErrorCountersForDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14648 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7180 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8707 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      829 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ExtentComponentView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      751 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ExtentInDiskGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCActiveConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5244 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCAdapterEventCounters.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14817 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2304 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2780 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortRateStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2343 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10378 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2310 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2010 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4377 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCTopologyView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      544 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FailoverStorageExtentsCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4093 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Fan.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16147 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibreChannelAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11617 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7332 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortActiveLogin.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4346 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortEventCounters.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1256 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortOnFCAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      504 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibreProtocolService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1978 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemGroupSynchronized.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15133 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    57887 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8796 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemSynchronized.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1723 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FlatPanel.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1661 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GPTDiskPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1572 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GenericDiskPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      724 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupInDiskGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6786 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13492 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      437 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HDSLModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2446 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HardwareThread.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      266 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HeatPipe.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      784 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      803 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePoolView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1713 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IBSubnetManager.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      247 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IDEController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      322 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ISDNModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8447 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLED.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4813 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLEDCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      265 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InfraredController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2598 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorTargetLogicalUnitPath.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      810 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InstalledPartitionTable.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1669 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InterLibraryPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1072 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Keyboard.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    26624 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5396 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1776 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReader.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      780 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1848 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      982 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LibraryExchange.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      751 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LibraryPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2546 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LimitedAccessPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4298 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDisk.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      888 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1414 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      774 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolume.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      692 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolumeSet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2463 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2758 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      878 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1429 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1651 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1191 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      318 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MagnetoOpticalDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      337 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ManagementController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6859 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MappingProtocolControllerView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      904 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3258 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingExposedDeviceView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6469 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11413 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1831 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3236 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2885 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      906 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaPresent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      391 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaTransferDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8502 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Memory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2896 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4590 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2000 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3298 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6354 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryError.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      288 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Modem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      585 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ModulePort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2998 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MonitorResolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      623 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MonitorSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      256 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MultiStateSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4282 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2779 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapterRedundancyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3953 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1891 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1455 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1222 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1404 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkVirtualAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2444 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NonVolatileStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17045 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NumericSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      751 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1341 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      770 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5259 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1236 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifestCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2019 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2610 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9699 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1435 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OwningPrintQueue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5177 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIBridge.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5367 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2709 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      641 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      355 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIPortGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      598 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIeSwitch.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      252 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCMCIAController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCVideoController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1050 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PExtentRedundancyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5890 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_POTSModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1553 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PSExtentBasedOnPExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1098 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageAlarm.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1266 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageCooling.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      765 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1007 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageTempSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2120 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ParallelController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6669 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PassThroughModule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1934 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2667 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      521 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespace.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2446 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespaceSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4008 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2585 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PhysicalExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1570 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      819 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerForChanger.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      704 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerLabelReader.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1012 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2144 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1531 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PointingDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1035 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortActiveConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1480 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      921 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortImplementsEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      548 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortOnDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4896 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerAllocationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1386 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerSource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8530 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerSupply.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1281 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3227 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      614 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PoweredStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14294 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintInputTray.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10421 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintInterpreter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16592 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintJob.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      618 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintJobFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11200 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintMarker.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9040 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintQueue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1490 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9679 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13255 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintSupply.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    41074 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Printer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5050 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      560 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingJob.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      661 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingQueue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9362 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Processor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      867 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2964 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCore.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2890 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedExtentBasedOn.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2407 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedSpaceExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      710 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2546 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerAccessesUnit.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2369 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      839 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2415 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnit.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnitView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17354 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerMaskingCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4889 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueryStatisticsCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      850 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueueForPrintService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      670 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueueForwardsToPrintSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1288 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizedOnSide.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      993 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesAggregatePExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1178 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesDiskPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1276 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      969 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesPExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      704 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesTapePartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      276 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Refrigeration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RemoteReplicationCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RemoteResources.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16317 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPairView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      956 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPoolForStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4653 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationEntity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2638 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)   128552 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)   117170 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16588 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1584 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SASPHY.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      565 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SASPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2022 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SBProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1704 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIArbitraryLogicalUnit.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2986 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3575 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInitiatorTargetLogicalUnitPath.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4807 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInterface.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10438 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5062 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7724 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIPathConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIProtocolController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7797 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSITargetPortGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      374 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SDSLModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      295 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SSAController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      262 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Scanner.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5533 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Sensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2532 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SerialController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1643 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SerialInterface.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4823 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SharedDeviceManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4182 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SharingDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2570 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Snapshot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1113 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SnapshotOfExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3688 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11151 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1329 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      590 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    22826 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    24631 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    53704 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      753 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageDefect.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7281 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17467 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      779 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementDriveDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1117 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1780 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      738 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1347 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageError.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5591 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibrary.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1135 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibraryCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17395 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      995 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      939 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2326 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12366 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2092 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProcessorAffinity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1792 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4582 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2649 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15541 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageRelocationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    18051 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageReplicationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1246 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageResourceLoadGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4497 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageServerAsymmetryCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    33857 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2923 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingWithHints.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1399 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsAssociatedToCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2117 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsGeneratedFromCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9144 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSynchronized.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3409 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageTier.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3371 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageTierCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7330 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageVolume.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      852 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SuppliesPower.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6097 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SynchronizationAspect.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1775 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SystemRegistrationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1054 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Tachometer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapeDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      470 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapeDriveResourceUsage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1287 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapePartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      790 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapePartitionOnSurface.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1368 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TargetMaskingGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1636 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TargetPortGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3459 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TemperatureSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4792 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13151 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6505 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6702 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15988 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5569 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6666 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      587 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1481 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      638 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBControllerHasHub.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9018 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      792 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBHub.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1913 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      610 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBPortOnHub.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12242 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Unimodem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4697 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_UninterruptiblePowerSupply.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      586 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_UserDevice.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      384 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VDSLModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10011 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLResourceUsage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1485 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    24235 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2101 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTOCDiskPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6015 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoController.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4133 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoControllerResolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3298 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoHead.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3382 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoHeadResolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      983 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      867 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ViewCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1157 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolatileStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3373 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VoltageSensor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2802 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1757 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSetBasedOnPSExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14567 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5249 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WBEMServerDeviceRegistrationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      298 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WORMDrive.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      726 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnModem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      743 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3818 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Watchdog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2654 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1237 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13391 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1383 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiRadio.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2436 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Zone.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2514 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1482 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneMembershipSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    19989 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1186 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneSet.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.611572 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/
+-rw-r--r--   0 maiera     (501) staff       (20)    10175 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AbstractIndicationSubscription.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16025 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AlertIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1056 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AlertInstIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      288 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassCreation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      286 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassDeletion.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      829 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      722 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassModification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2938 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      773 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollectionSubscription.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5261 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FormattedIndicationSubscription.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11244 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_Indication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9189 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationFilter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      825 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandler.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      827 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandlerCIMXML.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3418 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3119 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3689 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1222 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationSubscription.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      267 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstCreation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      273 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstDeletion.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1402 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2702 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstMethodCall.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1560 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstModification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      277 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstRead.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4499 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestination.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      702 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationCIMXML.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4901 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationWSManagement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      565 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ProcessIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6625 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_SNMPTrapIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1575 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ThresholdIndication.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.632877 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/
+-rw-r--r--   0 maiera     (501) staff       (20)     1705 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedProposal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1976 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedTransform.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3506 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7502 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEProposal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2021 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKERule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4332 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1227 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1356 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      526 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecProposal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      378 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecRule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      375 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTransportAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      874 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTunnelAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1040 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PacketConditionInSARule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1140 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForPreconfiguredTunnel.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForTunnel.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2884 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredSAAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      574 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTransportAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1065 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTunnelAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      690 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_RuleThatGeneratedSA.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      808 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3268 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SANegotiationAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1125 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAProposal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1664 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SARule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1700 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAStaticAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2293 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_TransformOfPreconfiguredAction.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.663066 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/
+-rw-r--r--   0 maiera     (501) staff       (20)     6105 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMOMStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      887 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5780 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCommunicationMechanism.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1230 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForManager.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1317 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForObjectManagerAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1043 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ElementConformsToProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    19379 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Error.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4805 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_GenericOperationCapabilitiesStructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      720 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_IdentificationOfManagedSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2785 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Message.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4764 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Namespace.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      879 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_NamespaceInManager.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3807 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManager.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3433 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7932 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerCommunicationMechanism.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2132 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ProtocolAdapter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3315 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_QueryCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      641 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      773 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedSpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15774 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6997 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSpecification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      485 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSubProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1449 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SchemaInformationStructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      980 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SubProfileRequiresProfile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3807 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SystemIdentification.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1836 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SystemInNamespace.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1959 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMProtocolServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2370 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      721 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3343 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerNamespace.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      565 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      857 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WSManagementCapabilities.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.684516 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/
+-rw-r--r--   0 maiera     (501) staff       (20)     2572 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricDefinition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1669 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricValue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10859 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricDefinition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7001 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricValue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      851 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementPerformsUoW.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      898 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementUnitOfWorkDef.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1706 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefForME.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1446 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefinition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      613 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricForME.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1089 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricInstance.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    28010 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6084 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      672 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_StartedUoW.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1458 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoW.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1181 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoWDef.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5035 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_TraceLevelType.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6450 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2998 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWorkDefinition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      916 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWDefTraceLevelType.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1295 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetric.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      948 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetricDefinition.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.937493 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/
+-rw-r--r--   0 maiera     (501) staff       (20)     1150 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AFRelatedServices.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2601 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AFService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2037 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AHTransform.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      791 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ASBGPEndpoints.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1817 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ATAProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3752 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AdministrativeDistance.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2773 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AllocationSchedulingElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1403 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AreaOfConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      914 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AssociatedNextHop.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5316 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AutonomousSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1326 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AverageRateMeterService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      862 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAdminDistance.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4460 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1915 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributesForRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1242 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPCluster.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      695 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPClustersInAS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3109 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPEndpointStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1779 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPIPRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6647 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPathAttributes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3872 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      657 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroupService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1067 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerUsesRouteMap.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9078 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4194 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMap.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1085 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMapsInRoutingPolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      689 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRoutingPolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3063 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1213 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceAttributes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1096 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3677 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1111 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BindsToLANEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BoundedPrioritySchedulingElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3331 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BufferPool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2565 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4829 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5269 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1358 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculatedRoutes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1205 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculatesAmong.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      910 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculationBasedOnQueue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1046 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculationServiceForDropper.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1613 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1734 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementInClassifierService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementUsesFilterList.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2324 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierFilterSet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1742 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      651 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CollectedBufferPool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2208 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2352 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningServiceOnEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1585 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Confederation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1596 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1664 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityMembershipSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4706 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7366 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11421 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSGeneralSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3041 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3033 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1079 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DSCPMarkerService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2073 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DiffServService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2059 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DropThresholdCalculationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4437 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DropperService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2363 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DynamicForwardingEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1506 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EFService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1432 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EGPRouteCalcDependency.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4478 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ESPTransform.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1928 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EWMAMeterService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1489 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EgressConditioningServiceOnEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ElementInSchedulingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      742 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointForIPNetworkConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1150 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      597 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInArea.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      610 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInLink.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1382 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointOfNetworkPipe.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EntriesInFilterList.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1644 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ExtendedStaticIPAssignmentSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1473 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FailNextScheduler.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4085 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2477 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryBase.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1385 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3365 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterList.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1274 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterListInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      639 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterListsInBGPRouteMap.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      795 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterOfSecurityAssociation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      774 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilteredBGPAttributes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      623 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FlowService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1024 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardedRoutes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2643 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      753 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardsAmong.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4677 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021Filter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1490 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021PService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1265 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropQueueBinding.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1107 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropper.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      824 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedAdminDistance.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      752 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPAttributes.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      741 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPPeerGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      732 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPRouteMap.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      791 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterEntryBase.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      707 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterList.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedForwardingServices.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      765 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedNetworkPipe.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      688 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      813 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingPolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1137 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingServices.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1397 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10938 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5622 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IKESAEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3009 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPAddressRange.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3995 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPAssignmentSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2042 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPCOMPTransform.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10047 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1406 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPConnectivitySubnet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13624 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPHeadersFilter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2794 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPInterfaceSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      802 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPNetworkConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5400 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5504 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4511 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPSOFilterEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1784 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPSubnet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      912 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPVersionSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      427 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPXConnectivityNetwork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      723 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPXNetwork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1009 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPXProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1613 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPsecSAEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      666 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InBGPPeerGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1201 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InLogicalNetwork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1097 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InSegment.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3689 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InboundVLAN.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1315 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IngressConditioningServiceOnEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1772 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_KVMRedirectionSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1536 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANConnectivitySegment.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2912 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1915 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANSegment.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      941 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ListsInRoutingPolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3497 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetwork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1228 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetworkService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1544 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MarkerService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4853 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2916 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3002 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MeterService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      833 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NamedAddressCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1625 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Network.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4950 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipe.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2873 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipeComposition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2272 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPortConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3131 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1288 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkServicesInAdminDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2295 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkVLAN.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1270 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworksInAdminDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1593 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopIPRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3565 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRoute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2315 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRouting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1332 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextScheduler.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1289 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1182 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterClassifierElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1911 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterMeter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      538 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NonWorkConservingSchedulingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1650 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFArea.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4487 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFAreaConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1674 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFLink.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1947 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2668 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpointBase.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2453 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1013 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1597 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      705 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFVirtualInterface.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1470 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OutboundVLAN.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2580 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PacketSchedulingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3071 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PeerIDPayloadFilterEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      587 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PeerOfSAEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      840 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Phase1SAUsedForPhase2.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2399 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PreambleFilter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1963 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PreambleMarkerService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1557 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PrecedenceService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1076 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Priority8021QMarkerService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1589 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PrioritySchedulingElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1443 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ProtocolServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      980 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSConditioningSubService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2019 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1405 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSSubService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1260 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueAllocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1502 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueHierarchy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1260 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueToSchedule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1204 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueuingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4452 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_REDDropperService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1424 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RangeOfIPAddresses.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1330 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RangesOfConfiguration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3691 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      695 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      761 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorClientService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      760 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorNonClientService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      756 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      788 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RelatedSpanningTree.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1146 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RelatedTransparentBridgingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1433 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RemoteAccessAvailableToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1832 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteCalculationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1718 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteForwardedByService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      700 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteUsesEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2349 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInAS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      853 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInBGPCluster.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      776 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutesBGP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5751 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingPolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      866 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomain.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      649 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomainInAS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      963 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointConnectionStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1327 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointRefreshSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3135 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SATransform.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3388 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SCSIProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2389 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPCommunityString.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      679 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1518 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPTrapTarget.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2316 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5116 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4891 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1497 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulerUsed.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3489 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingServiceToSchedule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2977 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SecurityAssociationEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      982 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SourceRoutingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5559 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      862 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      656 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Specific802dot1QVLANService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2675 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_StaticForwardingEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2979 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_StaticIPAssignmentSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      589 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPort.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      645 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortDynamicForwarding.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1407 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortPair.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4063 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRouting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4190 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRoutingStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3169 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTree.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      618 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTreeStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      622 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStaticForwarding.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      934 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1479 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortTransparentBridgingStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2197 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      743 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSourceRouting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      738 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSpanningTree.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      764 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceTransparentBridging.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      892 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceVLAN.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      968 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Switchable.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      596 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchesAmong.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      834 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TCPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2297 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4910 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4595 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1865 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1492 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1107 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ToSMarkerService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2359 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TokenBucketMeterService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      740 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransformOfSecurityAssociation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      787 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingDynamicForwarding.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      827 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      764 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStaticForwarding.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      712 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      694 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TrapSourceForSNMPService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      752 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_UDPProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9603 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2218 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12184 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3326 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLAN.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9347 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1409 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2686 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      640 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANFor.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3076 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANNetwork.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      922 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2445 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WRRSchedulingElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2914 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WeightedREDDropperService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12092 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6116 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9101 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2407 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiNetworkDetectionSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2851 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_X509CredentialFilterEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4024 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSICapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1435 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9241 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5713 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6941 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnectionSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8132 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSILoginStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2564 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIProtocolEndpoint.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7534 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISession.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2836 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionFailures.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6343 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1954 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionStatistics.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:08.980075 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/
+-rw-r--r--   0 maiera     (501) staff       (20)     1206 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_AdjacentSlots.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4011 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Card.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      721 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_CardInSlot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1481 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_CardOnCard.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7297 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Chassis.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1191 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ChassisInRack.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1048 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Chip.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6292 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConfigurationCapacity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      765 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectedTo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      763 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectorOnPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1487 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Container.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1023 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ContainerView.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      799 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Docked.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      867 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementCapacity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      729 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementInConnector.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      581 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementsLinked.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1148 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_HomeForMedia.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      730 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_LinkHasConnector.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2609 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Magazine.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1617 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3760 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2149 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryCapacity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      742 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryOnCard.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      673 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryWithMedia.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      756 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInChassis.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      994 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInConnector.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      847 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInSlot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1335 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1085 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackagedComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      567 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ParticipatesInSet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      945 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalAssetCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1178 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalCapacity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3770 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9406 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalConnector.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3775 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalFrame.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2256 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalLink.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8561 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMedia.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1641 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMediaInLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5079 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMemory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10134 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2212 2024-04-17 14:04:53.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalTape.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1697 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Rack.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      761 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ReplacementSet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6799 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Slot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1933 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_SlotInSlot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5917 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_StorageMediaLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2680 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_SystemBusCard.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.029184 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/
+-rw-r--r--   0 maiera     (501) staff       (20)     2227 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AcceptCredentialFrom.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      795 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AccountAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      848 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1003 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationRule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1533 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_BiometricAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2358 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      868 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1565 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_DocumentAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1094 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ElementInPolicyRoleCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1219 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_FilterOfPacketCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      602 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_KerberosAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6693 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_MethodAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1769 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkPacketAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      833 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkingIDAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1869 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PacketFilterCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1551 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PhysicalCredentialAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1880 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_Policy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3893 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      844 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1790 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRepository.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1743 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2861 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionStructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      800 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3814 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1127 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1829 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRepository.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1036 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2445 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionStructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      836 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyContainerInPolicyContainer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1327 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInPolicyGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      676 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1454 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      927 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepository.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1312 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepositoryInPolicyRepository.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3858 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      727 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollectionInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8585 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRule.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1151 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInPolicyGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      670 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1755 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleValidityPeriod.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4585 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySet.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1083 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetAppliesToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1835 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      830 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInRoleCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1477 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2410 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetValidityPeriod.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15588 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyTimePeriodCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      878 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PublicPrivateKeyAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3928 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_QueryCondition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      789 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_RejectConnectionAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      752 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      646 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicyContainer.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      872 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_SharedSecretAuthentication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1651 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyAction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1695 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyCondition.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.082167 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/
+-rw-r--r--   0 maiera     (501) staff       (20)     1737 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Activity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      483 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ActivityContact.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      530 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ActivityResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      556 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ActivityTransaction.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1200 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Address.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      482 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AddressLocation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      580 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdminAssociation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3197 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Administrative.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      558 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeContact.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      560 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeRevision.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      591 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Agreement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      506 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Attached.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2139 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Attachment.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      899 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Categorization.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1209 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Category.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      603 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_CategoryParentChild.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      419 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Contact.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      959 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactContactItem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      386 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactItem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      495 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactItemAddress.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      525 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactOrganization.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      501 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactPerson.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2339 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ExchangeElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      794 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Expression.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      403 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      735 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionLink.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1294 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Feature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      590 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_FeatureResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      562 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Location.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      461 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Organization.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1074 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Person.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1099 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Problem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      745 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Product.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      654 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductAsset.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      677 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1170 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductParentChild.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      532 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Reference.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      937 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Resolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      476 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ResolutionResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      817 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Resource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2295 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Revision.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      506 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_RevisionContact.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10185 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SISService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      548 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceActivity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      528 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceAgreement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3520 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceIncident.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      602 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProblem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      572 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProvider.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      766 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceRequester.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      685 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceResolutionSolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1797 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Solution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      640 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionCategory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      760 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      626 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionExpression.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      918 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionHasElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      596 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionProblem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      617 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionReference.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      620 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionResolution.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4283 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Statement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      468 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_StatementFeature.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2115 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Transaction.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.277534 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/
+-rw-r--r--   0 maiera     (501) staff       (20)     2097 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AffectedJobElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      873 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AllocatedDMA.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      628 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AllocatedResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      934 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AssociatedFileSystemStatisticsManifestCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      685 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AssociatedJobMethodResult.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2010 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AvailableDiagnosticService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5015 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSAttribute.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1619 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSEnumeration.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1792 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSInteger.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2786 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSPassword.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    24356 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2363 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2335 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSString.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3632 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootConfigSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      773 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootOSFromFS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      258 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11057 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      571 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootServiceAccessBySAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6172 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1981 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3277 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootSourceSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5484 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CIFSSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      988 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CIFSShare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2086 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Cluster.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      616 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ClusterServiceAccessBySAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      280 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ClusteringSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1969 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ClusteringService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2168 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComponentCS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9819 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      669 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemDMA.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      652 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemIRQ.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      718 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemMappedIO.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1595 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemNodeCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      913 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      680 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      646 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingDataRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      636 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingsRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4549 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DMA.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      303 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DataFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      903 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DefaultElementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      626 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DeviceAccessedByFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      531 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DeviceFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2270 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticCompletionRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      643 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4800 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14007 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResult.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      802 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForMSE.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      813 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1151 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultInPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6099 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7866 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1896 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceJobCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3806 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    21804 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16506 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      611 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingDataRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      958 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingForTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7268 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      774 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSubTestRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    18382 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2858 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestForMSE.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1271 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestInPackage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      897 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticsLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      355 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Directory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      649 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DirectoryContainsFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1966 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4538 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5779 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      774 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Export.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     8651 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13000 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1301 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5961 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3776 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticTest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      843 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FIFOPipeFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1461 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSDomainIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      479 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSIPInterfaceSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      494 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      779 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToPrincipal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      741 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToTree.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3987 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6329 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaConfigEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2170 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaIndication.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12452 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5190 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaReportRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4426 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileExportCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    28439 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileExportService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      916 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7631 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2606 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    18483 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2607 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerSettings.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1050 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileShare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      714 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileShareSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      688 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10207 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    16452 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2548 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    33217 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    17873 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1929 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15481 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticalData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2537 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    25622 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifest.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1400 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifestCollection.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    11333 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5670 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HelpService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1250 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HelpServiceAvailableToFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      911 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedBootSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      764 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedBootService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      930 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      916 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      752 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedFileSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      984 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedJobDestination.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1872 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedShare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      626 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostingCS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3254 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_IRQ.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1230 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_InstalledOS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1554 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobDestination.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      619 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobDestinationJobs.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2877 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobQueue.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9492 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1702 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LastAppliedSnapshot.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocalAccessAvailableToFS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6206 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocalFileSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7236 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    19865 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemSetting.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3903 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Log.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4482 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogEntry.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      794 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInDataFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      894 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInDeviceFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1109 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInStorage.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      524 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogManagesRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2823 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      682 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogToLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4441 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogicalFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2029 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MemoryMappedIO.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      805 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MemoryResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    26072 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MessageLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3802 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MethodResult.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1544 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Mount.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3230 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2151 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFSSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      839 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFSShare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      723 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NISSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4911 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OOBAlertService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      714 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OSProcess.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    13462 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1567 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystemCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      784 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperationLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1067 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OwningJobElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2003 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ParticipatingCS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6261 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2364 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogServiceCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      803 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PortResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6393 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Process.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      624 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessExecutable.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1101 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessOfJob.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      665 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessThread.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      786 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordAppliesToElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5139 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordForLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      576 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordInLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2311 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1008 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordLogCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      751 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RemoteFileSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      585 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ReportRecord.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      814 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResidesOnExtent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      711 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResourceAllocationFromPool.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      749 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResourceOfSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      858 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RunningOS.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      903 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SAPAvailableForFileShare.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2329 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ServiceProcess.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1462 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SettingAssociatedToCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2307 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Share.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      964 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SharedElement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1059 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SnapshotOfVirtualSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3154 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SummaryDiagnostics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      599 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SymbolicLink.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1540 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SystemPartition.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1235 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SystemResource.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3872 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Thread.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    10122 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_TimeZone.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4014 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnitaryComputerSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1477 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixDeviceFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      736 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixDirectory.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5741 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixFile.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1602 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixLocalFileSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2943 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcess.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4607 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatisticalInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      724 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatistics.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2630 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixThread.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      971 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UseOfLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      674 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UseOfMessageLog.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      617 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualComputerSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5785 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemMigrationSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    12628 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1153 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingDataComponent.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2350 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_WakeUpService.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.380642 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/
+-rw-r--r--   0 maiera     (501) staff       (20)     5088 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccessControlInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14806 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Account.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1034 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5433 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7068 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1169 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountMapsToAccount.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      770 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountOnSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3473 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      634 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AssignedIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    14648 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AssociatedPrivilege.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1032 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticateForUse.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3321 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationRequirement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      731 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1405 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationTarget.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      394 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1159 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationSubject.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1311 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationTarget.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      863 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedPrivilege.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1253 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedSubject.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      657 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedTarget.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      930 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedUse.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      821 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CAHasPublicCertificate.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1348 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CASignsPublicKeyCertificate.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2650 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateAuthority.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4098 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    32809 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      763 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CollectionInOrganization.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1100 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CollectionInSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2489 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Credential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3060 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialContext.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3946 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      413 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementSAP.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      334 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3012 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialStore.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1704 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ElementAsUser.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      681 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ElementSecuritySensitivity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1684 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_GatewayPathID.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2250 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Group.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1162 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_HostedACI.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1126 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_HostedAuthenticationRequirement.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      913 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IKESecretIsNamed.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2306 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IPNetworkIdentity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5014 2024-04-17 14:04:54.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Identity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      817 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IdentityContext.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      311 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IdentityManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      863 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KDCIssuesKerberosTicket.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3363 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      543 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosKeyDistributionCenter.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2702 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosTicket.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7759 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KeyBasedCredentialManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1532 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Keystore.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      404 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_LocalCredentialManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      950 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_LocallyManagedPublicKey.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      795 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagedCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      606 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccount.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1132 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccountOnSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2291 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MemberPrincipal.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      649 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreGroupInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      662 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreOrgUnitInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      696 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreOrganizationInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      654 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MorePersonInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      641 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreRoleInfo.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4052 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NamedCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3679 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NamedSharedIKESecret.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1903 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Notary.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1257 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NotaryVerifiesBiometric.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1249 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OpaqueManagementDataOwner.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      862 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OrgStructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2911 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OrgUnit.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3030 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Organization.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      344 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OrganizationalEntity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3293 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherGroupInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6126 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherOrgUnitInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7376 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherOrganizationInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15051 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherPersonInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6173 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherRoleInformation.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4031 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Person.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9572 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Privilege.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4145 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    15814 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1940 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyCertificate.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      403 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2208 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PublicPrivateKeyPair.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1478 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RequireCredentialsFrom.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4260 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Role.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9766 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedAuthorizationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1279 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedManagementCapabilities.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      779 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleLimitedToTarget.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     6065 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecuritySensitivity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      254 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecurityService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1077 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceForSystem.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      606 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceUsesAccount.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      800 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ServiceUsesSecurityService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3208 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2688 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecret.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      818 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretIsShared.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1030 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3698 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SignedCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3585 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageClientSettingData.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1267 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareID.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     9721 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareIDManagementService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      663 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministrator.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      615 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorGroup.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      577 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorRole.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      788 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_TrustHierarchy.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2948 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UnsignedCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2715 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UnsignedPublicKey.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     3191 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UserContact.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      331 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UserEntity.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2822 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersAccess.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1030 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersAccount.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1122 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersCredential.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      463 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_VerificationService.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2745 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509CRL.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     7494 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509Certificate.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     4071 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509Infrastructure.mof
+-rw-r--r--   0 maiera     (501) staff       (20)    92023 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/cim_schema_2.49.0.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5668 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/qualifiers.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1299 2024-04-17 14:04:55.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/qualifiers_optional.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      380 2024-04-17 13:52:37.000000 pywbem-1.7.1/tests/schema/mofFinal2.49.0/test_partial_schema.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.381764 pywbem-1.7.1/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.383071 pywbem-1.7.1/tests/unittest/end2endtest_utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/end2endtest_utils/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.384752 pywbem-1.7.1/tests/unittest/functiontest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/functiontest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2251 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/functiontest/test_conftest.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.427500 pywbem-1.7.1/tests/unittest/pywbem/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2024-04-17 13:52:39.000000 pywbem-1.7.1/tests/unittest/pywbem/moflog.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2024-04-17 13:52:39.000000 pywbem-1.7.1/tests/unittest/pywbem/moflog2.txt
+-rw-r--r--   0 maiera     (501) staff       (20)     5002 2022-03-09 17:42:38.000000 pywbem-1.7.1/tests/unittest/pywbem/test.mof
+-rwxr-xr-x   0 maiera     (501) staff       (20)    35002 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_cim_http.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)  1334024 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_cim_obj.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    46272 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_cim_operations.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    45416 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_cim_types.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)   130414 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_cim_xml.py
+-rw-r--r--   0 maiera     (501) staff       (20)    14912 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_exceptions.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    38707 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_indicationlistener.py
+-rw-r--r--   0 maiera     (501) staff       (20)   103399 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_itermethods.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    19785 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_logging.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)   115625 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_mof_compiler.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     5335 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_nocasedict.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     5585 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_perf_equality.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)   112392 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_recorder.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    23026 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_statistics.py
+-rw-r--r--   0 maiera     (501) staff       (20)    86377 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_subscriptionmanager.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)   469334 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_tupleparse.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    30974 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_tupletree.py
+-rw-r--r--   0 maiera     (501) staff       (20)    24429 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_units.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21935 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)    37379 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_valuemapping.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4352 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_warnings.py
+-rw-r--r--   0 maiera     (501) staff       (20)    16961 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem/test_wbemserverclass.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.434950 pywbem-1.7.1/tests/unittest/pywbem/testmofs/
+-rw-r--r--   0 maiera     (501) staff       (20)     1372 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error01.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1349 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error02.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      889 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error03.mof
+-rw-r--r--   0 maiera     (501) staff       (20)       76 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error04.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     5668 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/qualifiers.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     2431 2022-03-30 06:07:16.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/test_instance.mof
+-rw-r--r--   0 maiera     (501) staff       (20)     1338 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/test_refs.mof
+-rw-r--r--   0 maiera     (501) staff       (20)      462 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem/testmofs/test_types.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.443715 pywbem-1.7.1/tests/unittest/pywbem_mock/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3065 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/conftest.py
+-rw-r--r--   0 maiera     (501) staff       (20)    39127 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_complexassoc.py
+-rw-r--r--   0 maiera     (501) staff       (20)    28707 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_inmemory_repository.py
+-rw-r--r--   0 maiera     (501) staff       (20)    64912 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_multi_ns_assoc.py
+-rw-r--r--   0 maiera     (501) staff       (20)    13646 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_providerdependentregistry.py
+-rw-r--r--   0 maiera     (501) staff       (20)    13623 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_providerregistry.py
+-rw-r--r--   0 maiera     (501) staff       (20)    19122 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_system_providers.py
+-rw-r--r--   0 maiera     (501) staff       (20)   423818 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/pywbem_mock/test_wbemconnection_mock.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.447461 pywbem-1.7.1/tests/unittest/resourcetest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-11-09 03:23:37.000000 pywbem-1.7.1/tests/unittest/resourcetest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7498 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/resourcetest/test_memory_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2493 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/simple_mock_model.mof
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.448750 pywbem-1.7.1/tests/unittest/unittest_utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/unittest_utils/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-18 09:04:09.454848 pywbem-1.7.1/tests/unittest/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2022-03-09 17:32:21.000000 pywbem-1.7.1/tests/unittest/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3031 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/dmtf_mof_schema_def.py
+-rw-r--r--   0 maiera     (501) staff       (20)     9047 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/pytest_extensions.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1886 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/unichr2.py
+-rw-r--r--   0 maiera     (501) staff       (20)    14313 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/unittest_extensions.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)     8737 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/validate.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21400 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/unittest/utils/wbemserver_mock.py
+-rw-r--r--   0 maiera     (501) staff       (20)    11719 2024-04-18 06:23:07.000000 pywbem-1.7.1/tests/utils.py
```

### Comparing `pywbem-1.7.0/INSTALL.md` & `pywbem-1.7.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/LICENSE.txt` & `pywbem-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/MANIFEST.in` & `pywbem-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/PKG-INFO` & `pywbem-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywbem
-Version: 1.7.0
+Version: 1.7.1
 Summary: pywbem - A WBEM client
 Home-page: https://pywbem.github.io/pywbem/
 Author: Tim Potter
 Author-email: tpot@hp.com
 Maintainer: Andreas Maier, Karl Schopmeyer
 Maintainer-email: maiera@de.ibm.com, k.schopmeyer@swbell.net
 License: LGPL version 2.1, or (at your option) any later version
```

### Comparing `pywbem-1.7.0/README.md` & `pywbem-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/README_PYPI.md` & `pywbem-1.7.1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/build_moftab.py` & `pywbem-1.7.1/build_moftab.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/mof_compiler` & `pywbem-1.7.1/mof_compiler`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/__init__.py` & `pywbem-1.7.1/pywbem/__init__.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_constants.py` & `pywbem-1.7.1/pywbem/_cim_constants.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_http.py` & `pywbem-1.7.1/pywbem/_cim_http.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_obj.py` & `pywbem-1.7.1/pywbem/_cim_obj.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_operations.py` & `pywbem-1.7.1/pywbem/_cim_operations.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_types.py` & `pywbem-1.7.1/pywbem/_cim_types.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cim_xml.py` & `pywbem-1.7.1/pywbem/_cim_xml.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_cliutils.py` & `pywbem-1.7.1/pywbem/_cliutils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_exceptions.py` & `pywbem-1.7.1/pywbem/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_features.py` & `pywbem-1.7.1/pywbem/_features.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_listener.py` & `pywbem-1.7.1/pywbem/_listener.py`

 * *Files 7% similar despite different names*

```diff
@@ -851,19 +851,17 @@
         self._https_thread = None  # Thread for HTTPS
 
         self._logger = logging.getLogger(
             _format("pywbem.listener.{0}", id(self)))
 
         self._callbacks = []  # Registered callback functions
 
-        # Set up callback queue and callback thread.
-        self.rcvd_indication_queue = queue.Queue()
-        self.callback_thread = StoppableThread(
-            target=self.deliver_indications_from_queue,
-            args=(self.rcvd_indication_queue,))
+        # define callback queue and callback thread.
+        self.rcvd_indication_queue = None
+        self.callback_thread = None
 
     def __str__(self):
         """
         Return a representation of the :class:`~pywbem.WBEMListener` object
         with a subset of its attributes.
         """
         return _format(
@@ -997,14 +995,30 @@
         where `{id}` is a unique string for each listener object.
 
         Users of the listener should not look up the logger object by name, but
         should use this property to get to it.
         """
         return self._logger
 
+    def stop_callback_thread(self):
+        """
+        Stop the indication delivery thread and queue and eliminate them. This
+        allows the delivery of indications already in the queue. and then
+        closes the thread and queue.
+        """
+        assert self.callback_thread
+        assert self.rcvd_indication_queue
+        self.logger.info("Stopping queued delivery")
+        self.callback_thread.stop()
+        self.logger.info("Joining queued delivery")
+        self.callback_thread.join()
+        self.logger.info("Join finished threaded Deliver queue")
+        self.callback_thread = None
+        self.rcvd_indication_queue = None
+
     def start(self):
         """
         Start the WBEM listener threads, if they are not yet running.
 
         A thread serving CIM-XML over HTTP is started if an HTTP port was
         specified for the listener.
         A thread serving CIM-XML over HTTPS is started if an HTTPS
@@ -1034,26 +1048,34 @@
           :exc:`pywbem.ListenerPortError`: WBEM listener port is already
             in use.
           :exc:`pywbem.ListenerPromptError`: Error when prompting for the
             password of the private key file when using HTTPS.
           :exc:`py:OSError`: Other error
           :exc:`py:IOError`: Other error (Python 2.7 only)
         """
-        # Start delivery queue
-        self.callback_thread.start()
-        self.logger.info("Callback queue thread started")
+        # Start delivery queue and thread if not started
+        if not self.callback_thread:
+            self.rcvd_indication_queue = queue.Queue()
+            self.callback_thread = StoppableThread(
+                target=self.deliver_indications_from_queue,
+                args=(self.rcvd_indication_queue,))
+            # This insures that thread stops when process stopped
+            self.callback_thread.daemon = True
+            self.callback_thread.start()
+            self.logger.info("Callback queue thread started")
 
         if self._http_port:
             if not self._http_server:
                 self.logger.info("Starting threaded HTTP server on port %s",
                                  self._http_port)
                 try:
                     server = ThreadedHTTPServer((self._host, self._http_port),
                                                 ListenerRequestHandler)
                 except (IOError, OSError) as exc:
+                    self.stop_callback_thread()
                     # Linux/macOS on py2: socket.error (derived from IOError);
                     # Linux/macOS on py3: OSError;
                     # Windows does not raise any exception if port is used
                     if getattr(exc, 'errno', None) == errno.EADDRINUSE:
                         new_exc = ListenerPortError(
                             "WBEM listener port {0} is already in use".
                             format(self._http_port))
@@ -1083,14 +1105,15 @@
                 self.logger.info("Starting threaded HTTPS server on port %s",
                                  self._https_port)
 
                 try:
                     server = ThreadedHTTPServer((self._host, self._https_port),
                                                 ListenerRequestHandler)
                 except (IOError, OSError) as exc:
+                    self.stop_callback_thread()
                     # Linux/macOS on py2: socket.error (derived from IOError);
                     # Linux/macOS on py3: OSError;
                     # Windows does not raise any exception if port is used
                     if getattr(exc, 'errno', None) == errno.EADDRINUSE:
                         new_exc = ListenerPortError(
                             "WBEM listener port {0} is already in use".
                             format(self._https_port))
@@ -1170,15 +1193,15 @@
         else:
             # Just in case someone changed self._https_port after init...
             self._https_server = None
             self._https_thread = None
 
     def stop(self):
         """
-        Stop the WBEM listener threads, if they are running.
+        Stop the WBEM listener threads and callback thread, if they are running.
         """
 
         # Stopping the server will cause its `serve_forever()` method
         # to return, which will cause the server thread to terminate.
 
         if self._http_server:
             self.logger.info("Stopping threaded HTTP server")
@@ -1192,45 +1215,41 @@
             self.logger.info("Stopping threaded Queue")
             self._https_server.shutdown()
             self._https_server.server_close()
             self._https_server = None
             self._https_thread = None
             self.logger.info("Stopped threaded Queue")
 
-        self.logger.info("Stopping queued delivery")
-        self.callback_thread.stop()
-        self.logger.info("Joining queued delivery")
-        self.callback_thread.join()
-        self.logger.info("Join finished threaded Deliver queue")
+        if self.callback_thread:
+            self.stop_callback_thread()
 
     def deliver_indications_from_queue(self, delivery_queue):
         """
         Deliver indications from delivery_queue to the defined consumer. This
-        function runs a loop in its own thread and only exits the thread when
-        the listener is shut down (i.e. when the stop_event is set).
+        function runs a loop in its own thread and only returns when the
+        stop_event is set.
+
+        It delivers remaining indications in the queue before it returns.
 
         """
-        # queue get wait timeout in seconds. This is short because it impacts
+        # Queue get wait timeout in seconds. This is short because it impacts
         # time to stop the thread.
-        queue_timeout = 2
+        queue_get_timeout = 2
         self.logger.debug("Start deliver indications from queue.")
-        # NOTE: Loop continues to deliver queued indications until empty
-        #       even if the stop_event is set.
+        # Continues to deliver queued indications until empty after stop_event
+        # set.
         while True:
             try:
                 self.logger.debug("Get from queue. %d in queue",
                                   delivery_queue.qsize())
                 indication_tuple = delivery_queue.get(block=True,
-                                                      timeout=queue_timeout)
+                                                      timeout=queue_get_timeout)
                 # self.logger.debug("Got from queue")
                 self.deliver_indication_to_callback(indication_tuple[0],
                                                     indication_tuple[1])
-            # FUTURE: Should we be able to turn off this thread if there are
-            # no indications received for a defined time? Now just continues
-            # the receive process with wait loop.
             # FUTURE: add test for excessive indications in queue.
             # Probably stop and get out with some indication of problem.
             except queue.Empty:
                 self.logger.debug("Queue empty")
                 if self.callback_thread.stop_event.is_set():
                     self.logger.debug("Stop Deliver: stop_event set")
                     break
```

### Comparing `pywbem-1.7.0/pywbem/_logging.py` & `pywbem-1.7.1/pywbem/_logging.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_mof_compiler.py` & `pywbem-1.7.1/pywbem/_mof_compiler.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_moflextab.py` & `pywbem-1.7.1/pywbem/_moflextab.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_mofparsetab.py` & `pywbem-1.7.1/pywbem/_mofparsetab.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_nocasedict.py` & `pywbem-1.7.1/pywbem/_nocasedict.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_recorder.py` & `pywbem-1.7.1/pywbem/_recorder.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_server.py` & `pywbem-1.7.1/pywbem/_server.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_statistics.py` & `pywbem-1.7.1/pywbem/_statistics.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_subscription_manager.py` & `pywbem-1.7.1/pywbem/_subscription_manager.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_tupleparse.py` & `pywbem-1.7.1/pywbem/_tupleparse.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_tupletree.py` & `pywbem-1.7.1/pywbem/_tupletree.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_units.py` & `pywbem-1.7.1/pywbem/_units.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_utils.py` & `pywbem-1.7.1/pywbem/_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_valuemapping.py` & `pywbem-1.7.1/pywbem/_valuemapping.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocasedict/LICENSE` & `pywbem-1.7.1/pywbem/_vendor/nocasedict/LICENSE`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocasedict/_hashable.py` & `pywbem-1.7.1/pywbem/_vendor/nocasedict/_hashable.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocasedict/_keyableby.py` & `pywbem-1.7.1/pywbem/_vendor/nocasedict/_keyableby.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocasedict/_nocasedict.py` & `pywbem-1.7.1/pywbem/_vendor/nocasedict/_nocasedict.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocasedict/_utils.py` & `pywbem-1.7.1/pywbem/_vendor/nocasedict/_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocaselist/LICENSE` & `pywbem-1.7.1/pywbem/_vendor/nocaselist/LICENSE`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_vendor/nocaselist/_nocaselist.py` & `pywbem-1.7.1/pywbem/_vendor/nocaselist/_nocaselist.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/_version.py` & `pywbem-1.7.1/pywbem/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.devD": Development level D of a not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.7.0'
+__version__ = '1.7.1'
```

### Comparing `pywbem-1.7.0/pywbem/_warnings.py` & `pywbem-1.7.1/pywbem/_warnings.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem/config.py` & `pywbem-1.7.1/pywbem/config.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem.egg-info/PKG-INFO` & `pywbem-1.7.1/pywbem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywbem
-Version: 1.7.0
+Version: 1.7.1
 Summary: pywbem - A WBEM client
 Home-page: https://pywbem.github.io/pywbem/
 Author: Tim Potter
 Author-email: tpot@hp.com
 Maintainer: Andreas Maier, Karl Schopmeyer
 Maintainer-email: maiera@de.ibm.com, k.schopmeyer@swbell.net
 License: LGPL version 2.1, or (at your option) any later version
```

### Comparing `pywbem-1.7.0/pywbem.egg-info/SOURCES.txt` & `pywbem-1.7.1/pywbem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem.egg-info/requires.txt` & `pywbem-1.7.1/pywbem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/__init__.py` & `pywbem-1.7.1/pywbem_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_baseprovider.py` & `pywbem-1.7.1/pywbem_mock/_baseprovider.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_baserepository.py` & `pywbem-1.7.1/pywbem_mock/_baserepository.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_dmtf_cim_schema.py` & `pywbem-1.7.1/pywbem_mock/_dmtf_cim_schema.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_inmemoryrepository.py` & `pywbem-1.7.1/pywbem_mock/_inmemoryrepository.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_instancewriteprovider.py` & `pywbem-1.7.1/pywbem_mock/_instancewriteprovider.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_mainprovider.py` & `pywbem-1.7.1/pywbem_mock/_mainprovider.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_methodprovider.py` & `pywbem-1.7.1/pywbem_mock/_methodprovider.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_mockmofwbemconnection.py` & `pywbem-1.7.1/pywbem_mock/_mockmofwbemconnection.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_namespaceprovider.py` & `pywbem-1.7.1/pywbem_mock/_namespaceprovider.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_providerdependentregistry.py` & `pywbem-1.7.1/pywbem_mock/_providerdependentregistry.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_providerdispatcher.py` & `pywbem-1.7.1/pywbem_mock/_providerdispatcher.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_providerregistry.py` & `pywbem-1.7.1/pywbem_mock/_providerregistry.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_resolvermixin.py` & `pywbem-1.7.1/pywbem_mock/_resolvermixin.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_subscriptionproviders.py` & `pywbem-1.7.1/pywbem_mock/_subscriptionproviders.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_utils.py` & `pywbem-1.7.1/pywbem_mock/_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/_wbemconnection_mock.py` & `pywbem-1.7.1/pywbem_mock/_wbemconnection_mock.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/pywbem_mock/config.py` & `pywbem-1.7.1/pywbem_mock/config.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/requirements.txt` & `pywbem-1.7.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/setup.py` & `pywbem-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/test-requirements.txt` & `pywbem-1.7.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/README` & `pywbem-1.7.1/tests/README`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/__init__.py` & `pywbem-1.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/dtd/CIM_DTD_V22.dtd` & `pywbem-1.7.1/tests/dtd/CIM_DTD_V22.dtd`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/dtd/DSP0203_2.2.0.dtd` & `pywbem-1.7.1/tests/dtd/DSP0203_2.2.0.dtd`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/dtd/DSP0203_2.3.1.dtd` & `pywbem-1.7.1/tests/dtd/DSP0203_2.3.1.dtd`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/dtd/DSP0203_2.4.0.dtd` & `pywbem-1.7.1/tests/dtd/DSP0203_2.4.0.dtd`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/elapsed_timer.py` & `pywbem-1.7.1/tests/elapsed_timer.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/es_schema.yml` & `pywbem-1.7.1/tests/end2endtest/es_schema.yml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/es_server.yml` & `pywbem-1.7.1/tests/end2endtest/es_server.yml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/es_vault.yml` & `pywbem-1.7.1/tests/end2endtest/es_vault.yml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_indications.py` & `pywbem-1.7.1/tests/end2endtest/test_indications.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_operation_timeouts.py` & `pywbem-1.7.1/tests/end2endtest/test_operation_timeouts.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_profile_generic.py` & `pywbem-1.7.1/tests/end2endtest/test_profile_generic.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_profile_snia_server.py` & `pywbem-1.7.1/tests/end2endtest/test_profile_snia_server.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_profile_snia_smis.py` & `pywbem-1.7.1/tests/end2endtest/test_profile_snia_smis.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/test_server.py` & `pywbem-1.7.1/tests/end2endtest/test_server.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/utils/assertions.py` & `pywbem-1.7.1/tests/end2endtest/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/utils/pytest_extensions.py` & `pywbem-1.7.1/tests/end2endtest/utils/pytest_extensions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/end2endtest/utils/utils.py` & `pywbem-1.7.1/tests/end2endtest/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/README.md` & `pywbem-1.7.1/tests/functiontest/README.md`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/associatornames_classes.yaml` & `pywbem-1.7.1/tests/functiontest/associatornames_classes.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/associatornames_instances.yaml` & `pywbem-1.7.1/tests/functiontest/associatornames_instances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/associators_classes.yaml` & `pywbem-1.7.1/tests/functiontest/associators_classes.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/associators_instances.yaml` & `pywbem-1.7.1/tests/functiontest/associators_instances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/clienterror.yaml` & `pywbem-1.7.1/tests/functiontest/clienterror.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/closeenumeration.yaml` & `pywbem-1.7.1/tests/functiontest/closeenumeration.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/conftest.py` & `pywbem-1.7.1/tests/functiontest/conftest.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/createclass.yaml` & `pywbem-1.7.1/tests/functiontest/createclass.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/createinstance.yaml` & `pywbem-1.7.1/tests/functiontest/createinstance.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/deleteclass.yaml` & `pywbem-1.7.1/tests/functiontest/deleteclass.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/deleteinstance.yaml` & `pywbem-1.7.1/tests/functiontest/deleteinstance.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/deletequalifier.yaml` & `pywbem-1.7.1/tests/functiontest/deletequalifier.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/embeddedinstances.yaml` & `pywbem-1.7.1/tests/functiontest/embeddedinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/embeddedobjectclasses.yaml` & `pywbem-1.7.1/tests/functiontest/embeddedobjectclasses.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/embeddedobjectinstances.yaml` & `pywbem-1.7.1/tests/functiontest/embeddedobjectinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/enumerateclasses.yaml` & `pywbem-1.7.1/tests/functiontest/enumerateclasses.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/enumerateclassnames.yaml` & `pywbem-1.7.1/tests/functiontest/enumerateclassnames.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/enumerateinstancenames.yaml` & `pywbem-1.7.1/tests/functiontest/enumerateinstancenames.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/enumerateinstances.yaml` & `pywbem-1.7.1/tests/functiontest/enumerateinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/enumeratequalifiers.yaml` & `pywbem-1.7.1/tests/functiontest/enumeratequalifiers.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/execquery.yaml` & `pywbem-1.7.1/tests/functiontest/execquery.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/exportindication.yaml` & `pywbem-1.7.1/tests/functiontest/exportindication.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/getalltypes.yaml` & `pywbem-1.7.1/tests/functiontest/getalltypes.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/getclass.yaml` & `pywbem-1.7.1/tests/functiontest/getclass.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/getinstance.yaml` & `pywbem-1.7.1/tests/functiontest/getinstance.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/getqualifier.yaml` & `pywbem-1.7.1/tests/functiontest/getqualifier.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/headers.yaml` & `pywbem-1.7.1/tests/functiontest/headers.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/invalidexpresponseerror.yaml` & `pywbem-1.7.1/tests/functiontest/invalidexpresponseerror.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/invalidresponseerror.yaml` & `pywbem-1.7.1/tests/functiontest/invalidresponseerror.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/invokemethod.yaml` & `pywbem-1.7.1/tests/functiontest/invokemethod.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/modifyclass.yaml` & `pywbem-1.7.1/tests/functiontest/modifyclass.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/modifyinstance.yaml` & `pywbem-1.7.1/tests/functiontest/modifyinstance.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/networkerror.yaml` & `pywbem-1.7.1/tests/functiontest/networkerror.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openassociatorinstances.yaml` & `pywbem-1.7.1/tests/functiontest/openassociatorinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openasssociatorinstancepaths.yaml` & `pywbem-1.7.1/tests/functiontest/openasssociatorinstancepaths.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openenumerateinstancepaths.yaml` & `pywbem-1.7.1/tests/functiontest/openenumerateinstancepaths.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openenumerateinstances.yaml` & `pywbem-1.7.1/tests/functiontest/openenumerateinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openqueryinstances.yaml` & `pywbem-1.7.1/tests/functiontest/openqueryinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openreferenceinstancepaths.yaml` & `pywbem-1.7.1/tests/functiontest/openreferenceinstancepaths.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/openreferenceinstances.yaml` & `pywbem-1.7.1/tests/functiontest/openreferenceinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/pullinstancepaths.yaml` & `pywbem-1.7.1/tests/functiontest/pullinstancepaths.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/pullinstances.yaml` & `pywbem-1.7.1/tests/functiontest/pullinstances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/pullinstanceswithpath.yaml` & `pywbem-1.7.1/tests/functiontest/pullinstanceswithpath.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/referencenames_classes.yaml` & `pywbem-1.7.1/tests/functiontest/referencenames_classes.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/referencenames_instances.yaml` & `pywbem-1.7.1/tests/functiontest/referencenames_instances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/references_classes.yaml` & `pywbem-1.7.1/tests/functiontest/references_classes.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/references_instances.yaml` & `pywbem-1.7.1/tests/functiontest/references_instances.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/functiontest/setqualifier.yaml` & `pywbem-1.7.1/tests/functiontest/setqualifier.yaml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/installtest/test_install.sh` & `pywbem-1.7.1/tests/installtest/test_install.sh`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_cim_obj.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_cim_obj.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_cim_xml.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_cim_xml.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_dict.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_dict.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_elementtree.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_elementtree.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_minidom.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_minidom.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/leaktest/test_leaks_statistics.py` & `pywbem-1.7.1/tests/leaktest/test_leaks_statistics.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_cim_operations.py` & `pywbem-1.7.1/tests/manualtest/run_cim_operations.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_enum_performance.py` & `pywbem-1.7.1/tests/manualtest/run_enum_performance.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_enum_performancesimple.py` & `pywbem-1.7.1/tests/manualtest/run_enum_performancesimple.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_mof_compiler_script.sh` & `pywbem-1.7.1/tests/manualtest/run_mof_compiler_script.sh`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_operationtimeouts.py` & `pywbem-1.7.1/tests/manualtest/run_operationtimeouts.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_response_performance.py` & `pywbem-1.7.1/tests/manualtest/run_response_performance.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/run_uprint.py` & `pywbem-1.7.1/tests/manualtest/run_uprint.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/test_uprint.bat` & `pywbem-1.7.1/tests/manualtest/test_uprint.bat`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/manualtest/test_uprint.sh` & `pywbem-1.7.1/tests/manualtest/test_uprint.sh`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/perftest/test_indications.py` & `pywbem-1.7.1/tests/perftest/test_indications.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/profiles/profiles.yml` & `pywbem-1.7.1/tests/profiles/profiles.yml`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/resourcetest/memory_utils.py` & `pywbem-1.7.1/tests/resourcetest/memory_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/resourcetest/random_objects.py` & `pywbem-1.7.1/tests/resourcetest/random_objects.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/resourcetest/resource_measurement.py` & `pywbem-1.7.1/tests/resourcetest/resource_measurement.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/resourcetest/test_enuminst.py` & `pywbem-1.7.1/tests/resourcetest/test_enuminst.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/resourcetest/timers.py` & `pywbem-1.7.1/tests/resourcetest/timers.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/cim_schema_2.49.0Final-MOFs.zip` & `pywbem-1.7.1/tests/schema/cim_schema_2.49.0Final-MOFs.zip`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_AGPSoftwareFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_AGPSoftwareFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_Action.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_Action.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ActionSequence.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ActionSequence.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDirectory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemDirectory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemHierarchy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemHierarchy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemSoftwareFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ApplicationSystemSoftwareFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ArchitectureCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ArchitectureCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_AssociatedAppSystemOverviewStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_AssociatedAppSystemOverviewStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeatureBIOSElements.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_BIOSFeatureBIOSElements.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_Check.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_Check.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareElements.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareElements.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareFeatures.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CollectedSoftwareFeatures.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_CopyFileAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_CopyFileAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DiagnosticTestSoftware.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DiagnosticTestSoftware.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectoryAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectoryAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecificationFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DirectorySpecificationFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_DiskSpaceCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_DiskSpaceCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ExecuteProgram.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ExecuteProgram.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FRUIncludesSoftwareFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FRUIncludesSoftwareFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FileSpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FileSpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectoryAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectoryAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectorySpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_FromDirectorySpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProduct.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProduct.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProductImage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledProductImage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_InstalledSoftwareElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_InstalledSoftwareElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationHostedOnServer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationHostedOnServer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeApplicationModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionFactoryAvailableToJCAResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionFactoryAvailableToJCAResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionPoolStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionPoolStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeConnectionStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDeployedObject.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDeployedObject.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJB.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJB.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBInModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBInModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEJBStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBeanStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeEntityBeanStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactoryManagedConnectionFactory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionFactoryManagedConnectionFactory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionPools.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAConnectionPools.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAManagedConnectionFactory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCAManagedConnectionFactory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCANonpooledConnections.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJCANonpooledConnections.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCConnectionPools.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCConnectionPools.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSourceDriver.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDataSourceDriver.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDriver.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCDriver.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCNonpooledConnections.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCNonpooledConnections.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResourceUsesDataSource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJDBCResourceUsesDataSource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionSessions.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionSessions.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConnectionStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConsumerStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSConsumerStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSEndpointStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSEndpointStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSProducerStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSProducerStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionConsumers.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionConsumers.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionProducers.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionProducers.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSSessionStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStatConnections.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJMSStatConnections.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJTAStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVM.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVM.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVMStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJVMStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeJavaMailStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObject.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObject.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObjectCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeManagedObjectCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBeanStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeMessageDrivenBeanStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModuleUsesJVM.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeModuleUsesJVM.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeNotification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeNotification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterInModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceAdapterInModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceOnServer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeResourceOnServer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerInDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerInDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerUsesJVM.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServerUsesJVM.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServlet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServlet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletInModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletInModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeServletStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBeanStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeSessionBeanStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBeanStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatefulSessionBeanStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatistic.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeStatistic.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLStats.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_J2eeURLStats.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_MemoryCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_MemoryCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ModifySettingAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ModifySettingAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_OSVersionCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_OSVersionCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_OperatingSystemSoftwareFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_OperatingSystemSoftwareFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ProductSoftwareFeatures.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ProductSoftwareFeatures.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_RemoveDirectoryAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_RemoveDirectoryAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SettingCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SettingCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementActions.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementActions.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementChecks.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementChecks.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementSAPImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementSAPImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementServiceImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementServiceImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementVersionCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareElementVersionCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSAPImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSAPImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureServiceImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureServiceImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSoftwareElements.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SoftwareFeatureSoftwareElements.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_StatisticalRuntimeOverview.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_StatisticalRuntimeOverview.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SwapSpaceCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SwapSpaceCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_SystemBIOS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_SystemBIOS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectoryAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectoryAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectorySpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_ToDirectorySpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VersionCompatibilityCheck.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VersionCompatibilityCheck.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeatureVideoBIOSElements.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Application/CIM_VideoBIOSFeatureVideoBIOSElements.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractBasedOn.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractBasedOn.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementAllocatedFromPool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementAllocatedFromPool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AbstractElementStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ActiveConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ActiveConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ActsAsSpare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ActsAsSpare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AdminDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AdminDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AllocatedLogicalElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AllocatedLogicalElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AllocationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AllocationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_AssociatedPowerManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_AssociatedPowerManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_BasedOn.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_BasedOn.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_BindsTo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_BindsTo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Capabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Capabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectedCollections.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectedCollections.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectedMSEs.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectedMSEs.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionOfMSEs.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionOfMSEs.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CollectionSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CollectionSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_CompatibleProduct.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_CompatibleProduct.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Component.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Component.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponentView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteComponentView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteJob.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConcreteJob.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Configuration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Configuration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationForSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ConfigurationForSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ContainedDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ContainedDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ContainedLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ContainedLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DefaultSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DefaultSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Dependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Dependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DependencyContext.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DependencyContext.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceSAPImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceSAPImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceServiceImplementation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceServiceImplementation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_DeviceStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementAllocatedFromPool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementAllocatedFromPool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementProfile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementProfile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementSoftwareIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementSoftwareIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ElementView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ElementView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EnabledLogicalElementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_EthernetPortAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_EthernetPortAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ExtentRedundancyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ExtentRedundancyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ExtraCapacityGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ExtraCapacityGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_FRU.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_FRU.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_FRUIncludesProduct.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_FRUIncludesProduct.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_GroupSynchronized.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_GroupSynchronized.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedAccessPoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedAccessPoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedResourcePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedResourcePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_HostedService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_HostedService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ImplementationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ImplementationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_InstalledSoftwareIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_InstalledSoftwareIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_IsSpare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_IsSpare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Job.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Job.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_JobCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_JobCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LaunchInContextService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LocalizationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LocalizationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Location.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Location.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDeviceView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalDeviceView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_LogicalIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_LogicalIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ManagedElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ManagedElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ManagedSystemElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ManagedSystemElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_MemberOfCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_MemberOfCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_MethodParameters.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_MethodParameters.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OpaqueManagementDataService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OrderedMemberOfCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OrderedMemberOfCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_OwningCollectionElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_OwningCollectionElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ParameterValueSources.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ParameterValueSources.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ParametersForMethod.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ParametersForMethod.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalComputerSystemView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalComputerSystemView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElementLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalElementLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PhysicalStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_PowerManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProcessorAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProcessorAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Product.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Product.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductElementComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductElementComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductFRU.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductFRU.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductParentChild.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductParentChild.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalElements.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductPhysicalElements.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductProductDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductProductDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductServiceComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductServiceComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductSoftwareComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductSoftwareComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProductSupport.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProductSupport.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Profile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Profile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProtocolService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesServiceToElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ProvidesServiceToElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RawMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RawMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Realizes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Realizes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancyGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RedundancySet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RedundancySet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedElementCausingError.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedElementCausingError.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RelatedStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RemotePort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RemotePort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_RemoteServiceAccessPoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_RemoteServiceAccessPoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ReplaceableProductFRU.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ReplaceableProductFRU.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ReplacementFRU.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ReplacementFRU.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourceAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourceAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ResourcePoolConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPAvailableForElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPAvailableForElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPSAPDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPSAPDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SAPStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ScopedView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ScopedView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Service.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Service.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessBySAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessBySAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessPoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessPoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessURI.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAccessURI.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElementWithQuota.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAffectsElementWithQuota.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAvailableToElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceAvailableToElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceSAPDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceSAPDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceServiceDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceServiceDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ServiceStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Setting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Setting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingContext.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingContext.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingForSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingForSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineState.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SettingsDefineState.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SoftwareInstallationServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SpareGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SpareGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Spared.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Spared.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticalSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Statistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Statistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StatisticsCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StatisticsCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancyGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancyGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancySet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_StorageRedundancySet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SupportAccess.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SupportAccess.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_Synchronized.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_Synchronized.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_System.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_System.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemDeviceView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemDeviceView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemPackaging.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemPackaging.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSettingContext.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSettingContext.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemSpecificCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemSpecificCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_SystemStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_TimeService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_TimeService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_View.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_View.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_ViewOnSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_ViewOnSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualEthernetSwitchSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualEthernetSwitchSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VirtualSystemSnapshotServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Core/CIM_VisibleMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Core/CIM_VisibleMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_AssociatedDatabaseSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_AssociatedDatabaseSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabase.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabase.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_CommonDatabaseStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseAdministrator.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseAdministrator.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseControlFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseControlFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseParameter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseParameter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseResourceStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseResourceStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegment.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegment.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegmentSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSegmentSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseServiceStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseServiceStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorageArea.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseStorageArea.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_DatabaseSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_SNMPDatabaseParameter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_SNMPDatabaseParameter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Database/CIM_ServiceAvailableToDatabase.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Database/CIM_ServiceAvailableToDatabase.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ADSLModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ADSLModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AGPVideoController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AGPVideoController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ATAPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ATAPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AbstractProtocolControllerForDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AbstractProtocolControllerForDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AccessLabelReader.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AccessLabelReader.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AdapterActiveConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AdapterActiveConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AdvancedStorageSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AdvancedStorageSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnAggregatePExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnAggregatePExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnPExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregatePSExtentBasedOnPExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AggregateRedundancyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AggregateRedundancyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDeviceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AlarmDeviceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolViewView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedFromStoragePoolViewView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedResources.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AllocatedResources.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedAlarm.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedAlarm.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBattery.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBattery.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBlockStatisticsManifestCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedBlockStatisticsManifestCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCacheMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCacheMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedComponentExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedComponentExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCooling.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedCooling.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedDeviceMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedDeviceMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedElementTier.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedElementTier.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedIndicatorLED.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedIndicatorLED.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedInitiatorMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedInitiatorMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedLabelReader.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedLabelReader.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProcessorMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProcessorMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProtocolController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedProtocolController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedRemainingExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedRemainingExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedResourcePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedResourcePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyCurrentSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyCurrentSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyVoltageSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedSupplyVoltageSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedTargetMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AssociatedTargetMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_AsymmetricAccessibility.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_AsymmetricAccessibility.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BIOSLoadedInNV.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BIOSLoadedInNV.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BasedOnView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BasedOnView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Battery.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Battery.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BinarySensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BinarySensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifestCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsManifestCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStatisticsService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_BlockStorageStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_BlockStorageStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CacheMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CacheMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CallBasedModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CallBasedModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ChangerDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ChangerDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CollectionOfSensors.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CollectionOfSensors.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtentBasedOn.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CompositeExtentBasedOn.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemProcessor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ComputerSystemProcessor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ConfigurationReportingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ConfigurationReportingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ConnectionBasedModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ConnectionBasedModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ControlledBy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ControlledBy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Controller.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Controller.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ControllerConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ControllerConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_CurrentSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_CurrentSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DVDDrive.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DVDDrive.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DesktopMonitor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DesktopMonitor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorCounts.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorCounts.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceErrorData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceServicesLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceServicesLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSharingCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSharingCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSoftware.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DeviceSoftware.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiscreteSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiscreteSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskDrive.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskDrive.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskDriveView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskDriveView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionBasedOnVolume.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionBasedOnVolume.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DiskPartitionConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DisplayController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DisplayController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Door.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Door.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToPhysicalElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DoorAccessToPhysicalElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DriveComponentViewView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DriveComponentViewView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_DriveInDiskGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_DriveInDiskGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ElementStatisticalDataView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ElementStatisticalDataView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ElementStorageProtectionSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ElementStorageProtectionSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ErrorCountersForDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ErrorCountersForDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_EthernetPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ExtentComponentView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ExtentComponentView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ExtentInDiskGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ExtentInDiskGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCActiveConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCActiveConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCAdapterEventCounters.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCAdapterEventCounters.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortRateStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortRateStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCSwitchSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FCTopologyView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FCTopologyView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FailoverStorageExtentsCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FailoverStorageExtentsCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Fan.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Fan.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibreChannelAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibreChannelAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortActiveLogin.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortActiveLogin.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortEventCounters.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortEventCounters.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortOnFCAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FibrePortOnFCAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemGroupSynchronized.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemGroupSynchronized.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemReplicationServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemSynchronized.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FileSystemSynchronized.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_FlatPanel.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_FlatPanel.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GPTDiskPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GPTDiskPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GenericDiskPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GenericDiskPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupInDiskGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupInDiskGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_GroupMaskingMappingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HardwareThread.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HardwareThread.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePoolView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_HostedStoragePoolView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IBSubnetManager.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IBSubnetManager.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLED.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLED.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLEDCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_IndicatorLEDCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorTargetLogicalUnitPath.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InitiatorTargetLogicalUnitPath.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InstalledPartitionTable.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InstalledPartitionTable.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_InterLibraryPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_InterLibraryPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Keyboard.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Keyboard.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LLDPEthernetPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReader.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReader.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LabelReaderStatInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LibraryExchange.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LibraryExchange.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LibraryPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LibraryPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LimitedAccessPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LimitedAccessPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDisk.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDisk.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolume.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolume.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolumeSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalDiskBasedOnVolumeSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_LogicalPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MappingProtocolControllerView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MappingProtocolControllerView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingExposedDeviceView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingExposedDeviceView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MaskingMappingView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaAccessStatInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MediaPresent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MediaPresent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Memory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Memory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MemoryError.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MemoryError.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ModulePort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ModulePort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MonitorResolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MonitorResolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_MonitorSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_MonitorSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapterRedundancyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkAdapterRedundancyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NetworkVirtualAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NetworkVirtualAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NonVolatileStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NonVolatileStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_NumericSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_NumericSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OOBAlertServiceOnNetworkPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifestCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerManifestCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OperationalPowerStatisticsService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_OwningPrintQueue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_OwningPrintQueue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIBridge.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIBridge.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCIeSwitch.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCIeSwitch.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PCVideoController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PCVideoController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PExtentRedundancyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PExtentRedundancyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_POTSModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_POTSModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PSExtentBasedOnPExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PSExtentBasedOnPExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageAlarm.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageAlarm.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageCooling.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageCooling.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PackageTempSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PackageTempSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ParallelController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ParallelController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PassThroughModule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PassThroughModule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespace.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespace.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespaceSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryNamespaceSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PersistentMemoryService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PhysicalExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PhysicalExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerForChanger.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerForChanger.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerLabelReader.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerLabelReader.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PickerStatInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PointingDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PointingDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortActiveConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortActiveConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortImplementsEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortImplementsEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PortOnDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PortOnDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerAllocationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerAllocationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerSource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerSource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerSupply.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerSupply.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PowerUtilizationManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PoweredStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PoweredStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintInputTray.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintInputTray.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintInterpreter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintInterpreter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintJob.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintJob.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintJobFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintJobFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintMarker.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintMarker.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintQueue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintQueue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrintSupply.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrintSupply.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Printer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Printer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingJob.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingJob.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingQueue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_PrinterServicingQueue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Processor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Processor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCore.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProcessorCore.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedExtentBasedOn.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedExtentBasedOn.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedSpaceExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtectedSpaceExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerAccessesUnit.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerAccessesUnit.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnit.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnit.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnitView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerForUnitView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerMaskingCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ProtocolControllerMaskingCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueryStatisticsCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueryStatisticsCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueueForPrintService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueueForPrintService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_QueueForwardsToPrintSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_QueueForwardsToPrintSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizedOnSide.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizedOnSide.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesAggregatePExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesAggregatePExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesDiskPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesDiskPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesPExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesPExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RealizesTapePartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RealizesTapePartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RemoteReplicationCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RemoteReplicationCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_RemoteResources.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_RemoteResources.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPairView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPairView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPoolForStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicaPoolForStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationEntity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationEntity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ReplicationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SASPHY.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SASPHY.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SASPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SASPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SBProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SBProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIArbitraryLogicalUnit.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIArbitraryLogicalUnit.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInitiatorTargetLogicalUnitPath.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInitiatorTargetLogicalUnitPath.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInterface.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIInterface.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIMultipathSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIPathConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIPathConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSIProtocolController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSIProtocolController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SCSITargetPortGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SCSITargetPortGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Sensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Sensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SerialController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SerialController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SerialInterface.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SerialInterface.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SharedDeviceManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SharedDeviceManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SharingDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SharingDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Snapshot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Snapshot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SnapshotOfExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SnapshotOfExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SpareConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StatisticsService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageDefect.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageDefect.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementCompositionService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementDriveDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageElementDriveDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageErasureSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageError.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageError.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibrary.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibrary.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibraryCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageLibraryCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolDiagnosticTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StoragePoolView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProcessorAffinity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProcessorAffinity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageProtectionSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageRelocationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageRelocationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageReplicationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageReplicationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageResourceLoadGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageResourceLoadGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageServerAsymmetryCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageServerAsymmetryCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingWithHints.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingWithHints.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsAssociatedToCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsAssociatedToCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsGeneratedFromCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSettingsGeneratedFromCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageSynchronized.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageSynchronized.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageTier.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageTier.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageTierCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageTierCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_StorageVolume.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_StorageVolume.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SuppliesPower.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SuppliesPower.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SynchronizationAspect.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SynchronizationAspect.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_SystemRegistrationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_SystemRegistrationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Tachometer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Tachometer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapeDrive.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapeDrive.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapePartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapePartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TapePartitionOnSurface.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TapePartitionOnSurface.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TargetMaskingGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TargetMaskingGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TargetPortGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TargetPortGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TemperatureSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TemperatureSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TierSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TierSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_TokenRingPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBControllerHasHub.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBControllerHasHub.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBHub.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBHub.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_USBPortOnHub.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_USBPortOnHub.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Unimodem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Unimodem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_UninterruptiblePowerSupply.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_UninterruptiblePowerSupply.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_UserDevice.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_UserDevice.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLResourceUsage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLResourceUsage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTLStatisticalDataServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VTOCDiskPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VTOCDiskPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoController.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoController.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoControllerResolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoControllerResolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoHead.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoHead.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoHeadResolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoHeadResolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VideoSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VideoSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ViewCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ViewCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolatileStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolatileStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VoltageSensor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VoltageSensor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSetBasedOnPSExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeSetBasedOnPSExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_VolumeView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_VolumeView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WBEMServerDeviceRegistrationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WBEMServerDeviceRegistrationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnModem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnModem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WakeUpServiceOnNetworkPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Watchdog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Watchdog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiPortConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_WiFiRadio.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_WiFiRadio.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_Zone.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_Zone.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneMembershipSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneMembershipSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Device/CIM_ZoneSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Device/CIM_ZoneSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AbstractIndicationSubscription.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AbstractIndicationSubscription.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AlertIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AlertIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_AlertInstIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_AlertInstIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ClassModification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ClassModification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollectionSubscription.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FilterCollectionSubscription.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_FormattedIndicationSubscription.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_FormattedIndicationSubscription.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_Indication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_Indication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationFilter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationFilter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandler.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandler.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandlerCIMXML.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationHandlerCIMXML.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationServiceSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_IndicationSubscription.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_IndicationSubscription.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstMethodCall.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstMethodCall.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_InstModification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_InstModification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestination.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestination.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationCIMXML.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationCIMXML.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationWSManagement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ListenerDestinationWSManagement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ProcessIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ProcessIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_SNMPTrapIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_SNMPTrapIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Event/CIM_ThresholdIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Event/CIM_ThresholdIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedProposal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedProposal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedTransform.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_ContainedTransform.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEProposal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKEProposal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKERule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IKERule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecPolicyForSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecProposal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecProposal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTunnelAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_IPsecTunnelAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PacketConditionInSARule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PacketConditionInSARule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForPreconfiguredTunnel.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForPreconfiguredTunnel.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForTunnel.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PeerGatewayForTunnel.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredSAAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredSAAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTransportAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTransportAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTunnelAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_PreconfiguredTunnelAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_RuleThatGeneratedSA.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_RuleThatGeneratedSA.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SANegotiationAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SANegotiationAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAProposal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAProposal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SARule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SARule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAStaticAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_SAStaticAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_TransformOfPreconfiguredAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/IPsecPolicy/CIM_TransformOfPreconfiguredAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMOMStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMOMStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCommunicationMechanism.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CIMXMLCommunicationMechanism.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForManager.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForManager.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForObjectManagerAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_CommMechanismForObjectManagerAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ElementConformsToProfile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ElementConformsToProfile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Error.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Error.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_GenericOperationCapabilitiesStructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_GenericOperationCapabilitiesStructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_IdentificationOfManagedSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_IdentificationOfManagedSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Message.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Message.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_Namespace.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_Namespace.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_NamespaceInManager.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_NamespaceInManager.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManager.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManager.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerCommunicationMechanism.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ObjectManagerCommunicationMechanism.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ProtocolAdapter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ProtocolAdapter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_QueryCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_QueryCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedProfile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedProfile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedSpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_ReferencedSpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredProfile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredProfile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSpecification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_RegisteredSpecification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SchemaInformationStructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SchemaInformationStructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SubProfileRequiresProfile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SubProfileRequiresProfile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SystemIdentification.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SystemIdentification.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_SystemInNamespace.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_SystemInNamespace.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMProtocolServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMProtocolServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerNamespace.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMServerNamespace.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WBEMService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Interop/CIM_WSManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Interop/CIM_WSManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricDefinition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricDefinition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricValue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_AggregationMetricValue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricDefinition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricDefinition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricValue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_BaseMetricValue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementPerformsUoW.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementPerformsUoW.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementUnitOfWorkDef.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_LogicalElementUnitOfWorkDef.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefForME.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefForME.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefinition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricDefinition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricForME.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricForME.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricInstance.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricInstance.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_MetricServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_StartedUoW.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_StartedUoW.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoW.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoW.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoWDef.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_SubUoWDef.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_TraceLevelType.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_TraceLevelType.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWork.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWork.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWorkDefinition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UnitOfWorkDefinition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWDefTraceLevelType.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWDefTraceLevelType.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetric.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetric.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetricDefinition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Metrics/CIM_UoWMetricDefinition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AFRelatedServices.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AFRelatedServices.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AFService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AFService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AHTransform.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AHTransform.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ASBGPEndpoints.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ASBGPEndpoints.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ATAProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ATAProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AdministrativeDistance.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AdministrativeDistance.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AllocationSchedulingElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AllocationSchedulingElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AreaOfConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AreaOfConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AssociatedNextHop.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AssociatedNextHop.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AutonomousSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AutonomousSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_AverageRateMeterService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_AverageRateMeterService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAdminDistance.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAdminDistance.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributesForRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPAttributesForRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPCluster.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPCluster.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPClustersInAS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPClustersInAS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPEndpointStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPEndpointStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPIPRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPIPRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPathAttributes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPathAttributes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroupService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerGroupService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerUsesRouteMap.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPPeerUsesRouteMap.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMap.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMap.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMapsInRoutingPolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRouteMapsInRoutingPolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPRoutingPolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPRoutingPolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceAttributes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceAttributes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPServiceStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BGPStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BGPStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BindsToLANEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BindsToLANEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BoundedPrioritySchedulingElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BoundedPrioritySchedulingElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_BufferPool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_BufferPool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CLPSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CLPSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculatedRoutes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculatedRoutes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculatesAmong.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculatesAmong.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculationBasedOnQueue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculationBasedOnQueue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CalculationServiceForDropper.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CalculationServiceForDropper.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementInClassifierService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementInClassifierService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementUsesFilterList.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierElementUsesFilterList.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierFilterSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierFilterSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ClassifierService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_CollectedBufferPool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_CollectedBufferPool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningServiceOnEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConditioningServiceOnEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Confederation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Confederation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityMembershipSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ConnectivityMembershipSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DHCPSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DHCPSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSGeneralSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSGeneralSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DNSSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DNSSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DSCPMarkerService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DSCPMarkerService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DiffServService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DiffServService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DropThresholdCalculationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DropThresholdCalculationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DropperService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DropperService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_DynamicForwardingEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_DynamicForwardingEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EFService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EFService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EGPRouteCalcDependency.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EGPRouteCalcDependency.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ESPTransform.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ESPTransform.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EWMAMeterService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EWMAMeterService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EgressConditioningServiceOnEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EgressConditioningServiceOnEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ElementInSchedulingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ElementInSchedulingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointForIPNetworkConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointForIPNetworkConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInArea.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInArea.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInLink.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointInLink.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EndpointOfNetworkPipe.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EndpointOfNetworkPipe.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_EntriesInFilterList.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_EntriesInFilterList.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ExtendedStaticIPAssignmentSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ExtendedStaticIPAssignmentSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FailNextScheduler.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FailNextScheduler.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryBase.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryBase.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterEntryInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterList.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterList.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterListInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterListInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterListsInBGPRouteMap.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterListsInBGPRouteMap.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilterOfSecurityAssociation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilterOfSecurityAssociation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FilteredBGPAttributes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FilteredBGPAttributes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_FlowService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_FlowService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardedRoutes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardedRoutes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ForwardsAmong.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ForwardsAmong.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021Filter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021Filter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021PService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Hdr8021PService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropQueueBinding.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropQueueBinding.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropper.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HeadTailDropper.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedAdminDistance.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedAdminDistance.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPAttributes.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPAttributes.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPPeerGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPPeerGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPRouteMap.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedBGPRouteMap.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterEntryBase.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterEntryBase.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterList.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedFilterList.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedForwardingServices.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedForwardingServices.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedNetworkPipe.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedNetworkPipe.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingPolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingPolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingServices.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_HostedRoutingServices.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IEEE8021xSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IKESAEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IKESAEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPAddressRange.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPAddressRange.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPAssignmentSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPAssignmentSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPCOMPTransform.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPCOMPTransform.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPConnectivitySubnet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPConnectivitySubnet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPHeadersFilter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPHeadersFilter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPInterfaceSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPInterfaceSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPNetworkConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPNetworkConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPSOFilterEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPSOFilterEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPSubnet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPSubnet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPVersionSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPVersionSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPXNetwork.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPXNetwork.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPXProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPXProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IPsecSAEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IPsecSAEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InBGPPeerGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InBGPPeerGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InLogicalNetwork.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InLogicalNetwork.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InSegment.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InSegment.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_InboundVLAN.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_InboundVLAN.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_IngressConditioningServiceOnEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_IngressConditioningServiceOnEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_KVMRedirectionSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_KVMRedirectionSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANConnectivitySegment.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANConnectivitySegment.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LANSegment.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LANSegment.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ListsInRoutingPolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ListsInRoutingPolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetwork.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetwork.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetworkService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_LogicalNetworkService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MarkerService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MarkerService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MediaRedirectionSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_MeterService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_MeterService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NamedAddressCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NamedAddressCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Network.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Network.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipe.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipe.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipeComposition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPipeComposition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPortConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkPortConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkServicesInAdminDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkServicesInAdminDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworkVLAN.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworkVLAN.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NetworksInAdminDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NetworksInAdminDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopIPRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopIPRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRoute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRoute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRouting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextHopRouting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextScheduler.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextScheduler.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterClassifierElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterClassifierElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterMeter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NextServiceAfterMeter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_NonWorkConservingSchedulingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_NonWorkConservingSchedulingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFArea.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFArea.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFAreaConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFAreaConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFLink.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFLink.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpointBase.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFProtocolEndpointBase.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFServiceConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OSPFVirtualInterface.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OSPFVirtualInterface.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_OutboundVLAN.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_OutboundVLAN.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PacketSchedulingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PacketSchedulingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PeerIDPayloadFilterEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PeerIDPayloadFilterEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PeerOfSAEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PeerOfSAEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Phase1SAUsedForPhase2.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Phase1SAUsedForPhase2.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PreambleFilter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PreambleFilter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PreambleMarkerService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PreambleMarkerService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PrecedenceService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PrecedenceService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Priority8021QMarkerService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Priority8021QMarkerService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_PrioritySchedulingElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_PrioritySchedulingElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ProtocolServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ProtocolServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSConditioningSubService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSConditioningSubService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QoSSubService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QoSSubService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueAllocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueAllocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueHierarchy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueHierarchy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueueToSchedule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueueToSchedule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_QueuingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_QueuingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_REDDropperService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_REDDropperService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RangeOfIPAddresses.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RangeOfIPAddresses.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RangesOfConfiguration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RangesOfConfiguration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RedirectionServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorClientService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorClientService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorNonClientService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorNonClientService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ReflectorService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RelatedSpanningTree.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RelatedSpanningTree.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RelatedTransparentBridgingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RelatedTransparentBridgingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RemoteAccessAvailableToElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RemoteAccessAvailableToElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteCalculationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteCalculationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteForwardedByService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteForwardedByService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RouteUsesEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RouteUsesEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInAS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInAS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInBGPCluster.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutersInBGPCluster.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutesBGP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutesBGP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingPolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingPolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomain.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomain.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomainInAS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_RoutingProtocolDomainInAS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointConnectionStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointConnectionStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointRefreshSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SAEndpointRefreshSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SATransform.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SATransform.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SCSIProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SCSIProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPCommunityString.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPCommunityString.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SNMPTrapTarget.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SNMPTrapTarget.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SSHSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SSHSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulerUsed.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulerUsed.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingServiceToSchedule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SchedulingServiceToSchedule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SecurityAssociationEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SecurityAssociationEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SourceRoutingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SourceRoutingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SpanningTreeStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Specific802dot1QVLANService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Specific802dot1QVLANService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_StaticForwardingEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_StaticForwardingEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_StaticIPAssignmentSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_StaticIPAssignmentSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPort.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPort.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortDynamicForwarding.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortDynamicForwarding.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortPair.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortPair.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRouting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRouting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRoutingStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSourceRoutingStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTree.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTree.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTreeStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortSpanningTreeStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStaticForwarding.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStaticForwarding.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortTransparentBridgingStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchPortTransparentBridgingStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSourceRouting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSourceRouting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSpanningTree.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceSpanningTree.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceTransparentBridging.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceTransparentBridging.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceVLAN.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchServiceVLAN.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_Switchable.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_Switchable.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_SwitchesAmong.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_SwitchesAmong.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TCPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TCPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TelnetSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TelnetSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TextRedirectionService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_ToSMarkerService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_ToSMarkerService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TokenBucketMeterService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TokenBucketMeterService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransformOfSecurityAssociation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransformOfSecurityAssociation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingDynamicForwarding.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingDynamicForwarding.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStaticForwarding.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStaticForwarding.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TransparentBridgingStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_TrapSourceForSNMPService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_TrapSourceForSNMPService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_UDPProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_UDPProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_USBRedirectionService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLAN.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLAN.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANEndpointSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANFor.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANFor.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANNetwork.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANNetwork.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_VLANService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_VLANService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WRRSchedulingElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WRRSchedulingElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WeightedREDDropperService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WeightedREDDropperService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiEndpointSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_WiFiNetworkDetectionSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_WiFiNetworkDetectionSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_X509CredentialFilterEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_X509CredentialFilterEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSICapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSICapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnectionSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIConnectionSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSILoginStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSILoginStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIProtocolEndpoint.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSIProtocolEndpoint.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISession.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISession.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionFailures.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionFailures.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Network/CIM_iSCSISessionStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_AdjacentSlots.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_AdjacentSlots.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Card.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Card.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_CardInSlot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_CardInSlot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_CardOnCard.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_CardOnCard.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Chassis.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Chassis.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ChassisInRack.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ChassisInRack.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Chip.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Chip.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConfigurationCapacity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConfigurationCapacity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectedTo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectedTo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectorOnPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ConnectorOnPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Container.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Container.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ContainerView.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ContainerView.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Docked.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Docked.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementCapacity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementCapacity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementInConnector.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementInConnector.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ElementsLinked.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ElementsLinked.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_HomeForMedia.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_HomeForMedia.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_LinkHasConnector.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_LinkHasConnector.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Magazine.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Magazine.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MediaPhysicalStatInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryCapacity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryCapacity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryOnCard.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryOnCard.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryWithMedia.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_MemoryWithMedia.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInChassis.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInChassis.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInConnector.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInConnector.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInSlot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageInSlot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackageLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackageLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PackagedComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PackagedComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ParticipatesInSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ParticipatesInSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalAssetCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalAssetCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalCapacity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalCapacity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalConnector.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalConnector.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalFrame.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalFrame.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalLink.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalLink.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMedia.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMedia.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMediaInLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMediaInLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMemory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalMemory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalTape.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_PhysicalTape.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Rack.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Rack.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_ReplacementSet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_ReplacementSet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_Slot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_Slot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_SlotInSlot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_SlotInSlot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_StorageMediaLocation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_StorageMediaLocation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Physical/CIM_SystemBusCard.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Physical/CIM_SystemBusCard.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AcceptCredentialFrom.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AcceptCredentialFrom.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AccountAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AccountAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationRule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_AuthenticationRule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_BiometricAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_BiometricAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_CompoundPolicyCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_DocumentAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_DocumentAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ElementInPolicyRoleCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ElementInPolicyRoleCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_FilterOfPacketCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_FilterOfPacketCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_KerberosAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_KerberosAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_MethodAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_MethodAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkPacketAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkPacketAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkingIDAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_NetworkingIDAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PacketFilterCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PacketFilterCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PhysicalCredentialAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PhysicalCredentialAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_Policy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_Policy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRepository.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRepository.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionInPolicyRule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionStructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyActionStructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRepository.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRepository.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionInPolicyRule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionStructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyConditionStructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyContainerInPolicyContainer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyContainerInPolicyContainer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInPolicyGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInPolicyGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyGroupInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepository.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepository.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepositoryInPolicyRepository.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRepositoryInPolicyRepository.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollectionInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRoleCollectionInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRule.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRule.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInPolicyGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInPolicyGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleValidityPeriod.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyRuleValidityPeriod.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySet.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySet.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetAppliesToElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetAppliesToElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInRoleCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInRoleCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetValidityPeriod.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicySetValidityPeriod.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyTimePeriodCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PolicyTimePeriodCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_PublicPrivateKeyAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_PublicPrivateKeyAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_QueryCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_QueryCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_RejectConnectionAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_RejectConnectionAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicyContainer.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_ReusablePolicyContainer.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_SharedSecretAuthentication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_SharedSecretAuthentication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyAction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyAction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyCondition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Policy/CIM_VendorPolicyCondition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Activity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Activity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ActivityResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ActivityResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ActivityTransaction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ActivityTransaction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Address.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Address.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdminAssociation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdminAssociation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Administrative.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Administrative.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeContact.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeContact.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeRevision.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_AdministrativeRevision.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Agreement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Agreement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Attachment.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Attachment.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Categorization.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Categorization.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Category.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Category.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_CategoryParentChild.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_CategoryParentChild.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactContactItem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactContactItem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ContactOrganization.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ContactOrganization.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ExchangeElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ExchangeElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Expression.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Expression.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionLink.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ExpressionLink.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Feature.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Feature.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_FeatureResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_FeatureResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Location.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Location.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Person.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Person.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Problem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Problem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Product.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Product.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductAsset.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductAsset.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ProductParentChild.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ProductParentChild.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Reference.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Reference.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Resolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Resolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Resource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Resource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Revision.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Revision.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SISService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SISService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceActivity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceActivity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceAgreement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceAgreement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceIncident.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceIncident.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProblem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProblem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProvider.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceProvider.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceRequester.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceRequester.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_ServiceResolutionSolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_ServiceResolutionSolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Solution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Solution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionCategory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionCategory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionExpression.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionExpression.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionHasElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionHasElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionProblem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionProblem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionReference.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionReference.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_SolutionResolution.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_SolutionResolution.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Statement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Statement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/Support/PRS_Transaction.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/Support/PRS_Transaction.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AffectedJobElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AffectedJobElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AllocatedDMA.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AllocatedDMA.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AllocatedResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AllocatedResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AssociatedFileSystemStatisticsManifestCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AssociatedFileSystemStatisticsManifestCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AssociatedJobMethodResult.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AssociatedJobMethodResult.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_AvailableDiagnosticService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_AvailableDiagnosticService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSAttribute.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSAttribute.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSEnumeration.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSEnumeration.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSInteger.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSInteger.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSPassword.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSPassword.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BIOSString.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BIOSString.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootConfigSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootConfigSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootOSFromFS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootOSFromFS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootServiceAccessBySAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootServiceAccessBySAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_BootSourceSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_BootSourceSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CIFSSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CIFSSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CIFSShare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CIFSShare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Cluster.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Cluster.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ClusterServiceAccessBySAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ClusterServiceAccessBySAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ClusteringService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ClusteringService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComponentCS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComponentCS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemDMA.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemDMA.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemIRQ.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemIRQ.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemMappedIO.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemMappedIO.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemNodeCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemNodeCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ComputerSystemResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingDataRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingDataRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingsRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_CorrespondingSettingsRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DMA.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DMA.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DefaultElementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DefaultElementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DeviceAccessedByFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DeviceAccessedByFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DeviceFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DeviceFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticCompletionRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticCompletionRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResult.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResult.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForMSE.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForMSE.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultForTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultInPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticResultInPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceJobCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceJobCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticServiceRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingDataRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingDataRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingForTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingForTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSettingRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSubTestRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticSubTestRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestForMSE.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestForMSE.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestInPackage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticTestInPackage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticsLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiagnosticsLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DirectoryContainsFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DirectoryContainsFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_DiskDriveDiagnosticTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Export.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Export.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ExportedFileShareSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticTest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FCHBADiagnosticTest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FIFOPipeFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FIFOPipeFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSDomainIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSDomainIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToPrincipal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToPrincipal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToTree.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaAppliesToTree.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaConfigEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaConfigEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaIndication.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaIndication.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaReportRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FSQuotaReportRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileExportCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileExportCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileExportService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileExportService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileServerSettings.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileServerSettings.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileShare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileShare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileShareSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileShareSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemConfigurationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticalData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticalData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifest.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifest.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifestCollection.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsManifestCollection.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_FileSystemStatisticsService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HelpService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HelpService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HelpServiceAvailableToFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HelpServiceAvailableToFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedBootSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedBootSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedBootService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedBootService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterSAP.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterSAP.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedClusterService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedFileSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedFileSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedJobDestination.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedJobDestination.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostedShare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostedShare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_HostingCS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_HostingCS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_IRQ.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_IRQ.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_InstalledOS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_InstalledOS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobDestination.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobDestination.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobDestinationJobs.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobDestinationJobs.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobQueue.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobQueue.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_JobSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_JobSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LastAppliedSnapshot.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LastAppliedSnapshot.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocalAccessAvailableToFS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocalAccessAvailableToFS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocalFileSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocalFileSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemSetting.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LocallyAccessibleFileSystemSetting.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Log.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Log.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogEntry.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogEntry.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInDataFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInDataFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInDeviceFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInDeviceFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogInStorage.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogInStorage.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogManagesRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogManagesRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogToLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogToLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_LogicalFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_LogicalFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MemoryMappedIO.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MemoryMappedIO.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MemoryResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MemoryResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MessageLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MessageLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_MethodResult.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_MethodResult.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Mount.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Mount.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFSSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFSSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NFSShare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NFSShare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_NISSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_NISSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OOBAlertService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OOBAlertService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OSProcess.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OSProcess.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystemCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperatingSystemCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OperationLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OperationLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_OwningJobElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_OwningJobElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ParticipatingCS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ParticipatingCS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogServiceCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PlatformWatchdogServiceCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_PortResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_PortResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Process.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Process.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessExecutable.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessExecutable.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessOfJob.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessOfJob.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ProcessThread.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ProcessThread.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordAppliesToElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordAppliesToElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordForLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordForLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordInLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordInLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RecordLogCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RecordLogCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RemoteFileSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RemoteFileSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ReportRecord.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ReportRecord.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResidesOnExtent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResidesOnExtent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResourceAllocationFromPool.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResourceAllocationFromPool.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ResourceOfSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ResourceOfSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_RunningOS.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_RunningOS.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SAPAvailableForFileShare.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SAPAvailableForFileShare.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_ServiceProcess.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_ServiceProcess.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SettingAssociatedToCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SettingAssociatedToCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Share.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Share.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SharedElement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SharedElement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SnapshotOfVirtualSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SnapshotOfVirtualSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SummaryDiagnostics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SummaryDiagnostics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SymbolicLink.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SymbolicLink.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SystemPartition.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SystemPartition.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_SystemResource.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_SystemResource.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_Thread.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_Thread.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_TimeZone.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_TimeZone.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnitaryComputerSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnitaryComputerSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixDeviceFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixDeviceFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixDirectory.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixDirectory.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixFile.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixFile.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixLocalFileSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixLocalFileSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcess.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcess.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatisticalInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatisticalInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatistics.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixProcessStatistics.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UnixThread.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UnixThread.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UseOfLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UseOfLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_UseOfMessageLog.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_UseOfMessageLog.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualComputerSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualComputerSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemMigrationSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemMigrationSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingDataComponent.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_VirtualSystemSettingDataComponent.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/System/CIM_WakeUpService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/System/CIM_WakeUpService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccessControlInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccessControlInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Account.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Account.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountMapsToAccount.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountMapsToAccount.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountOnSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountOnSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AccountSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AccountSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AssignedIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AssignedIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AssociatedPrivilege.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AssociatedPrivilege.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticateForUse.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticateForUse.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationRequirement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationRequirement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationTarget.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthenticationTarget.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationSubject.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationSubject.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationTarget.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizationTarget.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedPrivilege.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedPrivilege.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedSubject.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedSubject.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedTarget.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedTarget.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedUse.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_AuthorizedUse.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CAHasPublicCertificate.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CAHasPublicCertificate.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CASignsPublicKeyCertificate.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CASignsPublicKeyCertificate.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateAuthority.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateAuthority.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CertificateManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CollectionInOrganization.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CollectionInOrganization.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CollectionInSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CollectionInSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Credential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Credential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialContext.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialContext.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_CredentialStore.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_CredentialStore.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ElementAsUser.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ElementAsUser.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ElementSecuritySensitivity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ElementSecuritySensitivity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_GatewayPathID.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_GatewayPathID.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Group.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Group.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_HostedACI.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_HostedACI.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_HostedAuthenticationRequirement.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_HostedAuthenticationRequirement.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IKESecretIsNamed.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IKESecretIsNamed.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IPNetworkIdentity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IPNetworkIdentity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Identity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Identity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_IdentityContext.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_IdentityContext.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KDCIssuesKerberosTicket.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KDCIssuesKerberosTicket.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosKeyDistributionCenter.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosKeyDistributionCenter.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KerberosTicket.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KerberosTicket.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_KeyBasedCredentialManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_KeyBasedCredentialManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Keystore.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Keystore.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_LocallyManagedPublicKey.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_LocallyManagedPublicKey.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagedCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagedCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccount.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccount.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccountOnSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ManagesAccountOnSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MemberPrincipal.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MemberPrincipal.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreGroupInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreGroupInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreOrgUnitInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreOrgUnitInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreOrganizationInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreOrganizationInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MorePersonInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MorePersonInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_MoreRoleInfo.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_MoreRoleInfo.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NamedCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NamedCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NamedSharedIKESecret.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NamedSharedIKESecret.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Notary.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Notary.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_NotaryVerifiesBiometric.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_NotaryVerifiesBiometric.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OpaqueManagementDataOwner.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OpaqueManagementDataOwner.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OrgStructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OrgStructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OrgUnit.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OrgUnit.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Organization.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Organization.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherGroupInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherGroupInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherOrgUnitInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherOrgUnitInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherOrganizationInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherOrganizationInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherPersonInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherPersonInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_OtherRoleInformation.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_OtherRoleInformation.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Person.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Person.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Privilege.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Privilege.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PrivilegeManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyCertificate.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PublicKeyCertificate.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_PublicPrivateKeyPair.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_PublicPrivateKeyPair.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RequireCredentialsFrom.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RequireCredentialsFrom.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_Role.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_Role.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedAuthorizationService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedAuthorizationService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedManagementCapabilities.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleBasedManagementCapabilities.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_RoleLimitedToTarget.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_RoleLimitedToTarget.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecuritySensitivity.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecuritySensitivity.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceForSystem.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceForSystem.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceUsesAccount.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SecurityServiceUsesAccount.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_ServiceUsesSecurityService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_ServiceUsesSecurityService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecret.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecret.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretIsShared.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretIsShared.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SharedSecretService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SignedCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SignedCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageClientSettingData.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageClientSettingData.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareID.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareID.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareIDManagementService.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_StorageHardwareIDManagementService.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministrator.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministrator.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorGroup.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorGroup.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorRole.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_SystemAdministratorRole.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_TrustHierarchy.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_TrustHierarchy.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UnsignedCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UnsignedCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UnsignedPublicKey.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UnsignedPublicKey.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UserContact.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UserContact.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersAccess.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersAccess.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersAccount.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersAccount.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_UsersCredential.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_UsersCredential.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509CRL.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509CRL.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509Certificate.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509Certificate.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/User/CIM_X509Infrastructure.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/User/CIM_X509Infrastructure.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/cim_schema_2.49.0.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/cim_schema_2.49.0.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/qualifiers.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/qualifiers.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/schema/mofFinal2.49.0/qualifiers_optional.mof` & `pywbem-1.7.1/tests/schema/mofFinal2.49.0/qualifiers_optional.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/functiontest/test_conftest.py` & `pywbem-1.7.1/tests/unittest/functiontest/test_conftest.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test.mof` & `pywbem-1.7.1/tests/unittest/pywbem/test.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_cim_http.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_cim_http.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_cim_obj.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_cim_obj.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_cim_operations.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_cim_operations.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_cim_types.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_cim_types.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_cim_xml.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_cim_xml.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_exceptions.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_indicationlistener.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_indicationlistener.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_itermethods.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_itermethods.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_logging.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_logging.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_mof_compiler.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_mof_compiler.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_nocasedict.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_nocasedict.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_perf_equality.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_perf_equality.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_recorder.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_recorder.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_statistics.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_statistics.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_subscriptionmanager.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_subscriptionmanager.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_tupleparse.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_tupleparse.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_tupletree.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_tupletree.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_units.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_units.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_utils.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_valuemapping.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_valuemapping.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_warnings.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/test_wbemserverclass.py` & `pywbem-1.7.1/tests/unittest/pywbem/test_wbemserverclass.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error01.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error01.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error02.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error02.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/parse_error03.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/parse_error03.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/qualifiers.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/qualifiers.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/test_instance.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/test_instance.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem/testmofs/test_refs.mof` & `pywbem-1.7.1/tests/unittest/pywbem/testmofs/test_refs.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/conftest.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/conftest.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_complexassoc.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_complexassoc.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_inmemory_repository.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_inmemory_repository.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_multi_ns_assoc.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_multi_ns_assoc.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_providerdependentregistry.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_providerdependentregistry.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_providerregistry.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_providerregistry.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_system_providers.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_system_providers.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/pywbem_mock/test_wbemconnection_mock.py` & `pywbem-1.7.1/tests/unittest/pywbem_mock/test_wbemconnection_mock.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/resourcetest/test_memory_utils.py` & `pywbem-1.7.1/tests/unittest/resourcetest/test_memory_utils.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/simple_mock_model.mof` & `pywbem-1.7.1/tests/unittest/simple_mock_model.mof`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/dmtf_mof_schema_def.py` & `pywbem-1.7.1/tests/unittest/utils/dmtf_mof_schema_def.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/pytest_extensions.py` & `pywbem-1.7.1/tests/unittest/utils/pytest_extensions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/unichr2.py` & `pywbem-1.7.1/tests/unittest/utils/unichr2.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/unittest_extensions.py` & `pywbem-1.7.1/tests/unittest/utils/unittest_extensions.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/validate.py` & `pywbem-1.7.1/tests/unittest/utils/validate.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/unittest/utils/wbemserver_mock.py` & `pywbem-1.7.1/tests/unittest/utils/wbemserver_mock.py`

 * *Files identical despite different names*

### Comparing `pywbem-1.7.0/tests/utils.py` & `pywbem-1.7.1/tests/utils.py`

 * *Files identical despite different names*

