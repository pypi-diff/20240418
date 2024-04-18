# Comparing `tmp/pyicat-plus-0.1.8b0.tar.gz` & `tmp/pyicat_plus-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyicat-plus-0.1.8b0.tar", last modified: Fri Dec  8 10:51:43 2023, max compression
+gzip compressed data, was "pyicat_plus-0.2.0rc0.tar", last modified: Thu Apr 18 16:50:17 2024, max compression
```

## Comparing `pyicat-plus-0.1.8b0.tar` & `pyicat_plus-0.2.0rc0.tar`

### file list

```diff
@@ -1,85 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1672 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-12-08 10:48:32.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_raw.py
--rw-rw-rw-   0 root         (0) root         (0)    17511 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/apps/sync_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/archive.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     7690 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     5248 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     9073 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/investigation.py
--rw-rw-rw-   0 root         (0) root         (0)    13930 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3986 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2662 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/null.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/client/xmlns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/query_pool/
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/query_pool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/query_pool/gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/query_pool/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10120 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/namespace_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/nexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9624 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/icat.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/proc.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2879 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/activemq_rest_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/icat_db.py
--rw-rw-rw-   0 root         (0) root         (0)     9199 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/icatplus_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/stomp_publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/stomp_subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     9884 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_investigations.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_mockup.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     8762 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_sync.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)     4610 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_query_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/tests/utils/compare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-08 10:51:35.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/utils/maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-12-08 10:41:30.000000 pyicat-plus-0.1.8b0/src/pyicat_plus/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1672 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2612 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      414 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-12-08 10:51:43.000000 pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-18 16:48:56.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/icat_as_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_raw.py
+-rw-rw-rw-   0 root         (0) root         (0)    17512 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/sync_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     7708 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    14265 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/investigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19360 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/xmlns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11075 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2024-04-18 15:13:55.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/namespace_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/nexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11429 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/icat.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/activemq_rest_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icat_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     9204 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icatplus_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15798 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_investigations.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_mockup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    21005 2024-04-03 00:12:57.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     4548 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-07 16:03:54.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/path_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6944 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/raw_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12868 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyicat-plus-0.1.8b0/LICENSE.md` & `pyicat_plus-0.2.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/setup.cfg` & `pyicat_plus-0.2.0rc0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,49 +22,55 @@
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	requests
 	stompest
 	numpy
+	querypool
 	icat-esrf-definitions
+	tqdm
+	h5py
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	icat-store-raw=pyicat_plus.apps.store_raw:main
 	icat-sync-raw=pyicat_plus.apps.sync_raw:main
 	icat-store-processed=pyicat_plus.apps.store_processed:main
 	icat-store-from-file=pyicat_plus.apps.store_from_file:main
+	icat-nexus-definitions=pyicat_plus.apps.icat_as_nexus:main
 
 [options.package_data]
 * = hdf5_cfg.xml
 
 [options.extras_require]
 bliss = 
-	blissdata
+	blissdata[beacon]
 test = 
 	%(bliss)s
 	pytest >=7
 	pytest-timeout >=2.1
 	numpy >=1.15
 	psutil
 	coilmq
 	stomp.py >=7
 	xmltodict
+	h5py >=3.5
 dev = 
 	%(test)s
 	black >=22
 	flake8 >=4
 doc = 
 	%(test)s
 	sphinx >=4.5
 	sphinx-autodoc-typehints >=1.16
+	pydata-sphinx-theme < 0.15
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_from_file.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_from_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import os
 import sys
+import logging
 import argparse
 from glob import glob
-from ..client.main import IcatClient
+
 from ..client import defaults
+from ..client.main import IcatClient
+from ..utils.log_utils import basic_config
+
+logger = logging.getLogger(__name__)
 
 
 def main(argv=None):
+    basic_config(logger=logger, level=logging.DEBUG, format="%(message)s")
+
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser(description="Register stored data with ICAT")
     add_store_parameters(parser)
     args = parser.parse_args(argv[1:])
     apply_store_parameters(args)
 
     client = IcatClient(metadata_urls=args.metadata_urls)
 
     for filename in args.files:
-        print("Register", filename)
+        logger.debug("Register", filename)
         client.store_dataset_from_file(filename)
 
+    client.disconnect()
+
 
 def add_store_parameters(parser):
     parser.add_argument("filter", help="File search filter")
 
     parser.add_argument(
         "--queue",
         dest="metadata_urls",
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_processed.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_processed.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         proposal=args.proposal,
         dataset=args.dataset,
         path=args.path,
         metadata=args.metadata,
         raw=args.raw,
     )
 
+    client.disconnect()
+
 
 def add_process_parameters(parser):
     parser.add_argument(
         "--raw",
         action="append",
         required=True,
         help="Raw dataset directories",
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/apps/store_raw.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_raw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import json
 import argparse
-from configparser import RawConfigParser
 from typing import Any, Tuple
+from configparser import RawConfigParser
+
 from ..client.main import IcatClient
 from ..client import defaults
 
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
@@ -20,14 +21,15 @@
     client.store_dataset(
         beamline=args.beamline,
         proposal=args.proposal,
         dataset=args.dataset,
         path=args.path,
         metadata=args.metadata,
     )
+    client.disconnect()
 
 
 def add_store_parameters(parser):
     parser.add_argument("--beamline", required=True, help="Beamline name")
 
     parser.add_argument("--proposal", required=True, help="Proposal name")
 
@@ -61,15 +63,18 @@
         help="ActiveMQ queue URLS",
         default=[],
     )
 
 
 def apply_store_parameters(args):
     if args.metadatafile:
-        parameters = _parameters_from_file()
+        try:
+            parameters = _parameters_from_file(args.metadatafile.read())
+        finally:
+            args.metadatafile.close()
     else:
         parameters = dict()
     if args.parameters:
         parameters.update(_parse_parameter(s) for s in args.parameters)
     if args.sample:
         parameters["Sample_name"] = args.sample
     args.metadata = parameters
@@ -86,16 +91,15 @@
 def _parse_value(value: str) -> Any:
     try:
         return json.loads(value)
     except Exception:
         return value
 
 
-def _parameters_from_file(path: str) -> dict:
+def _parameters_from_file(content: str) -> dict:
     config = RawConfigParser()
-    with open(path, "r") as f:
-        config.read_string("[config]\n" + f.read())
-        return dict(config["config"].items())
+    config.read_string("[config]\n" + content)
+    return {key: _parse_value(value) for key, value in config["config"].items()}
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/archive.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
             queue_name = defaults.ARCHIVE_QUEUE
         if queue_urls is None:
             queue_urls = defaults.ARCHIVE_BROKERS
         self._client = IcatMessagingClient(
             queue_urls, queue_name, monitor_port=monitor_port, timeout=timeout
         )
 
+    def disconnect(self):
+        self._client.disconnect()
+
     def send_archive_status(
         self, dataset_id: int, type: StatusType, level: StatusLevel, message: str
     ):
         assert dataset_id, "ICAT requires the datasetId"
         assert type, "ICAT requires the type"
         assert level, "ICAT requires the level"
         root = {
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/bliss.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/bliss.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,8 +19,9 @@
             f"Beacon host {beacon_host} does not provide ICAT configuration"
         )
     return IcatClient(
         metadata_urls=config["metadata_urls"],
         elogbook_url=config["elogbook_url"],
         elogbook_token=config["elogbook_token"],
         feedback_timeout=timeout,
+        add_files_urls=config["metadata_urls"],
     )
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/elogbook.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/elogbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from enum import Enum
-from datetime import datetime
-import requests
 import base64
-import mimetypes
 import socket
+import logging
+import datetime
+import mimetypes
+from enum import Enum
 from urllib.parse import urljoin
 from typing import Optional, Iterable, List
-import logging
+
+import requests
 
 from ..utils.url import normalize_url
 from .. import __version__
 from . import defaults
 
 logger = logging.getLogger(__name__)
 
@@ -110,15 +111,17 @@
                     tags.append(tag)
         return tags
 
     def _post_with_payload(
         self, url: str, message_payload: dict, call_payload: dict
     ) -> None:
         payload = self._merge_payloads(message_payload, call_payload)
-        payload.setdefault("creationDate", datetime.now().astimezone().isoformat())
+        payload.setdefault(
+            "creationDate", datetime.datetime.now().astimezone().isoformat()
+        )
         try:
             response = requests.post(url, json=payload, timeout=self.timeout)
         except requests.exceptions.ReadTimeout:
             return  # we have no confirmation that the call succeeded
         except Exception as e:
             if self.raise_error:
                 raise
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/interface.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,57 @@
-from datetime import datetime
-from typing import Optional, List, Tuple, Sequence
-from dataclasses import dataclass
+import datetime
+import dataclasses
+from typing import Optional, List, Tuple, Sequence, Union, Dict, Any
 
 
-@dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True)
 class DatasetId:
     name: str
     path: str
 
 
+@dataclasses.dataclass(frozen=True)
+class DatasetMetadata:
+    file_count: int
+
+
+@dataclasses.dataclass(frozen=True)
+class Dataset:
+    dataset_id: DatasetId
+    icat_dataset_id: int
+    dataset_metadata: DatasetMetadata
+
+    def as_dict(self) -> Dict[str, Any]:
+        return dataclasses.asdict(self)
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> "Dataset":
+        """Factory method to create a Dataset instance from a dictionary."""
+        data = data.copy()
+        data["dataset_id"] = DatasetId(**data["dataset_id"])
+        data["dataset_metadata"] = DatasetMetadata(**data["dataset_metadata"])
+        return cls(**data)
+
+
 class IcatClientInterface:
     def send_message(
         self,
         msg: str,
         msg_type="comment",
         beamline: Optional[str] = None,
         proposal: Optional[str] = None,
         dataset: Optional[str] = None,
         beamline_only: Optional[bool] = None,
         **payload
     ):
         raise NotImplementedError
 
+    def disconnect(self):
+        pass
+
     def send_data(
         self,
         data: bytes,
         mimetype: Optional[str] = None,
         beamline: Optional[str] = None,
         proposal: Optional[str] = None,
         beamline_only: Optional[bool] = None,
@@ -112,45 +138,55 @@
     def store_dataset_from_file(self, store_filename: Optional[str] = None):
         raise NotImplementedError
 
     def investigation_info(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[dict]:
         raise NotImplementedError
 
     def registered_dataset_ids(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[List[DatasetId]]:
         raise NotImplementedError
 
+    def registered_datasets(
+        self,
+        beamline: str,
+        proposal: str,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
+        allow_open_ended: bool = True,
+        timeout: Optional[float] = None,
+    ) -> Optional[List[Dataset]]:
+        raise NotImplementedError
+
     def investigation_info_string(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> str:
         raise NotImplementedError
 
     def investigation_summary(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> List[Tuple]:
         raise NotImplementedError
 
     @property
     def expire_datasets_on_close(self) -> bool:
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/investigation.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/investigation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
-from datetime import datetime
-from typing import Optional, List
+import logging
+import datetime
 from urllib.parse import urljoin
+from typing import Optional, List, Union, Sequence
+
 import requests
 import numpy
-import logging
 
-from ..concurrency.query_pool import QueryPool
-from .interface import DatasetId
+from ..concurrency import QueryPool
+from .interface import DatasetId, Dataset, DatasetMetadata
 from ..utils.maxsizedict import MaxSizeDict
 from ..utils.url import normalize_url
 from . import defaults
 
 logger = logging.getLogger(__name__)
 
+_DEFAULT_START_TIME = datetime.time(hour=8)
+
 
 class IcatInvestigationClient:
     """Client for the investigation part of the ICAT+ REST API.
 
     An "investigation" is a time slot assigned to a particular proposal
     at a particular beamline.
 
@@ -60,16 +63,16 @@
     def timeout(self, value: Optional[float] = None):
         self.__query_pool.timeout = value
 
     def _get_with_response_parsing(
         self, url: str, timeout: Optional[float] = None
     ) -> Optional[list]:
         """Return `None` means the information is not available at this moment.
-        An empty list means that an error has occured or an actual empty list
-        is returned.
+        An empty list means that an error has occured on the server side or an
+        actual empty list is returned.
         """
         try:
             response = self.__query_pool.execute(
                 requests.get, args=(url,), timeout=timeout, default=None
             )
         except requests.exceptions.ReadTimeout:
             return None
@@ -89,15 +92,15 @@
         else:
             return list()
 
     def investigation_info(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[dict]:
         """An investigation is defined by a time slot. Find an investigation (if any)
         for a beamline, proposal and date ("now" when not provided). When there is
         more than one investigation, select the closest one started before or at the date.
         If there is no such investigation, get the closest investigation which starts after the date.
@@ -123,29 +126,29 @@
         # Normalize information
         for key in ["parameters", "visitId"]:
             investigation.pop(key, None)
         ninfo = dict()
         ninfo["proposal"] = investigation.pop("name", None)
         ninfo["beamline"] = investigation.pop("instrument", dict()).get("name", None)
         ninfo.update(investigation)
-        ninfo[
-            "e-logbook"
-        ] = f"https://data.esrf.fr/investigation/{investigation['id']}/events"
-        ninfo[
-            "data portal"
-        ] = f"https://data.esrf.fr/investigation/{investigation['id']}/datasets"
+        ninfo["e-logbook"] = (
+            f"https://data.esrf.fr/investigation/{investigation['id']}/events"
+        )
+        ninfo["data portal"] = (
+            f"https://data.esrf.fr/investigation/{investigation['id']}/datasets"
+        )
 
         self.__investigation_info[investigation_key] = ninfo
         return ninfo
 
     def _investigation_id(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[int]:
         info = self.investigation_info(
             beamline=beamline,
             proposal=proposal,
             date=date,
@@ -156,15 +159,15 @@
             return None
         return info.get("id", None)
 
     def registered_dataset_ids(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[List[DatasetId]]:
         investigation_id = self._investigation_id(
             beamline=beamline,
             proposal=proposal,
             date=date,
@@ -172,95 +175,227 @@
             timeout=timeout,
         )
         if investigation_id is None:
             return None
         url = self._dataset_url.format(investigation_id=investigation_id)
         datasets = self._get_with_response_parsing(url, timeout=timeout)
         if datasets is None:
-            return None
+            return None  # not available at the moment
         return [self._icat_dataset_to_datasetid(dataset) for dataset in datasets]
 
+    def registered_datasets(
+        self,
+        beamline: str,
+        proposal: str,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
+        allow_open_ended: bool = True,
+        timeout: Optional[float] = None,
+    ) -> Optional[List[Dataset]]:
+        investigation_id = self._investigation_id(
+            beamline=beamline,
+            proposal=proposal,
+            date=date,
+            allow_open_ended=allow_open_ended,
+            timeout=timeout,
+        )
+        if investigation_id is None:
+            return None
+        url = self._dataset_url.format(investigation_id=investigation_id)
+        datasets = self._get_with_response_parsing(url, timeout=timeout)
+        if datasets is None:
+            return None  # not available at the moment
+        return [self._icat_dataset_to_dataset(dataset) for dataset in datasets]
+
     @staticmethod
-    def _icat_dataset_to_datasetid(dataset: dict) -> DatasetId:
+    def _get_dataset_parameter_value_by_name(
+        dataset: dict, parameter_name: str
+    ) -> Optional[str]:
+        if "parameters" in dataset:
+            for p in dataset["parameters"]:
+                if p["name"] == parameter_name:
+                    return p["value"]
+
+    @classmethod
+    def _icat_dataset_to_datasetid(cls, dataset: dict) -> DatasetId:
         location = dataset["location"]
         location, name = os.path.split(location)
         while location and not name:
             location, name = os.path.split(location)
         return DatasetId(name=name, path=dataset["location"])
 
+    @classmethod
+    def _icat_dataset_to_dataset(cls, dataset: dict) -> Dataset:
+        dataset_id = cls._icat_dataset_to_datasetid(dataset)
+        file_count = cls._get_dataset_parameter_value_by_name(dataset, "__fileCount")
+        dataset_metadata = DatasetMetadata(
+            file_count=int(0 if file_count is None else file_count)
+        )
+        return Dataset(
+            dataset_id=dataset_id,
+            icat_dataset_id=dataset["id"],
+            dataset_metadata=dataset_metadata,
+        )
+
 
 def _select_investigation(
     investigations: List[dict],
-    date: Optional[datetime] = None,
+    date: Optional[Union[datetime.datetime, datetime.date]] = None,
     allow_open_ended: bool = True,
 ) -> Optional[dict]:
     """When `date` is not provided we take it to be "now".
 
     This method returns the last investigation that contains
     the date or has a start/end closest to the date. The
     investigations are ordered from first to last created.
 
     Optionally all open-ended investigations can be ignored.
     Open-ended investigations have a start date but no end date.
     These investigations are created by sending dataset or
     investigation messages with start dates 48h outside any
     official investigation.
+
+    :param investigations: unsorted list of investigations
+    :param date: possibly not fully deterministic date
+    :param allow_open_ended: validation option
+    :returns: matching investigation according to the selection rules
+    """
+    investigations = _filter_valid_investigations(
+        investigations, allow_open_ended=allow_open_ended
+    )
+    if not investigations:
+        return
+    if len(investigations) == 1:
+        return investigations[0]
+
+    # Sort investigations by order of importance: database creation time
+    investigations = sorted(
+        investigations, key=lambda investigation: investigation["id"]
+    )
+
+    date = _deterministic_date(date, investigations)
+    return _select_investigation_from_sorted_list(investigations, date)
+
+
+def _filter_valid_investigations(
+    investigations: List[dict], allow_open_ended: bool = True
+) -> List[dict]:
+    """Filter out investigations with invalid time slots.
+
+    :param investigations: unsorted list of investigations
+    :param allow_open_ended: validation option
+    :returns: list of valid investigations (preserve order)
     """
-    # Select valid investigations
     if allow_open_ended:
-        valid = [
+        return [
             investigation
             for investigation in investigations
             if investigation.get("startDate")
         ]
+    return [
+        investigation
+        for investigation in investigations
+        if investigation.get("startDate") and investigation.get("endDate")
+    ]
+
+
+def _deterministic_date(
+    date: Optional[Union[datetime.datetime, datetime.date]], investigations: List[dict]
+) -> datetime.datetime:
+    """The date might
+
+    * not exist: take now
+    * have no time zone: add local timezone
+    * be a day without time: select time from the investigations or the default 8 a.m.
+
+    The resulting date is fully deterministic.
+
+    :param date: possibly not fully deterministic date
+    :param investigations: sorted by order of importance
+    :returns: fully deterministic date
+    """
+    if date is None:
+        return datetime.datetime.now().astimezone()
+
+    if isinstance(date, datetime.datetime):
+        return date.astimezone()
+
+    # Get the time from the investigations that start on the same day
+    start_dates = [
+        _tz_aware_fromisoformat(investigation["startDate"])
+        for investigation in investigations
+    ]
+    is_start_date = [dt.date() == date for dt in start_dates]
+    last_is_start_date = _last_where_true(is_start_date)
+    if last_is_start_date is None:
+        # No investigation starts on the same day
+        start_time = _DEFAULT_START_TIME
     else:
-        valid = [
-            investigation
-            for investigation in investigations
-            if investigation.get("startDate") and investigation.get("endDate")
-        ]
-    if not valid:
-        return
-    if len(valid) == 1:
-        return valid[0]
+        # Last investigation that starts on the same day
+        start_time = start_dates[last_is_start_date].time()
 
-    if date is None:
-        date = datetime.now()
-    date = date.astimezone()
+    date = datetime.datetime.combine(date, start_time)
+    return date.astimezone()
 
-    # Sorted by creation order
-    valid_sorted = sorted(valid, key=lambda investigation: investigation["id"])
 
+def _select_investigation_from_sorted_list(
+    investigations: List[dict], date: datetime.datetime
+) -> dict:
+    """
+    :param investigations: sorted by order of importance
+    :param date: point in time for which we want to find the corresponding investigation
+    :returns: matching investigation according to the selection rules
+    """
     # Seconds between date and start/end of each investigation
-    n = len(valid_sorted)
+    n = len(investigations)
     startdiff = numpy.zeros(n)
     enddiff = numpy.full(n, numpy.inf)
-    for i, investigation in enumerate(valid_sorted):
+    for i, investigation in enumerate(investigations):
         startdate = _tz_aware_fromisoformat(investigation["startDate"])
         startdiff[i] = (date - startdate).total_seconds()
         enddate = investigation.get("endDate")
         if enddate is not None:
             enddate = _tz_aware_fromisoformat(enddate)
             enddiff[i] = (enddate - date).total_seconds()
 
-    # Last investigation which contains the date
+    # Close open-ended investigation when the next investigation starts (if any)
+    closed_ended = numpy.isfinite(enddiff)
+    starttime_order = numpy.argsort(-startdiff)
+    for i in range(n - 1):
+        idx = starttime_order[i]
+        if not closed_ended[idx]:
+            idx_next = starttime_order[i + 1]
+            enddiff[idx] = -startdiff[idx_next]
+
+    # Return the last closed investigation which contains the date (if any)
     contains_date = (startdiff >= 0) & (enddiff >= 0)
-    if contains_date.any():
-        i = numpy.argwhere(contains_date)[-1][0]
-        return valid_sorted[i]
+    contains_date_and_closed = contains_date & closed_ended
+    idx = _last_where_true(contains_date_and_closed)
+    if idx is not None:
+        return investigations[idx]
+
+    # Return the last investigation which contains the date (if any)
+    idx = _last_where_true(contains_date)
+    if idx is not None:
+        return investigations[idx]
 
-    # Last investigation with the closest start or end date
+    # Return the last investigation with the closest start or end date
     startdiff = numpy.abs(startdiff)
     enddiff = numpy.abs(enddiff)
     istart = numpy.argmin(startdiff)
     iend = numpy.argmin(enddiff)
     min_startdiff = startdiff[istart]
     min_enddiff = enddiff[iend]
     if min_startdiff < min_enddiff:
-        return valid_sorted[istart]
+        return investigations[istart]
     if min_startdiff > min_enddiff:
-        return valid_sorted[iend]
-    return valid_sorted[max(istart, iend)]
+        return investigations[iend]
+    return investigations[max(istart, iend)]
+
+
+def _tz_aware_fromisoformat(date: str) -> datetime.datetime:
+    return datetime.datetime.fromisoformat(date).astimezone()
 
 
-def _tz_aware_fromisoformat(date: str) -> datetime:
-    return datetime.fromisoformat(date).astimezone()
+def _last_where_true(bool_arr: Sequence[bool]) -> Optional[int]:
+    indices = numpy.argwhere(bool_arr)
+    if indices.size:
+        return indices[-1][0]
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/main.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import List, Mapping, Optional, Sequence, Tuple
-from datetime import datetime
+from typing import List, Mapping, Optional, Sequence, Tuple, Union
+import datetime
 
 import numpy
 
 from .archive import IcatArchiveStatusClient, StatusLevel, StatusType
 from .elogbook import IcatElogbookClient
-from .interface import DatasetId, IcatClientInterface
+from .interface import DatasetId, Dataset, IcatClientInterface
 from .investigation import IcatInvestigationClient
 from .metadata import IcatMetadataClient
+from .update_metadata import IcatUpdateMetadataClient
+from .add_files import IcatAddFilesClient
 
 
 class IcatClient(IcatClientInterface):
-    """Direct communication with ICAT: e-logbook, metadata and archive status"""
+    """Direct communication with ICAT: e-logbook, metadata, archive status, update sample, add files"""
 
     def __init__(
         self,
         metadata_urls: Optional[List[str]] = None,
         elogbook_url: Optional[str] = None,
         elogbook_token: Optional[str] = None,
         metadata_queue: Optional[str] = None,
@@ -25,53 +27,64 @@
         queue_timeout: Optional[float] = None,
         beamline: Optional[str] = None,
         proposal: Optional[str] = None,
         elogbook_metadata: Optional[Mapping] = None,
         archive_urls: Optional[List[str]] = None,
         archive_queue: Optional[str] = None,
         archive_queue_monitor_port: Optional[int] = None,
+        update_metadata_urls: Optional[List[str]] = None,
+        update_metadata_queue: Optional[str] = None,
+        update_metadata_queue_monitor_port: Optional[int] = None,
+        add_files_urls: Optional[List[str]] = None,
+        add_files_queue: Optional[str] = None,
+        add_files_queue_monitor_port: Optional[int] = None,
     ):
         self.current_proposal = proposal
         self.current_beamline = beamline
         self.current_dataset = None
         self.current_path = None
         self.current_dataset_metadata = None
-        if metadata_urls:
-            self._metadata_client = IcatMetadataClient(
-                queue_urls=metadata_urls,
-                queue_name=metadata_queue,
-                monitor_port=metadata_queue_monitor_port,
-                timeout=queue_timeout,
-            )
-        else:
-            self._metadata_client = None
-        if archive_urls:
-            self._archive_client = IcatArchiveStatusClient(
-                queue_urls=archive_urls,
-                queue_name=archive_queue,
-                monitor_port=archive_queue_monitor_port,
-                timeout=queue_timeout,
-            )
-        else:
-            self._archive_client = None
-        if elogbook_url and elogbook_token:
-            self._investigation_client = IcatInvestigationClient(
-                url=elogbook_url, api_key=elogbook_token, timeout=feedback_timeout
-            )
-            if elogbook_metadata is None:
-                elogbook_metadata = dict()
-            self._elogbook_client = IcatElogbookClient(
-                url=elogbook_url,
-                api_key=elogbook_token,
-                timeout=elogbook_timeout,
-                **elogbook_metadata,
-            )
-        else:
-            self._investigation_client = None
-            self._elogbook_client = None
+        self._init_metadata(
+            queue_timeout, metadata_urls, metadata_queue, metadata_queue_monitor_port
+        )
+        self._init_archive(
+            queue_timeout,
+            archive_urls,
+            archive_queue,
+            archive_queue_monitor_port,
+        )
+        self._init_update_metadata(
+            queue_timeout,
+            update_metadata_urls,
+            update_metadata_queue,
+            update_metadata_queue_monitor_port,
+        )
+        self._init_logbook(
+            feedback_timeout,
+            elogbook_metadata,
+            elogbook_url,
+            elogbook_token,
+            elogbook_timeout,
+        )
+        self._init_add_files(
+            queue_timeout,
+            add_files_urls,
+            add_files_queue,
+            add_files_queue_monitor_port,
+        )
+
+    def disconnect(self):
+        if self._metadata_client is not None:
+            self._metadata_client.disconnect()
+        if self._update_metadata_client is not None:
+            self._update_metadata_client.disconnect()
+        if self._add_files_client is not None:
+            self._add_files_client.disconnect()
+        if self._archive_client is not None:
+            self._archive_client.disconnect()
 
     @property
     def metadata_client(self):
         if self._metadata_client is None:
             raise RuntimeError("The message queue URL's are missing")
         return self._metadata_client
 
@@ -129,14 +142,118 @@
 
     @property
     def archive_client(self):
         if self._archive_client is None:
             raise RuntimeError("The message queue URL's are missing")
         return self._archive_client
 
+    @property
+    def update_metadata_client(self):
+        if self._update_metadata_client is None:
+            raise RuntimeError("The message queue URL's are missing")
+        return self._update_metadata_client
+
+    @property
+    def add_files_client(self):
+        if self._add_files_client is None:
+            raise RuntimeError("The message queue URL's are missing")
+        return self._add_files_client
+
+    def _init_metadata(
+        self,
+        queue_timeout: Optional[float] = None,
+        metadata_urls: Optional[List[str]] = None,
+        metadata_queue: Optional[str] = None,
+        metadata_queue_monitor_port: Optional[int] = None,
+    ):
+        if metadata_urls:
+            self._metadata_client = IcatMetadataClient(
+                queue_urls=metadata_urls,
+                queue_name=metadata_queue,
+                monitor_port=metadata_queue_monitor_port,
+                timeout=queue_timeout,
+            )
+        else:
+            self._metadata_client = None
+
+    def _init_archive(
+        self,
+        queue_timeout: Optional[float] = None,
+        archive_urls: Optional[List[str]] = None,
+        archive_queue: Optional[str] = None,
+        archive_queue_monitor_port: Optional[int] = None,
+    ):
+        if archive_urls:
+            self._archive_client = IcatArchiveStatusClient(
+                queue_urls=archive_urls,
+                queue_name=archive_queue,
+                monitor_port=archive_queue_monitor_port,
+                timeout=queue_timeout,
+            )
+        else:
+            self._archive_client = None
+
+    def _init_update_metadata(
+        self,
+        queue_timeout: Optional[float] = None,
+        update_metadata_urls: Optional[List[str]] = None,
+        update_metadata_queue: Optional[str] = None,
+        update_metadata_queue_monitor_port: Optional[int] = None,
+    ):
+        if update_metadata_urls:
+            self._update_metadata_client = IcatUpdateMetadataClient(
+                queue_urls=update_metadata_urls,
+                queue_name=update_metadata_queue,
+                monitor_port=update_metadata_queue_monitor_port,
+                timeout=queue_timeout,
+            )
+        else:
+            self._update_metadata_client = None
+
+    def _init_logbook(
+        self,
+        feedback_timeout,
+        elogbook_metadata,
+        elogbook_url,
+        elogbook_token,
+        elogbook_timeout,
+    ):
+        if elogbook_url and elogbook_token:
+            self._investigation_client = IcatInvestigationClient(
+                url=elogbook_url, api_key=elogbook_token, timeout=feedback_timeout
+            )
+            if elogbook_metadata is None:
+                elogbook_metadata = dict()
+            self._elogbook_client = IcatElogbookClient(
+                url=elogbook_url,
+                api_key=elogbook_token,
+                timeout=elogbook_timeout,
+                **elogbook_metadata,
+            )
+        else:
+            self._investigation_client = None
+            self._elogbook_client = None
+
+    def _init_add_files(
+        self,
+        queue_timeout: Optional[float] = None,
+        add_files_urls: Optional[List[str]] = None,
+        add_files_queue: Optional[str] = None,
+        add_files_queue_monitor_port: Optional[int] = None,
+    ):
+        if add_files_urls:
+            self._add_files_client = IcatAddFilesClient(
+                queue_urls=add_files_urls,
+                queue_name=add_files_queue,
+                monitor_port=add_files_queue_monitor_port,
+                timeout=queue_timeout,
+            )
+        else:
+            self._add_files_client = None
+
     def send_message(
         self,
         msg: str,
         msg_type="comment",
         beamline: Optional[str] = None,
         proposal: Optional[str] = None,
         dataset: Optional[str] = None,
@@ -319,15 +436,15 @@
     def store_dataset_from_file(self, store_filename: Optional[str] = None):
         self.metadata_client.send_metadata_from_file(store_filename)
 
     def investigation_info(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[dict]:
         return self.investigation_client.investigation_info(
             beamline=beamline,
             proposal=proposal,
             date=date,
@@ -335,31 +452,47 @@
             timeout=timeout,
         )
 
     def registered_dataset_ids(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> Optional[List[DatasetId]]:
         return self.investigation_client.registered_dataset_ids(
             beamline=beamline,
             proposal=proposal,
             date=date,
             allow_open_ended=allow_open_ended,
             timeout=timeout,
         )
 
+    def registered_datasets(
+        self,
+        beamline: str,
+        proposal: str,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
+        allow_open_ended: bool = True,
+        timeout: Optional[float] = None,
+    ) -> Optional[List[Dataset]]:
+        return self.investigation_client.registered_datasets(
+            beamline=beamline,
+            proposal=proposal,
+            date=date,
+            allow_open_ended=allow_open_ended,
+            timeout=timeout,
+        )
+
     def investigation_info_string(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> str:
         info = self.investigation_info(
             beamline=beamline,
             proposal=proposal,
             date=date,
@@ -378,15 +511,15 @@
             infostr = "Proposal NOT available in the data portal"
         return infostr
 
     def investigation_summary(
         self,
         beamline: str,
         proposal: str,
-        date: Optional[datetime] = None,
+        date: Optional[Union[datetime.datetime, datetime.date]] = None,
         allow_open_ended: bool = True,
         timeout: Optional[float] = None,
     ) -> List[Tuple]:
         info = self.investigation_info(
             beamline=beamline,
             proposal=proposal,
             date=date,
@@ -415,14 +548,42 @@
         level: StatusLevel = StatusLevel.INFO,
         message: Optional[str] = None,
     ):
         self.archive_client.send_archive_status(
             dataset_id=dataset_id, type=type, level=level, message=message
         )
 
+    def update_metadata(
+        self,
+        proposal: str = None,
+        beamline: str = None,
+        dataset_paths: str = None,
+        metadata_name: str = None,
+        metadata_value: str = None,
+    ):
+        if proposal is None:
+            proposal = self.current_proposal
+        if beamline is None:
+            beamline = self.current_beamline
+        self._update_metadata_client.send_update_metadata(
+            proposal=proposal,
+            beamline=beamline,
+            dataset_paths=dataset_paths,
+            metadata_name=metadata_name,
+            metadata_value=metadata_value,
+        )
+
+    def add_files(
+        self,
+        dataset_id: int = None,
+    ):
+        self._add_files_client.add_files(
+            dataset_id=dataset_id,
+        )
+
     @property
     def expire_datasets_on_close(self) -> bool:
         return False
 
     @property
     def reason_for_missing_information(self) -> str:
         return "ICAT communication timeout"
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/messaging.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
-import requests
 from typing import Optional, List
 
+import requests
 from stompest.config import StompConfig
 from stompest.protocol import StompSpec
 from stompest.protocol import StompSession
 from stompest.sync import Stomp
 from stompest.error import StompConnectionError
 
 from ..utils.url import normalize_url
@@ -59,19 +59,22 @@
         self.__consumer_count_url = f"{self.MONITOR_SCHEME}://{{host}}:{monitor_port}/api/jolokia/read/org.apache.activemq:type=Broker,brokerName=metadata,destinationType=Queue,destinationName={queue_name}/ConsumerCount"
         self.__jolokia_headers = {
             "Authorization": b"Basic "
             + base64.b64encode(f"{self.MONITOR_USER}:{self.MONITOR_PWD}".encode())
         }
 
     def reconnect(self):
+        self.disconnect()
+        self._connect()
+
+    def disconnect(self):
         try:
             self.__client.disconnect()
         except StompConnectionError:
-            pass  # not connected
-        self._connect()
+            self.__client.close(flush=True)
 
     def _connect(self):
         self.__client.connect(
             versions=[self.__max_version],
             connectTimeout=self._socket_timeout,
             connectedTimeout=self._connect_timeout,
         )
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/metadata.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
             defaults.METADATA_BROKERS
         if queue_name is None:
             queue_name = defaults.METADATA_QUEUE
         self._client = IcatMessagingClient(
             queue_urls, queue_name, monitor_port=monitor_port, timeout=timeout
         )
 
+    def disconnect(self):
+        self._client.disconnect()
+
     def send_metadata(
         self,
         beamline: str,
         proposal: str,
         dataset: str,
         path: str,
         metadata: dict,
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/null.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/null.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from .interface import IcatClientInterface
 
 
 class IcatNullClient(IcatClientInterface):
     def __init__(self, expire_datasets_on_close=True) -> None:
         self.__expire_datasets_on_close = expire_datasets_on_close
 
+    def disconnect(self):
+        pass
+
     def send_message(self, *args, **kw):
         pass
 
     def send_data(self, *args, **kw):
         pass
 
     def send_text_file(self, *args, **kw):
@@ -32,14 +35,17 @@
 
     def investigation_info(self, *args, **kwargs) -> None:
         pass
 
     def registered_dataset_ids(self, *args, **kwargs) -> None:
         pass
 
+    def registered_datasets(self, *args, **kwargs) -> None:
+        pass
+
     def investigation_info_string(self, *args, **kwargs) -> str:
         return f"Proposal information not available ({self.reason_for_missing_information})"
 
     def investigation_summary(self, *args, **kwargs) -> List[Tuple]:
         keys = ["e-logbook", "data portal"]
         return [
             (key, f"information not available ({self.reason_for_missing_information})")
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/serialize.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections.abc import Iterable, Mapping
 from numbers import Number
 from typing import Union
-from datetime import datetime
+import datetime
 
 
 def serialize_metadata(
     obj: Union[str, bytes, Number, None, Mapping, Iterable], **_recursive_info
 ) -> Union[str, None, dict]:
     """Serialize metadata for ICAT"""
     _recursive_info.setdefault("depth", 0)
     _recursive_info.setdefault("iterable_depth", 0)
     if isinstance(obj, str):
         return obj
     elif isinstance(obj, bytes):
         return obj.decode()
     elif isinstance(obj, Number):
         return str(obj)
-    elif isinstance(obj, datetime):
+    elif isinstance(obj, datetime.datetime):
         return obj.isoformat()
     elif isinstance(obj, Mapping):
         if _recursive_info["depth"]:
             raise TypeError(obj)
         _recursive_info["depth"] += 1
         return {
             serialize_metadata(k, **_recursive_info): serialize_metadata(
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/client/xmlns.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/xmlns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+import datetime
 import xml.etree.ElementTree as etree
 from .serialize import serialize_metadata
 
 ICAT_NAMESPACE_URL = "http://www.esrf.fr/icat"
 
 etree.register_namespace("tns", ICAT_NAMESPACE_URL)
 
@@ -44,17 +44,17 @@
         metadata = dict()
 
     # Required metadata
     assert "Sample_name" in metadata, "ICAT metadata field 'Sample_name' is missing"
 
     # Metadata with defaults
     if "startDate" not in metadata:
-        metadata["startDate"] = datetime.now().astimezone()
+        metadata["startDate"] = datetime.datetime.now().astimezone()
     if "endDate" not in metadata:
-        metadata["endDate"] = datetime.now().astimezone()
+        metadata["endDate"] = datetime.datetime.now().astimezone()
 
     root = root_node("dataset", attrib={"complete": "true"})
     data_node(root, "investigation", proposal)
     data_node(root, "instrument", beamline)
     data_node(root, "name", dataset)
     data_node(root, "location", path)
 
@@ -76,12 +76,12 @@
 def investigation_as_xml(
     beamline: str, proposal: str, start_datetime=None, end_datetime=None
 ):
     root = root_node("investigation")
     data_node(root, "experiment", proposal)
     data_node(root, "instrument", beamline)
     if start_datetime is None:
-        start_datetime = datetime.now().astimezone()
+        start_datetime = datetime.datetime.now().astimezone()
     data_node(root, "startDate", start_datetime)
     if end_datetime is not None:
         data_node(root, "endDate", end_datetime)
     return root
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/concurrency/__init__.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/concurrency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 try:
-    import gevent
+    import gevent.monkey
 except ImportError:
-    gevent = None
+    GEVENT_PATCHED = False
 else:
-    from gevent.monkey import is_anything_patched
+    GEVENT_PATCHED = gevent.monkey.is_anything_patched()
 
-    if not is_anything_patched():
-        gevent = None
+from querypool.pools import CooperativeQueryPool as QueryPool  # noqa F401
 
+if GEVENT_PATCHED:
+    from gevent import Timeout
+    from gevent import spawn  # noqa F401
+    from gevent.queue import Queue, Empty
 
-if gevent is None:
+    def wait_process(process, timeout) -> bool:
+        """
+        :param process: A process object from `subprocess` or `psutil`
+        """
+        try:
+            with Timeout(timeout) as local_timeout:
+                # gevent timeout has to be used here
+                # See https://github.com/gevent/gevent/issues/622
+                process.wait()
+            return True
+        except Timeout as raised_timeout:
+            if local_timeout is not raised_timeout:
+                raise
+            return False
+
+else:
     import threading
     from subprocess import TimeoutExpired
     from queue import Queue, Empty
 
     def spawn(func, *args, **kwargs):
         thread = threading.Thread(target=func, args=args, kwargs=kwargs)
         thread.start()
@@ -25,33 +43,14 @@
         """
         try:
             process.wait(timeout)
             return True
         except (TimeoutError, TimeoutExpired):
             return False
 
-else:
-    from gevent import spawn  # noqa F401
-    from gevent.queue import Queue, Empty
-
-    def wait_process(process, timeout) -> bool:
-        """
-        :param process: A process object from `subprocess` or `psutil`
-        """
-        try:
-            with gevent.Timeout(timeout) as local_timeout:
-                # gevent timeout has to be used here
-                # See https://github.com/gevent/gevent/issues/622
-                process.wait()
-            return True
-        except gevent.Timeout as raised_timeout:
-            if local_timeout is not raised_timeout:
-                raise
-            return False
-
 
 def flush_queue(q: Queue):
     while True:
         try:
             yield q.get(timeout=0)
         except Empty:
             break
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/definitions.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
-import requests
 from enum import Enum
 from io import StringIO
+from xml.etree import ElementTree
 from dataclasses import dataclass
 from collections.abc import Mapping, Sequence
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Union
-from xml.etree import ElementTree
 
+import requests
 import icat_esrf_definitions
 
 from .namespace_wrapper import NamespaceWrapper
 
 
 IcatNodeIdLike = Union[str, Iterable[str]]
 IcatItemType = Union["IcatField", "IcatFieldGroup"]
@@ -189,17 +189,19 @@
 
     def iter_groups_with_type(
         self, categories: Union[IcatCategory, str, Iterable[Union[IcatCategory, str]]]
     ) -> Iterable["IcatFieldGroup"]:
         if isinstance(categories, (IcatCategory, str)):
             categories = {categories}
         categories = {
-            category
-            if isinstance(category, IcatCategory)
-            else IcatCategory.__members__[category]
+            (
+                category
+                if isinstance(category, IcatCategory)
+                else IcatCategory.__members__[category]
+            )
             for category in categories
         }
         for group in self.iter_groups():
             if group.info.category in categories:
                 yield group
 
     def iter_items_with_node_id_suffix(
@@ -304,22 +306,41 @@
         )
         nodes[icat_item.info.name] = icat_item
 
     return IcatFieldGroup(info, nodes)
 
 
 def icat_fields_source(url: Optional[str] = None) -> Union[str, StringIO]:
-    """Get XML description of all ICAT fields from a URL (local file by default)"""
+    """Get XML description of all ICAT fields from a URL.
+
+    :param url: supports filenames or strings with the scheme prefix "file://",
+                "xml://" or anything the `requests` library can handle.
+    :returns: filename or a file object
+    """
     if not url:
         return icat_esrf_definitions.DEFINITIONS_FILE
-    r = requests.get(url)
-    return StringIO(r.text)
+    if re.match(r"[a-z]+://", url) is None:
+        return url
+    if url.startswith("file://") or url.startswith("xml://"):
+        return re.sub(r"^[a-z]+://", "", url)
+    try:
+        response = requests.get(url)
+        response.raise_for_status()
+    except Exception:
+        working_url = "https://gitlab.esrf.fr/icat/hdf5-master-config/-/raw/master/src/icat_esrf_definitions/hdf5_cfg.xml"
+        raise RuntimeError(
+            "The ICAT definitions URL is wrong. Do not specify a URL to fall back to the"
+            f" definitions from the 'icat-esrf-definitions' package or use '{working_url}'"
+        )
+    return StringIO(response.text)
 
 
 def load_icat_fields(url: Optional[str] = None) -> IcatFieldGroup:
     """Returns an object which allows browsing the ICAT metadata definitions.
 
-    Example URL: "https://gitlab.esrf.fr/icat/hdf5-master-config/-/raw/master/hdf5_cfg.xml"
+    :param url: supports filenames or strings with the scheme prefix
+                "file://", "xml://" or anything the `requests` library can handle.
+    :returns: a mapping object representing the tree relationship of ICAT fields
     """
     tree = ElementTree.parse(icat_fields_source(url=url))
     in_node = tree.getroot()
     return load_group(in_node, name="", parent=IcatNodeId(), NX_class="NXentry")
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/namespace_wrapper.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/namespace_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from functools import partial
 from typing import Callable, Iterable, Optional
 
 
 class NamespaceWrapper:
     """Namespace which delegates attribute getting and setting to a getter and setter method."""
 
+    _PROPERTY_NAMES = ()
+
     def __new__(
         cls,
         property_names: Iterable[str],
         getter: Callable,
         setter: Optional[Callable] = None,
         property_decorator: Optional[Callable] = None,
     ):
         cls = type(cls.__name__, (cls,), {})
         if property_decorator is None:
             property_decorator = property
+        property_names = tuple(sorted(property_names))
+        cls._PROPERTY_NAMES = property_names
         for key in property_names:
             prop = property_decorator(partial(NamespaceWrapper._getter, key=key))
             if setter is not None:
                 prop = prop.setter(partial(NamespaceWrapper._setter, key=key))
             setattr(cls, key, prop)
         return object.__new__(cls)
 
@@ -29,14 +33,24 @@
         setter: Optional[Callable] = None,
         property_decorator: Optional[Callable] = None,
     ):
         self.__property_names = property_names
         self.__getter = getter
         self.__setter = setter
 
+    def __str__(self) -> str:
+        if self._PROPERTY_NAMES:
+            return "NameSpace:\n " + "\n ".join(self._PROPERTY_NAMES)
+        else:
+            return "NameSpace: <empty>"
+
+    def __info__(self) -> str:
+        # For the Bliss shell
+        return str(self)
+
     def _getter(self, key):
         return self.__getter(key)
 
     def _setter(self, value, key):
         return self.__setter(key, value)
 
     def get_content(self) -> str:
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/metadata/nexus.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/nexus.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,19 @@
         return int(value)
     elif nxtype == "NX_FLOAT":
         return float(value)
     else:
         return value
 
 
-def create_nxtreedict(metadata: dict, icat_fields: Optional[IcatFieldGroup] = None):
+def create_nxtreedict(
+    metadata: dict,
+    icat_fields: Optional[IcatFieldGroup] = None,
+    add_icat_attrs: bool = False,
+):
     if icat_fields is None:
         icat_fields = load_icat_fields()
     nxtreedict = dict()
     for field_name, field_value in metadata.items():
         field = icat_fields.get_field_with_field_name(field_name)
         if field is None:
             logger.warning(f"{field_name} not a valid ICAT field")
@@ -58,10 +62,13 @@
             group = group[name]
             adict = adict.setdefault(name, dict())
             if group.info.NX_class:
                 adict["@NX_class"] = group.info.NX_class
 
         # Add value
         adict[field.name] = as_nxtype(field_value, field.nxtype)
+        if add_icat_attrs:
+            adict[f"{field.name}@icat_field"] = field.field_name
         if field.units:
             adict[f"{field.name}@units"] = field.units
+
     return nxtreedict
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/icat.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/icat.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from . import proc
 from . import tcp
 from ...concurrency import flush_queue
 from ...client.archive import IcatArchiveStatusClient
 from ...client.elogbook import IcatElogbookClient
 from ...client.metadata import IcatMetadataClient
+from ...client.update_metadata import IcatUpdateMetadataClient
+from ...client.add_files import IcatAddFilesClient
 from ...client.main import IcatClient
 
 
 __all__ = [
     # Backends
     "icat_data_dir",
     "cleanup_backend",
@@ -23,24 +25,28 @@
     "activemq_rest_server",
     "icat_backend",
     # Read from the backend
     "icat_subscriber",
     "icat_subscriber_archive",
     "session_icat_logbook_subscriber",
     "icat_logbook_subscriber",
+    "icat_subscriber_update_metadata",
+    "icat_subscriber_add_files",
     # Write to the backend
     "session_icat_publisher",
     "icat_publisher",
     "session_elogbook_client",
     "elogbook_client",
     "session_elogbook_ebs_client",
     "elogbook_ebs_client",
     "icat_metadata_client",
     "icat_archive_client",
     "icat_main_client",
+    "icat_update_metadata_client",
+    "icat_add_files_client",
 ]
 
 
 @pytest.fixture(scope="session")
 def icat_data_dir(tmpdir_factory):
     """Directory where the ICAT dataset backend icat_subscriber can store state."""
     yield tmpdir_factory.mktemp("icat_backend")
@@ -53,15 +59,15 @@
 
 
 @pytest.fixture(scope="session")
 def stomp_server():
     """One of the ICAT backends (for dataset metadata)"""
     port = tcp.get_open_port()
     # Add arguments ["--debug", "TEXT"] for debugging
-    p = subprocess.Popen(["coilmq", "-b", "0.0.0.0", "-p", str(port)])
+    p = subprocess.Popen(["coilmq", "-b", "127.0.0.1", "-p", str(port)])
     tcp.wait_tcp_online("localhost", port)
     try:
         yield "localhost", port
     finally:
         proc.wait_terminate(p)
 
 
@@ -99,14 +105,15 @@
         "metadata_urls": metadata_urls,
         "elogbook_url": elogbook_url,
         "elogbook_token": elogbook_token,
         "metadata_queue_monitor_port": metadata_queue_monitor_port,
         "elogbook_timeout": 5,
         "feedback_timeout": 5,
         "queue_timeout": 5,
+        "add_files_urls": metadata_urls,
     }
     yield icat_servers
 
 
 @pytest.fixture(scope="session")
 def icat_subscriber(stomp_server, icat_data_dir):
     with _icat_subscriber(stomp_server, icat_data_dir, "/queue/icatIngest") as messages:
@@ -117,14 +124,30 @@
 def icat_subscriber_archive(stomp_server, icat_data_dir):
     with _icat_subscriber(
         stomp_server, icat_data_dir, "/queue/icatArchiveRestoreStatus"
     ) as messages:
         yield messages
 
 
+@pytest.fixture(scope="session")
+def icat_subscriber_update_metadata(stomp_server, icat_data_dir):
+    with _icat_subscriber(
+        stomp_server, icat_data_dir, "/queue/icatUpdateDatasetMetadata"
+    ) as messages:
+        yield messages
+
+
+@pytest.fixture(scope="session")
+def icat_subscriber_add_files(stomp_server, icat_data_dir):
+    with _icat_subscriber(
+        stomp_server, icat_data_dir, "/queue/icatDataFiles"
+    ) as messages:
+        yield messages
+
+
 @contextmanager
 def _icat_subscriber(stomp_server, icat_data_dir, queue):
     """Receive messages from the stomp_server backend"""
     with tcp.tcp_message_server() as (port_out, messages):
         host, port = stomp_server
         p = subprocess.Popen(
             [
@@ -293,28 +316,60 @@
     receives everything the ICAT backend receives.
     """
     _, jport = activemq_rest_server
     host, port = stomp_server
     messages = icat_subscriber
     client = IcatMetadataClient(queue_urls=[f"{host}:{port}"], monitor_port=jport)
     yield client, messages
+    client.disconnect()
 
 
 @pytest.fixture()
 def icat_archive_client(
     stomp_server, activemq_rest_server, icat_subscriber_archive, cleanup_backend
 ):
     """Client to update dataset archive/restore status and a queue that
     receives everything the ICAT backend receives.
     """
     _, jport = activemq_rest_server
     host, port = stomp_server
     messages = icat_subscriber_archive
     client = IcatArchiveStatusClient(queue_urls=[f"{host}:{port}"], monitor_port=jport)
     yield client, messages
+    client.disconnect()
+
+
+@pytest.fixture()
+def icat_update_metadata_client(
+    stomp_server, activemq_rest_server, icat_subscriber_update_metadata, cleanup_backend
+):
+    """Client to update dataset sample and a queue that
+    receives everything the ICAT backend receives.
+    """
+    _, jport = activemq_rest_server
+    host, port = stomp_server
+    messages = icat_subscriber_update_metadata
+    client = IcatUpdateMetadataClient(queue_urls=[f"{host}:{port}"], monitor_port=jport)
+    yield client, messages
+    client.disconnect()
+
+
+@pytest.fixture()
+def icat_add_files_client(
+    stomp_server, activemq_rest_server, icat_subscriber_add_files, cleanup_backend
+):
+    """Client to add missing files and a queue that
+    receives everything the ICAT backend receives.
+    """
+    _, jport = activemq_rest_server
+    host, port = stomp_server
+    messages = icat_subscriber_add_files
+    client = IcatAddFilesClient(queue_urls=[f"{host}:{port}"], monitor_port=jport)
+    yield client, messages
+    client.disconnect()
 
 
 @pytest.fixture()
 def icat_main_client(icat_backend, icat_subscriber, cleanup_backend):
     """Client to update dataset archive/restore status and a queue that
     receives everything the ICAT backend receives.
     """
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/proc.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/proc.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/fixtures/tcp.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/tcp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import time
 import json
 import socket
 from contextlib import contextmanager
+
+import xmltodict
+
 from .misc import eprint
-from ...concurrency import gevent, Queue, spawn
+from ...concurrency import Queue
+from ...concurrency import spawn
+from ...concurrency import GEVENT_PATCHED
 
 
 def get_open_port():
     s = socket.socket()
     try:
         s.bind(("", 0))
         return s.getsockname()[1]
@@ -47,44 +52,56 @@
 
     # Listen to this socket
     messages = Queue()
     stop = False
 
     def listener():
         buffer = b""
-        while True:
-            try:
-                conn, addr = sock.accept()
-                break
-            except socket.timeout:
+        conn = None
+        try:
+            while True:
+                try:
+                    conn, addr = sock.accept()
+                    break
+                except socket.timeout:
+                    time.sleep(0.1)
+            while True:
+                try:
+                    buffer += conn.recv(16384)
+                except socket.timeout:
+                    pass
+                if buffer:
+                    out, sep, buffer = buffer.rpartition(b"\n")
+                    if sep:
+                        for bdata in out.split(b"\n"):
+                            if data_parser == "json":
+                                messages.put(json.loads(bdata))
+                            elif b'xmlns:tns="http://www.esrf.fr/icat"' in bdata:
+                                data = xmltodict.parse(
+                                    bdata.decode(),
+                                    process_namespaces=True,
+                                    namespaces={"http://www.esrf.fr/icat": None},
+                                )
+                                messages.put(data)
+                            else:
+                                messages.put(bdata.decode())
+                if stop:
+                    return
                 time.sleep(0.1)
-        while True:
-            try:
-                buffer += conn.recv(16384)
-            except socket.timeout:
-                pass
-            if buffer:
-                out, sep, buffer = buffer.rpartition(b"\n")
-                if sep:
-                    for bdata in out.split(b"\n"):
-                        if data_parser == "json":
-                            messages.put(json.loads(bdata))
-                        else:
-                            messages.put(bdata.decode())
-            if stop:
-                return
-            time.sleep(0.1)
+        finally:
+            if conn is not None:
+                conn.close()
 
     glistener = spawn(listener)
     try:
         yield port, messages
     finally:
         messages.put(StopIteration)
         stop = True
         if validate_all:
             for msg in iter(messages.get, StopIteration):
                 eprint(f"Unvalidated message: {msg}")
-        if gevent:
+        if GEVENT_PATCHED:
             glistener.kill()
         else:
             glistener.join()
         sock.close()
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/activemq_rest_server.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/activemq_rest_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import sys
 import time
-from datetime import datetime, timedelta
+import datetime
 import socketserver
 import logging
 
-from pyicat_plus.tests.servers.utils import basic_config
-from pyicat_plus.tests.servers.utils import ReuseAddrTCPServer
-
+from .utils import ReuseAddrTCPServer
+from ...utils.log_utils import basic_config
 
 logger = logging.getLogger("ACTIVEMQ REST SERVER")
-basic_config(
-    logger=logger,
-    level=logging.DEBUG,
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-)
-logger.addHandler(logging.StreamHandler(sys.stdout))
+
+ICAT_QUEUES = [
+    "icatIngest",
+    "icatArchiveRestoreStatus",
+    "icatUpdateDatasetMetadata",
+    "icatDataFiles",
+]
 
 
 class MyTCPRequestHandler(socketserver.StreamRequestHandler):
     def handle(self):
         request = self._read_request()
-        queues = ["icatIngest", "icatArchiveRestoreStatus"]
         expected_requests = list(
             map(
                 lambda q: f"GET /api/jolokia/read/org.apache.activemq:type=Broker,brokerName=metadata,destinationType=Queue,destinationName={q}/ConsumerCount".encode(
                     "utf-8"
                 ),
-                queues,
+                ICAT_QUEUES,
             )
         )
         if len([e for e in expected_requests if e in request]) > 0:
             logger.info(f"Send response to {self.client_address[0]}")
             self._send_response()
         elif request:
             logger.info(f"Unknown request\n {request}")
@@ -43,16 +41,16 @@
             n = self.rfile.readinto1(buff)
             request = bytes(buff[0:n])
         except Exception as e:
             raise RuntimeError("Error reading request") from e
         return request
 
     def _send_response(self):
-        now = datetime.now().astimezone()
-        t1 = now + timedelta(hours=5)
+        now = datetime.datetime.now().astimezone()
+        t1 = now + datetime.timedelta(hours=5)
         out = (
             b"HTTP/1.1 200 OK\r\nContent-Type: text/plain;charset=UTF-8\r\nCache-Control: no-cache\r\nPragma: no-cache\r\nDate: "
             + now.strftime("%a, %d %b %Y %H:%M:%S GTM").encode()
             + b"\r\nExpires: "
             + t1.strftime("%a, %d %b %Y %H:%M:%S GTM").encode()
             + b'\r\nConnection: close\r\nServer: Jetty(7.6.9.v20130131)\r\n\r\n{"timestamp":'
             + str(int(time.time())).encode()
@@ -72,11 +70,17 @@
     finally:
         logger.info("Exit.")
 
 
 if __name__ == "__main__":
     import argparse
 
+    basic_config(
+        logger=logger,
+        level=logging.DEBUG,
+        format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    )
+
     parser = argparse.ArgumentParser(description="ActiveMQ REST server")
     parser.add_argument("--port", default=8778, type=int, help="server port")
     args = parser.parse_args()
     main(port=args.port)
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/icat_db.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icat_db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,138 @@
 import os
 import json
 import logging
-from datetime import datetime
-from typing import Optional, Dict, List
+import datetime
+from glob import glob
+from contextlib import contextmanager
+from typing import Optional, Dict, List, Generator
 
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("STOMP SUBSCRIBER")
 
 
 class IcatDb:
     def __init__(self, root_dir: Optional[str] = None):
         if root_dir is None:
             root_dir = "."
         if root_dir:
             os.makedirs(root_dir, exist_ok=True)
         self._root_dir = root_dir
         self._investigations = os.path.join(root_dir, "investigations.json")
 
     def start_investigation(self, investigation: dict) -> None:
         investigation["instrument"] = {"name": investigation["instrument"]}
+        investigation["proposal"] = investigation["experiment"]
         _add_table(self._investigations, investigation)
 
     def store_dataset(self, dataset: dict) -> None:
         investigation = _find_data(self._investigations, dataset["startDate"])
         if investigation is None:
             logger.error(
                 "Dataset not stored because no investigation found: %s", dataset
             )
             return
         filename = os.path.join(self._root_dir, f"datasets{investigation['id']}.json")
+        dataset["id"] = self._get_next_dataset_id()
         _add_table(filename, dataset)
 
+    @contextmanager
+    def update_dataset(self, dataset_id: int) -> Generator[dict, None, None]:
+        for filename in glob(os.path.join(self._root_dir, "datasets*.json")):
+            data = _get_row(filename, dataset_id)
+            if data is None:
+                continue
+            yield data
+            _edit_table(filename, data)
+            break
+        else:
+            yield
+
     def get_investigations(self, instrument: str, experiment: str) -> List[Dict]:
         return [
             investigation
             for investigation in _read_table(self._investigations)
             if experiment == investigation["experiment"]
             and instrument == investigation["instrument"]["name"]
         ]
 
     def get_datasets(self, investigation_id) -> List[Dict]:
         filename = os.path.join(self._root_dir, f"datasets{investigation_id}.json")
         return _read_table(filename)
 
+    def _get_next_dataset_id(self) -> int:
+        max_ids = [
+            _get_max_id(filename)
+            for filename in glob(os.path.join(self._root_dir, "datasets*.json"))
+        ]
+        if max_ids:
+            return max(max_ids) + 1
+        return 0
+
 
 def _read_table(filename: str) -> List[dict]:
     if not os.path.isfile(filename):
         return list()
     with open(filename, "r") as f:
         return json.load(f)
 
 
-def _update_table(filename: str, data: dict) -> Dict:
+def _write_table(filename: str, data: dict) -> Dict:
     with open(filename, "w") as f:
         json.dump(data, f)
     logger.info("Metadata in %s updated", filename)
 
 
-def _add_table(filename: str, data: dict) -> int:
+def _add_table(filename: str, data: dict) -> None:
     table = _read_table(filename)
-    if table:
-        data_id = max(row["id"] for row in table) + 1
-    else:
-        data_id = 0
-    data = dict(data)
-    data["id"] = data_id
+    if "id" not in data:
+        if table:
+            data_id = max(row["id"] for row in table) + 1
+        else:
+            data_id = 0
+        data = dict(data)
+        data["id"] = data_id
     table.append(data)
     logger.info("Add metadata to %s: %s", filename, data)
-    _update_table(filename, table)
-    return data_id
+    _write_table(filename, table)
+
+
+def _edit_table(filename: str, data: dict) -> None:
+    table = _read_table(filename)
+    for row in table:
+        if row["id"] == data["id"]:
+            logger.info("Edit metadata of %s: %s", filename, data)
+            row.update(data)
+            _write_table(filename, table)
+            break
+    else:
+        _add_table(filename, data)
+
+
+def _get_row(filename: str, dataset_id: int) -> Optional[dict]:
+    table = _read_table(filename)
+    for row in table:
+        if row["id"] == dataset_id:
+            return row
+
+
+def _get_max_id(filename: str) -> int:
+    table = _read_table(filename)
+    if table:
+        return max(row["id"] for row in table)
+    return -1
 
 
 def _find_data(filename: str, date: str) -> Optional[Dict]:
-    date = datetime.fromisoformat(date).astimezone()
+    date = datetime.datetime.fromisoformat(date).astimezone()
     for data in _read_table(filename):
-        start_date = datetime.fromisoformat(data["startDate"]).astimezone()
+        start_date = datetime.datetime.fromisoformat(data["startDate"]).astimezone()
         end_date = data.get("endDate")
         if end_date is None:
             # infinite timeslot
             inside_timeslot = date >= start_date
         else:
             # finite timeslot
-            end_date = datetime.fromisoformat(end_date).astimezone()
+            end_date = datetime.datetime.fromisoformat(end_date).astimezone()
             inside_timeslot = date >= start_date and date <= end_date
         if inside_timeslot:
             return data
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/icatplus_server.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icatplus_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,19 @@
 import re
 import socket
 import json
 import http.server
 import logging
 from typing import Iterator, Tuple, Optional
 
-from pyicat_plus.tests.servers.utils import ReuseAddrTCPServer
-from pyicat_plus.tests.servers.utils import basic_config
-from pyicat_plus.tests.servers.icat_db import IcatDb
+from .icat_db import IcatDb
+from .utils import ReuseAddrTCPServer
+from ...utils.log_utils import basic_config
 
 logger = logging.getLogger("ICATPLUS SERVER")
-basic_config(
-    logger=logger,
-    level=logging.DEBUG,
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-)
 
 
 class MyTCPRequestHandler(http.server.BaseHTTPRequestHandler):
     def __init__(self, *args, s_out=None, icat_data_dir: Optional[str] = None, **kw):
         self.s_out = s_out
         self.icatdb = IcatDb(icat_data_dir)
         super().__init__(*args, **kw)
@@ -236,20 +231,28 @@
     if port_out:
         logger.info(f"Redirect received messages to port {port_out}")
         s_out.sendall(json.dumps({"STATUS": "LISTENING"}).encode() + b"\n")
     try:
         logger.info("CTRL-C to stop")
         aServer.serve_forever()
     finally:
+        if port_out:
+            s_out.close()
         logger.info("Exit.")
 
 
 if __name__ == "__main__":
     import argparse
 
+    basic_config(
+        logger=logger,
+        level=logging.DEBUG,
+        format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    )
+
     parser = argparse.ArgumentParser(description="ICAT plus server")
     parser.add_argument("--port", default=8443, type=int, help="server port")
     parser.add_argument("--port_out", default=0, type=int, help="output socket")
     parser.add_argument(
         "--icat_data_dir", default=None, type=str, help="One file per dataset"
     )
     args = parser.parse_args()
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/stomp_publisher.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_publisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import socket
 import logging
 from stompest.config import StompConfig
 from stompest.protocol import StompSpec
 from stompest.sync import Stomp
 
-from pyicat_plus.tests.servers.utils import basic_config
+from ...utils.log_utils import basic_config
 
 logger = logging.getLogger("STOMP PUBLISHER")
-basic_config(
-    logger=logger,
-    level=logging.DEBUG,
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-)
 
 
 def read_socket(host, port):
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.connect((host, port))
     buffer = b""
     try:
@@ -55,14 +50,20 @@
             body = input(f"Message to send to '{queue}': ")
             client.send(queue, body=body.encode(), headers=header)
 
 
 if __name__ == "__main__":
     import argparse
 
+    basic_config(
+        logger=logger,
+        level=logging.DEBUG,
+        format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    )
+
     parser = argparse.ArgumentParser(
         description="Redirect socket input to a STOMP queue"
     )
     parser.add_argument(
         "--host", default="localhost", type=str, help="STOMP server host"
     )
     parser.add_argument("--port", default=60001, type=int, help="STOMP server port")
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/stomp_subscriber.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_subscriber.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-import stomp
+import os
 import json
 import socket
 import logging
 import threading
 from enum import Enum
 from typing import Optional
 from json.decoder import JSONDecodeError
 
+import stomp
 import xmltodict
 from xml.parsers.expat import ExpatError
 
-from pyicat_plus.tests.servers.utils import basic_config
-from pyicat_plus.tests.servers.icat_db import IcatDb
+from .icat_db import IcatDb
+from ...utils.log_utils import basic_config
+from .activemq_rest_server import ICAT_QUEUES
 
 logger = logging.getLogger("STOMP SUBSCRIBER")
-basic_config(
-    logger=logger,
-    level=logging.DEBUG,
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-)
 
-MessageType = Enum("MessageType", "investigation dataset archiving unknown")
+MessageType = Enum("MessageType", "investigation dataset archiving addfiles unknown")
 
 
 class MyListener(stomp.ConnectionListener):
     def __init__(self, conn, icat_data_dir: Optional[str] = None):
         self.conn = conn
         self.s_out = None
         self.icatdb = IcatDb(icat_data_dir)
@@ -35,52 +32,64 @@
             self.s_out.close()
         self.s_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.s_out.connect(("localhost", port))
         logger.info(f"Redirect received messages to port {port}")
 
     def on_message(self, frame):
         message = frame.body
-        logger.info(f"received message:\n {message}")
+        logger.info("received message:\n %s", message)
 
         message_type = None
         try:
             message = xmltodict.parse(
                 message,
                 process_namespaces=True,
                 namespaces={"http://www.esrf.fr/icat": None},
             )
         except ExpatError:
             try:
                 message = json.loads(message)
             except JSONDecodeError:
                 message_type = MessageType.unknown
             else:
-                message_type = MessageType.archiving
+                keys = set(message)
+                if keys == {"datasetId", "type", "level", "message"}:
+                    message_type = MessageType.archiving
+                elif keys == {"datasetId"}:
+                    message_type = MessageType.addfiles
+                else:
+                    message_type = MessageType.unknown
         else:
             if "investigation" in message:
                 message_type = MessageType.investigation
             elif "dataset" in message:
                 message_type = MessageType.dataset
 
+        logger.info("parsed message (%s):\n %s", message_type, message)
+
         # Only access specific destinations
         header = frame.headers
-        if header.get("destination") not in [
-            "/queue/icatIngest",
-            "/queue/icatArchiveRestoreStatus",
-        ]:
+        icat_queues = ["/queue/" + q for q in ICAT_QUEUES]
+        if header.get("destination") not in icat_queues:
             return
 
         # Only accept valid proposals
         if message_type in (message_type.investigation, message_type.dataset):
             if message_type is message_type.investigation:
                 data = message["investigation"]
                 proposal = data["experiment"]
             else:
                 data = message["dataset"]
                 proposal = data["investigation"]
+                # Convert to backend format
+                file_count = 0
+                if os.path.exists(data["location"]):
+                    file_count = len(os.listdir(data["location"]))
+                data["parameter"].append({"name": "__fileCount", "value": file_count})
+                data["parameters"] = data.pop("parameter")
             if "666" in proposal:
                 logger.info(
                     "Do not register %s for invalid proposal '%s'",
                     message_type,
                     proposal,
                 )
                 return
@@ -88,14 +97,37 @@
         # Store data
         if message_type in (message_type.investigation, message_type.dataset):
             if message_type is message_type.investigation:
                 self.icatdb.start_investigation(data)
             else:
                 self.icatdb.store_dataset(data)
 
+        if message_type == message_type.addfiles:
+            dataset_id = message["datasetId"]
+            with self.icatdb.update_dataset(dataset_id) as data:
+                if data is None:
+                    logger.error("datasetId %s does not exist", dataset_id)
+                else:
+                    file_count = 0
+                    dirname = data["location"]
+                    if os.path.exists(dirname):
+                        file_count = len(os.listdir(dirname))
+                    for parameter in data["parameters"]:
+                        if parameter["name"] == "__fileCount":
+                            logger.info(
+                                "Update file count for %s to %d", dirname, file_count
+                            )
+                            parameter["value"] = file_count
+                            break
+                    else:
+                        logger.info("Add file count for %s to %d", dirname, file_count)
+                        data["parameters"].append(
+                            {"name": "__fileCount", "value": file_count}
+                        )
+
         # Notify that data is valid
         if self.s_out is not None:
             self.s_out.sendall(frame.body.encode() + b"\n")
 
 
 def main(
     host=None, port=60001, queue=None, port_out=0, icat_data_dir: Optional[str] = None
@@ -120,14 +152,20 @@
     finally:
         logger.info("Exit.")
 
 
 if __name__ == "__main__":
     import argparse
 
+    basic_config(
+        logger=logger,
+        level=logging.DEBUG,
+        format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    )
+
     parser = argparse.ArgumentParser(
         description="STOMP client which subscribes to a STOMP queue and redirect its output to a socket"
     )
     parser.add_argument(
         "--host", default="localhost", type=str, help="STOMP server host"
     )
     parser.add_argument("--port", default=60001, type=int, help="STOMP server port")
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/servers/utils.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/log_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import sys
 import logging
-import socketserver
+from typing import Optional
 
 
-def basic_config(logger=None, level=None, format=None):
+def basic_config(
+    logger: Optional[logging.Logger] = None,
+    level: Optional[int] = None,
+    format: Optional[str] = None,
+) -> None:
     """
     :param logger: root logger when not provided
     :param level: logger log level
     :param str format:
     """
     if logger is None:
         logger = logging.getLogger()
     if level is not None:
         logger.setLevel(level)
-    if format:
-        formatter = logging.Formatter(format)
-    else:
-        formatter = None
+
+    threshold_level = logging.WARNING
 
     class StdOutFilter(logging.Filter):
         def filter(self, record):
-            return record.levelno < logging.WARNING
+            return record.levelno < threshold_level
 
     class StdErrFilter(logging.Filter):
         def filter(self, record):
-            return record.levelno >= logging.WARNING
+            return record.levelno >= threshold_level
 
-    h = logging.StreamHandler(sys.stdout)
-    h.addFilter(StdOutFilter())
-    h.setLevel(logging.DEBUG)
-    if formatter is not None:
-        h.setFormatter(formatter)
-    logger.addHandler(h)
-
-    h = logging.StreamHandler(sys.stderr)
-    h.addFilter(StdErrFilter())
-    h.setLevel(logging.WARNING)
-    if formatter is not None:
-        h.setFormatter(formatter)
-    logger.addHandler(h)
+    stdout_handler = logging.StreamHandler(sys.stdout)
+    stdout_handler.addFilter(StdOutFilter())
+    stdout_handler.setLevel(logging.DEBUG)
+    logger.addHandler(stdout_handler)
+
+    stderr_handler = logging.StreamHandler(sys.stderr)
+    stderr_handler.addFilter(StdErrFilter())
+    stderr_handler.setLevel(threshold_level)
+    logger.addHandler(stderr_handler)
 
-
-class ReuseAddrTCPServer(socketserver.TCPServer):
-    allow_reuse_address = True
+    if format:
+        formatter = logging.Formatter(format)
+        stdout_handler.setFormatter(formatter)
+        stderr_handler.setFormatter(formatter)
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_cli.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import xml.etree.ElementTree as etree
 from ..apps import store_raw
 from ..apps import store_processed
+from .utils.message import assert_dataset_message
 
 
 def test_store_raw(icat_metadata_client, icat_backend):
     _, messages = icat_metadata_client
 
     argv = [
         "",
@@ -24,30 +24,84 @@
         "field2=[1, 2, 3]",
         "--queue",
         icat_backend["metadata_urls"][0],
     ]
     store_raw.main(argv)
 
     message = messages.get(timeout=10)
+    assert messages.empty()
 
-    root = etree.fromstring(message)
-    names = {child.tag.replace("{http://www.esrf.fr/icat}", "") for child in root}
     expected = {
-        "endDate",
-        "location",
-        "startDate",
-        "parameter",
-        "sample",
-        "investigation",
-        "instrument",
-        "name",
+        "dataset": {
+            "@complete": "true",
+            "@xmlns": {"tns": "http://www.esrf.fr/icat"},
+            "instrument": "id00",
+            "investigation": "hg123",
+            "location": "/path/of/dataset",
+            "name": "datasetname",
+            "parameter": [
+                {"name": "field1", "value": "value1"},
+                {"name": "field2", "value": "1,2,3"},
+                {"name": "Sample_name", "value": "samplename"},
+            ],
+            "sample": {"name": "samplename"},
+        }
     }
-    assert names == expected
+    assert_dataset_message(message, expected)
+
+
+def test_store_raw_metadatafile(icat_metadata_client, icat_backend, tmpdir):
+    metadatafile = str(tmpdir / "metadata.txt")
+
+    with open(metadatafile, "w") as f:
+        f.write("field1=value1\n")
+        f.write("field2=[1, 2, 3]\n")
+
+    _, messages = icat_metadata_client
+
+    argv = [
+        "",
+        "--beamline",
+        "id00",
+        "--proposal",
+        "hg123",
+        "--dataset",
+        "datasetname",
+        "--path",
+        "/path/of/dataset",
+        "--sample",
+        "samplename",
+        "--metadatafile",
+        metadatafile,
+        "--queue",
+        icat_backend["metadata_urls"][0],
+    ]
+    store_raw.main(argv)
+
+    message = messages.get(timeout=10)
     assert messages.empty()
 
+    expected = {
+        "dataset": {
+            "@complete": "true",
+            "@xmlns": {"tns": "http://www.esrf.fr/icat"},
+            "instrument": "id00",
+            "investigation": "hg123",
+            "location": "/path/of/dataset",
+            "name": "datasetname",
+            "parameter": [
+                {"name": "field1", "value": "value1"},
+                {"name": "field2", "value": "1,2,3"},
+                {"name": "Sample_name", "value": "samplename"},
+            ],
+            "sample": {"name": "samplename"},
+        }
+    }
+    assert_dataset_message(message, expected)
+
 
 def test_store_processed(icat_metadata_client, icat_backend):
     _, messages = icat_metadata_client
 
     argv = [
         "",
         "--beamline",
@@ -69,23 +123,31 @@
         "--raw",
         "/path/of/dataset1",
         "--raw",
         "/path/of/dataset2",
     ]
     store_processed.main(argv)
 
-    message = messages.get(timeout=10)
-
-    root = etree.fromstring(message)
-    names = {child.tag.replace("{http://www.esrf.fr/icat}", "") for child in root}
     expected = {
-        "endDate",
-        "location",
-        "startDate",
-        "parameter",
-        "sample",
-        "investigation",
-        "instrument",
-        "name",
+        "dataset": {
+            "@complete": "true",
+            "@xmlns": {"tns": "http://www.esrf.fr/icat"},
+            "instrument": "id00",
+            "investigation": "hg123",
+            "location": "/path/of/processed",
+            "name": "datasetname",
+            "parameter": [
+                {"name": "field1", "value": "value1"},
+                {"name": "field2", "value": "1,2,3"},
+                {"name": "Sample_name", "value": "samplename"},
+                {
+                    "name": "input_datasets",
+                    "value": "/path/of/dataset1,/path/of/dataset2",
+                },
+            ],
+            "sample": {"name": "samplename"},
+        }
     }
-    assert names == expected
+    message = messages.get(timeout=10)
     assert messages.empty()
+
+    assert_dataset_message(message, expected)
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_elogbook.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_archive.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_archive.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_datasets.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
-import xml.etree.ElementTree as etree
+
 from ..concurrency import Empty
+from .utils.message import assert_dataset_message
+from .utils.message import assert_investigation_message
 
 
 def test_start_investigation(icat_metadata_client):
     client, messages = icat_metadata_client
     client.check_health()
     client.start_investigation(proposal="hg123", beamline="id00")
     message = messages.get(timeout=10)
-
-    root = etree.fromstring(message)
-    names = {child.tag.replace("{http://www.esrf.fr/icat}", "") for child in root}
-    expected = {"startDate", "experiment", "instrument"}
-    assert names == expected
     assert messages.empty()
 
+    expected = {"investigation": {"experiment": "hg123", "instrument": "id00"}}
+    assert_investigation_message(message, expected)
+
 
 def test_start_bad_investigation(icat_metadata_client):
     client, messages = icat_metadata_client
     client.check_health()
     client.start_investigation(proposal="hg666", beamline="id00")
     with pytest.raises(Empty):
         messages.get(timeout=2)
@@ -30,29 +30,33 @@
         proposal="hg123",
         beamline="id00",
         dataset="datasetname",
         path="/path-of-dataset",
         metadata={"Sample_name": "samplename", "field1": "value1", "field2": [1, 2, 3]},
     )
     message = messages.get(timeout=10)
+    assert messages.empty()
 
-    root = etree.fromstring(message)
-    names = {child.tag.replace("{http://www.esrf.fr/icat}", "") for child in root}
     expected = {
-        "endDate",
-        "location",
-        "startDate",
-        "parameter",
-        "sample",
-        "investigation",
-        "instrument",
-        "name",
+        "dataset": {
+            "@complete": "true",
+            "@xmlns": {"tns": "http://www.esrf.fr/icat"},
+            "instrument": "id00",
+            "investigation": "hg123",
+            "location": "/path-of-dataset",
+            "name": "datasetname",
+            "parameter": [
+                {"name": "Sample_name", "value": "samplename"},
+                {"name": "field1", "value": "value1"},
+                {"name": "field2", "value": "1,2,3"},
+            ],
+            "sample": {"name": "samplename"},
+        }
     }
-    assert names == expected
-    assert messages.empty()
+    assert_dataset_message(message, expected)
 
 
 def test_send_metadata_via_file(icat_metadata_client, tmpdir):
     store_filename = tmpdir / "test.xml"
 
     client, messages = icat_metadata_client
     client.store_metadata(
@@ -68,29 +72,33 @@
         message = messages.get(timeout=1)
 
     assert store_filename.exists()
 
     client.send_metadata_from_file(str(store_filename))
 
     message = messages.get(timeout=10)
+    assert messages.empty()
 
-    root = etree.fromstring(message)
-    names = {child.tag.replace("{http://www.esrf.fr/icat}", "") for child in root}
     expected = {
-        "endDate",
-        "location",
-        "startDate",
-        "parameter",
-        "sample",
-        "investigation",
-        "instrument",
-        "name",
+        "dataset": {
+            "@complete": "true",
+            "@xmlns": {"tns": "http://www.esrf.fr/icat"},
+            "instrument": "id00",
+            "investigation": "hg123",
+            "location": "/path-of-dataset",
+            "name": "datasetname",
+            "parameter": [
+                {"name": "Sample_name", "value": "samplename"},
+                {"name": "field1", "value": "value1"},
+                {"name": "field2", "value": "1,2,3"},
+            ],
+            "sample": {"name": "samplename"},
+        }
     }
-    assert names == expected
-    assert messages.empty()
+    assert_dataset_message(message, expected)
 
 
 def test_send_missing_data(icat_metadata_client):
     client, messages = icat_metadata_client
     with pytest.raises(AssertionError, match="ICAT requires the beamline name"):
         client.send_metadata(
             proposal=None,
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_definitions.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_nexus.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_nexus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-from ..metadata.nexus import create_nxtreedict
-from .utils.compare import deep_compare
+import h5py
 
+from .utils.compare import deep_compare
+from ..metadata.nexus import create_nxtreedict
+from ..apps.icat_as_nexus import save_icat_as_nexus
 
-def test_icat_metadata_to_nexus(icat_fields):
-    metadict = dict()
-
-    def getter(key):
-        nonlocal metadict
-        return metadict[key]
-
-    def setter(key, value):
-        nonlocal metadict
-        metadict[key] = value
 
-    metadata = icat_fields.namespace(getter=getter, setter=setter)
+def test_icat_metadata_to_nexus(icat_namespace):
+    icat_fields, metadata, metadict = icat_namespace
 
     metadata.instrument.detector01.name = "diode1"
     metadata.instrument.detector02.name = "diode2"
 
     metadata.instrument.variables.name = ["roby", "robz"]
     metadata.instrument.variables.value = [0, 0]
 
@@ -34,15 +27,15 @@
     metadata.sample.positioners.name = "roby"
     metadata.sample.positioners.value = 0
 
     metadata.FLUO.i0 = 1
     metadata.FLUO.measurement.i0_start = 0.5
     metadata.definition = "FLUO"
 
-    nxtreedict = create_nxtreedict(metadict, icat_fields)
+    nxtreedict = create_nxtreedict(metadict, icat_fields=icat_fields)
     expected = {
         "@NX_class": "NXentry",
         "FLUO": {
             "@NX_class": "NXsubentry",
             "i0": 1.0,
             "measurement": {
                 "@NX_class": "NXcollection",
@@ -80,7 +73,53 @@
             "@NX_class": "NXsample",
             "name": "sample",
             "positioners": {"@NX_class": "NXpositioner", "name": "roby", "value": 0},
         },
         "definition": "FLUO",
     }
     deep_compare(nxtreedict, expected)
+
+
+def test_icat_metadata_to_hdf5(tmpdir):
+    filename = str(tmpdir / "test.h5")
+    save_icat_as_nexus(filename)
+
+    with h5py.File(filename, "r") as f:
+        assert set(f) == {"entryname"}
+        entry = f["entryname"]
+        top_level_names = {
+            "BCDI",
+            "EM",
+            "FLUO",
+            "HOLO",
+            "HTXRPD",
+            "MRT",
+            "MX",
+            "PTYCHO",
+            "SAXS",
+            "SXDM",
+            "TOMO",
+            "WAXS",
+            "aperture",
+            "dataset_type",
+            "definition",
+            "doi_abstract",
+            "doi_title",
+            "doi_users",
+            "end_time",
+            "external_references",
+            "folder_path",
+            "fresnel_zone_plate",
+            "instrument",
+            "mirror",
+            "notes",
+            "process",
+            "project_name",
+            "proposal",
+            "sample",
+            "scanNumber",
+            "start_time",
+            "technique_pid",
+            "title",
+            "workflow",
+        }
+        assert set(entry) == top_level_names
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_icat_serialize.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from datetime import datetime
+import datetime
 from ..client.serialize import serialize_metadata
 
 
 def test_icat_serialize_valid_data():
     assert serialize_metadata(None) is None
     assert serialize_metadata("string") == "string"
     assert serialize_metadata(b"string") == "string"
@@ -20,15 +20,15 @@
     assert serialize_metadata({"key": b"string"}) == {"key": "string"}
     assert serialize_metadata({"key": 123.456}) == {"key": "123.456"}
     assert serialize_metadata({"key": []}) == {"key": ""}
     assert serialize_metadata({"key": [None]}) == {"key": ""}
     assert serialize_metadata({"key": [1, 2]}) == {"key": "1,2"}
     assert serialize_metadata({"key": [[1, 2], [3, 4]]}) == {"key": "1,2 3,4"}
 
-    now = datetime.now().astimezone()
+    now = datetime.datetime.now().astimezone()
     assert serialize_metadata({"key": now}) == {"key": now.isoformat()}
 
 
 def test_icat_serialize_invalid_data():
     invalid_data = ([{}], [[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
     for data in invalid_data:
         with pytest.raises((TypeError, ValueError)):
```

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/test_url_utils.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/tests/utils/compare.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/utils/maxsizedict.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/maxsizedict.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus/utils/url.py` & `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.8b0/src/pyicat_plus.egg-info/SOURCES.txt` & `pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/pyicat_plus/__init__.py
+src/pyicat_plus/concurrency.py
 src/pyicat_plus.egg-info/PKG-INFO
 src/pyicat_plus.egg-info/SOURCES.txt
 src/pyicat_plus.egg-info/dependency_links.txt
 src/pyicat_plus.egg-info/entry_points.txt
 src/pyicat_plus.egg-info/requires.txt
 src/pyicat_plus.egg-info/top_level.txt
 src/pyicat_plus/apps/__init__.py
+src/pyicat_plus/apps/icat_as_nexus.py
 src/pyicat_plus/apps/store_from_file.py
 src/pyicat_plus/apps/store_processed.py
 src/pyicat_plus/apps/store_raw.py
 src/pyicat_plus/apps/sync_raw.py
 src/pyicat_plus/client/__init__.py
+src/pyicat_plus/client/add_files.py
 src/pyicat_plus/client/archive.py
 src/pyicat_plus/client/bliss.py
 src/pyicat_plus/client/defaults.py
 src/pyicat_plus/client/elogbook.py
 src/pyicat_plus/client/interface.py
 src/pyicat_plus/client/investigation.py
 src/pyicat_plus/client/main.py
 src/pyicat_plus/client/messaging.py
 src/pyicat_plus/client/metadata.py
 src/pyicat_plus/client/null.py
 src/pyicat_plus/client/serialize.py
+src/pyicat_plus/client/update_metadata.py
 src/pyicat_plus/client/xmlns.py
-src/pyicat_plus/concurrency/__init__.py
-src/pyicat_plus/concurrency/query_pool/__init__.py
-src/pyicat_plus/concurrency/query_pool/gevent.py
-src/pyicat_plus/concurrency/query_pool/threading.py
 src/pyicat_plus/metadata/__init__.py
 src/pyicat_plus/metadata/definitions.py
 src/pyicat_plus/metadata/namespace_wrapper.py
 src/pyicat_plus/metadata/nexus.py
 src/pyicat_plus/tests/__init__.py
 src/pyicat_plus/tests/conftest.py
 src/pyicat_plus/tests/test_cli.py
 src/pyicat_plus/tests/test_elogbook.py
+src/pyicat_plus/tests/test_icat_add_files.py
 src/pyicat_plus/tests/test_icat_archive.py
 src/pyicat_plus/tests/test_icat_datasets.py
 src/pyicat_plus/tests/test_icat_definitions.py
 src/pyicat_plus/tests/test_icat_investigations.py
 src/pyicat_plus/tests/test_icat_mockup.py
 src/pyicat_plus/tests/test_icat_nexus.py
 src/pyicat_plus/tests/test_icat_serialize.py
 src/pyicat_plus/tests/test_icat_sync.py
+src/pyicat_plus/tests/test_icat_update_metadata.py
 src/pyicat_plus/tests/test_maxsizedict.py
-src/pyicat_plus/tests/test_query_pool.py
+src/pyicat_plus/tests/test_namespace.py
 src/pyicat_plus/tests/test_url_utils.py
 src/pyicat_plus/tests/fixtures/__init__.py
 src/pyicat_plus/tests/fixtures/icat.py
 src/pyicat_plus/tests/fixtures/misc.py
 src/pyicat_plus/tests/fixtures/proc.py
 src/pyicat_plus/tests/fixtures/tcp.py
 src/pyicat_plus/tests/servers/__init__.py
@@ -61,10 +63,16 @@
 src/pyicat_plus/tests/servers/icat_db.py
 src/pyicat_plus/tests/servers/icatplus_server.py
 src/pyicat_plus/tests/servers/stomp_publisher.py
 src/pyicat_plus/tests/servers/stomp_subscriber.py
 src/pyicat_plus/tests/servers/utils.py
 src/pyicat_plus/tests/utils/__init__.py
 src/pyicat_plus/tests/utils/compare.py
+src/pyicat_plus/tests/utils/message.py
 src/pyicat_plus/utils/__init__.py
+src/pyicat_plus/utils/log_utils.py
 src/pyicat_plus/utils/maxsizedict.py
+src/pyicat_plus/utils/path_utils.py
+src/pyicat_plus/utils/raw_data.py
+src/pyicat_plus/utils/sync_store.py
+src/pyicat_plus/utils/sync_types.py
 src/pyicat_plus/utils/url.py
```

