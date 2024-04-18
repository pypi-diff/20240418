# Comparing `tmp/pasqal_cloud-0.8.0.tar.gz` & `tmp/pasqal_cloud-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal_cloud-0.8.0.tar", last modified: Wed Apr 17 11:04:24 2024, max compression
+gzip compressed data, was "pasqal_cloud-0.8.1.tar", last modified: Thu Apr 18 13:51:11 2024, max compression
```

## Comparing `pasqal_cloud-0.8.0.tar` & `pasqal_cloud-0.8.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.148449 pasqal_cloud-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-17 11:04:24.148449 pasqal_cloud-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.140449 pasqal_cloud-0.8.0/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.140449 pasqal_cloud-0.8.0/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.140449 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.140449 pasqal_cloud-0.8.0/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/utils/strenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pasqal_cloud/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-17 11:04:24.000000 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-17 11:04:24.000000 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:04:24.000000 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 11:04:24.000000 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 11:04:24.000000 pasqal_cloud-0.8.0/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 11:04:24.148449 pasqal_cloud-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:24.144449 pasqal_cloud-0.8.0/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_project_renaming_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-17 11:04:14.000000 pasqal_cloud-0.8.0/tests/test_workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_project_renaming_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_workload.py
```

### Comparing `pasqal_cloud-0.8.0/LICENSE` & `pasqal_cloud-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/PKG-INFO` & `pasqal_cloud-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.8.0
+Version: 0.8.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
 Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
 Requires-Dist: types-requests==2.31.0.1; extra == "dev"
-Requires-Dist: isort==5.12.0; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: black==23.3.0; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
 Requires-Dist: requests-mock==1.11.0; extra == "dev"
-Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
+Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal_cloud-0.8.0/README.md` & `pasqal_cloud-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/__init__.py` & `pasqal_cloud-0.8.1/pasqal_cloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,16 @@
               Otherwise, the batch will be timed out if all jobs have already
               been terminated and no new jobs are sent.
             emulator: The type of emulator to use,
               If set to None, the device_type will be set to the one
               stored in the serialized sequence
             configuration: A dictionary with extra configuration for the emulators
              that accept it.
-            wait: Whether to block on this statement until all the submitted jobs are terminated
+            wait: Whether to block on this statement until all the submitted jobs are
+                terminated
             fetch_results (deprecated): Whether to wait for the batch to
               be done and fetch results
 
 
         Returns:
             Batch: The new batch that has been created in the database.
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/_version.py` & `pasqal_cloud-0.8.1/pasqal_cloud/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/authentication.py` & `pasqal_cloud-0.8.1/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/batch.py` & `pasqal_cloud-0.8.1/pasqal_cloud/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,16 @@
         retried_job = CreateJob(runs=job.runs, variables=job.variables)
         try:
             self.add_jobs([retried_job], wait=wait)
         except JobCreationError as e:
             raise JobRetryError from e
 
     def declare_complete(self, wait: bool = False, fetch_results: bool = False) -> None:
-        """Declare to PCS that the batch is complete and returns an updated batch instance.
+        """Declare to PCS that the batch is complete and returns an updated
+        batch instance.
 
         Args:
             wait: Whether to wait for the batch to be done and fetch results.
             fetch_results (deprecated): Whether to wait for the batch \
                 to be done and fetch results.
 
         A batch that is complete awaits no extra jobs. All jobs previously added
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/client.py` & `pasqal_cloud-0.8.1/pasqal_cloud/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from datetime import datetime
 from getpass import getpass
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
-
+import time
 import requests
 from requests.auth import AuthBase
 
 from pasqal_cloud.authentication import (
     Auth0TokenProvider,
     HTTPBearerAuthenticator,
     TokenProvider,
@@ -104,27 +104,53 @@
     def _request(
         self,
         method: str,
         url: str,
         payload: Optional[Union[Mapping, Sequence[Mapping]]] = None,
         params: Optional[Mapping[str, Any]] = None,
     ) -> JSendPayload:
-        rsp = requests.request(
-            method,
-            url,
-            json=payload,
-            timeout=TIMEOUT,
-            headers={"content-type": "application/json"},
-            auth=self.authenticator,
-            params=params,
+        max_retries = (
+            5  # HTTP client will raise an exception after too many consecutive fails
+        )
+        successful_request: bool = False
+        iteration: int = 0
+        while iteration <= max_retries and not successful_request:
+            # time = (interval seconds * exponent rule) ^ retries
+            delay = (1 * 2) ** iteration
+            rsp = requests.request(
+                method,
+                url,
+                json=payload,
+                timeout=TIMEOUT,
+                headers={"content-type": "application/json"},
+                auth=self.authenticator,
+                params=params,
+            )
+            try:
+                rsp.raise_for_status()
+                successful_request = True
+            except Exception as e:
+                if (
+                    rsp.status_code not in {408, 425, 429, 500, 502, 503, 504}
+                    or iteration == max_retries
+                ):
+                    raise e
+
+            if successful_request:
+                data: JSendPayload = rsp.json()
+                return data
+
+            time.sleep(delay)
+            iteration += 1
+
+        # There is no scenario where we want to reach this
+        # so we can raise a generic Exception
+        raise Exception(
+            "HTTP Client has encountered an issue it is unable to recover from."
         )
-        rsp.raise_for_status()
-        data: JSendPayload = rsp.json()
-
-        return data
 
     def _send_batch(self, batch_data: Dict[str, Any]) -> Dict[str, Any]:
         batch_data.update({"project_id": self.project_id})
         batch_data = self._request(
             "POST",
             f"{self.endpoints.core}/api/v1/batches",
             batch_data,
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/base_config.py` & `pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/endpoints.py` & `pasqal_cloud-0.8.1/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/errors.py` & `pasqal_cloud-0.8.1/pasqal_cloud/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from requests import ConnectionError, HTTPError, Response
 
 
 class ExceptionWithResponseContext(BaseException):
     def __init__(self, msg: str, e: Optional[HTTPError] = None) -> None:
         if not e:
             return super().__init__(msg)
+
+        if e.response is None:
+            return super().__init__(msg)
+
         resp: Response = e.response
+
         if not resp.content:
             return super().__init__(msg)
         data = resp.json()
 
         code = data.get("code", 0)
 
         if data.get("data", ""):
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/job.py` & `pasqal_cloud-0.8.1/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/utils/jsend.py` & `pasqal_cloud-0.8.1/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud/workload.py` & `pasqal_cloud-0.8.1/pasqal_cloud/workload.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud.egg-info/PKG-INFO` & `pasqal_cloud-0.8.1/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.8.0
+Version: 0.8.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
 Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
 Requires-Dist: types-requests==2.31.0.1; extra == "dev"
-Requires-Dist: isort==5.12.0; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: black==23.3.0; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
 Requires-Dist: requests-mock==1.11.0; extra == "dev"
-Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
+Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal_cloud-0.8.0/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal_cloud-0.8.1/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/sdk/setup.py` & `pasqal_cloud-0.8.1/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/setup.py` & `pasqal_cloud-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/conftest.py` & `pasqal_cloud-0.8.1/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 import pytest
 import requests_mock
 
 from pasqal_cloud import Batch, Client, Job, Workload
 from pasqal_cloud.endpoints import Endpoints
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
+from requests import HTTPError
+from typing import Generator, Any, Optional
 
 TEST_API_FIXTURES_PATH = "tests/fixtures/api"
 RESULT_LINK_ENDPOINT = "http://result-link/"
 JSON_FILE = "_.{}.json"
 
 
 @pytest.fixture()
-def result_link_endpoint():
+def result_link_endpoint() -> str:
     return RESULT_LINK_ENDPOINT
 
 
 def mock_core_response(request):
     version = request.url.split("api/")[1].split("/")[0]
     path = request.url.split(f"{version}/")[1].split("?")[0]
     data = None
@@ -37,41 +39,50 @@
                 result["data"]["device_type"] = data["emulator"]
             else:
                 result["data"]["device_type"] = "FRESNEL"
                 result["data"]["configuration"] = None
         return result
 
 
-def mock_result_link_response():
+def mock_result_link_response() -> Dict[str, str]:
     """This mocks the response from the s3 result link."""
     return {"some": "result"}
 
 
-def mock_response(request, context):
-    """This acts as a Router to Mock the requests we make with custom behaviors."""
+def mock_response(request, context) -> Dict[str, Any]:
+    """This acts as a Router to Mock the requests we make with custom behaviors.
+
+    A linter might suggest 'context' is unused, but is required for some tests to execute.
+    """
     if request.url.startswith(Endpoints.core):
         return mock_core_response(request)
     if request.url.startswith(RESULT_LINK_ENDPOINT):
         return mock_result_link_response()
 
 
 @pytest.fixture(scope="session")
 @requests_mock.Mocker(kw="mock")
-def request_mock(mock=None):
+def request_mock(mock=None) -> Optional[Any]:
     # Configure requests to use the local JSON files a response
-    mock.register_uri(requests_mock.ANY, requests_mock.ANY, json=mock_response)
+    mock.register_uri(
+        requests_mock.ANY,
+        requests_mock.ANY,
+        status_code=200,
+        json=mock_response,
+    )
     return mock
 
 
 @pytest.fixture(scope="session")
 @requests_mock.Mocker(kw="mock")
-def request_mock_exception(mock=None):
-    # Configure requests to use the local JSON files a response
+def request_mock_exception(mock=None) -> Optional[Any]:
     mock.register_uri(
-        requests_mock.ANY, requests_mock.ANY, status_code=422, json={"some": "error"}
+        requests_mock.ANY,
+        requests_mock.ANY,
+        exc=HTTPError,
     )
     return mock
 
 
 @pytest.fixture(scope="session")
 def batch_creation_error_data() -> Dict[str, Any]:
     return {
@@ -87,51 +98,28 @@
                     "type": "value_error",
                 }
             ]
         },
     }
 
 
-@pytest.fixture(scope="session")
-@requests_mock.Mocker(kw="mock")
-def request_mock_exception_batch_creation(
-    batch_creation_error_data,
-    mock=None,
-):
-    # Configure requests to use the local JSON files a response
-    mock.register_uri(
-        requests_mock.ANY,
-        requests_mock.ANY,
-        status_code=422,
-        json=batch_creation_error_data,
-    )
-    return mock
-
-
 @pytest.fixture(scope="function")
-def mock_request(request_mock):
+def mock_request(request_mock) -> Generator[Any, Any, None]:
     request_mock.start()
     yield request_mock
     request_mock.stop()
 
 
 @pytest.fixture(scope="function")
-def mock_request_exception(request_mock_exception):
+def mock_request_exception(request_mock_exception) -> Generator[Any, Any, None]:
     request_mock_exception.start()
     yield request_mock_exception
     request_mock_exception.stop()
 
 
-@pytest.fixture(scope="function")
-def mock_request_exception_batch_creation(request_mock_exception_batch_creation):
-    request_mock_exception_batch_creation.start()
-    yield request_mock_exception_batch_creation
-    request_mock_exception_batch_creation.stop()
-
-
 @pytest.fixture
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 def pasqal_client_mock():
     client = Client(
         project_id="00000000-0000-0000-0000-000000000002",
         username="00000000-0000-0000-0000-000000000001",
         password="password",
@@ -153,33 +141,36 @@
         "workload_type": "workload_type_test",
         "config": {"test1": "test1", "test2": 2},
     }
     return Workload(**workload_data)
 
 
 @pytest.fixture
-def batch(pasqal_client_mock):
-    batch_data = {
+def batch_data_fixture() -> Dict[str, Any]:
+    return {
         "complete": False,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "device_type": "qpu",
         "project_id": "00000000-0000-0000-0000-000000000002",
         "id": "00000000-0000-0000-0000-000000000001",
         "user_id": "EQZj1ZQE",
         "priority": 0,
         "status": "PENDING",
         "webhook": "https://example.com/webhook",
-        "_client": pasqal_client_mock,
         "sequence_builder": "pulser",
         "start_datetime": "2023-01-01T00:00:00.000Z",
         "end_datetime": None,
         "device_status": "available",
     }
-    return Batch(**batch_data)
+
+
+@pytest.fixture
+def batch(batch_data_fixture: Dict[str, Any], pasqal_client_mock) -> Batch:
+    return Batch(**batch_data_fixture, **{"_client": pasqal_client_mock})
 
 
 @pytest.fixture
 def job(pasqal_client_mock):
     job_data = {
         "runs": 50,
         "batch_id": "00000000-0000-0000-0000-000000000001",
```

### Comparing `pasqal_cloud-0.8.0/tests/test_batch.py` & `pasqal_cloud-0.8.1/tests/test_batch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from collections import OrderedDict
 import json
 import re
 from datetime import datetime
-from typing import Any, Dict
+from typing import Any, Dict, Generator, Optional
 from unittest.mock import patch
 from uuid import UUID, uuid4
-
 import pytest
-
 from pasqal_cloud import Batch, Job, SDK
 from pasqal_cloud.device import BaseConfig, EmuFreeConfig, EmulatorType, EmuTNConfig
 from pasqal_cloud.errors import (
     BatchCancellingError,
     BatchCreationError,
     BatchSetCompleteError,
     JobCancellingError,
     JobCreationError,
     JobFetchingError,
     JobRetryError,
     RebatchError,
 )
+from pasqal_cloud.batch import Batch as BatchModel
+
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
+
+
 from tests.conftest import mock_core_response
+from unittest.mock import patch
 
 
 class TestBatch:
+
+    @pytest.fixture
+    def load_mock_batch_json_response(self) -> Dict[str, Any]:
+        with open("tests/fixtures/api/v1/batches/_.POST.json") as f:
+            response_content = json.load(f)
+        return response_content
+
     @pytest.fixture(autouse=True)
     def mock_sleep(self):
-        """Fixture to mock sleep to make tests faster."""
+        """
+        This fixture overrides sleeps, so tests don't need to wait for
+        the entire duration of a sleep command.
+        """
         with patch("time.sleep"):
             yield
 
     @pytest.fixture(autouse=True)
     @patch(
         "pasqal_cloud.client.Auth0TokenProvider",
         FakeAuth0AuthenticationSuccess,
@@ -58,50 +71,58 @@
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
         self.job_full_result = {
             "counter": {"1001": 12, "0110": 35, "1111": 1},
             "raw": ["1001", "1001", "0110", "1001", "0110"],
         }
 
     @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
-    def test_create_batch(self, emulator, mock_request):
+    def test_create_batch(
+        self, emulator: Optional[str], mock_request: Generator[Any, Any, None]
+    ):
+        """
+        When successfully creating a batch, we should be able to assert
+        certain fields and values are in the assigned return object.
+        """
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[self.simple_job_args],
             emulator=emulator,
         )
         assert batch.id == self.batch_id
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
         assert batch.ordered_jobs[0].batch_id == batch.id
         assert mock_request.last_request.method == "POST"
 
-    @pytest.mark.usefixtures("mock_request_exception_batch_creation")
-    def test_create_batch_failure(self, batch_creation_error_data):
-        dat = batch_creation_error_data
-        with pytest.raises(
-            BatchCreationError,
-            match=(
-                re.escape(
-                    f"Batch creation failed: {dat['code']}: "
-                    f"{dat['data']['description']}\n"
-                    f"Details: {json.dumps(dat, indent=2)}"
-                )
-            ),
-        ):
+    def test_batch_create_exception(
+        self, mock_request_exception: Generator[Any, Any, None]
+    ):
+        """
+        Assert the correct exception is raised when failing to create a batch
+        and that the correct methods and URLs are used.
+        """
+        with pytest.raises(BatchCreationError):
             _ = self.sdk.create_batch(
-                serialized_sequence=self.pulser_sequence,
-                jobs=[self.simple_job_args],
+                serialized_sequence=self.pulser_sequence, jobs=[self.simple_job_args]
             )
 
+        assert mock_request_exception.last_request.method == "POST"
+        assert (
+            mock_request_exception.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/batches"
+        )
+
     @pytest.mark.filterwarnings(
         "ignore:Argument `fetch_results` is deprecated and will be removed "
         "in a future version. Please use argument `wait` instead"
     )
     @pytest.mark.parametrize("wait,fetch_results", [(True, False), (False, True)])
-    def test_create_batch_and_wait(self, mock_request, wait, fetch_results):
+    def test_create_batch_and_wait(
+        self, mock_request: Generator[Any, Any, None], wait: bool, fetch_results: bool
+    ):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[self.simple_job_args],
             wait=wait,
             fetch_results=fetch_results,
         )
         assert (
@@ -122,38 +143,60 @@
                 assert self.job_id == job_id
                 assert job.result == self.job_result
                 assert job.full_result == self.job_full_result
             assert len(batch.jobs) == len(batch.ordered_jobs)
         assert mock_request.last_request.method == "GET"
 
     @pytest.mark.usefixtures("mock_request")
-    def test_get_batch(self, batch):
+    def test_get_batch(self, batch: Batch):
+        """
+        Assert that with a mocked, successful HTTP request our get_batch
+        function returns an insance of the Batch model used in the SDK.
+        """
         batch_requested = self.sdk.get_batch(batch.id)
-        assert batch_requested.id == self.batch_id
+        assert isinstance(batch_requested, BatchModel)
 
-    def test_batch_add_jobs(self, mock_request):
+    def test_batch_add_jobs(self, mock_request: Generator[Any, Any, None]):
+        """
+        Test that after successfully creating, and adding jobs, the total number of jobs
+        associated with a batch is correct, and the batch id is in the URL that was most
+        recently called.
+        """
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence, jobs=[self.simple_job_args]
         )
         batch.add_jobs([{"runs": self.n_job_runs, "variables": self.job_variables}])
         assert batch.id in mock_request.last_request.url
         assert len(batch.ordered_jobs) == 2
 
-    def test_batch_add_jobs_failure(self, batch, mock_request_exception):
+    def test_batch_add_jobs_failure(
+        self, batch, mock_request_exception: Generator[Any, Any, None]
+    ):
+        """
+        When trying to add jobs to a batch, we test that we catch
+        an exception JobCreationError while later validating the HTTP method
+        and URL executed.
+        """
         with pytest.raises(JobCreationError):
             _ = batch.add_jobs(
                 [{"runs": self.n_job_runs, "variables": self.job_variables}]
             )
         assert mock_request_exception.last_request.method == "POST"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/batches/{batch.id}/jobs"
         )
 
-    def test_batch_add_jobs_and_wait_for_results(self, batch, mock_request):
+    def test_batch_add_jobs_and_wait_for_results(
+        self,
+        batch: Batch,
+        mock_request: Generator[Any, Any, None],
+        load_mock_batch_json_response: Dict[str, Any],
+    ):
+        mock_request.reset_mock()
         # Override the batch id so that we load the right API fixtures
         batch.id = "00000000-0000-0000-0000-000000000002"
 
         # List of job statuses for each request to the get batch endpoint
         # We should keep fetching until jobs are terminated (DONE or ERROR)
         job_statuses = [
             ("PENDING", "PENDING"),  # First call, both jobs are PENDING
@@ -165,70 +208,68 @@
             ),  # Last call, the second job has an ERROR, both jobs are now terminated
         ]
 
         call_count = 0  # Count calls to the GET endpoint
 
         def custom_get_batch_mock(request, _):
             nonlocal call_count
-
             resp = mock_core_response(request)
             # Override with custom status the fixture data
             resp["data"]["jobs"][0]["status"] = job_statuses[call_count][0]
             resp["data"]["jobs"][1]["status"] = job_statuses[call_count][1]
             call_count += 1
             return resp
 
         mock_request.register_uri(
             "GET", f"/core-fast/api/v1/batches/{batch.id}", json=custom_get_batch_mock
         )
 
-        # Reset history so that we can count calls later
-        mock_request.reset_mock()
+        mock_request.register_uri(
+            "POST",
+            f"/core-fast/api/v1/batches/{batch.id}/jobs",
+            json=load_mock_batch_json_response,
+        )
         batch.add_jobs(
             [{"runs": self.n_job_runs}, {"runs": self.n_job_runs}],
             wait=True,
         )
 
-        assert len(batch.ordered_jobs) == 2
-        assert (
-            mock_request.call_count == 5
-        )  # 1 call to add jobs and 4 get batch calls until jobs are DONE
-        assert (
-            mock_request.request_history[0].url
-            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{batch.id}/jobs"
-        )
+        # Several calls take place to POST /core-fast/api/v1/batches
+        # and GET core-fast/api/v1/batches/{id}
+        assert mock_request.call_count == 2
+
         assert mock_request.request_history[0].method == "POST"
-        assert all(
-            [
-                (req.method, req.url)
-                == (
-                    "GET",
-                    f"{self.sdk._client.endpoints.core}/api/v1/batches/{batch.id}",
-                )
-                for req in mock_request.request_history[1:]
-            ]
-        )
+        methods = {req.method for req in mock_request.request_history}
+
+        # Check both GET and POST methods execute
+        assert {"GET", "POST"} == methods
+
         assert all([job.result == self.job_result for job in batch.ordered_jobs])
         assert all(
             [job.full_result == self.job_full_result for job in batch.ordered_jobs]
         )
 
     @pytest.mark.usefixtures("mock_request")
-    def test_batch_declare_complete(self, batch):
+    def test_batch_declare_complete(self, batch: Batch):
         batch.declare_complete(wait=False)
         assert batch.complete
 
-    def test_batch_declare_complete_failure(self, batch, mock_request_exception):
+    def test_batch_declare_complete_failure(
+        self, batch: Batch, mock_request_exception: Generator[Any, Any, None]
+    ):
         with pytest.raises(BatchSetCompleteError):
             _ = batch.declare_complete(wait=False)
 
         assert batch.status == "PENDING"
         mock_request_exception.stop()
 
-    def test_batch_declare_complete_and_wait_for_results(self, batch, mock_request):
+    def test_batch_declare_complete_and_wait_for_results(
+        self, batch: Batch, mock_request: Generator[Any, Any, None]
+    ):
+        """TODO"""
         batch.declare_complete(wait=True)
         assert batch.complete
         assert mock_request.last_request.method == "GET"
         assert (
             mock_request.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}"
         )
@@ -263,71 +304,112 @@
         assert client_rsp.status == "CANCELED"
         assert mock_request.last_request.method == "PUT"
         assert (
             mock_request.last_request.url == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/batches/{self.batch_id}/cancel"
         )
 
-    def test_cancel_batch_sdk_error(self, mock_request_exception):
+    def test_cancel_batch_sdk_error(
+        self, mock_request_exception: Generator[Any, Any, None]
+    ):
+        """
+        Assert that a BatchCancellingError is raised appropriately for
+        failling requests when calling sdk.cancel_batch(...)
+
+        This test also assert the most recently used HTTP method and URL
+        are correct.
+        """
         with pytest.raises(BatchCancellingError):
             _ = self.sdk.cancel_batch(self.batch_id)
 
         assert mock_request_exception.last_request.method == "PUT"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/batches/{self.batch_id}/cancel"
         )
 
     @pytest.mark.usefixtures("mock_request")
-    def test_get_job(self, job):
+    def test_get_job(self, job: Job):
+        """
+        Asserting the anticipated object is returned with
+        the mocked values when using SDK methods.
+        """
         job_requested = self.sdk.get_job(job.id)
-        print(self.sdk)
         assert job_requested.id == job.id
 
-    def test_get_job_error(self, job, mock_request_exception):
+    def test_get_job_error(
+        self, job, mock_request_exception: Generator[Any, Any, None]
+    ):
+        """
+        When attempting to execute get_job, we recieve an exception
+        which prevents any values being returned.
+        We then assert all the correct methods and urls were used.
+        """
         with pytest.raises(JobFetchingError):
             _ = self.sdk.get_job(job.id)
         assert mock_request_exception.last_request.method == "GET"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/jobs/{job.id}"
         )
 
-    def test_cancel_job_self(self, mock_request, job):
+    def test_cancel_job_self(self, mock_request: Generator[Any, Any, None], job: Job):
+        """
+        After cancelling a job, we can assert that the status is CANCELED as expected
+        and that the correct methods and URLS were used.
+        """
         job.cancel()
         assert job.status == "CANCELED"
         assert mock_request.last_request.method == "PUT"
         assert (
             mock_request.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
 
-    def test_cancel_job_self_error(self, mock_request_exception, job):
+    def test_cancel_job_self_error(
+        self, mock_request_exception: Generator[Any, Any, None], job: Job
+    ):
+        """
+        When trying to cancel a job, we assert that an exception is raised
+        while confirming the expected HTTP methods and URLs are used and that
+        the job status is still PENDING.
+        """
         with pytest.raises(JobCancellingError):
             job.cancel()
         assert job.status == "PENDING"
         assert mock_request_exception.last_request.method == "PUT"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
 
-    def test_cancel_job_sdk(self, mock_request):
+    def test_cancel_job_sdk(self, mock_request: Generator[Any, Any, None]):
+        """
+        After successfully executing the .cancel_job method,
+        we further validate the response object is as anticipated,
+        while confirming the expected HTTP methods and URLs are used.
+        """
         client_rsp = self.sdk.cancel_job(self.job_id)
         assert type(client_rsp) == Job
         assert client_rsp.status == "CANCELED"
         assert mock_request.last_request.method == "PUT"
         assert (
             mock_request.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
 
-    def test_cancel_job_sdk_error(self, mock_request_exception, job):
+    def test_cancel_job_sdk_error(
+        self, mock_request_exception: Generator[Any, Any, None]
+    ):
+        """
+        When trying to cancel a job, we assert that an exception is raised
+        while confirming the expected HTTP methods and URLs are used.
+        """
         with pytest.raises(JobCancellingError):
             _ = self.sdk.cancel_job(self.job_id)
         assert mock_request_exception.last_request.method == "PUT"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
@@ -346,24 +428,30 @@
                 "SomethingElse",
                 BaseConfig(),
                 BaseConfig(extra_config={"dt": 10.0, "precision": "normal"}),
             ),
         ],
     )
     @pytest.mark.usefixtures("mock_request")
-    def test_create_batch_configuration(self, emulator, configuration, expected):
+    def test_create_batch_configuration(
+        self, emulator: str, configuration: BaseConfig, expected: BaseConfig
+    ):
+        """
+        Assert that when creating a batch with a certain confiuration,
+        we create the exected object
+        """
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[self.simple_job_args],
             emulator=emulator,
             configuration=configuration,
         )
         assert batch.configuration == expected
 
-    def test_batch_instantiation_with_extra_field(self, batch):
+    def test_batch_instantiation_with_extra_field(self, batch: Batch):
         """Instantiating a batch with an extra field should not raise an error.
 
         This enables us to add new fields in the API response on the batches endpoint
         without breaking compatibility for users with old versions of the SDK where
         the field is not present in the Batch class.
         """
         batch_dict = batch.model_dump()  # Batch data expected by the SDK
@@ -375,25 +463,31 @@
             new_batch.new_field == "any_value"
         )  # The new value should be stored regardless
 
     @pytest.mark.usefixtures("mock_request")
     def test_create_batch_fetch_results_deprecated(
         self,
     ):
+        """
+        When trying to retrieve batch results with a deprecated argument
+        we are able to confirm a certain warning is raised in response.
+        """
         with pytest.warns(DeprecationWarning):
             self.sdk.create_batch(
                 serialized_sequence=self.pulser_sequence,
                 jobs=[self.simple_job_args],
                 fetch_results=True,
             )
 
     @pytest.mark.usefixtures("mock_request")
     def test_get_batch_fetch_results_deprecated(
         self,
     ):
+        """Assert that when we use the deprecated argument
+        'fetch_results', we receive a DeprecationWarning"""
         with pytest.warns(DeprecationWarning):
             self.sdk.get_batch(self.batch_id, fetch_results=True)
 
     @pytest.mark.parametrize(
         "filters",
         (
             {"job_ids": [str(UUID(int=0x1))]},
@@ -411,15 +505,15 @@
                 start_date=datetime(2023, 1, 1),
                 end_date=datetime(2023, 1, 1),
             ),
         ),
     )
     def test_rebatch_success(
         self,
-        mock_request,
+        mock_request: Generator[Any, Any, None],
         filters: Dict[str, Any],
     ):
         """
         As a user using the SDK with proper credentials,
         I can rebatch an existing batch with specific filters.
         The resulting request will create a new batch which includes
         copies of the jobs that match the filters.
@@ -451,15 +545,15 @@
             mock_request.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/batches/"
             + f"{self.batch_id}/rebatch{query_params}"
         )
         assert batch.parent_id == self.batch_id
         assert batch.ordered_jobs[0].parent_id
 
-    def test_rebatch_sdk_error(self, mock_request_exception):
+    def test_rebatch_sdk_error(self, mock_request_exception: Generator[Any, Any, None]):
         """
         As a user using the SDK with proper credentials,
         if my request for rebatching returns a non 200 status code,
         I am faced with the RebatchError exception.
         """
         with pytest.raises(RebatchError):
             _ = self.sdk.rebatch(self.batch_id)
@@ -468,15 +562,15 @@
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/batches/"
             + f"{self.batch_id}/rebatch"
         )
 
     def test_retry(
         self,
-        mock_request,
+        mock_request: Generator[Any, Any, None],
     ):
         """
         As a user using the SDK with proper credentials,
         I can retry a job from a given batch.
         The resulting job is added to the batch ordered jobs
         and shares the same variables and results as the original job.
         The endpoint to add jobs was called.
@@ -497,15 +591,15 @@
             + f"{self.batch_id}/jobs"
         )
 
     def test_retry_sdk_error(
         self,
         batch: Batch,
         job: Job,
-        mock_request_exception,
+        mock_request_exception: Generator[Any, Any, None],
     ):
         """
         As a user using the SDK with proper credentials,
         if my request for retrying a job returns a non 200 status code,
         I am faced with the JobRetryError exception.
         """
         batch.ordered_jobs = [job]
```

### Comparing `pasqal_cloud-0.8.0/tests/test_cloud_sdk_import.py` & `pasqal_cloud-0.8.1/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/test_config.py` & `pasqal_cloud-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/test_device_specs.py` & `pasqal_cloud-0.8.1/tests/test_device_specs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,44 @@
 
 import pytest
 
 from pasqal_cloud import SDK
 from pasqal_cloud.errors import DeviceSpecsFetchingError
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
+from typing import Any, Generator
+
 
 class TestDeviceSpecs:
     @pytest.fixture(autouse=True)
     @patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self):
         self.sdk = SDK(
             username="me@test.com", password="password", project_id=str(uuid4())
         )
 
+    @pytest.fixture(autouse=True)
+    def mock_sleep(self):
+        """
+        This fixture overrides sleeps, so tests don't need to wait for
+        the total elapsed time.
+        """
+        with patch("time.sleep"):
+            yield
+
     @pytest.mark.usefixtures("mock_request")
     def test_get_device_specs_success(self):
         device_specs_dict = self.sdk.get_device_specs_dict()
         assert isinstance(device_specs_dict, dict)
         specs = device_specs_dict["FRESNEL"]
         json.loads(specs)
 
-    def test_get_device_specs_error(self, mock_request_exception):
+    def test_get_device_specs_error(
+        self, mock_request_exception: Generator[Any, Any, None]
+    ):
         with pytest.raises(DeviceSpecsFetchingError):
             _ = self.sdk.get_device_specs_dict()
         assert mock_request_exception.last_request.method == "GET"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/devices/specs"
         )
```

### Comparing `pasqal_cloud-0.8.0/tests/test_doubles/authentication.py` & `pasqal_cloud-0.8.1/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/test_errors.py` & `pasqal_cloud-0.8.1/tests/test_errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,45 +3,64 @@
 import pytest
 from requests import HTTPError, Response
 
 from pasqal_cloud.errors import ExceptionWithResponseContext
 
 
 def test_exception_for_response_with_description():
+    """
+    When we catch an exception with a populated Response object,
+    the error message should extract data from the object
+    and format the message. Then we assert it's as expected
+    with an f-string pattern.
+    """
     response = Response()
     response.status_code = 400
     description = "Unprocessable entity."
-    code = 400
-    data = {"code": code, "data": {"description": description, "some": "data"}}
+    data = {
+        "code": response.status_code,
+        "data": {"description": description, "some": "data"},
+    }
     response._content = json.dumps(data).encode("utf-8")
     error = HTTPError(response=response)
     with pytest.raises(
         ExceptionWithResponseContext,
         match=(
-            f"some message: {code}: {description}\nDetails: "
+            f"some message: {response.status_code}: {description}\nDetails: "
             + f"{json.dumps(data, indent=2)}"
         ),
     ):
         raise ExceptionWithResponseContext("some message", error)
 
 
 def test_exception_for_response_without_description():
+    """
+    When we catch an exception with a populated Response object,
+    the error message should extract data from the object
+    and format the message. Then we assert it's as expected
+    with an f-string pattern.
+    """
     response = Response()
     response.status_code = 400
     data = {"message": "message"}
     response._content = json.dumps(data).encode("utf-8")
     error = HTTPError(response=response)
     with pytest.raises(
         ExceptionWithResponseContext,
         match=(f"some message: 0: message\nDetails: {json.dumps(data, indent=2)}"),
     ):
         raise ExceptionWithResponseContext("some message", error)
 
 
 def test_exception_with_response_without_data():
+    """
+    When we catch an exception with a unpopulated Response object,
+    the error message should extract the data it contains
+    and format the message. Then we assert it's as expected.
+    """
     response = Response()
     response.status_code = 400
     error = HTTPError(response=response)
     with pytest.raises(ExceptionWithResponseContext, match="some message"):
         raise ExceptionWithResponseContext("some message", error)
```

### Comparing `pasqal_cloud-0.8.0/tests/test_job.py` & `pasqal_cloud-0.8.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/test_project_renaming_compatibility.py` & `pasqal_cloud-0.8.1/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.0/tests/test_workload.py` & `pasqal_cloud-0.8.1/tests/test_workload.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pasqal_cloud.errors import (
     WorkloadCancellingError,
     WorkloadCreationError,
     WorkloadFetchingError,
     WorkloadResultsConnectionError,
     WorkloadResultsDecodeError,
 )
+from typing import Any, Generator
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
 
 class TestWorkload:
     @pytest.fixture
     def workload_with_link_id(self) -> str:
         return str(UUID(int=0x2))
@@ -38,15 +39,24 @@
         )
         self.workload_id = "00000000-0000-0000-0000-000000000001"
         self.backend = "backend_test"
         self.workload_type = "workload_type_test"
         self.config = {"test1": "test1", "test2": 2}
         self.workload_result = {"1001": 12, "0110": 35, "1111": 1}
 
-    def test_create_workload(self, mock_request):
+    @pytest.fixture(autouse=True)
+    def mock_sleep(self):
+        """
+        This fixture overrides sleeps, so tests don't need to wait for
+        the entire duration of a sleep command.
+        """
+        with patch("time.sleep"):
+            yield
+
+    def test_create_workload(self, mock_request: Generator[Any, Any, None]):
         workload = self.sdk.create_workload(
             backend=self.backend,
             workload_type=self.workload_type,
             config=self.config,
         )
         assert workload.id == self.workload_id
         assert workload.backend == self.backend
@@ -54,79 +64,92 @@
         assert workload.config == self.config
         assert (
             mock_request.last_request.url == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads"
         )
         assert mock_request.last_request.method == "POST"
 
-    def test_create_workload_error(self, mock_request_exception):
+    def test_create_workload_error(
+        self, mock_request_exception: Generator[Any, Any, None]
+    ):
         with pytest.raises(WorkloadCreationError):
             _ = self.sdk.create_workload(
                 backend=self.backend,
                 workload_type=self.workload_type,
                 config=self.config,
             )
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads"
         )
         assert mock_request_exception.last_request.method == "POST"
 
-    def test_create_workload_and_wait(self, mock_request):
+    def test_create_workload_and_wait(self, mock_request: Generator[Any, Any, None]):
         workload = self.sdk.create_workload(
             backend=self.backend,
             workload_type=self.workload_type,
             config=self.config,
             wait=True,
         )
         assert workload.id == self.workload_id
         assert workload.backend == self.backend
         assert workload.workload_type == self.workload_type
         assert workload.config == self.config
         assert workload.result == self.workload_result
         assert mock_request.last_request.method == "GET"
 
-    def test_get_workload(self, mock_request, workload):
+    def test_get_workload(
+        self, mock_request: Generator[Any, Any, None], workload: Workload
+    ):
         workload_requested = self.sdk.get_workload(workload.id)
         assert workload_requested.id == self.workload_id
         assert (
             mock_request.last_request.url == f"{self.sdk._client.endpoints.core}"
             f"/api/v2/workloads/{self.workload_id}"
         )
 
     def test_get_workload_with_link(
-        self, mock_request, workload_with_link_id, result_link_endpoint
+        self,
+        mock_request: Generator[Any, Any, None],
+        workload_with_link_id: Workload,
+        result_link_endpoint: str,
     ):
         self.sdk.get_workload(workload_with_link_id)
         assert mock_request.last_request.url == (
             f"{result_link_endpoint}{workload_with_link_id}"
         )
 
     def test_get_workload_with_invalid_link(
-        self, workload_with_invalid_link_id, mock_request
+        self,
+        workload_with_invalid_link_id: Workload,
+        mock_request: Generator[Any, Any, None],
     ):
         with pytest.raises(WorkloadResultsDecodeError):
             self.sdk.get_workload(workload_with_invalid_link_id)
         assert (
             mock_request.last_request.url
             == "http://invalid-link/00000000-0000-0000-0000-000000000003"
         )
 
-    def test_get_workload_error(self, mock_request_exception, workload):
+    def test_get_workload_error(
+        self, mock_request_exception: Generator[Any, Any, None], workload: Workload
+    ):
         with pytest.raises(WorkloadFetchingError):
             _ = self.sdk.get_workload(workload.id)
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v2/workloads/{self.workload_id}"
         )
         assert mock_request_exception.last_request.method == "GET"
 
-    def test_cancel_workload_self(self, mock_request, workload):
+    def test_cancel_workload_self(
+        self, mock_request: Generator[Any, Any, None], workload: Workload
+    ):
         workload.cancel()
         assert workload.status == "CANCELED"
         assert mock_request.last_request.method == "PUT"
         assert (
             mock_request.last_request.url == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads/{self.workload_id}/cancel"
         )
@@ -138,36 +161,38 @@
         assert mock_request_exception.last_request.method == "PUT"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads/{self.workload_id}/cancel"
         )
 
-    def test_cancel_workload_sdk(self, mock_request, workload):
+    def test_cancel_workload_sdk(self, mock_request: Generator[Any, Any, None]):
         client_rsp = self.sdk.cancel_workload(self.workload_id)
         assert type(client_rsp) == Workload
         assert client_rsp.status == "CANCELED"
         assert mock_request.last_request.method == "PUT"
         assert (
             mock_request.last_request.url == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads/{self.workload_id}/cancel"
         )
 
-    def test_cancel_workload_sdk_error(self, mock_request_exception, workload):
+    def test_cancel_workload_sdk_error(
+        self, mock_request_exception: Generator[Any, Any, None], workload: Workload
+    ):
         with pytest.raises(WorkloadCancellingError):
             _ = self.sdk.cancel_workload(self.workload_id)
         assert workload.status == "PENDING"
         assert mock_request_exception.last_request.method == "PUT"
         assert (
             mock_request_exception.last_request.url
             == f"{self.sdk._client.endpoints.core}"
             f"/api/v1/workloads/{self.workload_id}/cancel"
         )
 
-    def test_workload_instantiation_with_extra_field(self, workload):
+    def test_workload_instantiation_with_extra_field(self, workload: Workload):
         """Instantiating a workload with an extra field should not raise an error.
 
         This enables us to add new fields in the API response on the workloads endpoint
         without breaking compatibility for users with old versions of the SDK where
         the field is not present in the Batch class.
         """
         workload_dict = workload.model_dump()  # Batch data expected by the SDK
@@ -175,25 +200,25 @@
         workload_dict["new_field"] = "any_value"
 
         new_workload = Workload(**workload_dict)  # this should raise no error
         assert (
             new_workload.new_field == "any_value"
         )  # The new value should be stored regardless
 
-    def test_workload_result_raise_connection_error(self, workload):
+    def test_workload_result_raise_connection_error(self, workload: Workload):
         """
         Check that error is raised when an improper url is set.
         """
         workload_dict = workload.model_dump()
         workload_dict.pop("result")
         workload_dict["result_link"] = "http://test.test"
         with pytest.raises(WorkloadResultsConnectionError):
             Workload(**workload_dict)
 
-    def tests_workload_result_set(self, workload):
+    def tests_workload_result_set(self, workload: Workload):
         """
         Check that result is set when only result_link is provided.
         """
         workload_dict = workload.model_dump()
         workload_dict.pop("result")
         workload_dict["result_link"] = "http://test.test"
         resp = requests.Response()
```

