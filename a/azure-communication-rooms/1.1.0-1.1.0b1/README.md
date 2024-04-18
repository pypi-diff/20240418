# Comparing `tmp/azure-communication-rooms-1.1.0.tar.gz` & `tmp/azure-communication-rooms-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-communication-rooms-1.1.0.tar", last modified: Wed Apr 17 23:10:52 2024, max compression
+gzip compressed data, was "azure-communication-rooms-1.1.0b1.tar", last modified: Thu Oct 12 21:59:01 2023, max compression
```

## Comparing `azure-communication-rooms-1.1.0.tar` & `azure-communication-rooms-1.1.0b1.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1715 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      202 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10097 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9155 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.176310 azure-communication-rooms-1.1.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.180310 azure-communication-rooms-1.1.0/azure/communication/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.180310 azure-communication-rooms-1.1.0/azure/communication/rooms/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2074 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      390 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_api_versions.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.180310 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      749 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4572 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2425 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      873 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.180310 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      749 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4698 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2435 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.180310 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      747 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43996 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.184310 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      747 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    50249 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.184310 azure-communication-rooms-1.1.0/azure/communication/rooms/_models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      642 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5403 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_models/_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11873 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_rooms_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.184310 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      310 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2596 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/auth_policy_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15664 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4651 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6575 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/user_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6865 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/user_credential_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3356 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1008 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/utils_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      398 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.184310 azure-communication-rooms-1.1.0/azure/communication/rooms/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12127 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/aio/_rooms_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/azure/communication/rooms/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.184310 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10097 2024-04-17 23:10:52.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2474 2024-04-17 23:10:52.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-17 23:10:52.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-17 23:10:51.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       77 2024-04-17 23:10:52.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-17 23:10:52.000000 azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       99 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7803 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/samples/rooms_client_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8163 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/samples/rooms_client_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2613 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-17 23:10:52.188310 azure-communication-rooms-1.1.0/tests/_shared/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      326 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/async_fake_token_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      436 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/communication_service_preparer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      537 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/fake_token_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      920 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/helper.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2615 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/_shared/utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1038 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/acs_rooms_test_case.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3179 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1174 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/test_hmac.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26540 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/test_rooms_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27281 2024-04-17 23:09:01.000000 azure-communication-rooms-1.1.0/tests/test_rooms_client_async.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1420 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      202 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    10191 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9159 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.523051 azure-communication-rooms-1.1.0b1/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.523051 azure-communication-rooms-1.1.0b1/azure/communication/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1378 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      414 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_api_versions.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      748 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3667 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2529 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79436 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      873 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      748 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3779 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2539 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      746 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43759 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      746 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    50039 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      642 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5403 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_models/_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11881 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_rooms_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      310 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2596 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/auth_policy_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15269 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4651 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6575 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/user_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6865 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/user_credential_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3352 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1008 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/utils_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      400 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.527051 azure-communication-rooms-1.1.0b1/azure/communication/rooms/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12127 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/aio/_rooms_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/azure/communication/rooms/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    10191 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2531 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       83 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-10-12 21:59:01.000000 azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       99 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7805 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/samples/rooms_client_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8165 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/samples/rooms_client_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2581 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 21:59:01.531051 azure-communication-rooms-1.1.0b1/tests/_shared/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      326 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/async_fake_token_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1075 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/asynctestcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      436 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/communication_service_preparer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      537 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/fake_token_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3303 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/helper.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4553 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/testcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2615 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/_shared/utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1038 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/acs_rooms_test_case.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3179 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1174 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/test_hmac.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26540 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/test_rooms_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27281 2023-10-12 21:57:45.000000 azure-communication-rooms-1.1.0b1/tests/test_rooms_client_async.py
```

### Comparing `azure-communication-rooms-1.1.0/CHANGELOG.md` & `azure-communication-rooms-1.1.0b1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 # Release History
 
-## 1.1.0 (2024-04-15)
-- General Availability version of PSTN dial-out capability feature.
-
-### Features Added
-- Added support for a new communication identifier `MicrosoftTeamsAppIdentifier`.
-
-### Other Changes
-- The `MicrosoftBotIdentifier` and `MicrosoftBotProperties` have been deprecated.
-
 ## 1.1.0b1 (2023-10-31)
 
 ### Features Added
 
 - Added support for PSTN dial-out capability
 
 ## 1.0.0 (2023-06-12)
@@ -41,8 +32,8 @@
  - Invalid datestrings for `valid_from` and `valid_until` raises exception
 
 ### Other Changes
 Python 3.6 is no longer supported. Please use Python version 3.7 or later. For more details, please read our page on [Azure SDK for Python version support policy](https://github.com/Azure/azure-sdk-for-python/wiki/Azure-SDKs-Python-version-support-policy).
 
 ## 1.0.0b1 (2022-08-10)
 
-- Initial version
+- Initial version
```

### Comparing `azure-communication-rooms-1.1.0/LICENSE` & `azure-communication-rooms-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/PKG-INFO` & `azure-communication-rooms-1.1.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: azure-communication-rooms
-Version: 1.1.0
+Version: 1.1.0b1
 Summary: Microsoft Communication Rooms Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: azure-core<2.0.0,>=1.24.0
+Requires-Dist: msrest>=0.7.1
+Requires-Dist: typing-extensions; python_version < "3.8"
 
 # Azure Communication Rooms client library for Python
 This package contains a Python SDK for Azure Communication Services for Rooms.
 Read more about Azure Communication Services [here](https://docs.microsoft.com/azure/communication-services/overview)
 
 ## _Disclaimer_
 
@@ -68,15 +70,15 @@
 - `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
 valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
 - `pstn_dial_out_enabled`: Set this flag to true if, at the time of the call, dial out to a PSTN number is enabled in a particular room. This flag is optional.
 
 ### Create a room
 To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
 
 ```python
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
 from azure.communication.rooms import (
     RoomsClient,
     RoomParticipant,
@@ -102,15 +104,15 @@
 
     )
 except HttpResponseError as ex:
     print(ex)
 ```
 ### Update a room
 The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
 
 ```python
 try:
     update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4),
```

### Comparing `azure-communication-rooms-1.1.0/README.md` & `azure-communication-rooms-1.1.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
 valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
 - `pstn_dial_out_enabled`: Set this flag to true if, at the time of the call, dial out to a PSTN number is enabled in a particular room. This flag is optional.
 
 ### Create a room
 To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
 
 ```python
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
 from azure.communication.rooms import (
     RoomsClient,
     RoomParticipant,
@@ -79,15 +79,15 @@
 
     )
 except HttpResponseError as ex:
     print(ex)
 ```
 ### Update a room
 The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
 
 ```python
 try:
     update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4),
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/__init__.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import AzureCommunicationRoomsService
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_client.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,79 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any
+from typing import Any, Awaitable
 
-from azure.core import PipelineClient
-from azure.core.pipeline import policies
-from azure.core.rest import HttpRequest, HttpResponse
+from azure.core import AsyncPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 
+from .._serialization import Deserializer, Serializer
 from ._configuration import AzureCommunicationRoomsServiceConfiguration
-from ._serialization import Deserializer, Serializer
 from .operations import ParticipantsOperations, RoomsOperations
 
 
 class AzureCommunicationRoomsService:  # pylint: disable=client-accepts-api-version-keyword
     """Azure Communication Room Service.
 
     :ivar rooms: RoomsOperations operations
-    :vartype rooms: azure.communication.rooms.operations.RoomsOperations
+    :vartype rooms: azure.communication.rooms.aio.operations.RoomsOperations
     :ivar participants: ParticipantsOperations operations
-    :vartype participants: azure.communication.rooms.operations.ParticipantsOperations
+    :vartype participants: azure.communication.rooms.aio.operations.ParticipantsOperations
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-04-15". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-10-30-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
         _endpoint = "{endpoint}"
         self._config = AzureCommunicationRoomsServiceConfiguration(endpoint=endpoint, **kwargs)
-        _policies = kwargs.pop("policies", None)
-        if _policies is None:
-            _policies = [
-                policies.RequestIdPolicy(**kwargs),
-                self._config.headers_policy,
-                self._config.user_agent_policy,
-                self._config.proxy_policy,
-                policies.ContentDecodePolicy(**kwargs),
-                self._config.redirect_policy,
-                self._config.retry_policy,
-                self._config.authentication_policy,
-                self._config.custom_hook_policy,
-                self._config.logging_policy,
-                policies.DistributedTracingPolicy(**kwargs),
-                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
-                self._config.http_logging_policy,
-            ]
-        self._client: PipelineClient = PipelineClient(base_url=_endpoint, policies=_policies, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.rooms = RoomsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.participants = ParticipantsOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = client.send_request(request)
-        <HttpResponse: 200 OK>
+        >>> response = await client.send_request(request)
+        <AsyncHttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
         request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
-        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
+        return self._client.send_request(request_copy, **kwargs)
 
-    def close(self) -> None:
-        self._client.close()
+    async def close(self) -> None:
+        await self._client.close()
 
-    def __enter__(self) -> "AzureCommunicationRoomsService":
-        self._client.__enter__()
+    async def __aenter__(self) -> "AzureCommunicationRoomsService":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details: Any) -> None:
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details: Any) -> None:
+        await self._client.__aexit__(*exc_details)
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_configuration.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
+from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
 VERSION = "unknown"
 
 
-class AzureCommunicationRoomsServiceConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
+class AzureCommunicationRoomsServiceConfiguration(  # pylint: disable=too-many-instance-attributes,name-too-long
+    Configuration
+):
     """Configuration for AzureCommunicationRoomsService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-04-15". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-10-30-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-04-15")
+        super(AzureCommunicationRoomsServiceConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2023-10-30-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "communication-rooms/{}".format(VERSION))
-        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_patch.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_serialization.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError
-from azure.core.serialization import NULL as CoreNull
+from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError as err:
+            except ET.ParseError:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise DeserializationError("XML is invalid") from err
+                raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,14 +166,21 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
+try:
+    basestring  # type: ignore
+    unicode_str = unicode  # type: ignore
+except NameError:
+    basestring = str
+    unicode_str = str
+
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -284,15 +291,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Optional[Dict[str, Any]] = {}
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -329,26 +336,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to server from this model.
+        """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -379,15 +386,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -404,15 +411,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
+        return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -434,15 +441,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
+        return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -534,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, type]] = None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -550,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -638,15 +645,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = str(new_attr)
+                            local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -657,15 +664,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise SerializationError(msg) from err
+            raise_with_traceback(SerializationError, msg, err)
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -699,15 +706,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise SerializationError("Unable to build a model: " + str(err)) from err
+                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -719,14 +726,15 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                # https://github.com/Azure/autorest.python/issues/2063
                 output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
@@ -734,24 +742,24 @@
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str, list
+        :rtype: str
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
+                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -794,15 +802,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is CoreNull:
+            if data is AzureCoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -814,15 +822,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise SerializationError(msg.format(data, data_type)) from err
+            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -983,15 +991,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is str:
+        if obj_type is unicode_str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1160,18 +1168,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise SerializationError(msg) from err
+            raise_with_traceback(SerializationError, msg, err)
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise TypeError(msg) from err
+            raise_with_traceback(TypeError, msg, err)
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1199,14 +1207,15 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
+            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1219,14 +1228,15 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
+            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1359,15 +1369,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, type]] = None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1379,15 +1389,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1432,15 +1442,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, str):
+        if isinstance(response, basestring):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1469,15 +1479,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1503,22 +1513,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, str):
+        if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)  # type: ignore
+            target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1566,15 +1576,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1640,15 +1650,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1688,15 +1698,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, str):
+        if isinstance(attr, basestring):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1745,15 +1755,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, str):
+            elif isinstance(attr, basestring):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1796,14 +1806,15 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
+            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1849,18 +1860,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(str(attr))  # type: ignore
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1880,15 +1891,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1932,15 +1943,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1969,15 +1980,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1985,14 +1996,13 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
-            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise DeserializationError(msg) from err
+            raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/_vendor.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/__init__.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import AzureCommunicationRoomsService
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/_configuration.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
+from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
 VERSION = "unknown"
 
 
-class AzureCommunicationRoomsServiceConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
+class AzureCommunicationRoomsServiceConfiguration(  # pylint: disable=too-many-instance-attributes,name-too-long
+    Configuration
+):
     """Configuration for AzureCommunicationRoomsService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2024-04-15". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-10-30-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2024-04-15")
+        super(AzureCommunicationRoomsServiceConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2023-10-30-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "communication-rooms/{}".format(VERSION))
-        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/_patch.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/__init__.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import RoomsOperations
 from ._operations import ParticipantsOperations
 
 from ._patch import __all__ as _patch_all
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/_operations.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pylint: disable=too-many-lines,too-many-statements
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
@@ -58,15 +58,14 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
     async def create(self, create_room_request: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
         :type create_room_request: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -116,24 +115,21 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @overload
-    async def create(
-        self, create_room_request: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
-    ) -> JSON:
-        # pylint: disable=line-too-long
+    async def create(self, create_room_request: IO, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
-        :type create_room_request: IO[bytes]
+        :type create_room_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -156,23 +152,25 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @distributed_trace_async
-    async def create(self, create_room_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    async def create(self, create_room_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
-        :param create_room_request: The create room request body. Is either a JSON type or a IO[bytes]
-         type. Required.
-        :type create_room_request: JSON or IO[bytes]
+        :param create_room_request: The create room request body. Is either a JSON type or a IO type.
+         Required.
+        :type create_room_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -233,30 +231,30 @@
         _json = None
         _content = None
         if isinstance(create_room_request, (IOBase, bytes)):
             _content = create_room_request
         else:
             _json = create_room_request
 
-        _request = build_rooms_create_request(
+        request = build_rooms_create_request(
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
@@ -265,21 +263,20 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable[JSON]:
-        # pylint: disable=line-too-long
         """Retrieves all created rooms.
 
         Retrieves all created rooms.
 
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -317,61 +314,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                _request = build_rooms_list_request(
+                request = build_rooms_list_request(
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                _request = HttpRequest(
+                request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
-            return _request
+            return request
 
         async def extract_data(pipeline_response):
             deserialized = pipeline_response.http_response.json()
             list_of_elem = deserialized["value"]
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.get("nextLink") or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            _request = prepare_request(next_link)
+            request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 if _stream:
                     await response.read()  # Load the body in memory and close the socket
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
@@ -379,15 +376,14 @@
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace_async
     async def get(self, room_id: str, **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
         """Retrieves an existing room by id.
 
         Retrieves an existing room by id.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :return: JSON object
@@ -424,28 +420,28 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_rooms_get_request(
+        request = build_rooms_get_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
@@ -454,28 +450,27 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @overload
     async def update(
         self,
         room_id: str,
         update_room_request: JSON,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :param update_room_request: The update room request. Required.
@@ -522,28 +517,27 @@
                 }
         """
 
     @overload
     async def update(
         self,
         room_id: str,
-        update_room_request: IO[bytes],
+        update_room_request: IO,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :param update_room_request: The update room request. Required.
-        :type update_room_request: IO[bytes]
+        :type update_room_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -566,25 +560,27 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @distributed_trace_async
-    async def update(self, room_id: str, update_room_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    async def update(self, room_id: str, update_room_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :param update_room_request: The update room request. Is either a JSON type or a IO[bytes] type.
+        :param update_room_request: The update room request. Is either a JSON type or a IO type.
          Required.
-        :type update_room_request: JSON or IO[bytes]
+        :type update_room_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
+         'application/merge-patch+json'. Default value is None.
+        :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -637,31 +633,31 @@
         _json = None
         _content = None
         if isinstance(update_room_request, (IOBase, bytes)):
             _content = update_room_request
         else:
             _json = update_room_request
 
-        _request = build_rooms_update_request(
+        request = build_rooms_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
@@ -670,17 +666,17 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @distributed_trace_async
     async def delete(self, room_id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
         """Delete a room.
 
         Delete a room.
 
@@ -699,40 +695,40 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        _request = build_rooms_delete_request(
+        request = build_rooms_delete_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
-            return cls(pipeline_response, None, {})  # type: ignore
+            return cls(pipeline_response, None, {})
 
 
 class ParticipantsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
@@ -746,15 +742,14 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, room_id: str, **kwargs: Any) -> AsyncIterable[JSON]:
-        # pylint: disable=line-too-long
         """Get participants in a room.
 
         Get participants in a room.
 
         :param room_id: The id of the room to get participants from. Required.
         :type room_id: str
         :return: An iterator like instance of JSON object
@@ -787,62 +782,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                _request = build_participants_list_request(
+                request = build_participants_list_request(
                     room_id=room_id,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                _request = HttpRequest(
+                request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
-            return _request
+            return request
 
         async def extract_data(pipeline_response):
             deserialized = pipeline_response.http_response.json()
             list_of_elem = deserialized["value"]
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.get("nextLink") or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            _request = prepare_request(next_link)
+            request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 if _stream:
                     await response.read()  # Load the body in memory and close the socket
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
@@ -857,15 +852,14 @@
         self,
         room_id: str,
         update_participants_request: JSON,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Required.
@@ -892,47 +886,49 @@
                 }
         """
 
     @overload
     async def update(
         self,
         room_id: str,
-        update_participants_request: IO[bytes],
+        update_participants_request: IO,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Required.
-        :type update_participants_request: IO[bytes]
+        :type update_participants_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def update(self, room_id: str, update_participants_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    async def update(self, room_id: str, update_participants_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Is either a
-         JSON type or a IO[bytes] type. Required.
-        :type update_participants_request: JSON or IO[bytes]
+         JSON type or a IO type. Required.
+        :type update_participants_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
+         'application/merge-patch+json'. Default value is None.
+        :paramtype content_type: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -965,31 +961,31 @@
         _json = None
         _content = None
         if isinstance(update_participants_request, (IOBase, bytes)):
             _content = update_participants_request
         else:
             _json = update_participants_request
 
-        _request = build_participants_update_request(
+        request = build_participants_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
@@ -998,10 +994,10 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/aio/operations/_patch.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/__init__.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import RoomsOperations
 from ._operations import ParticipantsOperations
 
 from ._patch import __all__ as _patch_all
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/_operations.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pylint: disable=too-many-lines,too-many-statements
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.13.7)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.6)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import datetime
 from io import IOBase
 import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
@@ -40,42 +40,40 @@
 
 
 def build_rooms_create_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if "Repeatability-Request-ID" not in _headers:
         _headers["Repeatability-Request-ID"] = str(uuid.uuid4())
     if "Repeatability-First-Sent" not in _headers:
-        _headers["Repeatability-First-Sent"] = _SERIALIZER.serialize_data(
-            datetime.datetime.now(datetime.timezone.utc), "rfc-1123"
-        )
+        _headers["Repeatability-First-Sent"] = _SERIALIZER.serialize_data(datetime.datetime.now(), "rfc-1123")
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_rooms_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -86,15 +84,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_rooms_get_request(room_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms/{roomId}"
     path_format_arguments = {
         "roomId": _SERIALIZER.url("room_id", room_id, "str"),
     }
@@ -111,15 +109,15 @@
 
 
 def build_rooms_update_request(room_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms/{roomId}"
     path_format_arguments = {
         "roomId": _SERIALIZER.url("room_id", room_id, "str"),
     }
@@ -137,15 +135,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_rooms_delete_request(room_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms/{roomId}"
     path_format_arguments = {
         "roomId": _SERIALIZER.url("room_id", room_id, "str"),
     }
@@ -161,15 +159,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_participants_list_request(room_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms/{roomId}/participants"
     path_format_arguments = {
         "roomId": _SERIALIZER.url("room_id", room_id, "str"),
     }
@@ -186,15 +184,15 @@
 
 
 def build_participants_update_request(room_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-15"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-30-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/rooms/{roomId}/participants"
     path_format_arguments = {
         "roomId": _SERIALIZER.url("room_id", room_id, "str"),
     }
@@ -227,15 +225,14 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
     def create(self, create_room_request: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
         :type create_room_request: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -285,22 +282,21 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @overload
-    def create(self, create_room_request: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    def create(self, create_room_request: IO, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
-        :type create_room_request: IO[bytes]
+        :type create_room_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -323,23 +319,25 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @distributed_trace
-    def create(self, create_room_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    def create(self, create_room_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
-        :param create_room_request: The create room request body. Is either a JSON type or a IO[bytes]
-         type. Required.
-        :type create_room_request: JSON or IO[bytes]
+        :param create_room_request: The create room request body. Is either a JSON type or a IO type.
+         Required.
+        :type create_room_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -400,30 +398,30 @@
         _json = None
         _content = None
         if isinstance(create_room_request, (IOBase, bytes)):
             _content = create_room_request
         else:
             _json = create_room_request
 
-        _request = build_rooms_create_request(
+        request = build_rooms_create_request(
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
@@ -432,21 +430,20 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable[JSON]:
-        # pylint: disable=line-too-long
         """Retrieves all created rooms.
 
         Retrieves all created rooms.
 
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.paging.ItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -484,61 +481,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                _request = build_rooms_list_request(
+                request = build_rooms_list_request(
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                _request = HttpRequest(
+                request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
-            return _request
+            return request
 
         def extract_data(pipeline_response):
             deserialized = pipeline_response.http_response.json()
             list_of_elem = deserialized["value"]
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.get("nextLink") or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            _request = prepare_request(next_link)
+            request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 if _stream:
                     response.read()  # Load the body in memory and close the socket
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
@@ -546,15 +543,14 @@
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @distributed_trace
     def get(self, room_id: str, **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
         """Retrieves an existing room by id.
 
         Retrieves an existing room by id.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :return: JSON object
@@ -591,28 +587,28 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_rooms_get_request(
+        request = build_rooms_get_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
@@ -621,28 +617,27 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @overload
     def update(
         self,
         room_id: str,
         update_room_request: JSON,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :param update_room_request: The update room request. Required.
@@ -689,28 +684,27 @@
                 }
         """
 
     @overload
     def update(
         self,
         room_id: str,
-        update_room_request: IO[bytes],
+        update_room_request: IO,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
         :param update_room_request: The update room request. Required.
-        :type update_room_request: IO[bytes]
+        :type update_room_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -733,25 +727,27 @@
                     "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
                       no longer be joined. The timestamp is in RFC3339 format:
                       ``yyyy-MM-ddTHH:mm:ssZ``. Required.
                 }
         """
 
     @distributed_trace
-    def update(self, room_id: str, update_room_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    def update(self, room_id: str, update_room_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :param update_room_request: The update room request. Is either a JSON type or a IO[bytes] type.
+        :param update_room_request: The update room request. Is either a JSON type or a IO type.
          Required.
-        :type update_room_request: JSON or IO[bytes]
+        :type update_room_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
+         'application/merge-patch+json'. Default value is None.
+        :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -804,31 +800,31 @@
         _json = None
         _content = None
         if isinstance(update_room_request, (IOBase, bytes)):
             _content = update_room_request
         else:
             _json = update_room_request
 
-        _request = build_rooms_update_request(
+        request = build_rooms_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
@@ -837,17 +833,17 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
 
     @distributed_trace
     def delete(self, room_id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
         """Delete a room.
 
         Delete a room.
 
@@ -866,40 +862,40 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        _request = build_rooms_delete_request(
+        request = build_rooms_delete_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
-            return cls(pipeline_response, None, {})  # type: ignore
+            return cls(pipeline_response, None, {})
 
 
 class ParticipantsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
@@ -913,15 +909,14 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, room_id: str, **kwargs: Any) -> Iterable[JSON]:
-        # pylint: disable=line-too-long
         """Get participants in a room.
 
         Get participants in a room.
 
         :param room_id: The id of the room to get participants from. Required.
         :type room_id: str
         :return: An iterator like instance of JSON object
@@ -954,62 +949,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                _request = build_participants_list_request(
+                request = build_participants_list_request(
                     room_id=room_id,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                _request = HttpRequest(
+                request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
                     ),
                 }
-                _request.url = self._client.format_url(_request.url, **path_format_arguments)
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
-            return _request
+            return request
 
         def extract_data(pipeline_response):
             deserialized = pipeline_response.http_response.json()
             list_of_elem = deserialized["value"]
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.get("nextLink") or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            _request = prepare_request(next_link)
+            request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 if _stream:
                     response.read()  # Load the body in memory and close the socket
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
@@ -1024,15 +1019,14 @@
         self,
         room_id: str,
         update_participants_request: JSON,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
-        # pylint: disable=line-too-long
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Required.
@@ -1059,47 +1053,49 @@
                 }
         """
 
     @overload
     def update(
         self,
         room_id: str,
-        update_participants_request: IO[bytes],
+        update_participants_request: IO,
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Required.
-        :type update_participants_request: IO[bytes]
+        :type update_participants_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def update(self, room_id: str, update_participants_request: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
+    def update(self, room_id: str, update_participants_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
         :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
         :param update_participants_request: An updated set of participants of the room. Is either a
-         JSON type or a IO[bytes] type. Required.
-        :type update_participants_request: JSON or IO[bytes]
+         JSON type or a IO type. Required.
+        :type update_participants_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
+         'application/merge-patch+json'. Default value is None.
+        :paramtype content_type: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -1132,31 +1128,31 @@
         _json = None
         _content = None
         if isinstance(update_participants_request, (IOBase, bytes)):
             _content = update_participants_request
         else:
             _json = update_participants_request
 
-        _request = build_participants_update_request(
+        request = build_participants_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        _request.url = self._client.format_url(_request.url, **path_format_arguments)
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
@@ -1165,10 +1161,10 @@
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(JSON, deserialized)
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_generated/operations/_patch.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_models/__init__.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_models/_models.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_rooms_client.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_rooms_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     This client provides operations to manage rooms.
 
     :param str endpoint:
         The endpoint url for Azure Communication Service resource.
     param Union[TokenCredential, AzureKeyCredential] credential:
         The access key we use to authenticate against the service.
     :keyword api_version: Azure Communication Rooms API version.
-        Default value is "2024-04-15".
+        Default value is "2023-10-30-preview".
         Note that overriding this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
     def __init__(
             self,
             endpoint: str,
             credential: Union[TokenCredential, AzureKeyCredential],
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/auth_policy_utils.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/auth_policy_utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/models.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,335 +1,313 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 from enum import Enum
-import warnings
-from typing import Mapping, Optional, Union, Any, cast
-from typing_extensions import Literal, TypedDict, Protocol, runtime_checkable
+from typing import Mapping, Optional, Union, Any
 
+from typing_extensions import TypedDict, Protocol
 from azure.core import CaseInsensitiveEnumMeta
 
 
-class DeprecatedEnumMeta(CaseInsensitiveEnumMeta):
-
-    def __getattribute__(cls, item):
-        if item.upper() == "MICROSOFT_BOT":
-            warnings.warn("MICROSOFT_BOT is deprecated and has been replaced by \
-                          MICROSOFT_TEAMS_APP identifier.", DeprecationWarning)
-            item = "MICROSOFT_TEAMS_APP"
-        return super().__getattribute__(item)
-
-
-class CommunicationIdentifierKind(str, Enum, metaclass=DeprecatedEnumMeta):
+class CommunicationIdentifierKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Communication Identifier Kind.
 
     For checking yet unknown identifiers it is better to rely on the presence of the `raw_id` property,
     as new or existing distinct type identifiers always contain the `raw_id` property.
     It is not advisable to rely on the `kind` property with a value `unknown`,
     as it could become a new or existing distinct type in the future.
     """
 
     UNKNOWN = "unknown"
     COMMUNICATION_USER = "communication_user"
     PHONE_NUMBER = "phone_number"
     MICROSOFT_TEAMS_USER = "microsoft_teams_user"
-    MICROSOFT_TEAMS_APP = "microsoft_teams_app"
+    MICROSOFT_BOT = "microsoft_bot"
 
 
 class CommunicationCloudEnvironment(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The cloud environment that the identifier belongs to"""
 
     PUBLIC = "PUBLIC"
     DOD = "DOD"
     GCCH = "GCCH"
 
 
-@runtime_checkable
 class CommunicationIdentifier(Protocol):
-    """Communication Identifier."""
-    @property
-    def raw_id(self) -> str:
-        """The raw ID of the identifier."""
-        ...
-    @property
-    def kind(self) -> CommunicationIdentifierKind:
-        """The type of identifier."""
-        ...
-    @property
-    def properties(self) -> Mapping[str, Any]:
-        """The properties of the identifier."""
-        ...
+    """Communication Identifier.
+
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar Mapping[str, Any] properties: The properties of the identifier.
+    """
 
+    raw_id = None  # type: Optional[str]
+    kind = None  # type: Optional[Union[CommunicationIdentifierKind, str]]
+    properties = {}  # type: Mapping[str, Any]
+
+
+CommunicationUserProperties = TypedDict("CommunicationUserProperties", {"id": str})
 
 PHONE_NUMBER_PREFIX = "4:"
 BOT_PREFIX = "28:"
 BOT_PUBLIC_CLOUD_PREFIX = "28:orgid:"
 BOT_DOD_CLOUD_PREFIX = "28:dod:"
 BOT_DOD_CLOUD_GLOBAL_PREFIX = "28:dod-global:"
 BOT_GCCH_CLOUD_PREFIX = "28:gcch:"
 BOT_GCCH_CLOUD_GLOBAL_PREFIX = "28:gcch-global:"
-TEAMS_APP_PUBLIC_CLOUD_PREFIX = "28:orgid:"
-TEAMS_APP_DOD_CLOUD_PREFIX = "28:dod:"
-TEAMS_APP_GCCH_CLOUD_PREFIX = "28:gcch:"
 TEAMS_USER_ANONYMOUS_PREFIX = "8:teamsvisitor:"
 TEAMS_USER_PUBLIC_CLOUD_PREFIX = "8:orgid:"
 TEAMS_USER_DOD_CLOUD_PREFIX = "8:dod:"
 TEAMS_USER_GCCH_CLOUD_PREFIX = "8:gcch:"
 ACS_USER_PREFIX = "8:acs:"
 ACS_USER_DOD_CLOUD_PREFIX = "8:dod-acs:"
 ACS_USER_GCCH_CLOUD_PREFIX = "8:gcch-acs:"
 SPOOL_USER_PREFIX = "8:spool:"
 
 
-class CommunicationUserProperties(TypedDict):
-    """Dictionary of properties for a CommunicationUserIdentifier."""
-    id: str
-    """ID of the Communication user as returned from Azure Communication Identity."""
+class CommunicationUserIdentifier:
+    """Represents a user in Azure Communication Service.
 
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar Mapping[str, Any] properties: The properties of the identifier.
+     The keys in this mapping include:
+        - `id`(str): ID of the Communication user as returned from Azure Communication Identity.
 
-class CommunicationUserIdentifier:
-    """Represents a user in Azure Communication Service."""
-    kind: Literal[CommunicationIdentifierKind.COMMUNICATION_USER] = CommunicationIdentifierKind.COMMUNICATION_USER
-    """The type of identifier."""
-    properties: CommunicationUserProperties
-    """The properties of the identifier."""
-    raw_id: str
-    """The raw ID of the identifier."""
+    :param str id: ID of the Communication user as returned from Azure Communication Identity.
+    """
+
+    kind = CommunicationIdentifierKind.COMMUNICATION_USER
 
     def __init__(self, id: str, **kwargs: Any) -> None:
-        """
-        :param str id: ID of the Communication user as returned from Azure Communication Identity.
-        :keyword str raw_id: The raw ID of the identifier. If not specified, the 'id' value will be used.
-        """
+        self.raw_id = kwargs.get("raw_id", id)
         self.properties = CommunicationUserProperties(id=id)
-        raw_id: Optional[str] = kwargs.get("raw_id")
-        self.raw_id = raw_id if raw_id is not None else id
+        if self.raw_id is None:
+            self.raw_id = _communication_user_raw_id(self)
 
     def __eq__(self, other):
         try:
-            if other.raw_id:
-                return self.raw_id == other.raw_id
             return self.raw_id == other.properties["id"]
         except Exception:  # pylint: disable=broad-except
             return False
 
 
-class PhoneNumberProperties(TypedDict):
-    """Dictionary of properties for a PhoneNumberIdentifier."""
-    value: str
-    """The phone number in E.164 format."""
+def _communication_user_raw_id(identifier: CommunicationUserIdentifier) -> str:
+    if identifier.raw_id:
+        return str(identifier.raw_id)
+    return str(identifier.properties["id"])
+
+
+PhoneNumberProperties = TypedDict("PhoneNumberProperties", {"value": str})
 
 
 class PhoneNumberIdentifier:
-    """Represents a phone number."""
-    kind: Literal[CommunicationIdentifierKind.PHONE_NUMBER] = CommunicationIdentifierKind.PHONE_NUMBER
-    """The type of identifier."""
-    properties: PhoneNumberProperties
-    """The properties of the identifier."""
-    raw_id: str
-    """The raw ID of the identifier."""
+    """Represents a phone number.
+
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar Mapping properties: The properties of the identifier.
+     The keys in this mapping include:
+        - `value`(str): The phone number in E.164 format.
+
+    :param str value: The phone number.
+    """
+
+    kind = CommunicationIdentifierKind.PHONE_NUMBER
 
     def __init__(self, value: str, **kwargs: Any) -> None:
-        """
-        :param str value: The phone number.
-        :keyword str raw_id: The raw ID of the identifier. If not specified, this will be constructed from
-          the 'value' parameter.
-        """
+        self.raw_id = kwargs.get("raw_id")
         self.properties = PhoneNumberProperties(value=value)
-        raw_id: Optional[str] = kwargs.get("raw_id")
-        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
+        if self.raw_id is None:
+            self.raw_id = _phone_number_raw_id(self)
 
     def __eq__(self, other):
         try:
-            if other.raw_id:
-                return self.raw_id == other.raw_id
-            return self.raw_id == self._format_raw_id(other.properties)
-        except Exception:  # pylint:disable=broad-except
+            return self.raw_id == _phone_number_raw_id(other)
+        except Exception:  # pylint: disable=broad-except
             return False
 
-    def _format_raw_id(self, properties: PhoneNumberProperties) -> str:
-        # We just assume correct E.164 format here because
-        # validation should only happen server-side, not client-side.
-        value = properties["value"]
-        return f"{PHONE_NUMBER_PREFIX}{value}"
+
+def _phone_number_raw_id(identifier: PhoneNumberIdentifier) -> str:
+    if identifier.raw_id:
+        return str(identifier.raw_id)
+    value = identifier.properties["value"]
+    # We just assume correct E.164 format here because
+    # validation should only happen server-side, not client-side.
+    return f"{PHONE_NUMBER_PREFIX}{value}"
 
 
 class UnknownIdentifier:
     """Represents an identifier of an unknown type.
 
     It will be encountered in communications with endpoints that are not
     identifiable by this version of the SDK.
 
     For checking yet unknown identifiers it is better to rely on the presence of the `raw_id` property,
     as new or existing distinct type identifiers always contain the `raw_id` property.
     It is not advisable to rely on the `kind` property with a value `unknown`,
     as it could become a new or existing distinct type in the future.
+
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar Mapping properties: The properties of the identifier.
+    :param str identifier: The ID of the identifier.
     """
-    kind: Literal[CommunicationIdentifierKind.UNKNOWN] = CommunicationIdentifierKind.UNKNOWN
-    """The type of identifier."""
-    properties: Mapping[str, Any]
-    """The properties of the identifier."""
-    raw_id: str
-    """The raw ID of the identifier."""
+
+    kind = CommunicationIdentifierKind.UNKNOWN
 
     def __init__(self, identifier: str) -> None:
-        """
-        :param str identifier: The ID of the identifier.
-        """
         self.raw_id = identifier
-        self.properties = {}
+        self.properties = {}  # type: Any
 
     def __eq__(self, other):
         try:
             return self.raw_id == other.raw_id
-        except AttributeError:
+        except Exception:  # pylint: disable=broad-except
             return False
 
 
-class MicrosoftTeamsUserProperties(TypedDict):
-    """Dictionary of properties for a MicrosoftTeamsUserIdentifier."""
-    user_id: str
-    """The id of the Microsoft Teams user. If the user isn't anonymous, the id is the AAD object id of the user."""
-    is_anonymous: bool
-    """Set this to true if the user is anonymous for example when joining a meeting with a share link."""
-    cloud: Union[CommunicationCloudEnvironment, str]
-    """Cloud environment that this identifier belongs to."""
+MicrosoftTeamsUserProperties = TypedDict(
+    "MicrosoftTeamsUserProperties",
+    {
+        "user_id": str,
+        "is_anonymous": bool,
+        "cloud": Union[CommunicationCloudEnvironment, str],
+    },
+)
 
 
 class MicrosoftTeamsUserIdentifier:
-    """Represents an identifier for a Microsoft Teams user."""
-    kind: Literal[CommunicationIdentifierKind.MICROSOFT_TEAMS_USER] = CommunicationIdentifierKind.MICROSOFT_TEAMS_USER
-    """The type of identifier."""
-    properties: MicrosoftTeamsUserProperties
-    """The properties of the identifier."""
-    raw_id: str
-    """The raw ID of the identifier."""
+    """Represents an identifier for a Microsoft Teams user.
+
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar Mapping properties: The properties of the identifier.
+     The keys in this mapping include:
+        - `user_id`(str): The id of the Microsoft Teams user. If the user isn't anonymous,
+          the id is the AAD object id of the user.
+        - `is_anonymous` (bool): Set this to true if the user is anonymous for example when joining
+          a meeting with a share link.
+        - `cloud` (str): Cloud environment that this identifier belongs to.
+
+    :param str user_id: Microsoft Teams user id.
+    :keyword bool is_anonymous: `True` if the identifier is anonymous. Default value is `False`.
+    :keyword cloud: Cloud environment that the user belongs to. Default value is `PUBLIC`.
+    :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
+    """
+
+    kind = CommunicationIdentifierKind.MICROSOFT_TEAMS_USER
 
     def __init__(self, user_id: str, **kwargs: Any) -> None:
-        """
-        :param str user_id: Microsoft Teams user id.
-        :keyword bool is_anonymous: `True` if the identifier is anonymous. Default value is `False`.
-        :keyword cloud: Cloud environment that the user belongs to. Default value is `PUBLIC`.
-        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
-        :keyword str raw_id: The raw ID of the identifier. If not specified, this value will be constructed from
-         the other properties.
-        """
+        self.raw_id = kwargs.get("raw_id")
         self.properties = MicrosoftTeamsUserProperties(
             user_id=user_id,
             is_anonymous=kwargs.get("is_anonymous", False),
             cloud=kwargs.get("cloud") or CommunicationCloudEnvironment.PUBLIC,
         )
-        raw_id: Optional[str] = kwargs.get("raw_id")
-        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
+        if self.raw_id is None:
+            self.raw_id = _microsoft_teams_user_raw_id(self)
 
     def __eq__(self, other):
         try:
-            if other.raw_id:
-                return self.raw_id == other.raw_id
-            return self.raw_id == self._format_raw_id(other.properties)
+            return self.raw_id == _microsoft_teams_user_raw_id(other)
         except Exception:  # pylint: disable=broad-except
             return False
 
-    def _format_raw_id(self, properties: MicrosoftTeamsUserProperties) -> str:
-        user_id = properties["user_id"]
-        if properties["is_anonymous"]:
-            return f"{TEAMS_USER_ANONYMOUS_PREFIX}{user_id}"
-        cloud = properties["cloud"]
-        if cloud == CommunicationCloudEnvironment.DOD:
-            return f"{TEAMS_USER_DOD_CLOUD_PREFIX}{user_id}"
-        if cloud == CommunicationCloudEnvironment.GCCH:
-            return f"{TEAMS_USER_GCCH_CLOUD_PREFIX}{user_id}"
-        if cloud == CommunicationCloudEnvironment.PUBLIC:
-            return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
+
+def _microsoft_teams_user_raw_id(identifier: MicrosoftTeamsUserIdentifier) -> str:
+    if identifier.raw_id:
+        return str(identifier.raw_id)
+    user_id = identifier.properties["user_id"]
+    if identifier.properties["is_anonymous"]:
+        return f"{TEAMS_USER_ANONYMOUS_PREFIX}{user_id}"
+    cloud = identifier.properties["cloud"]
+    if cloud == CommunicationCloudEnvironment.DOD:
+        return f"{TEAMS_USER_DOD_CLOUD_PREFIX}{user_id}"
+    if cloud == CommunicationCloudEnvironment.GCCH:
+        return f"{TEAMS_USER_GCCH_CLOUD_PREFIX}{user_id}"
+    if cloud == CommunicationCloudEnvironment.PUBLIC:
         return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
+    return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
 
 
-class MicrosoftTeamsAppProperties(TypedDict):
-    """Dictionary of properties for a MicrosoftTeamsAppIdentifier."""
-    app_id: str
-    """The id of the Microsoft Teams application."""
-    cloud: Union[CommunicationCloudEnvironment, str]
-    """Cloud environment that this identifier belongs to."""
+MicrosoftBotProperties = TypedDict(
+    "MicrosoftBotProperties",
+    {
+        "bot_id": str,
+        "is_resource_account_configured": bool,
+        "cloud": Union[CommunicationCloudEnvironment, str],
+    },
+)
 
 
-class _botbackcompatdict(dict):
-    """Backwards compatible properties."""
-    def __getitem__(self, __key: Any) -> Any:
-        try:
-            return super().__getitem__(__key)
-        except KeyError:
-            if __key == "bot_id":
-                return super().__getitem__("app_id")
-            if __key == "is_resource_account_configured":
-                return True
-            raise
-
-
-class MicrosoftTeamsAppIdentifier:
-    """Represents an identifier for a Microsoft Teams application."""
-    kind: Literal[CommunicationIdentifierKind.MICROSOFT_TEAMS_APP] = CommunicationIdentifierKind.MICROSOFT_TEAMS_APP
-    """The type of identifier."""
-    properties: MicrosoftTeamsAppProperties
-    """The properties of the identifier."""
-    raw_id: str
-    """The raw ID of the identifier."""
-
-    def __init__(self, app_id: str, **kwargs: Any) -> None:
-        """
-        :param str app_id: Microsoft Teams application id.
-        :keyword cloud: Cloud environment that the application belongs to. Default value is `PUBLIC`.
-        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
-        :keyword str raw_id: The raw ID of the identifier. If not specified, this value will be constructed
-         from the other properties.
-        """
-        self.properties = cast(MicrosoftTeamsAppProperties, _botbackcompatdict(
-            app_id=app_id,
+class MicrosoftBotIdentifier:
+    """Represents an identifier for a Microsoft bot.
+
+    :ivar str raw_id: Optional raw ID of the identifier.
+    :ivar kind: The type of identifier.
+    :vartype kind: str or CommunicationIdentifierKind
+    :ivar MicrosoftBotProperties: The properties of the identifier.
+     The keys in this mapping include:
+        - `bot_id`(str): The id of the Microsoft bot.
+        - `is_resource_account_configured` (bool): Set this to false if the bot is global.
+        The default is `true` for tennantized bots.
+        - `cloud` (str): Cloud environment that this identifier belongs to.
+
+    :param str bot_id: Microsoft bot id.
+    :keyword bool is_resource_account_configured: `False` if the identifier is global.
+    Default value is `True` for tennantzed bots.
+    :keyword cloud: Cloud environment that the bot belongs to. Default value is `PUBLIC`.
+    :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
+    """
+
+    kind = CommunicationIdentifierKind.MICROSOFT_BOT
+
+    def __init__(self, bot_id: str, **kwargs: Any) -> None:
+        self.raw_id = kwargs.get("raw_id")
+        self.properties = MicrosoftBotProperties(
+            bot_id=bot_id,
+            is_resource_account_configured=kwargs.get(
+                "is_resource_account_configured", True
+            ),
             cloud=kwargs.get("cloud") or CommunicationCloudEnvironment.PUBLIC,
-        ))
-        raw_id: Optional[str] = kwargs.get("raw_id")
-        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
+        )
+        if self.raw_id is None:
+            self.raw_id = _microsoft_bot_raw_id(self)
 
     def __eq__(self, other):
         try:
-            if other.raw_id:
-                return self.raw_id == other.raw_id
-            return self.raw_id == self._format_raw_id(other.properties)
+            return self.raw_id == _microsoft_bot_raw_id(other)
         except Exception:  # pylint: disable=broad-except
             return False
 
-    def _format_raw_id(self, properties: MicrosoftTeamsAppProperties) -> str:
-        app_id = properties["app_id"]
-        cloud = properties["cloud"]
+
+def _microsoft_bot_raw_id(identifier: MicrosoftBotIdentifier) -> str:  # pylint: disable=too-many-return-statements
+    if identifier.raw_id:
+        return str(identifier.raw_id)
+    bot_id = identifier.properties["bot_id"]
+    cloud = identifier.properties["cloud"]
+    if identifier.properties["is_resource_account_configured"] is False:
         if cloud == CommunicationCloudEnvironment.DOD:
-            return f"{TEAMS_APP_DOD_CLOUD_PREFIX}{app_id}"
+            return f"{BOT_DOD_CLOUD_GLOBAL_PREFIX}{bot_id}"
         if cloud == CommunicationCloudEnvironment.GCCH:
-            return f"{TEAMS_APP_GCCH_CLOUD_PREFIX}{app_id}"
-        return f"{TEAMS_APP_PUBLIC_CLOUD_PREFIX}{app_id}"
+            return f"{BOT_GCCH_CLOUD_GLOBAL_PREFIX}{bot_id}"
+        return f"{BOT_PREFIX}{bot_id}"
 
-
-class _MicrosoftBotIdentifier(MicrosoftTeamsAppIdentifier):
-    """Represents an identifier for a Microsoft bot.
-
-    DEPRECATED. Only used in cases of backwards compatibility.
-    """
-
-    def __init__(self, bot_id, **kwargs):
-        """
-        :param str bot_id: Microsoft bot id.
-        :keyword bool is_resource_account_configured: `False` if the identifier is global.
-         Default value is `True` for tennantzed bots.
-        :keyword cloud: Cloud environment that the bot belongs to. Default value is `PUBLIC`.
-        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
-        """
-        warnings.warn(
-            "The MicrosoftBotIdentifier is deprecated and has been replaced by MicrosoftTeamsAppIdentifier.",
-            DeprecationWarning
-        )
-        super().__init__(bot_id, **kwargs)
+    if cloud == CommunicationCloudEnvironment.DOD:
+        return f"{BOT_DOD_CLOUD_PREFIX}{bot_id}"
+    if cloud == CommunicationCloudEnvironment.GCCH:
+        return f"{BOT_GCCH_CLOUD_PREFIX}{bot_id}"
+    return f"{BOT_PUBLIC_CLOUD_PREFIX}{bot_id}"
 
 
 def identifier_from_raw_id(raw_id: str) -> CommunicationIdentifier:  # pylint: disable=too-many-return-statements
     """
     Creates a CommunicationIdentifier from a given raw ID.
 
     When storing raw IDs use this function to restore the identifier that was encoded in the raw ID.
@@ -337,66 +315,90 @@
     :param str raw_id: A raw ID to construct the CommunicationIdentifier from.
     :return: The CommunicationIdentifier parsed from the raw_id.
     :rtype: CommunicationIdentifier
     """
     if raw_id.startswith(PHONE_NUMBER_PREFIX):
         return PhoneNumberIdentifier(
             value=raw_id[len(PHONE_NUMBER_PREFIX) :], raw_id=raw_id
-        )
+        )  # type: ignore
 
     segments = raw_id.split(":", maxsplit=2)
-    if len(segments) < 3:
-        return UnknownIdentifier(identifier=raw_id)
+    if len(segments) != 3:
+        if len(segments) == 2 and raw_id.startswith(BOT_PREFIX):
+            return MicrosoftBotIdentifier(
+                bot_id=segments[1],
+                is_resource_account_configured=False,
+                cloud=CommunicationCloudEnvironment.PUBLIC,
+                raw_id=raw_id,
+            )  # type: ignore
+        return UnknownIdentifier(identifier=raw_id)  # type: ignore
 
     prefix = f"{segments[0]}:{segments[1]}:"
     suffix = segments[2]
     if prefix == TEAMS_USER_ANONYMOUS_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix, is_anonymous=True, raw_id=raw_id
-        )
+        )  # type: ignore
     if prefix == TEAMS_USER_PUBLIC_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.PUBLIC,
             raw_id=raw_id,
-        )
+        )  # type: ignore
     if prefix == TEAMS_USER_DOD_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.DOD,
             raw_id=raw_id,
-        )
+        )  # type: ignore
     if prefix == TEAMS_USER_GCCH_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.GCCH,
             raw_id=raw_id,
-        )
-    if prefix == TEAMS_APP_PUBLIC_CLOUD_PREFIX:
-        return MicrosoftTeamsAppIdentifier(
-            app_id=suffix,
-            cloud=CommunicationCloudEnvironment.PUBLIC,
-            raw_id=raw_id,
-        )
-    if prefix == TEAMS_APP_DOD_CLOUD_PREFIX:
-        return MicrosoftTeamsAppIdentifier(
-            app_id=suffix,
-            cloud=CommunicationCloudEnvironment.DOD,
-            raw_id=raw_id,
-        )
-    if prefix == TEAMS_APP_GCCH_CLOUD_PREFIX:
-        return MicrosoftTeamsAppIdentifier(
-            app_id=suffix,
-            cloud=CommunicationCloudEnvironment.GCCH,
-            raw_id=raw_id,
-        )
+        )  # type: ignore
     if prefix in [
         ACS_USER_PREFIX,
         ACS_USER_DOD_CLOUD_PREFIX,
         ACS_USER_GCCH_CLOUD_PREFIX,
         SPOOL_USER_PREFIX,
     ]:
-        return CommunicationUserIdentifier(id=raw_id, raw_id=raw_id)
-    return UnknownIdentifier(identifier=raw_id)
+        return CommunicationUserIdentifier(id=raw_id, raw_id=raw_id)  # type: ignore
+    if prefix == BOT_GCCH_CLOUD_GLOBAL_PREFIX:
+        return MicrosoftBotIdentifier(
+            bot_id=suffix,
+            is_resource_account_configured=False,
+            cloud=CommunicationCloudEnvironment.GCCH,
+            raw_id=raw_id,
+        )  # type: ignore
+    if prefix == BOT_PUBLIC_CLOUD_PREFIX:
+        return MicrosoftBotIdentifier(
+            bot_id=suffix,
+            is_resource_account_configured=True,
+            cloud=CommunicationCloudEnvironment.PUBLIC,
+            raw_id=raw_id,
+        )  # type: ignore
+    if prefix == BOT_DOD_CLOUD_GLOBAL_PREFIX:
+        return MicrosoftBotIdentifier(
+            bot_id=suffix,
+            is_resource_account_configured=False,
+            cloud=CommunicationCloudEnvironment.DOD,
+            raw_id=raw_id,
+        )  # type: ignore
+    if prefix == BOT_GCCH_CLOUD_PREFIX:
+        return MicrosoftBotIdentifier(
+            bot_id=suffix,
+            is_resource_account_configured=True,
+            cloud=CommunicationCloudEnvironment.GCCH,
+            raw_id=raw_id,
+        )  # type: ignore
+    if prefix == BOT_DOD_CLOUD_PREFIX:
+        return MicrosoftBotIdentifier(
+            bot_id=suffix,
+            is_resource_account_configured=True,
+            cloud=CommunicationCloudEnvironment.DOD,
+            raw_id=raw_id,
+        )  # type: ignore
+    return UnknownIdentifier(identifier=raw_id)  # type: ignore
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/policy.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/policy.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/user_credential.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/user_credential.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/user_credential_async.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/user_credential_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/utils.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -------------------------------------------------------------------------
 
 import base64
 import json
 import calendar
 from typing import cast, Tuple, Optional
 from datetime import datetime
-from azure.core.serialization import TZ_UTC
+from msrest.serialization import TZ_UTC
 from azure.core.credentials import AccessToken
 
 
 def _convert_datetime_to_utc_int(input_datetime) -> int:
     """
     Converts DateTime in local time to the Epoch in UTC in second.
```

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/_shared/utils_async.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/_shared/utils_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure/communication/rooms/aio/_rooms_client_async.py` & `azure-communication-rooms-1.1.0b1/azure/communication/rooms/aio/_rooms_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/PKG-INFO` & `azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: azure-communication-rooms
-Version: 1.1.0
+Version: 1.1.0b1
 Summary: Microsoft Communication Rooms Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: azure-core<2.0.0,>=1.24.0
+Requires-Dist: msrest>=0.7.1
+Requires-Dist: typing-extensions; python_version < "3.8"
 
 # Azure Communication Rooms client library for Python
 This package contains a Python SDK for Azure Communication Services for Rooms.
 Read more about Azure Communication Services [here](https://docs.microsoft.com/azure/communication-services/overview)
 
 ## _Disclaimer_
 
@@ -68,15 +70,15 @@
 - `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
 valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
 - `pstn_dial_out_enabled`: Set this flag to true if, at the time of the call, dial out to a PSTN number is enabled in a particular room. This flag is optional.
 
 ### Create a room
 To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To create room with PSTN Dial-Out property, call `create_room` function and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled` is not provided, then the default value for `pstn_dial_out_enabled` is false.
 
 ```python
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
 from azure.communication.rooms import (
     RoomsClient,
     RoomParticipant,
@@ -102,15 +104,15 @@
 
     )
 except HttpResponseError as ex:
     print(ex)
 ```
 ### Update a room
 The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
-Starting in 1.1.0 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
+Starting in 1.1.0b1 release, ACS Rooms supports PSTN Dial-Out feature. To update a room with PSTN Dial-Out property, call `update_room` and set `pstn_dial_out_enabled` to either true or false. If `pstn_dial_out_enabled`  is not provided, then there is no changes to PstnDialOutEnabled property in the room.
 
 ```python
 try:
     update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4),
```

### Comparing `azure-communication-rooms-1.1.0/azure_communication_rooms.egg-info/SOURCES.txt` & `azure-communication-rooms-1.1.0b1/azure_communication_rooms.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -50,11 +50,13 @@
 tests/acs_rooms_test_case.py
 tests/conftest.py
 tests/test_hmac.py
 tests/test_rooms_client.py
 tests/test_rooms_client_async.py
 tests/_shared/__init__.py
 tests/_shared/async_fake_token_credential.py
+tests/_shared/asynctestcase.py
 tests/_shared/communication_service_preparer.py
 tests/_shared/fake_token_credential.py
 tests/_shared/helper.py
+tests/_shared/testcase.py
 tests/_shared/utils.py
```

### Comparing `azure-communication-rooms-1.1.0/samples/rooms_client_sample.py` & `azure-communication-rooms-1.1.0b1/samples/rooms_client_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 )
 
 sys.path.append("..")
 
 class RoomsSample(object):
 
     def setUp(self):
-        self.connection_string = os.getenv("COMMUNICATION_CONNECTION_STRING_ROOMS")
+        self.connection_string = os.getenv("COMMUNICATION_SAMPLES_CONNECTION_STRING")
 
         self.rooms_client = RoomsClient.from_connection_string(self.connection_string)
         self.identity_client = CommunicationIdentityClient.from_connection_string(
             self.connection_string)
         self.rooms = []
         self.participant_1 = RoomParticipant(
             communication_identifier=self.identity_client.create_user(),
```

### Comparing `azure-communication-rooms-1.1.0/samples/rooms_client_sample_async.py` & `azure-communication-rooms-1.1.0b1/samples/rooms_client_sample_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 )
 
 sys.path.append("..")
 
 class RoomsSample(object):
 
     def setUp(self):
-        self.connection_string = os.getenv("COMMUNICATION_CONNECTION_STRING_ROOMS")
+        self.connection_string = os.getenv("COMMUNICATION_SAMPLES_CONNECTION_STRING")
 
         self.rooms_client = RoomsClient.from_connection_string(self.connection_string)
         self.identity_client = CommunicationIdentityClient.from_connection_string(
             self.connection_string)
         self.rooms = []
         self.participant_1 = RoomParticipant(
             communication_identifier=self.identity_client.create_user(),
```

### Comparing `azure-communication-rooms-1.1.0/setup.py` & `azure-communication-rooms-1.1.0b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,37 +40,36 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms",
     keywords="azure, azure sdk",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(
         exclude=[
             'tests',
             # Exclude packages that will be covered by PEP420 or nspkg
             "azure",
             "azure.communication",
         ]
     ),
     install_requires=[
-        "azure-core>=1.29.0",
-        "isodate>=0.6.1",
+        "azure-core<2.0.0,>=1.24.0",
+        "msrest>=0.7.1",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     include_package_data=True,
     extras_require={
         ":python_version<'3.8'": ["typing-extensions"]
     }
 )
```

### Comparing `azure-communication-rooms-1.1.0/tests/_shared/async_fake_token_credential.py` & `azure-communication-rooms-1.1.0b1/tests/_shared/async_fake_token_credential.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/_shared/fake_token_credential.py` & `azure-communication-rooms-1.1.0b1/tests/_shared/fake_token_credential.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/_shared/utils.py` & `azure-communication-rooms-1.1.0b1/tests/_shared/utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/acs_rooms_test_case.py` & `azure-communication-rooms-1.1.0b1/tests/acs_rooms_test_case.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/conftest.py` & `azure-communication-rooms-1.1.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/test_hmac.py` & `azure-communication-rooms-1.1.0b1/tests/test_hmac.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/test_rooms_client.py` & `azure-communication-rooms-1.1.0b1/tests/test_rooms_client.py`

 * *Files identical despite different names*

### Comparing `azure-communication-rooms-1.1.0/tests/test_rooms_client_async.py` & `azure-communication-rooms-1.1.0b1/tests/test_rooms_client_async.py`

 * *Files identical despite different names*

