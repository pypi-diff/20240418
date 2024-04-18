# Comparing `tmp/yamcs-client-1.9.5.tar.gz` & `tmp/yamcs_client-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs-client-1.9.5.tar", last modified: Mon Mar 25 16:16:22 2024, max compression
+gzip compressed data, was "yamcs_client-1.9.6.tar", last modified: Thu Apr 18 08:39:38 2024, max compression
```

## Comparing `yamcs-client-1.9.5.tar` & `yamcs_client-1.9.6.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.759535 yamcs-client-1.9.5/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs-client-1.9.5/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs-client-1.9.5/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-03-25 16:16:22.759286 yamcs-client-1.9.5/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs-client-1.9.5/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-03-25 16:16:22.759583 yamcs-client-1.9.5/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs-client-1.9.5/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.691738 yamcs-client-1.9.5/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.693585 yamcs-client-1.9.5/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.695044 yamcs-client-1.9.5/src/yamcs/api/
--rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/api/annotations_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/api/exception_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/api/httpbody_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/api/websocket_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.695916 yamcs-client-1.9.5/src/yamcs/archive/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/archive/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-03-25 12:07:53.000000 yamcs-client-1.9.5/src/yamcs/archive/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     8486 2024-02-24 16:12:05.000000 yamcs-client-1.9.5/src/yamcs/archive/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.696723 yamcs-client-1.9.5/src/yamcs/client/
--rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs-client-1.9.5/src/yamcs/client/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs-client-1.9.5/src/yamcs/client/activities.py
--rw-r--r--   0 fdi        (503) staff       (20)    24029 2024-03-01 16:53:25.000000 yamcs-client-1.9.5/src/yamcs/client/core.py
--rw-r--r--   0 fdi        (503) staff       (20)       22 2024-03-25 16:08:17.000000 yamcs-client-1.9.5/src/yamcs/clientversion.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.698637 yamcs-client-1.9.5/src/yamcs/core/
--rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/core/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-03-01 16:04:02.000000 yamcs-client-1.9.5/src/yamcs/core/auth.py
--rw-r--r--   0 fdi        (503) staff       (20)     4665 2024-02-25 21:21:09.000000 yamcs-client-1.9.5/src/yamcs/core/context.py
--rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/core/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs-client-1.9.5/src/yamcs/core/futures.py
--rw-r--r--   0 fdi        (503) staff       (20)    12930 2024-03-18 16:14:31.000000 yamcs-client-1.9.5/src/yamcs/core/helpers.py
--rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs-client-1.9.5/src/yamcs/core/pagination.py
--rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs-client-1.9.5/src/yamcs/core/subscriptions.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.699368 yamcs-client-1.9.5/src/yamcs/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/filetransfer/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    11297 2024-02-25 14:57:58.000000 yamcs-client-1.9.5/src/yamcs/filetransfer/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    16637 2024-02-25 14:34:09.000000 yamcs-client-1.9.5/src/yamcs/filetransfer/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.700166 yamcs-client-1.9.5/src/yamcs/link/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/link/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7884 2024-02-24 17:03:04.000000 yamcs-client-1.9.5/src/yamcs/link/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs-client-1.9.5/src/yamcs/link/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.700968 yamcs-client-1.9.5/src/yamcs/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/mdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs-client-1.9.5/src/yamcs/mdb/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs-client-1.9.5/src/yamcs/mdb/model.py
--rw-r--r--   0 fdi        (503) staff       (20)    12970 2024-02-24 16:07:18.000000 yamcs-client-1.9.5/src/yamcs/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.701326 yamcs-client-1.9.5/src/yamcs/protobuf/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.702606 yamcs-client-1.9.5/src/yamcs/protobuf/activities/
--rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/activities/activities_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/activities/activities_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.703972 yamcs-client-1.9.5/src/yamcs/protobuf/alarms/
--rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/alarms/alarms_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/alarms/alarms_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.724999 yamcs-client-1.9.5/src/yamcs/protobuf/archive/
--rw-r--r--   0 fdi        (503) staff       (20)    33536 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/archive/archive_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/archive/index_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    37199 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.725409 yamcs-client-1.9.5/src/yamcs/protobuf/audit/
--rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/audit/audit_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.725937 yamcs-client-1.9.5/src/yamcs/protobuf/auth/
--rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/auth/auth_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.726451 yamcs-client-1.9.5/src/yamcs/protobuf/buckets/
--rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/buckets/buckets_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.728849 yamcs-client-1.9.5/src/yamcs/protobuf/commanding/
--rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/commanding/clearance_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/commanding/commanding_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/commanding/commands_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/commanding/queues_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.729226 yamcs-client-1.9.5/src/yamcs/protobuf/config/
--rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/config/config_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.729636 yamcs-client-1.9.5/src/yamcs/protobuf/cop1/
--rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/cop1/cop1_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.730026 yamcs-client-1.9.5/src/yamcs/protobuf/database/
--rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/database/database_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.730950 yamcs-client-1.9.5/src/yamcs/protobuf/events/
--rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/events/events_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/events/events_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.731459 yamcs-client-1.9.5/src/yamcs/protobuf/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)    75244 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.732526 yamcs-client-1.9.5/src/yamcs/protobuf/iam/
--rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/iam/iam_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/iam/sessions_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.733657 yamcs-client-1.9.5/src/yamcs/protobuf/instances/
--rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/instances/instances_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/instances/instances_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.734865 yamcs-client-1.9.5/src/yamcs/protobuf/links/
--rw-r--r--   0 fdi        (503) staff       (20)    35324 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/links/links_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.735838 yamcs-client-1.9.5/src/yamcs/protobuf/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/mdb/mdb_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.737745 yamcs-client-1.9.5/src/yamcs/protobuf/packets/
--rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/packets/packets_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/packets/packets_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.738679 yamcs-client-1.9.5/src/yamcs/protobuf/plists/
--rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/plists/plists_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/plists/plists_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.739916 yamcs-client-1.9.5/src/yamcs/protobuf/processing/
--rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/processing/processing_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.740827 yamcs-client-1.9.5/src/yamcs/protobuf/pvalue/
--rw-r--r--   0 fdi        (503) staff       (20)    30466 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/pvalue/pvalue_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.741252 yamcs-client-1.9.5/src/yamcs/protobuf/replication/
--rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/replication/replication_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.741757 yamcs-client-1.9.5/src/yamcs/protobuf/server/
--rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/server/server_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.742595 yamcs-client-1.9.5/src/yamcs/protobuf/services/
--rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/services/services_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/services/services_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.742996 yamcs-client-1.9.5/src/yamcs/protobuf/table/
--rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/table/table_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.743699 yamcs-client-1.9.5/src/yamcs/protobuf/tco/
--rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/tco/tco_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.744244 yamcs-client-1.9.5/src/yamcs/protobuf/time/
--rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/time/time_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.744789 yamcs-client-1.9.5/src/yamcs/protobuf/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/timeline/timeline_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.745388 yamcs-client-1.9.5/src/yamcs/protobuf/yamcsManagement/
--rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-03-25 11:56:45.000000 yamcs-client-1.9.5/src/yamcs/protobuf/yamcs_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.746802 yamcs-client-1.9.5/src/yamcs/storage/
--rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/storage/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs-client-1.9.5/src/yamcs/storage/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     6493 2024-03-05 11:43:47.000000 yamcs-client-1.9.5/src/yamcs/storage/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.748252 yamcs-client-1.9.5/src/yamcs/tco/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/tco/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs-client-1.9.5/src/yamcs/tco/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs-client-1.9.5/src/yamcs/tco/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.749232 yamcs-client-1.9.5/src/yamcs/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs-client-1.9.5/src/yamcs/timeline/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-03-05 11:01:12.000000 yamcs-client-1.9.5/src/yamcs/timeline/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs-client-1.9.5/src/yamcs/timeline/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.750729 yamcs-client-1.9.5/src/yamcs/tmtc/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.5/src/yamcs/tmtc/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    50900 2024-03-18 15:51:13.000000 yamcs-client-1.9.5/src/yamcs/tmtc/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    35395 2024-03-25 12:03:49.000000 yamcs-client-1.9.5/src/yamcs/tmtc/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-25 16:16:22.758901 yamcs-client-1.9.5/src/yamcs_client.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-03-25 16:16:22.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     3462 2024-03-25 16:16:22.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-03-25 16:16:22.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       55 2024-03-25 16:16:22.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-03-25 16:16:22.000000 yamcs-client-1.9.5/src/yamcs_client.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.252878 yamcs_client-1.9.6/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs_client-1.9.6/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs_client-1.9.6/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-04-18 08:39:38.252608 yamcs_client-1.9.6/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs_client-1.9.6/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-18 08:39:38.252928 yamcs_client-1.9.6/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs_client-1.9.6/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.197042 yamcs_client-1.9.6/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.198778 yamcs_client-1.9.6/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.200385 yamcs_client-1.9.6/src/yamcs/api/
+-rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/annotations_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/exception_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/httpbody_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/websocket_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.201274 yamcs_client-1.9.6/src/yamcs/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/archive/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-04-17 19:59:36.000000 yamcs_client-1.9.6/src/yamcs/archive/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8466 2024-04-18 06:39:27.000000 yamcs_client-1.9.6/src/yamcs/archive/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.201991 yamcs_client-1.9.6/src/yamcs/client/
+-rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs_client-1.9.6/src/yamcs/client/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs_client-1.9.6/src/yamcs/client/activities.py
+-rw-r--r--   0 fdi        (503) staff       (20)    24029 2024-03-01 16:53:25.000000 yamcs_client-1.9.6/src/yamcs/client/core.py
+-rw-r--r--   0 fdi        (503) staff       (20)       22 2024-04-18 08:16:10.000000 yamcs_client-1.9.6/src/yamcs/clientversion.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.203987 yamcs_client-1.9.6/src/yamcs/core/
+-rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/core/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-03-01 16:04:02.000000 yamcs_client-1.9.6/src/yamcs/core/auth.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4665 2024-02-25 21:21:09.000000 yamcs_client-1.9.6/src/yamcs/core/context.py
+-rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/core/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs_client-1.9.6/src/yamcs/core/futures.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12888 2024-04-18 06:48:13.000000 yamcs_client-1.9.6/src/yamcs/core/helpers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs_client-1.9.6/src/yamcs/core/pagination.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs_client-1.9.6/src/yamcs/core/subscriptions.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.204803 yamcs_client-1.9.6/src/yamcs/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11570 2024-04-17 21:42:57.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15610 2024-04-17 21:47:07.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.205750 yamcs_client-1.9.6/src/yamcs/link/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/link/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8258 2024-04-17 21:22:59.000000 yamcs_client-1.9.6/src/yamcs/link/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs_client-1.9.6/src/yamcs/link/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.206534 yamcs_client-1.9.6/src/yamcs/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/mdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs_client-1.9.6/src/yamcs/mdb/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs_client-1.9.6/src/yamcs/mdb/model.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12970 2024-02-24 16:07:18.000000 yamcs_client-1.9.6/src/yamcs/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.206801 yamcs_client-1.9.6/src/yamcs/protobuf/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.207536 yamcs_client-1.9.6/src/yamcs/protobuf/actions/
+-rw-r--r--   0 fdi        (503) staff       (20)     4545 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/actions/actions_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.208397 yamcs_client-1.9.6/src/yamcs/protobuf/activities/
+-rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.209937 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/
+-rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.211784 yamcs_client-1.9.6/src/yamcs/protobuf/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)    33962 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/archive_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/index_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    43577 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.212188 yamcs_client-1.9.6/src/yamcs/protobuf/audit/
+-rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/audit/audit_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.212681 yamcs_client-1.9.6/src/yamcs/protobuf/auth/
+-rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/auth/auth_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.213122 yamcs_client-1.9.6/src/yamcs/protobuf/buckets/
+-rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/buckets/buckets_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215006 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/
+-rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/clearance_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commanding_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commands_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/queues_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215305 yamcs_client-1.9.6/src/yamcs/protobuf/config/
+-rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/config/config_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215799 yamcs_client-1.9.6/src/yamcs/protobuf/cop1/
+-rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/cop1/cop1_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.216244 yamcs_client-1.9.6/src/yamcs/protobuf/database/
+-rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/database/database_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.217338 yamcs_client-1.9.6/src/yamcs/protobuf/events/
+-rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/events/events_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/events/events_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.217692 yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)    80380 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.219027 yamcs_client-1.9.6/src/yamcs/protobuf/iam/
+-rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/iam/iam_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/iam/sessions_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.220243 yamcs_client-1.9.6/src/yamcs/protobuf/instances/
+-rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.220628 yamcs_client-1.9.6/src/yamcs/protobuf/links/
+-rw-r--r--   0 fdi        (503) staff       (20)    31906 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/links/links_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.221391 yamcs_client-1.9.6/src/yamcs/protobuf/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/mdb/mdb_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.224140 yamcs_client-1.9.6/src/yamcs/protobuf/packets/
+-rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.225528 yamcs_client-1.9.6/src/yamcs/protobuf/plists/
+-rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.226769 yamcs_client-1.9.6/src/yamcs/protobuf/processing/
+-rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/processing/processing_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.227713 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/
+-rw-r--r--   0 fdi        (503) staff       (20)    28924 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.228229 yamcs_client-1.9.6/src/yamcs/protobuf/replication/
+-rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/replication/replication_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.228655 yamcs_client-1.9.6/src/yamcs/protobuf/server/
+-rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/server/server_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.229846 yamcs_client-1.9.6/src/yamcs/protobuf/services/
+-rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/services/services_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/services/services_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.230343 yamcs_client-1.9.6/src/yamcs/protobuf/table/
+-rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/table/table_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.240360 yamcs_client-1.9.6/src/yamcs/protobuf/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/tco/tco_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.240969 yamcs_client-1.9.6/src/yamcs/protobuf/time/
+-rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/time/time_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.241481 yamcs_client-1.9.6/src/yamcs/protobuf/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/timeline/timeline_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.242290 yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/
+-rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/yamcs_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.243605 yamcs_client-1.9.6/src/yamcs/storage/
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/storage/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs_client-1.9.6/src/yamcs/storage/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6439 2024-04-16 20:50:12.000000 yamcs_client-1.9.6/src/yamcs/storage/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.245104 yamcs_client-1.9.6/src/yamcs/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/tco/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs_client-1.9.6/src/yamcs/tco/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs_client-1.9.6/src/yamcs/tco/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.246175 yamcs_client-1.9.6/src/yamcs/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs_client-1.9.6/src/yamcs/timeline/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-03-05 11:01:12.000000 yamcs_client-1.9.6/src/yamcs/timeline/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs_client-1.9.6/src/yamcs/timeline/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.247341 yamcs_client-1.9.6/src/yamcs/tmtc/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/tmtc/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    51419 2024-04-17 20:49:20.000000 yamcs_client-1.9.6/src/yamcs/tmtc/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    35330 2024-04-16 20:53:14.000000 yamcs_client-1.9.6/src/yamcs/tmtc/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.252208 yamcs_client-1.9.6/src/yamcs_client.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     3504 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/top_level.txt
```

### Comparing `yamcs-client-1.9.5/LICENSE` & `yamcs_client-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/PKG-INFO` & `yamcs_client-1.9.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.5
+Version: 1.9.6
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs-client-1.9.5/README.md` & `yamcs_client-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/setup.py` & `yamcs_client-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/api/annotations_pb2.py` & `yamcs_client-1.9.6/src/yamcs/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/api/exception_pb2.py` & `yamcs_client-1.9.6/src/yamcs/api/exception_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/api/httpbody_pb2.py` & `yamcs_client-1.9.6/src/yamcs/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/api/websocket_pb2.py` & `yamcs_client-1.9.6/src/yamcs/api/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/archive/client.py` & `yamcs_client-1.9.6/src/yamcs/archive/client.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/archive/model.py` & `yamcs_client-1.9.6/src/yamcs/archive/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,22 +271,22 @@
         self._proto = proto
 
     @property
     def start(self) -> datetime.datetime:
         """
         Start time of this range (inclusive).
         """
-        return parse_server_timestring(self._proto.timeStart)
+        return parse_server_time(self._proto.start)
 
     @property
     def stop(self) -> datetime.datetime:
         """
         Stop time of this range (exclusive).
         """
-        return parse_server_timestring(self._proto.timeStop)
+        return parse_server_time(self._proto.stop)
 
     @property
     def eng_value(self) -> Optional[Any]:
         """
         The engineering (calibrated) value within this range.
 
         If the request was made using ``min_range`` option,
```

### Comparing `yamcs-client-1.9.5/src/yamcs/client/__init__.py` & `yamcs_client-1.9.6/src/yamcs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/client/activities.py` & `yamcs_client-1.9.6/src/yamcs/client/activities.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/client/core.py` & `yamcs_client-1.9.6/src/yamcs/client/core.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/core/auth.py` & `yamcs_client-1.9.6/src/yamcs/core/auth.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/core/context.py` & `yamcs_client-1.9.6/src/yamcs/core/context.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/core/futures.py` & `yamcs_client-1.9.6/src/yamcs/core/futures.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/core/helpers.py` & `yamcs_client-1.9.6/src/yamcs/core/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 
 def parse_server_timestring(isostring: str) -> datetime:
     """
     Converts an ISO string to a timezone-aware ``datetime.datetime``.
     The timezone uses the system-default. This can be overriden to UTC
     by setting the environment variable ``PYTHON_YAMCS_CLIENT_UTC``.
     """
-    if not isostring:
-        return None
     naive = datetime.strptime(isostring.replace("Z", "GMT"), "%Y-%m-%dT%H:%M:%S.%f%Z")
     utctime = naive.replace(tzinfo=timezone.utc)
 
     if os.environ.get("PYTHON_YAMCS_CLIENT_UTC") not in (None, "0"):
         return utctime
     return utctime.astimezone(tz=None)
```

### Comparing `yamcs-client-1.9.5/src/yamcs/core/pagination.py` & `yamcs_client-1.9.6/src/yamcs/core/pagination.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/core/subscriptions.py` & `yamcs_client-1.9.6/src/yamcs/core/subscriptions.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/filetransfer/client.py` & `yamcs_client-1.9.6/src/yamcs/filetransfer/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import json
-from typing import Any, Callable, Iterable, List, Mapping, Optional
+from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional
 
+from google.protobuf import json_format, struct_pb2
 from yamcs.core.context import Context
 from yamcs.core.exceptions import NotFound
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
 from yamcs.filetransfer.model import RemoteFileListing, Service, Transfer
 from yamcs.protobuf.filetransfer import filetransfer_pb2
 
@@ -168,92 +169,70 @@
         self._service = proto.name
 
     def upload(
         self,
         bucket_name: str,
         object_name: str,
         remote_path: str,
-        source_entity: str,
-        destination_entity: str,
-        overwrite: bool,
-        parents: bool,
-        reliable: bool,
-        options: Mapping[str, Any],
+        source_entity: Optional[str],
+        destination_entity: Optional[str],
+        options: Optional[Mapping[str, Any]],
     ) -> Transfer:
         req = filetransfer_pb2.CreateTransferRequest()
         req.direction = filetransfer_pb2.TransferDirection.UPLOAD
         req.bucket = bucket_name
         req.objectName = object_name
         req.remotePath = remote_path
         if source_entity:
             req.source = source_entity
         if destination_entity:
             req.destination = destination_entity
-
-        # Old options for backwards compatibility
-        old_options = {
-            "overwrite": overwrite,
-            "createPath": parents,
-            "reliable": reliable,
-        }
-        req.options.update(old_options)
         if options:
             req.options.update(options)
 
         url = f"/filetransfer/{self._instance}/{self._service}/transfers"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
         message = filetransfer_pb2.TransferInfo()
         message.ParseFromString(response.content)
         return Transfer(message, self)
 
     def download(
         self,
         bucket_name: str,
         remote_path: str,
-        object_name: str,
-        source_entity: str,
-        destination_entity: str,
-        overwrite: bool,
-        parents: bool,
-        reliable: bool,
-        options: Mapping[str, Any],
+        object_name: Optional[str],
+        source_entity: Optional[str],
+        destination_entity: Optional[str],
+        options: Optional[Mapping[str, Any]],
     ) -> Transfer:
         req = filetransfer_pb2.CreateTransferRequest()
         req.direction = filetransfer_pb2.TransferDirection.DOWNLOAD
         req.bucket = bucket_name
         req.remotePath = remote_path
         if object_name:
             req.objectName = object_name
         if source_entity:
             req.source = source_entity
         if destination_entity:
             req.destination = destination_entity
-
-        # Old options for backwards compatibility
-        old_options = {
-            "overwrite": overwrite,
-            "createPath": parents,
-            "reliable": reliable,
-        }
-        req.options.update(old_options)
         if options:
             req.options.update(options)
 
         url = f"/filetransfer/{self._instance}/{self._service}/transfers"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
         message = filetransfer_pb2.TransferInfo()
         message.ParseFromString(response.content)
         return Transfer(message, self)
 
     def fetch_filelist(
         self,
         remote_path: str,
-        source_entity: str,
-        destination_entity: str,
-        options: Mapping[str, Any],
+        source_entity: Optional[str],
+        destination_entity: Optional[str],
+        options: Optional[Mapping[str, Any]],
     ):
         req = filetransfer_pb2.ListFilesRequest()
         req.remotePath = remote_path
         if source_entity:
             req.source = source_entity
         if destination_entity:
             req.destination = destination_entity
@@ -261,45 +240,65 @@
             req.options.update(options)
         url = f"/filetransfer/{self._instance}/{self._service}/files:sync"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
     def get_filelist(
         self,
         remote_path: str,
-        source_entity: str,
-        destination_entity: str,
-        options: Mapping[str, Any],
+        source_entity: Optional[str],
+        destination_entity: Optional[str],
+        options: Optional[Mapping[str, Any]],
     ) -> RemoteFileListing:
         params = {"remotePath": remote_path}
         if source_entity:
             params["source"] = source_entity
         if destination_entity:
             params["destination"] = destination_entity
         if options:
             params["options"] = json.dumps(options)
         url = f"/filetransfer/{self._instance}/{self._service}/files"
         response = self.ctx.get_proto(url, params=params)
         message = filetransfer_pb2.ListFilesResponse()
         message.ParseFromString(response.content)
         return RemoteFileListing(message)
 
-    def pause_transfer(self, id: str):
+    def pause_transfer(self, id: str) -> None:
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:pause"
         self.ctx.post_proto(url)
 
-    def resume_transfer(self, id: str):
+    def resume_transfer(self, id: str) -> None:
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:resume"
         self.ctx.post_proto(url)
 
-    def cancel_transfer(self, id: str):
+    def cancel_transfer(self, id: str) -> None:
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:cancel"
         self.ctx.post_proto(url)
 
+    def run_file_action(
+        self,
+        file: str,
+        action: str,
+        message: Optional[Mapping[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        req = filetransfer_pb2.RunFileActionRequest()
+        req.file = file
+        req.action = action
+        if message:
+            req.message.update(message)
+
+        url = f"/filetransfer/{self._instance}/{self._service}/files:runFileAction"
+        response = self.ctx.post_proto(url, data=req.SerializeToString())
+        response_message = struct_pb2.Struct()
+        response_message.ParseFromString(response.content)
+        return json_format.MessageToDict(response_message)
+
     def create_transfer_subscription(
-        self, on_data: Optional[Callable[[Transfer], None]] = None, timeout: float = 60
+        self,
+        on_data: Optional[Callable[[Transfer], None]] = None,
+        timeout: float = 60,
     ) -> TransferSubscription:
         options = filetransfer_pb2.SubscribeTransfersRequest()
         options.instance = self._instance
         options.serviceName = self._service
 
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="file-transfers", options=options
```

### Comparing `yamcs-client-1.9.5/src/yamcs/filetransfer/model.py` & `yamcs_client-1.9.6/src/yamcs/filetransfer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import datetime
 import threading
-from typing import Any, Callable, List, Mapping, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Mapping, Optional
 
 from yamcs.core.helpers import parse_server_time
 from yamcs.protobuf.filetransfer import filetransfer_pb2
 
+if TYPE_CHECKING:
+    from yamcs.filetransfer.client import (
+        FileListSubscription,
+        ServiceClient,
+        TransferSubscription,
+    )
+
 
 class Service:
-    def __init__(self, proto, service_client):
+    def __init__(self, proto, service_client: "ServiceClient"):
         self._proto = proto
         self._service_client = service_client
         self._local_entities = [EntityInfo(entity) for entity in proto.localEntities]
         self._remote_entities = [EntityInfo(entity) for entity in proto.remoteEntities]
         self._capabilities = FileTransferCapabilities(proto.capabilities)
         self._transfer_options = [
             FileTransferOption(option) for option in proto.transferOptions
@@ -50,124 +57,72 @@
     def upload(
         self,
         bucket_name: str,
         object_name: str,
         remote_path: str,
         source_entity: Optional[str] = None,
         destination_entity: Optional[str] = None,
-        overwrite: bool = True,
-        parents: bool = True,
-        reliable: bool = False,
         options: Optional[Mapping[str, Any]] = None,
     ) -> "Transfer":
         """
         Uploads a file located in a bucket to a remote destination path.
 
-        .. warning::
-            Prefer the use of ``options`` instead of the deprecated params
-            ``overwrite``, ``parents`` and ``reliable``.
-
         :param bucket_name:
             Name of the bucket containing the source object.
         :param object_name:
             Name of the source object.
         :param remote_path:
             Remote destination.
         :param source_entity:
             Use a specific source entity. (useful in case of multiples)
         :param destination_entity:
             Use a specific destination entity. (useful in case of multiples)
-        :param overwrite:
-            Replace file if it already exists.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``overwrite``)
-        :param parents:
-            Create the remote path if it does not yet exist.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``createPath``)
-        :param reliable:
-            Enable reliable transfers.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``reliable``)
         :param options:
-            file transfer options dict (may overwrite "overwrite", "parents"
-            or "reliable" parameters if set in these options).
+            file transfer options
         """
         return self._service_client.upload(
             bucket_name=bucket_name,
             object_name=object_name,
             remote_path=remote_path,
             source_entity=source_entity,
             destination_entity=destination_entity,
-            overwrite=overwrite,
-            parents=parents,
-            reliable=reliable,
             options=options,
         )
 
     def download(
         self,
         bucket_name: str,
         remote_path: str,
         object_name: Optional[str] = None,
         source_entity: Optional[str] = None,
         destination_entity: Optional[str] = None,
-        overwrite: bool = True,
-        parents: bool = True,
-        reliable: bool = False,
         options: Optional[Mapping[str, Any]] = None,
     ) -> "Transfer":
         """
         Downloads a file from the source to a bucket.
 
-        .. warning::
-            Prefer the use of ``options`` instead of the deprecated
-            params ``overwrite``, ``parents`` and ``reliable``.
-
         :param bucket_name:
             Name of the bucket to receive the file.
         :param object_name:
             Name of the file received in the bucket.
         :param remote_path:
             Name of the file to be downloaded from the source.
         :param source_entity:
             Use a specific source entity. (useful in case of multiples)
         :param destination_entity:
             Use a specific destination entity. (useful in case of multiples)
-        :param overwrite:
-            Replace file if it already exists.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``overwrite``)
-        :param parents:
-            Create the remote path if it does not yet exist.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``createPath``)
-        :param reliable:
-            Enable reliable transfers.
-
-            .. deprecated:: 1.8.6
-                Use ``options`` instead (option name: ``reliable``)
         :param options:
-            File transfer options dict (may overwrite ``overwrite``, ``parents``
-            or ``reliable`` parameters if set in these options).
+            File transfer options.
         """
         return self._service_client.download(
             bucket_name=bucket_name,
             remote_path=remote_path,
             object_name=object_name,
             source_entity=source_entity,
             destination_entity=destination_entity,
-            overwrite=overwrite,
-            parents=parents,
-            reliable=reliable,
             options=options,
         )
 
     def fetch_filelist(
         self,
         remote_path: str,
         source_entity: Optional[str] = None,
@@ -215,37 +170,62 @@
         return self._service_client.get_filelist(
             remote_path=remote_path,
             source_entity=source_entity,
             destination_entity=destination_entity,
             options=options,
         )
 
-    def pause_transfer(self, id: str):
+    def pause_transfer(self, id: str) -> None:
         """
         Pauses a transfer
         """
         self._service_client.pause_transfer(id)
 
-    def resume_transfer(self, id: str):
+    def resume_transfer(self, id: str) -> None:
         """
         Resume a transfer
         """
         self._service_client.resume_transfer(id)
 
-    def cancel_transfer(self, id: str):
+    def cancel_transfer(self, id: str) -> None:
         """
         Cancel a transfer
         """
         self._service_client.cancel_transfer(id)
 
+    def run_file_action(
+        self,
+        file: str,
+        action: str,
+        message: Optional[Mapping[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """
+        Run an action on a remote file.
+
+        Available actions depend on the specific file transfer implementation that
+        is in use use.
+
+        .. versionadded:: 1.9.6
+
+        :param file:
+            Remote file identifier
+        :param action:
+            Action identifier
+        :param message:
+            Action message
+        :return:
+            Action result (if the action returns anything)
+        """
+        return self._service_client.run_file_action(file, action, message)
+
     def create_transfer_subscription(
         self,
         on_data: Optional[Callable[["Transfer"], None]] = None,
         timeout: float = 60,
-    ):
+    ) -> "TransferSubscription":
         """
         Create a new transfer subscription.
 
         :param on_data:
             Function that gets called with :class:`.Transfer` updates.
         :param timeout:
             The amount of seconds to wait for the request to complete.
@@ -258,15 +238,15 @@
             on_data=on_data, timeout=timeout
         )
 
     def create_filelist_subscription(
         self,
         on_data: Optional[Callable[["RemoteFileListing"], None]] = None,
         timeout: float = 60,
-    ):
+    ) -> "FileListSubscription":
         """
         Create a new filelist subscription.
 
         :param on_data:
             Function that gets called with :class:`.Transfer` updates.
         :param timeout:
             The amount of seconds to wait for the request to complete.
```

### Comparing `yamcs-client-1.9.5/src/yamcs/link/client.py` & `yamcs_client-1.9.6/src/yamcs/link/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
-from typing import Callable, Mapping, Optional
+from typing import Any, Callable, Dict, Mapping, Optional
 
+from google.protobuf import json_format, struct_pb2
 from yamcs.core.context import Context
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
 from yamcs.link.model import Cop1Config, Cop1Status
 from yamcs.model import Link
 from yamcs.protobuf.cop1 import cop1_pb2
 from yamcs.protobuf.links import links_pb2
@@ -102,29 +103,38 @@
         """
         Disables this link.
         """
         req = links_pb2.DisableLinkRequest()
         url = f"/links/{self._instance}/{self._link}:disable"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def run_action(self, action: str, message: Optional[Mapping] = None):
+    def run_action(
+        self,
+        action: str,
+        message: Optional[Mapping[str, Any]] = None,
+    ) -> Dict[str, Any]:
         """
         Runs the given action for this link
 
         :param action:
             action identifier
         :param message:
             action message
+        :return:
+            Action result (if the action returns anything)
         """
         req = links_pb2.RunActionRequest()
         if message:
             req.message.update(message)
 
         url = f"/links/{self._instance}/{self._link}/actions/{action}"
-        self.ctx.post_proto(url, data=req.message.SerializeToString())
+        response = self.ctx.post_proto(url, data=req.message.SerializeToString())
+        response_message = struct_pb2.Struct()
+        response_message.ParseFromString(response.content)
+        return json_format.MessageToDict(response_message)
 
     def get_cop1_config(self) -> Cop1Config:
         """
         Gets the COP1 configuration for a data link.
         """
         response = self.ctx.get_proto(f"/cop1/{self._instance}/{self._link}/config")
         message = cop1_pb2.Cop1Config()
```

### Comparing `yamcs-client-1.9.5/src/yamcs/link/model.py` & `yamcs_client-1.9.6/src/yamcs/link/model.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/mdb/client.py` & `yamcs_client-1.9.6/src/yamcs/mdb/client.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/mdb/model.py` & `yamcs_client-1.9.6/src/yamcs/mdb/model.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/model.py` & `yamcs_client-1.9.6/src/yamcs/model.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/activities/activities_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/activities/activities_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/alarms/alarms_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/alarms/alarms_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/archive/archive_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/archive/archive_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/archive/archive.proto',
   package='yamcs.protobuf.archive',
   syntax='proto2',
   serialized_options=b'\n\022org.yamcs.protobuf',
-  serialized_pb=b'\n$yamcs/protobuf/archive/archive.proto\x12\x16yamcs.protobuf.archive\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a\"yamcs/protobuf/pvalue/pvalue.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xc2\x01\n\x1cStreamParameterValuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x03ids\x18\x04 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x0f\n\x07tmLinks\x18\x05 \x03(\t\"7\n\x12ParameterGroupInfo\x12\x11\n\x05group\x18\x01 \x03(\tB\x02\x18\x01\x12\x0e\n\x06groups\x18\x02 \x03(\t\".\n\x1aListParameterGroupsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\xa6\x02\n\x1bListParameterHistoryRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03pos\x18\x03 \x01(\x03\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x10\n\x08norepeat\x18\x05 \x01(\x08\x12)\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05order\x18\x08 \x01(\t\x12\x12\n\nnorealtime\x18\t \x01(\x08\x12\x11\n\tprocessor\x18\n \x01(\t\x12\x0e\n\x06source\x18\x0b \x01(\t\x12\x10\n\x08maxBytes\x18\r \x01(\x05\x12\x0c\n\x04next\x18\x0c \x01(\t\"s\n\x1cListParameterHistoryResponse\x12\x38\n\tparameter\x18\x01 \x03(\x0b\x32%.yamcs.protobuf.pvalue.ParameterValue\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\"\xec\x01\n\x1aGetParameterSamplesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x63ount\x18\x05 \x01(\x05\x12\x12\n\nnorealtime\x18\x06 \x01(\x08\x12\x13\n\x0buseRawValue\x18\t \x01(\x08\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12\x0e\n\x06source\x18\x08 \x01(\t\"\xc6\x02\n\x1c\x45xportParameterValuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nparameters\x18\x04 \x03(\t\x12\x0c\n\x04list\x18\x0e \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\x12\r\n\x05\x65xtra\x18\x06 \x03(\t\x12\x11\n\tdelimiter\x18\x07 \x01(\t\x12\x10\n\x08interval\x18\x08 \x01(\x05\x12\x19\n\x11preserveLastValue\x18\t \x01(\x08\x12\x0b\n\x03pos\x18\n \x01(\x03\x12\r\n\x05limit\x18\x0b \x01(\x05\x12\r\n\x05order\x18\x0c \x01(\t\x12\x10\n\x08\x66ilename\x18\r \x01(\t2\xb6\x07\n\x10StreamArchiveApi\x12\xa5\x01\n\x13ListParameterGroups\x12\x32.yamcs.protobuf.archive.ListParameterGroupsRequest\x1a*.yamcs.protobuf.archive.ParameterGroupInfo\".\x8a\x92\x03*\n(/api/archive/{instance}/parameter-groups\x12\xba\x01\n\x14ListParameterHistory\x12\x33.yamcs.protobuf.archive.ListParameterHistoryRequest\x1a\x34.yamcs.protobuf.archive.ListParameterHistoryResponse\"7\x8a\x92\x03\x33\n1/api/stream-archive/{instance}/parameters/{name*}\x12\xb4\x01\n\x15StreamParameterValues\x12\x34.yamcs.protobuf.archive.StreamParameterValuesRequest\x1a$.yamcs.protobuf.pvalue.ParameterData\"=\x8a\x92\x03\x39\x1a\x34/api/stream-archive/{instance}:streamParameterValues:\x01*0\x01\x12\xb5\x01\n\x13GetParameterSamples\x12\x32.yamcs.protobuf.archive.GetParameterSamplesRequest\x1a!.yamcs.protobuf.pvalue.TimeSeries\"G\x8a\x92\x03\x43\n9/api/stream-archive/{instance}/parameters/{name*}/samplesR\x06sample\x12\xcd\x01\n\x15\x45xportParameterValues\x12\x34.yamcs.protobuf.archive.ExportParameterValuesRequest\x1a\x13.yamcs.api.HttpBody\"g\x8a\x92\x03\x63\n-/api/archive/{instance}:exportParameterValuesZ2\x1a-/api/archive/{instance}:exportParameterValues:\x01*0\x01\x42\x14\n\x12org.yamcs.protobuf'
+  serialized_pb=b'\n$yamcs/protobuf/archive/archive.proto\x12\x16yamcs.protobuf.archive\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a\"yamcs/protobuf/pvalue/pvalue.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xc2\x01\n\x1cStreamParameterValuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x03ids\x18\x04 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x0f\n\x07tmLinks\x18\x05 \x03(\t\"7\n\x12ParameterGroupInfo\x12\x11\n\x05group\x18\x01 \x03(\tB\x02\x18\x01\x12\x0e\n\x06groups\x18\x02 \x03(\t\".\n\x1aListParameterGroupsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\xa6\x02\n\x1bListParameterHistoryRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03pos\x18\x03 \x01(\x03\x12\r\n\x05limit\x18\x04 \x01(\x05\x12\x10\n\x08norepeat\x18\x05 \x01(\x08\x12)\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05order\x18\x08 \x01(\t\x12\x12\n\nnorealtime\x18\t \x01(\x08\x12\x11\n\tprocessor\x18\n \x01(\t\x12\x0e\n\x06source\x18\x0b \x01(\t\x12\x10\n\x08maxBytes\x18\r \x01(\x05\x12\x0c\n\x04next\x18\x0c \x01(\t\"s\n\x1cListParameterHistoryResponse\x12\x38\n\tparameter\x18\x01 \x03(\x0b\x32%.yamcs.protobuf.pvalue.ParameterValue\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\"\xfd\x01\n\x1aGetParameterSamplesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x63ount\x18\x05 \x01(\x05\x12\x12\n\nnorealtime\x18\x06 \x01(\x08\x12\x13\n\x0buseRawValue\x18\t \x01(\x08\x12\x0f\n\x07gapTime\x18\n \x01(\x04\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12\x0e\n\x06source\x18\x08 \x01(\t\"\xc6\x02\n\x1c\x45xportParameterValuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nparameters\x18\x04 \x03(\t\x12\x0c\n\x04list\x18\x0e \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\x12\r\n\x05\x65xtra\x18\x06 \x03(\t\x12\x11\n\tdelimiter\x18\x07 \x01(\t\x12\x10\n\x08interval\x18\x08 \x01(\x05\x12\x19\n\x11preserveLastValue\x18\t \x01(\x08\x12\x0b\n\x03pos\x18\n \x01(\x03\x12\r\n\x05limit\x18\x0b \x01(\x05\x12\r\n\x05order\x18\x0c \x01(\t\x12\x10\n\x08\x66ilename\x18\r \x01(\t2\xb6\x07\n\x10StreamArchiveApi\x12\xa5\x01\n\x13ListParameterGroups\x12\x32.yamcs.protobuf.archive.ListParameterGroupsRequest\x1a*.yamcs.protobuf.archive.ParameterGroupInfo\".\x8a\x92\x03*\n(/api/archive/{instance}/parameter-groups\x12\xba\x01\n\x14ListParameterHistory\x12\x33.yamcs.protobuf.archive.ListParameterHistoryRequest\x1a\x34.yamcs.protobuf.archive.ListParameterHistoryResponse\"7\x8a\x92\x03\x33\n1/api/stream-archive/{instance}/parameters/{name*}\x12\xb4\x01\n\x15StreamParameterValues\x12\x34.yamcs.protobuf.archive.StreamParameterValuesRequest\x1a$.yamcs.protobuf.pvalue.ParameterData\"=\x8a\x92\x03\x39\x1a\x34/api/stream-archive/{instance}:streamParameterValues:\x01*0\x01\x12\xb5\x01\n\x13GetParameterSamples\x12\x32.yamcs.protobuf.archive.GetParameterSamplesRequest\x1a!.yamcs.protobuf.pvalue.TimeSeries\"G\x8a\x92\x03\x43\n9/api/stream-archive/{instance}/parameters/{name*}/samplesR\x06sample\x12\xcd\x01\n\x15\x45xportParameterValues\x12\x34.yamcs.protobuf.archive.ExportParameterValuesRequest\x1a\x13.yamcs.api.HttpBody\"g\x8a\x92\x03\x63\n-/api/archive/{instance}:exportParameterValuesZ2\x1a-/api/archive/{instance}:exportParameterValues:\x01*0\x01\x42\x14\n\x12org.yamcs.protobuf'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_api_dot_httpbody__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_pvalue_dot_pvalue__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,])
 
 
 
 
 _STREAMPARAMETERVALUESREQUEST = _descriptor.Descriptor(
@@ -364,22 +364,29 @@
       name='useRawValue', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.useRawValue', index=6,
       number=9, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='processor', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.processor', index=7,
+      name='gapTime', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.gapTime', index=7,
+      number=10, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='processor', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.processor', index=8,
       number=7, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='source', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.source', index=8,
+      name='source', full_name='yamcs.protobuf.archive.GetParameterSamplesRequest.source', index=9,
       number=8, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -390,15 +397,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=933,
-  serialized_end=1169,
+  serialized_end=1186,
 )
 
 
 _EXPORTPARAMETERVALUESREQUEST = _descriptor.Descriptor(
   name='ExportParameterValuesRequest',
   full_name='yamcs.protobuf.archive.ExportParameterValuesRequest',
   filename=None,
@@ -511,16 +518,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1172,
-  serialized_end=1498,
+  serialized_start=1189,
+  serialized_end=1515,
 )
 
 _STREAMPARAMETERVALUESREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _STREAMPARAMETERVALUESREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _STREAMPARAMETERVALUESREQUEST.fields_by_name['ids'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._NAMEDOBJECTID
 _LISTPARAMETERHISTORYREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _LISTPARAMETERHISTORYREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -593,16 +600,16 @@
 
 _STREAMARCHIVEAPI = _descriptor.ServiceDescriptor(
   name='StreamArchiveApi',
   full_name='yamcs.protobuf.archive.StreamArchiveApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1501,
-  serialized_end=2451,
+  serialized_start=1518,
+  serialized_end=2468,
   methods=[
   _descriptor.MethodDescriptor(
     name='ListParameterGroups',
     full_name='yamcs.protobuf.archive.StreamArchiveApi.ListParameterGroups',
     index=0,
     containing_service=None,
     input_type=_LISTPARAMETERGROUPSREQUEST,
```

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/archive/index_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/archive/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,127 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/archive/parameter_archive_service.proto',
   package='yamcs.protobuf.archive',
   syntax='proto2',
   serialized_options=b'\n\022org.yamcs.protobufB\034ParameterArchiveServiceProtoP\001',
-  serialized_pb=b'\n6yamcs/protobuf/archive/parameter_archive_service.proto\x12\x16yamcs.protobuf.archive\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a$yamcs/protobuf/archive/archive.proto\x1a\"yamcs/protobuf/pvalue/pvalue.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"|\n\x13RebuildRangeRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\" \n\x0cPurgeRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x8c\x02\n\x19GetParameterRangesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06minGap\x18\x05 \x01(\x03\x12\x0e\n\x06maxGap\x18\x06 \x01(\x03\x12\x12\n\nnorealtime\x18\x07 \x01(\x08\x12\x11\n\tprocessor\x18\x08 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x10\n\x08minRange\x18\n \x01(\x03\x12\x11\n\tmaxValues\x18\x0b \x01(\x05\"^\n GetArchivedParametersInfoRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\x03 \x01(\t\x12\r\n\x05limit\x18\x07 \x01(\x05\"\x99\x01\n#GetArchivedParameterSegmentsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0b\n\x03pid\x18\x02 \x01(\r\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x99\x01\n\x15\x41rchivedParameterInfo\x12\x0b\n\x03pid\x18\x01 \x01(\r\x12\x0b\n\x03\x66qn\x18\x02 \x01(\t\x12+\n\x07rawType\x18\x03 \x01(\x0e\x32\x1a.yamcs.protobuf.Value.Type\x12+\n\x07\x65ngType\x18\x04 \x01(\x0e\x32\x1a.yamcs.protobuf.Value.Type\x12\x0c\n\x04gids\x18\x05 \x03(\r\"c\n\x1e\x41rchivedParametersInfoResponse\x12\x41\n\nparameters\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo\"\x91\x01\n\x1b\x41rchiveParameterSegmentInfo\x12\x0f\n\x07groupId\x18\x01 \x01(\r\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03\x65nd\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x63ount\x18\x04 \x01(\r\"\xb0\x01\n!ArchivedParameterSegmentsResponse\x12\x44\n\rparameterInfo\x18\x01 \x01(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo\x12\x45\n\x08segments\x18\x02 \x03(\x0b\x32\x33.yamcs.protobuf.archive.ArchiveParameterSegmentInfo\"A\n GetArchivedParameterGroupRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0b\n\x03gid\x18\x02 \x01(\r\"p\n\x1e\x41rchivedParameterGroupResponse\x12\x0b\n\x03gid\x18\x01 \x01(\r\x12\x41\n\nparameters\x18\x02 \x03(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo2\xb9\x0b\n\x13ParameterArchiveApi\x12\x90\x01\n\x0cRebuildRange\x12+.yamcs.protobuf.archive.RebuildRangeRequest\x1a\x16.google.protobuf.Empty\";\x8a\x92\x03\x37\x1a\x30/api/archive/{instance}/parameterArchive:rebuild:\x01*H\x01\x12\xae\x01\n\x13GetParameterSamples\x12\x32.yamcs.protobuf.archive.GetParameterSamplesRequest\x1a!.yamcs.protobuf.pvalue.TimeSeries\"@\x8a\x92\x03<\n2/api/archive/{instance}/parameters/{name*}/samplesR\x06sample\x12\xa6\x01\n\x12GetParameterRanges\x12\x31.yamcs.protobuf.archive.GetParameterRangesRequest\x1a\x1d.yamcs.protobuf.pvalue.Ranges\">\x8a\x92\x03:\n1/api/archive/{instance}/parameters/{name*}/rangesR\x05range\x12\xb3\x01\n\x14ListParameterHistory\x12\x33.yamcs.protobuf.archive.ListParameterHistoryRequest\x1a\x34.yamcs.protobuf.archive.ListParameterHistoryResponse\"0\x8a\x92\x03,\n*/api/archive/{instance}/parameters/{name*}\x12\xcd\x01\n\x19GetArchivedParametersInfo\x12\x38.yamcs.protobuf.archive.GetArchivedParametersInfoRequest\x1a\x36.yamcs.protobuf.archive.ArchivedParametersInfoResponse\">\x8a\x92\x03:\n8/api/archive/{instance}/parameterArchive/info/parameters\x12\xdb\x01\n\x1cGetArchivedParameterSegments\x12;.yamcs.protobuf.archive.GetArchivedParameterSegmentsRequest\x1a\x39.yamcs.protobuf.archive.ArchivedParameterSegmentsResponse\"C\x8a\x92\x03?\n=/api/archive/{instance}/parameterArchive/info/segments/{pid*}\x12\xd0\x01\n\x19GetArchivedParameterGroup\x12\x38.yamcs.protobuf.archive.GetArchivedParameterGroupRequest\x1a\x36.yamcs.protobuf.archive.ArchivedParameterGroupResponse\"A\x8a\x92\x03=\n;/api/archive/{instance}/parameterArchive/info/groups/{gid*}\x12~\n\x05Purge\x12$.yamcs.protobuf.archive.PurgeRequest\x1a\x16.google.protobuf.Empty\"7\x8a\x92\x03\x33\x1a./api/archive/{instance}/parameterArchive:purge:\x01*B4\n\x12org.yamcs.protobufB\x1cParameterArchiveServiceProtoP\x01'
+  serialized_pb=b'\n6yamcs/protobuf/archive/parameter_archive_service.proto\x12\x16yamcs.protobuf.archive\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a$yamcs/protobuf/archive/archive.proto\x1a\"yamcs/protobuf/pvalue/pvalue.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"/\n\x1bSubscribeBackfillingRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\xfe\x01\n\x18SubscribeBackfillingData\x12W\n\x08\x66inished\x18\x01 \x03(\x0b\x32\x45.yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo\x1a\x88\x01\n\x14\x42\x61\x63kfillFinishedInfo\x12)\n\x05start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13processedParameters\x18\x03 \x01(\x04\"|\n\x13RebuildRangeRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\" \n\x0cPurgeRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x8c\x02\n\x19GetParameterRangesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06minGap\x18\x05 \x01(\x03\x12\x0e\n\x06maxGap\x18\x06 \x01(\x03\x12\x12\n\nnorealtime\x18\x07 \x01(\x08\x12\x11\n\tprocessor\x18\x08 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x10\n\x08minRange\x18\n \x01(\x03\x12\x11\n\tmaxValues\x18\x0b \x01(\x05\"^\n GetArchivedParametersInfoRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\x03 \x01(\t\x12\r\n\x05limit\x18\x07 \x01(\x05\"\x99\x01\n#GetArchivedParameterSegmentsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0b\n\x03pid\x18\x02 \x01(\r\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x99\x01\n\x15\x41rchivedParameterInfo\x12\x0b\n\x03pid\x18\x01 \x01(\r\x12\x0b\n\x03\x66qn\x18\x02 \x01(\t\x12+\n\x07rawType\x18\x03 \x01(\x0e\x32\x1a.yamcs.protobuf.Value.Type\x12+\n\x07\x65ngType\x18\x04 \x01(\x0e\x32\x1a.yamcs.protobuf.Value.Type\x12\x0c\n\x04gids\x18\x05 \x03(\r\"c\n\x1e\x41rchivedParametersInfoResponse\x12\x41\n\nparameters\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo\"\x91\x01\n\x1b\x41rchiveParameterSegmentInfo\x12\x0f\n\x07groupId\x18\x01 \x01(\r\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03\x65nd\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x63ount\x18\x04 \x01(\r\"\xb0\x01\n!ArchivedParameterSegmentsResponse\x12\x44\n\rparameterInfo\x18\x01 \x01(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo\x12\x45\n\x08segments\x18\x02 \x03(\x0b\x32\x33.yamcs.protobuf.archive.ArchiveParameterSegmentInfo\"A\n GetArchivedParameterGroupRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0b\n\x03gid\x18\x02 \x01(\r\"p\n\x1e\x41rchivedParameterGroupResponse\x12\x0b\n\x03gid\x18\x01 \x01(\r\x12\x41\n\nparameters\x18\x02 \x03(\x0b\x32-.yamcs.protobuf.archive.ArchivedParameterInfo2\xce\x0c\n\x13ParameterArchiveApi\x12\x90\x01\n\x0cRebuildRange\x12+.yamcs.protobuf.archive.RebuildRangeRequest\x1a\x16.google.protobuf.Empty\";\x8a\x92\x03\x37\x1a\x30/api/archive/{instance}/parameterArchive:rebuild:\x01*H\x01\x12\xae\x01\n\x13GetParameterSamples\x12\x32.yamcs.protobuf.archive.GetParameterSamplesRequest\x1a!.yamcs.protobuf.pvalue.TimeSeries\"@\x8a\x92\x03<\n2/api/archive/{instance}/parameters/{name*}/samplesR\x06sample\x12\xa6\x01\n\x12GetParameterRanges\x12\x31.yamcs.protobuf.archive.GetParameterRangesRequest\x1a\x1d.yamcs.protobuf.pvalue.Ranges\">\x8a\x92\x03:\n1/api/archive/{instance}/parameters/{name*}/rangesR\x05range\x12\xb3\x01\n\x14ListParameterHistory\x12\x33.yamcs.protobuf.archive.ListParameterHistoryRequest\x1a\x34.yamcs.protobuf.archive.ListParameterHistoryResponse\"0\x8a\x92\x03,\n*/api/archive/{instance}/parameters/{name*}\x12\xcd\x01\n\x19GetArchivedParametersInfo\x12\x38.yamcs.protobuf.archive.GetArchivedParametersInfoRequest\x1a\x36.yamcs.protobuf.archive.ArchivedParametersInfoResponse\">\x8a\x92\x03:\n8/api/archive/{instance}/parameterArchive/info/parameters\x12\xdb\x01\n\x1cGetArchivedParameterSegments\x12;.yamcs.protobuf.archive.GetArchivedParameterSegmentsRequest\x1a\x39.yamcs.protobuf.archive.ArchivedParameterSegmentsResponse\"C\x8a\x92\x03?\n=/api/archive/{instance}/parameterArchive/info/segments/{pid*}\x12\xd0\x01\n\x19GetArchivedParameterGroup\x12\x38.yamcs.protobuf.archive.GetArchivedParameterGroupRequest\x1a\x36.yamcs.protobuf.archive.ArchivedParameterGroupResponse\"A\x8a\x92\x03=\n;/api/archive/{instance}/parameterArchive/info/groups/{gid*}\x12~\n\x05Purge\x12$.yamcs.protobuf.archive.PurgeRequest\x1a\x16.google.protobuf.Empty\"7\x8a\x92\x03\x33\x1a./api/archive/{instance}/parameterArchive:purge:\x01*\x12\x92\x01\n\x14SubscribeBackfilling\x12\x33.yamcs.protobuf.archive.SubscribeBackfillingRequest\x1a\x30.yamcs.protobuf.archive.SubscribeBackfillingData\"\x11\xda\x92\x03\r\n\x0b\x62\x61\x63kfilling0\x01\x42\x34\n\x12org.yamcs.protobufB\x1cParameterArchiveServiceProtoP\x01'
   ,
   dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_archive_dot_archive__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_pvalue_dot_pvalue__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,])
 
 
 
 
+_SUBSCRIBEBACKFILLINGREQUEST = _descriptor.Descriptor(
+  name='SubscribeBackfillingRequest',
+  full_name='yamcs.protobuf.archive.SubscribeBackfillingRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='instance', full_name='yamcs.protobuf.archive.SubscribeBackfillingRequest.instance', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=275,
+  serialized_end=322,
+)
+
+
+_SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO = _descriptor.Descriptor(
+  name='BackfillFinishedInfo',
+  full_name='yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='start', full_name='yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo.start', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='stop', full_name='yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo.stop', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='processedParameters', full_name='yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo.processedParameters', index=2,
+      number=3, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=443,
+  serialized_end=579,
+)
+
+_SUBSCRIBEBACKFILLINGDATA = _descriptor.Descriptor(
+  name='SubscribeBackfillingData',
+  full_name='yamcs.protobuf.archive.SubscribeBackfillingData',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='finished', full_name='yamcs.protobuf.archive.SubscribeBackfillingData.finished', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[_SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=325,
+  serialized_end=579,
+)
+
+
 _REBUILDRANGEREQUEST = _descriptor.Descriptor(
   name='RebuildRangeRequest',
   full_name='yamcs.protobuf.archive.RebuildRangeRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
@@ -67,16 +173,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=275,
-  serialized_end=399,
+  serialized_start=581,
+  serialized_end=705,
 )
 
 
 _PURGEREQUEST = _descriptor.Descriptor(
   name='PurgeRequest',
   full_name='yamcs.protobuf.archive.PurgeRequest',
   filename=None,
@@ -98,16 +204,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=401,
-  serialized_end=433,
+  serialized_start=707,
+  serialized_end=739,
 )
 
 
 _GETPARAMETERRANGESREQUEST = _descriptor.Descriptor(
   name='GetParameterRangesRequest',
   full_name='yamcs.protobuf.archive.GetParameterRangesRequest',
   filename=None,
@@ -199,16 +305,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=436,
-  serialized_end=704,
+  serialized_start=742,
+  serialized_end=1010,
 )
 
 
 _GETARCHIVEDPARAMETERSINFOREQUEST = _descriptor.Descriptor(
   name='GetArchivedParametersInfoRequest',
   full_name='yamcs.protobuf.archive.GetArchivedParametersInfoRequest',
   filename=None,
@@ -251,16 +357,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=706,
-  serialized_end=800,
+  serialized_start=1012,
+  serialized_end=1106,
 )
 
 
 _GETARCHIVEDPARAMETERSEGMENTSREQUEST = _descriptor.Descriptor(
   name='GetArchivedParameterSegmentsRequest',
   full_name='yamcs.protobuf.archive.GetArchivedParameterSegmentsRequest',
   filename=None,
@@ -303,16 +409,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=803,
-  serialized_end=956,
+  serialized_start=1109,
+  serialized_end=1262,
 )
 
 
 _ARCHIVEDPARAMETERINFO = _descriptor.Descriptor(
   name='ArchivedParameterInfo',
   full_name='yamcs.protobuf.archive.ArchivedParameterInfo',
   filename=None,
@@ -362,16 +468,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=959,
-  serialized_end=1112,
+  serialized_start=1265,
+  serialized_end=1418,
 )
 
 
 _ARCHIVEDPARAMETERSINFORESPONSE = _descriptor.Descriptor(
   name='ArchivedParametersInfoResponse',
   full_name='yamcs.protobuf.archive.ArchivedParametersInfoResponse',
   filename=None,
@@ -393,16 +499,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1114,
-  serialized_end=1213,
+  serialized_start=1420,
+  serialized_end=1519,
 )
 
 
 _ARCHIVEPARAMETERSEGMENTINFO = _descriptor.Descriptor(
   name='ArchiveParameterSegmentInfo',
   full_name='yamcs.protobuf.archive.ArchiveParameterSegmentInfo',
   filename=None,
@@ -445,16 +551,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1216,
-  serialized_end=1361,
+  serialized_start=1522,
+  serialized_end=1667,
 )
 
 
 _ARCHIVEDPARAMETERSEGMENTSRESPONSE = _descriptor.Descriptor(
   name='ArchivedParameterSegmentsResponse',
   full_name='yamcs.protobuf.archive.ArchivedParameterSegmentsResponse',
   filename=None,
@@ -483,16 +589,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1364,
-  serialized_end=1540,
+  serialized_start=1670,
+  serialized_end=1846,
 )
 
 
 _GETARCHIVEDPARAMETERGROUPREQUEST = _descriptor.Descriptor(
   name='GetArchivedParameterGroupRequest',
   full_name='yamcs.protobuf.archive.GetArchivedParameterGroupRequest',
   filename=None,
@@ -521,16 +627,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1542,
-  serialized_end=1607,
+  serialized_start=1848,
+  serialized_end=1913,
 )
 
 
 _ARCHIVEDPARAMETERGROUPRESPONSE = _descriptor.Descriptor(
   name='ArchivedParameterGroupResponse',
   full_name='yamcs.protobuf.archive.ArchivedParameterGroupResponse',
   filename=None,
@@ -559,45 +665,73 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1609,
-  serialized_end=1721,
+  serialized_start=1915,
+  serialized_end=2027,
 )
 
+_SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO.containing_type = _SUBSCRIBEBACKFILLINGDATA
+_SUBSCRIBEBACKFILLINGDATA.fields_by_name['finished'].message_type = _SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO
 _REBUILDRANGEREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _REBUILDRANGEREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETPARAMETERRANGESREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETPARAMETERRANGESREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETARCHIVEDPARAMETERSEGMENTSREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETARCHIVEDPARAMETERSEGMENTSREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _ARCHIVEDPARAMETERINFO.fields_by_name['rawType'].enum_type = yamcs_dot_protobuf_dot_yamcs__pb2._VALUE_TYPE
 _ARCHIVEDPARAMETERINFO.fields_by_name['engType'].enum_type = yamcs_dot_protobuf_dot_yamcs__pb2._VALUE_TYPE
 _ARCHIVEDPARAMETERSINFORESPONSE.fields_by_name['parameters'].message_type = _ARCHIVEDPARAMETERINFO
 _ARCHIVEPARAMETERSEGMENTINFO.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _ARCHIVEPARAMETERSEGMENTINFO.fields_by_name['end'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _ARCHIVEDPARAMETERSEGMENTSRESPONSE.fields_by_name['parameterInfo'].message_type = _ARCHIVEDPARAMETERINFO
 _ARCHIVEDPARAMETERSEGMENTSRESPONSE.fields_by_name['segments'].message_type = _ARCHIVEPARAMETERSEGMENTINFO
 _ARCHIVEDPARAMETERGROUPRESPONSE.fields_by_name['parameters'].message_type = _ARCHIVEDPARAMETERINFO
+DESCRIPTOR.message_types_by_name['SubscribeBackfillingRequest'] = _SUBSCRIBEBACKFILLINGREQUEST
+DESCRIPTOR.message_types_by_name['SubscribeBackfillingData'] = _SUBSCRIBEBACKFILLINGDATA
 DESCRIPTOR.message_types_by_name['RebuildRangeRequest'] = _REBUILDRANGEREQUEST
 DESCRIPTOR.message_types_by_name['PurgeRequest'] = _PURGEREQUEST
 DESCRIPTOR.message_types_by_name['GetParameterRangesRequest'] = _GETPARAMETERRANGESREQUEST
 DESCRIPTOR.message_types_by_name['GetArchivedParametersInfoRequest'] = _GETARCHIVEDPARAMETERSINFOREQUEST
 DESCRIPTOR.message_types_by_name['GetArchivedParameterSegmentsRequest'] = _GETARCHIVEDPARAMETERSEGMENTSREQUEST
 DESCRIPTOR.message_types_by_name['ArchivedParameterInfo'] = _ARCHIVEDPARAMETERINFO
 DESCRIPTOR.message_types_by_name['ArchivedParametersInfoResponse'] = _ARCHIVEDPARAMETERSINFORESPONSE
 DESCRIPTOR.message_types_by_name['ArchiveParameterSegmentInfo'] = _ARCHIVEPARAMETERSEGMENTINFO
 DESCRIPTOR.message_types_by_name['ArchivedParameterSegmentsResponse'] = _ARCHIVEDPARAMETERSEGMENTSRESPONSE
 DESCRIPTOR.message_types_by_name['GetArchivedParameterGroupRequest'] = _GETARCHIVEDPARAMETERGROUPREQUEST
 DESCRIPTOR.message_types_by_name['ArchivedParameterGroupResponse'] = _ARCHIVEDPARAMETERGROUPRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+SubscribeBackfillingRequest = _reflection.GeneratedProtocolMessageType('SubscribeBackfillingRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SUBSCRIBEBACKFILLINGREQUEST,
+  '__module__' : 'yamcs.protobuf.archive.parameter_archive_service_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.archive.SubscribeBackfillingRequest)
+  })
+_sym_db.RegisterMessage(SubscribeBackfillingRequest)
+
+SubscribeBackfillingData = _reflection.GeneratedProtocolMessageType('SubscribeBackfillingData', (_message.Message,), {
+
+  'BackfillFinishedInfo' : _reflection.GeneratedProtocolMessageType('BackfillFinishedInfo', (_message.Message,), {
+    'DESCRIPTOR' : _SUBSCRIBEBACKFILLINGDATA_BACKFILLFINISHEDINFO,
+    '__module__' : 'yamcs.protobuf.archive.parameter_archive_service_pb2'
+    # @@protoc_insertion_point(class_scope:yamcs.protobuf.archive.SubscribeBackfillingData.BackfillFinishedInfo)
+    })
+  ,
+  'DESCRIPTOR' : _SUBSCRIBEBACKFILLINGDATA,
+  '__module__' : 'yamcs.protobuf.archive.parameter_archive_service_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.archive.SubscribeBackfillingData)
+  })
+_sym_db.RegisterMessage(SubscribeBackfillingData)
+_sym_db.RegisterMessage(SubscribeBackfillingData.BackfillFinishedInfo)
+
 RebuildRangeRequest = _reflection.GeneratedProtocolMessageType('RebuildRangeRequest', (_message.Message,), {
   'DESCRIPTOR' : _REBUILDRANGEREQUEST,
   '__module__' : 'yamcs.protobuf.archive.parameter_archive_service_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.archive.RebuildRangeRequest)
   })
 _sym_db.RegisterMessage(RebuildRangeRequest)
 
@@ -676,16 +810,16 @@
 
 _PARAMETERARCHIVEAPI = _descriptor.ServiceDescriptor(
   name='ParameterArchiveApi',
   full_name='yamcs.protobuf.archive.ParameterArchiveApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1724,
-  serialized_end=3189,
+  serialized_start=2030,
+  serialized_end=3644,
   methods=[
   _descriptor.MethodDescriptor(
     name='RebuildRange',
     full_name='yamcs.protobuf.archive.ParameterArchiveApi.RebuildRange',
     index=0,
     containing_service=None,
     input_type=_REBUILDRANGEREQUEST,
@@ -751,13 +885,22 @@
     full_name='yamcs.protobuf.archive.ParameterArchiveApi.Purge',
     index=7,
     containing_service=None,
     input_type=_PURGEREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=b'\212\222\0033\032./api/archive/{instance}/parameterArchive:purge:\001*',
   ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeBackfilling',
+    full_name='yamcs.protobuf.archive.ParameterArchiveApi.SubscribeBackfilling',
+    index=8,
+    containing_service=None,
+    input_type=_SUBSCRIBEBACKFILLINGREQUEST,
+    output_type=_SUBSCRIBEBACKFILLINGDATA,
+    serialized_options=b'\332\222\003\r\n\013backfilling',
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_PARAMETERARCHIVEAPI)
 
 DESCRIPTOR.services_by_name['ParameterArchiveApi'] = _PARAMETERARCHIVEAPI
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/archive/rocksdb_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/archive/rocksdb_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/audit/audit_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/audit/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/auth/auth_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/buckets/buckets_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/buckets/buckets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/commanding/clearance_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/clearance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/commanding/commanding_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commanding_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/commanding/commands_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commands_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/commanding/queues_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/queues_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/config/config_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/cop1/cop1_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/cop1/cop1_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/database/database_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/database/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/events/events_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/events/events_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/events/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from yamcs.api import annotations_pb2 as yamcs_dot_api_dot_annotations__pb2
+from yamcs.protobuf.actions import actions_pb2 as yamcs_dot_protobuf_dot_actions_dot_actions__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/filetransfer/filetransfer.proto',
   package='yamcs.protobuf.filetransfer',
   syntax='proto2',
   serialized_options=b'\n\022org.yamcs.protobufB\021FileTransferProtoP\001',
-  serialized_pb=b'\n.yamcs/protobuf/filetransfer/filetransfer.proto\x12\x1byamcs.protobuf.filetransfer\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1byamcs/api/annotations.proto\"@\n\rTransactionId\x12\x16\n\x0esequenceNumber\x18\x01 \x01(\r\x12\x17\n\x0finitiatorEntity\x18\x02 \x01(\x04\"3\n\x1fListFileTransferServicesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"F\n\x1dGetFileTransferServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"j\n ListFileTransferServicesResponse\x12\x46\n\x08services\x18\x01 \x03(\x0b\x32\x34.yamcs.protobuf.filetransfer.FileTransferServiceInfo\"\xc7\x01\n\x18\x46ileTransferCapabilities\x12\x0e\n\x06upload\x18\x01 \x01(\x08\x12\x10\n\x08\x64ownload\x18\x02 \x01(\x08\x12\x12\n\nremotePath\x18\x04 \x01(\x08\x12\x10\n\x08\x66ileList\x18\x05 \x01(\x08\x12\x17\n\x0fhasTransferType\x18\x06 \x01(\x08\x12J\n\x14\x66ileListExtraColumns\x18\x07 \x03(\x0b\x32,.yamcs.protobuf.filetransfer.ExtraColumnInfo\",\n\x0f\x45xtraColumnInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\xd1\x02\n\x17\x46ileTransferServiceInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\rlocalEntities\x18\x03 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12?\n\x0eremoteEntities\x18\x04 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12K\n\x0c\x63\x61pabilities\x18\x05 \x01(\x0b\x32\x35.yamcs.protobuf.filetransfer.FileTransferCapabilities\x12H\n\x0ftransferOptions\x18\x06 \x03(\x0b\x32/.yamcs.protobuf.filetransfer.FileTransferOption\"&\n\nEntityInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\"\xdc\x04\n\x0cTransferInfo\x12\n\n\x02id\x18\x01 \x01(\x04\x12-\n\tstartTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x05state\x18\x03 \x01(\x0e\x32*.yamcs.protobuf.filetransfer.TransferState\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\x12\x12\n\nobjectName\x18\x05 \x01(\t\x12\x12\n\nremotePath\x18\x06 \x01(\t\x12\x41\n\tdirection\x18\x07 \x01(\x0e\x32..yamcs.protobuf.filetransfer.TransferDirection\x12\x11\n\ttotalSize\x18\x08 \x01(\x04\x12\x17\n\x0fsizeTransferred\x18\t \x01(\x04\x12\x10\n\x08reliable\x18\n \x01(\x08\x12\x15\n\rfailureReason\x18\x0b \x01(\t\x12\x41\n\rtransactionId\x18\x0c \x01(\x0b\x32*.yamcs.protobuf.filetransfer.TransactionId\x12\x30\n\x0c\x63reationTime\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0ctransferType\x18\x0e \x01(\t\x12<\n\x0blocalEntity\x18\x0f \x01(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12=\n\x0cremoteEntity\x18\x10 \x01(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\"\x88\x02\n\x15\x43reateTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x08 \x01(\t\x12\x41\n\tdirection\x18\x02 \x01(\x0e\x32..yamcs.protobuf.filetransfer.TransferDirection\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x12\n\nobjectName\x18\x04 \x01(\t\x12\x12\n\nremotePath\x18\x05 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x13\n\x0b\x64\x65stination\x18\n \x01(\t\x12(\n\x07options\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\"I\n\x14PauseTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"J\n\x15\x43\x61ncelTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"J\n\x15ResumeTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"=\n\x14ListTransfersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"G\n\x12GetTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"U\n\x15ListTransfersResponse\x12<\n\ttransfers\x18\x01 \x03(\x0b\x32).yamcs.protobuf.filetransfer.TransferInfo\"B\n\x19SubscribeTransfersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"\x9c\x01\n\x10ListFilesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65stination\x18\x04 \x01(\t\x12\x12\n\nremotePath\x18\x05 \x01(\t\x12(\n\x07options\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa8\x01\n\nRemoteFile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x05 \x01(\t\x12\x13\n\x0bisDirectory\x18\x02 \x01(\x08\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12,\n\x08modified\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05\x65xtra\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xb1\x01\n\x11ListFilesResponse\x12\x36\n\x05\x66iles\x18\x01 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.RemoteFile\x12\x13\n\x0b\x64\x65stination\x18\x02 \x01(\t\x12\x12\n\nremotePath\x18\x03 \x01(\t\x12,\n\x08listTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05state\x18\x05 \x01(\t\"\xef\x02\n\x12\x46ileTransferOption\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x04type\x18\x02 \x01(\x0e\x32\x34.yamcs.protobuf.filetransfer.FileTransferOption.Type\x12\r\n\x05title\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x16\n\x0e\x61ssociatedText\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x06 \x01(\t\x12\x45\n\x06values\x18\x07 \x03(\x0b\x32\x35.yamcs.protobuf.filetransfer.FileTransferOption.Value\x12\x19\n\x11\x61llowCustomOption\x18\x08 \x01(\x08\x1a+\n\x05Value\x12\r\n\x05value\x18\x01 \x01(\t\x12\x13\n\x0bverboseName\x18\x02 \x01(\t\"+\n\x04Type\x12\x0b\n\x07\x42OOLEAN\x10\x00\x12\n\n\x06\x44OUBLE\x10\x01\x12\n\n\x06STRING\x10\x02*-\n\x11TransferDirection\x12\n\n\x06UPLOAD\x10\x01\x12\x0c\n\x08\x44OWNLOAD\x10\x02*_\n\rTransferState\x12\x0b\n\x07RUNNING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\r\n\tCOMPLETED\x10\x04\x12\n\n\x06QUEUED\x10\x05\x12\x0e\n\nCANCELLING\x10\x06\x32\x9c\x10\n\x0f\x46ileTransferApi\x12\xc4\x01\n\x18ListFileTransferServices\x12<.yamcs.protobuf.filetransfer.ListFileTransferServicesRequest\x1a=.yamcs.protobuf.filetransfer.ListFileTransferServicesResponse\"+\x8a\x92\x03\'\n%/api/filetransfer/{instance}/services\x12\xc5\x01\n\x16GetFileTransferService\x12:.yamcs.protobuf.filetransfer.GetFileTransferServiceRequest\x1a\x34.yamcs.protobuf.filetransfer.FileTransferServiceInfo\"9\x8a\x92\x03\x35\n3/api/filetransfer/{instance}/services/{serviceName}\x12\xb2\x01\n\rListTransfers\x12\x31.yamcs.protobuf.filetransfer.ListTransfersRequest\x1a\x32.yamcs.protobuf.filetransfer.ListTransfersResponse\":\x8a\x92\x03\x36\n4/api/filetransfer/{instance}/{serviceName}/transfers\x12\xaa\x01\n\x0bGetTransfer\x12/.yamcs.protobuf.filetransfer.GetTransferRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"?\x8a\x92\x03;\n9/api/filetransfer/{instance}/{serviceName}/transfers/{id}\x12\xae\x01\n\x0e\x43reateTransfer\x12\x32.yamcs.protobuf.filetransfer.CreateTransferRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"=\x8a\x92\x03\x39\x1a\x34/api/filetransfer/{instance}/{serviceName}/transfers:\x01*\x12\xa1\x01\n\rPauseTransfer\x12\x31.yamcs.protobuf.filetransfer.PauseTransferRequest\x1a\x16.google.protobuf.Empty\"E\x8a\x92\x03\x41\x1a?/api/filetransfer/{instance}/{serviceName}/transfers/{id}:pause\x12\xa4\x01\n\x0e\x43\x61ncelTransfer\x12\x32.yamcs.protobuf.filetransfer.CancelTransferRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a@/api/filetransfer/{instance}/{serviceName}/transfers/{id}:cancel\x12\xa4\x01\n\x0eResumeTransfer\x12\x32.yamcs.protobuf.filetransfer.ResumeTransferRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a@/api/filetransfer/{instance}/{serviceName}/transfers/{id}:resume\x12\x8f\x01\n\x12SubscribeTransfers\x12\x36.yamcs.protobuf.filetransfer.SubscribeTransfersRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"\x14\xda\x92\x03\x10\n\x0e\x66ile-transfers0\x01\x12\x9b\x01\n\x17SubscribeRemoteFileList\x12\x36.yamcs.protobuf.filetransfer.SubscribeTransfersRequest\x1a..yamcs.protobuf.filetransfer.ListFilesResponse\"\x16\xda\x92\x03\x12\n\x10remote-file-list0\x01\x12\x96\x01\n\rFetchFileList\x12-.yamcs.protobuf.filetransfer.ListFilesRequest\x1a\x16.google.protobuf.Empty\">\x8a\x92\x03:\x1a\x35/api/filetransfer/{instance}/{serviceName}/files:sync:\x01*\x12\xab\x01\n\x0bGetFileList\x12-.yamcs.protobuf.filetransfer.ListFilesRequest\x1a..yamcs.protobuf.filetransfer.ListFilesResponse\"=\x8a\x92\x03\x39\n0/api/filetransfer/{instance}/{serviceName}/filesR\x05\x66ilesB)\n\x12org.yamcs.protobufB\x11\x46ileTransferProtoP\x01'
+  serialized_pb=b'\n.yamcs/protobuf/filetransfer/filetransfer.proto\x12\x1byamcs.protobuf.filetransfer\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1byamcs/api/annotations.proto\x1a$yamcs/protobuf/actions/actions.proto\"@\n\rTransactionId\x12\x16\n\x0esequenceNumber\x18\x01 \x01(\r\x12\x17\n\x0finitiatorEntity\x18\x02 \x01(\x04\"3\n\x1fListFileTransferServicesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"F\n\x1dGetFileTransferServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"j\n ListFileTransferServicesResponse\x12\x46\n\x08services\x18\x01 \x03(\x0b\x32\x34.yamcs.protobuf.filetransfer.FileTransferServiceInfo\"\x80\x02\n\x18\x46ileTransferCapabilities\x12\x0e\n\x06upload\x18\x01 \x01(\x08\x12\x10\n\x08\x64ownload\x18\x02 \x01(\x08\x12\x12\n\nremotePath\x18\x04 \x01(\x08\x12\x10\n\x08\x66ileList\x18\x05 \x01(\x08\x12\x17\n\x0fhasTransferType\x18\x06 \x01(\x08\x12J\n\x14\x66ileListExtraColumns\x18\x07 \x03(\x0b\x32,.yamcs.protobuf.filetransfer.ExtraColumnInfo\x12\x37\n\x0b\x66ileActions\x18\x08 \x03(\x0b\x32\".yamcs.protobuf.actions.ActionInfo\",\n\x0f\x45xtraColumnInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\xd1\x02\n\x17\x46ileTransferServiceInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\rlocalEntities\x18\x03 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12?\n\x0eremoteEntities\x18\x04 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12K\n\x0c\x63\x61pabilities\x18\x05 \x01(\x0b\x32\x35.yamcs.protobuf.filetransfer.FileTransferCapabilities\x12H\n\x0ftransferOptions\x18\x06 \x03(\x0b\x32/.yamcs.protobuf.filetransfer.FileTransferOption\"&\n\nEntityInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\"\xdc\x04\n\x0cTransferInfo\x12\n\n\x02id\x18\x01 \x01(\x04\x12-\n\tstartTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x05state\x18\x03 \x01(\x0e\x32*.yamcs.protobuf.filetransfer.TransferState\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\x12\x12\n\nobjectName\x18\x05 \x01(\t\x12\x12\n\nremotePath\x18\x06 \x01(\t\x12\x41\n\tdirection\x18\x07 \x01(\x0e\x32..yamcs.protobuf.filetransfer.TransferDirection\x12\x11\n\ttotalSize\x18\x08 \x01(\x04\x12\x17\n\x0fsizeTransferred\x18\t \x01(\x04\x12\x10\n\x08reliable\x18\n \x01(\x08\x12\x15\n\rfailureReason\x18\x0b \x01(\t\x12\x41\n\rtransactionId\x18\x0c \x01(\x0b\x32*.yamcs.protobuf.filetransfer.TransactionId\x12\x30\n\x0c\x63reationTime\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0ctransferType\x18\x0e \x01(\t\x12<\n\x0blocalEntity\x18\x0f \x01(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\x12=\n\x0cremoteEntity\x18\x10 \x01(\x0b\x32\'.yamcs.protobuf.filetransfer.EntityInfo\"\x88\x02\n\x15\x43reateTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x08 \x01(\t\x12\x41\n\tdirection\x18\x02 \x01(\x0e\x32..yamcs.protobuf.filetransfer.TransferDirection\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x12\n\nobjectName\x18\x04 \x01(\t\x12\x12\n\nremotePath\x18\x05 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x13\n\x0b\x64\x65stination\x18\n \x01(\t\x12(\n\x07options\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\"I\n\x14PauseTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"J\n\x15\x43\x61ncelTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"J\n\x15ResumeTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"=\n\x14ListTransfersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"G\n\x12GetTransferRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\"U\n\x15ListTransfersResponse\x12<\n\ttransfers\x18\x01 \x03(\x0b\x32).yamcs.protobuf.filetransfer.TransferInfo\"B\n\x19SubscribeTransfersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\"\x9c\x01\n\x10ListFilesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65stination\x18\x04 \x01(\t\x12\x12\n\nremotePath\x18\x05 \x01(\t\x12(\n\x07options\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xa8\x01\n\nRemoteFile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x05 \x01(\t\x12\x13\n\x0bisDirectory\x18\x02 \x01(\x08\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12,\n\x08modified\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05\x65xtra\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xb1\x01\n\x11ListFilesResponse\x12\x36\n\x05\x66iles\x18\x01 \x03(\x0b\x32\'.yamcs.protobuf.filetransfer.RemoteFile\x12\x13\n\x0b\x64\x65stination\x18\x02 \x01(\t\x12\x12\n\nremotePath\x18\x03 \x01(\t\x12,\n\x08listTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05state\x18\x05 \x01(\t\"\x9b\x01\n\x14RunFileActionRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x13\n\x0bserviceName\x18\x02 \x01(\t\x12\x14\n\x0cremoteEntity\x18\x03 \x01(\t\x12\x0c\n\x04\x66ile\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\x12(\n\x07message\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xef\x02\n\x12\x46ileTransferOption\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x04type\x18\x02 \x01(\x0e\x32\x34.yamcs.protobuf.filetransfer.FileTransferOption.Type\x12\r\n\x05title\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x16\n\x0e\x61ssociatedText\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x06 \x01(\t\x12\x45\n\x06values\x18\x07 \x03(\x0b\x32\x35.yamcs.protobuf.filetransfer.FileTransferOption.Value\x12\x19\n\x11\x61llowCustomOption\x18\x08 \x01(\x08\x1a+\n\x05Value\x12\r\n\x05value\x18\x01 \x01(\t\x12\x13\n\x0bverboseName\x18\x02 \x01(\t\"+\n\x04Type\x12\x0b\n\x07\x42OOLEAN\x10\x00\x12\n\n\x06\x44OUBLE\x10\x01\x12\n\n\x06STRING\x10\x02*-\n\x11TransferDirection\x12\n\n\x06UPLOAD\x10\x01\x12\x0c\n\x08\x44OWNLOAD\x10\x02*_\n\rTransferState\x12\x0b\n\x07RUNNING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\r\n\tCOMPLETED\x10\x04\x12\n\n\x06QUEUED\x10\x05\x12\x0e\n\nCANCELLING\x10\x06\x32\xc3\x11\n\x0f\x46ileTransferApi\x12\xc4\x01\n\x18ListFileTransferServices\x12<.yamcs.protobuf.filetransfer.ListFileTransferServicesRequest\x1a=.yamcs.protobuf.filetransfer.ListFileTransferServicesResponse\"+\x8a\x92\x03\'\n%/api/filetransfer/{instance}/services\x12\xc5\x01\n\x16GetFileTransferService\x12:.yamcs.protobuf.filetransfer.GetFileTransferServiceRequest\x1a\x34.yamcs.protobuf.filetransfer.FileTransferServiceInfo\"9\x8a\x92\x03\x35\n3/api/filetransfer/{instance}/services/{serviceName}\x12\xb2\x01\n\rListTransfers\x12\x31.yamcs.protobuf.filetransfer.ListTransfersRequest\x1a\x32.yamcs.protobuf.filetransfer.ListTransfersResponse\":\x8a\x92\x03\x36\n4/api/filetransfer/{instance}/{serviceName}/transfers\x12\xaa\x01\n\x0bGetTransfer\x12/.yamcs.protobuf.filetransfer.GetTransferRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"?\x8a\x92\x03;\n9/api/filetransfer/{instance}/{serviceName}/transfers/{id}\x12\xae\x01\n\x0e\x43reateTransfer\x12\x32.yamcs.protobuf.filetransfer.CreateTransferRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"=\x8a\x92\x03\x39\x1a\x34/api/filetransfer/{instance}/{serviceName}/transfers:\x01*\x12\xa1\x01\n\rPauseTransfer\x12\x31.yamcs.protobuf.filetransfer.PauseTransferRequest\x1a\x16.google.protobuf.Empty\"E\x8a\x92\x03\x41\x1a?/api/filetransfer/{instance}/{serviceName}/transfers/{id}:pause\x12\xa4\x01\n\x0e\x43\x61ncelTransfer\x12\x32.yamcs.protobuf.filetransfer.CancelTransferRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a@/api/filetransfer/{instance}/{serviceName}/transfers/{id}:cancel\x12\xa4\x01\n\x0eResumeTransfer\x12\x32.yamcs.protobuf.filetransfer.ResumeTransferRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a@/api/filetransfer/{instance}/{serviceName}/transfers/{id}:resume\x12\x8f\x01\n\x12SubscribeTransfers\x12\x36.yamcs.protobuf.filetransfer.SubscribeTransfersRequest\x1a).yamcs.protobuf.filetransfer.TransferInfo\"\x14\xda\x92\x03\x10\n\x0e\x66ile-transfers0\x01\x12\x9b\x01\n\x17SubscribeRemoteFileList\x12\x36.yamcs.protobuf.filetransfer.SubscribeTransfersRequest\x1a..yamcs.protobuf.filetransfer.ListFilesResponse\"\x16\xda\x92\x03\x12\n\x10remote-file-list0\x01\x12\x96\x01\n\rFetchFileList\x12-.yamcs.protobuf.filetransfer.ListFilesRequest\x1a\x16.google.protobuf.Empty\">\x8a\x92\x03:\x1a\x35/api/filetransfer/{instance}/{serviceName}/files:sync:\x01*\x12\xab\x01\n\x0bGetFileList\x12-.yamcs.protobuf.filetransfer.ListFilesRequest\x1a..yamcs.protobuf.filetransfer.ListFilesResponse\"=\x8a\x92\x03\x39\n0/api/filetransfer/{instance}/{serviceName}/filesR\x05\x66iles\x12\xa4\x01\n\rRunFileAction\x12\x31.yamcs.protobuf.filetransfer.RunFileActionRequest\x1a\x17.google.protobuf.Struct\"G\x8a\x92\x03\x43\x1a>/api/filetransfer/{instance}/{serviceName}/files:runFileAction:\x01*B)\n\x12org.yamcs.protobufB\x11\x46ileTransferProtoP\x01'
   ,
-  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_struct__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_struct__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_actions_dot_actions__pb2.DESCRIPTOR,])
 
 _TRANSFERDIRECTION = _descriptor.EnumDescriptor(
   name='TransferDirection',
   full_name='yamcs.protobuf.filetransfer.TransferDirection',
   filename=None,
   file=DESCRIPTOR,
   values=[
@@ -40,16 +41,16 @@
     _descriptor.EnumValueDescriptor(
       name='DOWNLOAD', index=1, number=2,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3399,
-  serialized_end=3444,
+  serialized_start=3652,
+  serialized_end=3697,
 )
 _sym_db.RegisterEnumDescriptor(_TRANSFERDIRECTION)
 
 TransferDirection = enum_type_wrapper.EnumTypeWrapper(_TRANSFERDIRECTION)
 _TRANSFERSTATE = _descriptor.EnumDescriptor(
   name='TransferState',
   full_name='yamcs.protobuf.filetransfer.TransferState',
@@ -79,16 +80,16 @@
     _descriptor.EnumValueDescriptor(
       name='CANCELLING', index=5, number=6,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3446,
-  serialized_end=3541,
+  serialized_start=3699,
+  serialized_end=3794,
 )
 _sym_db.RegisterEnumDescriptor(_TRANSFERSTATE)
 
 TransferState = enum_type_wrapper.EnumTypeWrapper(_TRANSFERSTATE)
 UPLOAD = 1
 DOWNLOAD = 2
 RUNNING = 1
@@ -116,16 +117,16 @@
     _descriptor.EnumValueDescriptor(
       name='STRING', index=2, number=2,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3354,
-  serialized_end=3397,
+  serialized_start=3607,
+  serialized_end=3650,
 )
 _sym_db.RegisterEnumDescriptor(_FILETRANSFEROPTION_TYPE)
 
 
 _TRANSACTIONID = _descriptor.Descriptor(
   name='TransactionId',
   full_name='yamcs.protobuf.filetransfer.TransactionId',
@@ -155,16 +156,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=200,
-  serialized_end=264,
+  serialized_start=238,
+  serialized_end=302,
 )
 
 
 _LISTFILETRANSFERSERVICESREQUEST = _descriptor.Descriptor(
   name='ListFileTransferServicesRequest',
   full_name='yamcs.protobuf.filetransfer.ListFileTransferServicesRequest',
   filename=None,
@@ -186,16 +187,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=266,
-  serialized_end=317,
+  serialized_start=304,
+  serialized_end=355,
 )
 
 
 _GETFILETRANSFERSERVICEREQUEST = _descriptor.Descriptor(
   name='GetFileTransferServiceRequest',
   full_name='yamcs.protobuf.filetransfer.GetFileTransferServiceRequest',
   filename=None,
@@ -224,16 +225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=319,
-  serialized_end=389,
+  serialized_start=357,
+  serialized_end=427,
 )
 
 
 _LISTFILETRANSFERSERVICESRESPONSE = _descriptor.Descriptor(
   name='ListFileTransferServicesResponse',
   full_name='yamcs.protobuf.filetransfer.ListFileTransferServicesResponse',
   filename=None,
@@ -255,16 +256,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=391,
-  serialized_end=497,
+  serialized_start=429,
+  serialized_end=535,
 )
 
 
 _FILETRANSFERCAPABILITIES = _descriptor.Descriptor(
   name='FileTransferCapabilities',
   full_name='yamcs.protobuf.filetransfer.FileTransferCapabilities',
   filename=None,
@@ -309,28 +310,35 @@
     _descriptor.FieldDescriptor(
       name='fileListExtraColumns', full_name='yamcs.protobuf.filetransfer.FileTransferCapabilities.fileListExtraColumns', index=5,
       number=7, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='fileActions', full_name='yamcs.protobuf.filetransfer.FileTransferCapabilities.fileActions', index=6,
+      number=8, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=500,
-  serialized_end=699,
+  serialized_start=538,
+  serialized_end=794,
 )
 
 
 _EXTRACOLUMNINFO = _descriptor.Descriptor(
   name='ExtraColumnInfo',
   full_name='yamcs.protobuf.filetransfer.ExtraColumnInfo',
   filename=None,
@@ -359,16 +367,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=701,
-  serialized_end=745,
+  serialized_start=796,
+  serialized_end=840,
 )
 
 
 _FILETRANSFERSERVICEINFO = _descriptor.Descriptor(
   name='FileTransferServiceInfo',
   full_name='yamcs.protobuf.filetransfer.FileTransferServiceInfo',
   filename=None,
@@ -425,16 +433,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=748,
-  serialized_end=1085,
+  serialized_start=843,
+  serialized_end=1180,
 )
 
 
 _ENTITYINFO = _descriptor.Descriptor(
   name='EntityInfo',
   full_name='yamcs.protobuf.filetransfer.EntityInfo',
   filename=None,
@@ -463,16 +471,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1087,
-  serialized_end=1125,
+  serialized_start=1182,
+  serialized_end=1220,
 )
 
 
 _TRANSFERINFO = _descriptor.Descriptor(
   name='TransferInfo',
   full_name='yamcs.protobuf.filetransfer.TransferInfo',
   filename=None,
@@ -599,16 +607,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1128,
-  serialized_end=1732,
+  serialized_start=1223,
+  serialized_end=1827,
 )
 
 
 _CREATETRANSFERREQUEST = _descriptor.Descriptor(
   name='CreateTransferRequest',
   full_name='yamcs.protobuf.filetransfer.CreateTransferRequest',
   filename=None,
@@ -686,16 +694,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1735,
-  serialized_end=1999,
+  serialized_start=1830,
+  serialized_end=2094,
 )
 
 
 _PAUSETRANSFERREQUEST = _descriptor.Descriptor(
   name='PauseTransferRequest',
   full_name='yamcs.protobuf.filetransfer.PauseTransferRequest',
   filename=None,
@@ -731,16 +739,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2001,
-  serialized_end=2074,
+  serialized_start=2096,
+  serialized_end=2169,
 )
 
 
 _CANCELTRANSFERREQUEST = _descriptor.Descriptor(
   name='CancelTransferRequest',
   full_name='yamcs.protobuf.filetransfer.CancelTransferRequest',
   filename=None,
@@ -776,16 +784,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2076,
-  serialized_end=2150,
+  serialized_start=2171,
+  serialized_end=2245,
 )
 
 
 _RESUMETRANSFERREQUEST = _descriptor.Descriptor(
   name='ResumeTransferRequest',
   full_name='yamcs.protobuf.filetransfer.ResumeTransferRequest',
   filename=None,
@@ -821,16 +829,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2152,
-  serialized_end=2226,
+  serialized_start=2247,
+  serialized_end=2321,
 )
 
 
 _LISTTRANSFERSREQUEST = _descriptor.Descriptor(
   name='ListTransfersRequest',
   full_name='yamcs.protobuf.filetransfer.ListTransfersRequest',
   filename=None,
@@ -859,16 +867,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2228,
-  serialized_end=2289,
+  serialized_start=2323,
+  serialized_end=2384,
 )
 
 
 _GETTRANSFERREQUEST = _descriptor.Descriptor(
   name='GetTransferRequest',
   full_name='yamcs.protobuf.filetransfer.GetTransferRequest',
   filename=None,
@@ -904,16 +912,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2291,
-  serialized_end=2362,
+  serialized_start=2386,
+  serialized_end=2457,
 )
 
 
 _LISTTRANSFERSRESPONSE = _descriptor.Descriptor(
   name='ListTransfersResponse',
   full_name='yamcs.protobuf.filetransfer.ListTransfersResponse',
   filename=None,
@@ -935,16 +943,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2364,
-  serialized_end=2449,
+  serialized_start=2459,
+  serialized_end=2544,
 )
 
 
 _SUBSCRIBETRANSFERSREQUEST = _descriptor.Descriptor(
   name='SubscribeTransfersRequest',
   full_name='yamcs.protobuf.filetransfer.SubscribeTransfersRequest',
   filename=None,
@@ -973,16 +981,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2451,
-  serialized_end=2517,
+  serialized_start=2546,
+  serialized_end=2612,
 )
 
 
 _LISTFILESREQUEST = _descriptor.Descriptor(
   name='ListFilesRequest',
   full_name='yamcs.protobuf.filetransfer.ListFilesRequest',
   filename=None,
@@ -1039,16 +1047,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2520,
-  serialized_end=2676,
+  serialized_start=2615,
+  serialized_end=2771,
 )
 
 
 _REMOTEFILE = _descriptor.Descriptor(
   name='RemoteFile',
   full_name='yamcs.protobuf.filetransfer.RemoteFile',
   filename=None,
@@ -1105,16 +1113,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2679,
-  serialized_end=2847,
+  serialized_start=2774,
+  serialized_end=2942,
 )
 
 
 _LISTFILESRESPONSE = _descriptor.Descriptor(
   name='ListFilesResponse',
   full_name='yamcs.protobuf.filetransfer.ListFilesResponse',
   filename=None,
@@ -1164,16 +1172,82 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2850,
-  serialized_end=3027,
+  serialized_start=2945,
+  serialized_end=3122,
+)
+
+
+_RUNFILEACTIONREQUEST = _descriptor.Descriptor(
+  name='RunFileActionRequest',
+  full_name='yamcs.protobuf.filetransfer.RunFileActionRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='instance', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.instance', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='serviceName', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.serviceName', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='remoteEntity', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.remoteEntity', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='file', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.file', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='action', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.action', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='message', full_name='yamcs.protobuf.filetransfer.RunFileActionRequest.message', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3125,
+  serialized_end=3280,
 )
 
 
 _FILETRANSFEROPTION_VALUE = _descriptor.Descriptor(
   name='Value',
   full_name='yamcs.protobuf.filetransfer.FileTransferOption.Value',
   filename=None,
@@ -1202,16 +1276,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3309,
-  serialized_end=3352,
+  serialized_start=3562,
+  serialized_end=3605,
 )
 
 _FILETRANSFEROPTION = _descriptor.Descriptor(
   name='FileTransferOption',
   full_name='yamcs.protobuf.filetransfer.FileTransferOption',
   filename=None,
   file=DESCRIPTOR,
@@ -1282,20 +1356,21 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3030,
-  serialized_end=3397,
+  serialized_start=3283,
+  serialized_end=3650,
 )
 
 _LISTFILETRANSFERSERVICESRESPONSE.fields_by_name['services'].message_type = _FILETRANSFERSERVICEINFO
 _FILETRANSFERCAPABILITIES.fields_by_name['fileListExtraColumns'].message_type = _EXTRACOLUMNINFO
+_FILETRANSFERCAPABILITIES.fields_by_name['fileActions'].message_type = yamcs_dot_protobuf_dot_actions_dot_actions__pb2._ACTIONINFO
 _FILETRANSFERSERVICEINFO.fields_by_name['localEntities'].message_type = _ENTITYINFO
 _FILETRANSFERSERVICEINFO.fields_by_name['remoteEntities'].message_type = _ENTITYINFO
 _FILETRANSFERSERVICEINFO.fields_by_name['capabilities'].message_type = _FILETRANSFERCAPABILITIES
 _FILETRANSFERSERVICEINFO.fields_by_name['transferOptions'].message_type = _FILETRANSFEROPTION
 _TRANSFERINFO.fields_by_name['startTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TRANSFERINFO.fields_by_name['state'].enum_type = _TRANSFERSTATE
 _TRANSFERINFO.fields_by_name['direction'].enum_type = _TRANSFERDIRECTION
@@ -1307,14 +1382,15 @@
 _CREATETRANSFERREQUEST.fields_by_name['options'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
 _LISTTRANSFERSRESPONSE.fields_by_name['transfers'].message_type = _TRANSFERINFO
 _LISTFILESREQUEST.fields_by_name['options'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
 _REMOTEFILE.fields_by_name['modified'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _REMOTEFILE.fields_by_name['extra'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
 _LISTFILESRESPONSE.fields_by_name['files'].message_type = _REMOTEFILE
 _LISTFILESRESPONSE.fields_by_name['listTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_RUNFILEACTIONREQUEST.fields_by_name['message'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
 _FILETRANSFEROPTION_VALUE.containing_type = _FILETRANSFEROPTION
 _FILETRANSFEROPTION.fields_by_name['type'].enum_type = _FILETRANSFEROPTION_TYPE
 _FILETRANSFEROPTION.fields_by_name['values'].message_type = _FILETRANSFEROPTION_VALUE
 _FILETRANSFEROPTION_TYPE.containing_type = _FILETRANSFEROPTION
 DESCRIPTOR.message_types_by_name['TransactionId'] = _TRANSACTIONID
 DESCRIPTOR.message_types_by_name['ListFileTransferServicesRequest'] = _LISTFILETRANSFERSERVICESREQUEST
 DESCRIPTOR.message_types_by_name['GetFileTransferServiceRequest'] = _GETFILETRANSFERSERVICEREQUEST
@@ -1331,14 +1407,15 @@
 DESCRIPTOR.message_types_by_name['ListTransfersRequest'] = _LISTTRANSFERSREQUEST
 DESCRIPTOR.message_types_by_name['GetTransferRequest'] = _GETTRANSFERREQUEST
 DESCRIPTOR.message_types_by_name['ListTransfersResponse'] = _LISTTRANSFERSRESPONSE
 DESCRIPTOR.message_types_by_name['SubscribeTransfersRequest'] = _SUBSCRIBETRANSFERSREQUEST
 DESCRIPTOR.message_types_by_name['ListFilesRequest'] = _LISTFILESREQUEST
 DESCRIPTOR.message_types_by_name['RemoteFile'] = _REMOTEFILE
 DESCRIPTOR.message_types_by_name['ListFilesResponse'] = _LISTFILESRESPONSE
+DESCRIPTOR.message_types_by_name['RunFileActionRequest'] = _RUNFILEACTIONREQUEST
 DESCRIPTOR.message_types_by_name['FileTransferOption'] = _FILETRANSFEROPTION
 DESCRIPTOR.enum_types_by_name['TransferDirection'] = _TRANSFERDIRECTION
 DESCRIPTOR.enum_types_by_name['TransferState'] = _TRANSFERSTATE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 TransactionId = _reflection.GeneratedProtocolMessageType('TransactionId', (_message.Message,), {
   'DESCRIPTOR' : _TRANSACTIONID,
@@ -1476,14 +1553,21 @@
 ListFilesResponse = _reflection.GeneratedProtocolMessageType('ListFilesResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTFILESRESPONSE,
   '__module__' : 'yamcs.protobuf.filetransfer.filetransfer_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.filetransfer.ListFilesResponse)
   })
 _sym_db.RegisterMessage(ListFilesResponse)
 
+RunFileActionRequest = _reflection.GeneratedProtocolMessageType('RunFileActionRequest', (_message.Message,), {
+  'DESCRIPTOR' : _RUNFILEACTIONREQUEST,
+  '__module__' : 'yamcs.protobuf.filetransfer.filetransfer_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.filetransfer.RunFileActionRequest)
+  })
+_sym_db.RegisterMessage(RunFileActionRequest)
+
 FileTransferOption = _reflection.GeneratedProtocolMessageType('FileTransferOption', (_message.Message,), {
 
   'Value' : _reflection.GeneratedProtocolMessageType('Value', (_message.Message,), {
     'DESCRIPTOR' : _FILETRANSFEROPTION_VALUE,
     '__module__' : 'yamcs.protobuf.filetransfer.filetransfer_pb2'
     # @@protoc_insertion_point(class_scope:yamcs.protobuf.filetransfer.FileTransferOption.Value)
     })
@@ -1500,16 +1584,16 @@
 
 _FILETRANSFERAPI = _descriptor.ServiceDescriptor(
   name='FileTransferApi',
   full_name='yamcs.protobuf.filetransfer.FileTransferApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=3544,
-  serialized_end=5620,
+  serialized_start=3797,
+  serialized_end=6040,
   methods=[
   _descriptor.MethodDescriptor(
     name='ListFileTransferServices',
     full_name='yamcs.protobuf.filetransfer.FileTransferApi.ListFileTransferServices',
     index=0,
     containing_service=None,
     input_type=_LISTFILETRANSFERSERVICESREQUEST,
@@ -1611,13 +1695,22 @@
     full_name='yamcs.protobuf.filetransfer.FileTransferApi.GetFileList',
     index=11,
     containing_service=None,
     input_type=_LISTFILESREQUEST,
     output_type=_LISTFILESRESPONSE,
     serialized_options=b'\212\222\0039\n0/api/filetransfer/{instance}/{serviceName}/filesR\005files',
   ),
+  _descriptor.MethodDescriptor(
+    name='RunFileAction',
+    full_name='yamcs.protobuf.filetransfer.FileTransferApi.RunFileAction',
+    index=12,
+    containing_service=None,
+    input_type=_RUNFILEACTIONREQUEST,
+    output_type=google_dot_protobuf_dot_struct__pb2._STRUCT,
+    serialized_options=b'\212\222\003C\032>/api/filetransfer/{instance}/{serviceName}/files:runFileAction:\001*',
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_FILETRANSFERAPI)
 
 DESCRIPTOR.services_by_name['FileTransferApi'] = _FILETRANSFERAPI
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/iam/iam_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/iam/iam_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/iam/sessions_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/iam/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/instances/instances_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/instances/instances_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/links/links_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/links/links_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from yamcs.api import annotations_pb2 as yamcs_dot_api_dot_annotations__pb2
-from yamcs.protobuf.config import config_pb2 as yamcs_dot_protobuf_dot_config_dot_config__pb2
+from yamcs.protobuf.actions import actions_pb2 as yamcs_dot_protobuf_dot_actions_dot_actions__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/links/links.proto',
   package='yamcs.protobuf.links',
   syntax='proto2',
   serialized_options=b'\n\030org.yamcs.protobuf.linksB\021LinksServiceProtoP\001',
-  serialized_pb=b'\n yamcs/protobuf/links/links.proto\x12\x14yamcs.protobuf.links\x1a\x1byamcs/api/annotations.proto\x1a\"yamcs/protobuf/config/config.proto\x1a\x1cgoogle/protobuf/struct.proto\"$\n\x10ListLinksRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"B\n\x11ListLinksResponse\x12-\n\x05links\x18\x01 \x03(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfo\"0\n\x0eGetLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"3\n\x11\x45nableLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"4\n\x12\x44isableLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\":\n\x18ResetLinkCountersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"W\n\x0f\x45\x64itLinkRequest\x12\x10\n\x08instance\x18\x03 \x01(\t\x12\x0c\n\x04link\x18\x04 \x01(\t\x12\r\n\x05state\x18\x01 \x01(\t\x12\x15\n\rresetCounters\x18\x02 \x01(\x08\"l\n\x10RunActionRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12(\n\x07message\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xef\x01\n\tLinkEvent\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32$.yamcs.protobuf.links.LinkEvent.TypeB\x02\x18\x01\x12\x34\n\x08linkInfo\x18\x02 \x01(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfoB\x02\x18\x01\x12-\n\x05links\x18\x03 \x03(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfo\"E\n\x04Type\x12\x0e\n\nREGISTERED\x10\x01\x12\x10\n\x0cUNREGISTERED\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\x12\x0e\n\nUPDATE_ALL\x10\x04\")\n\x15SubscribeLinksRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\xbe\x02\n\x08LinkInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x10\n\x08\x64isabled\x18\x06 \x01(\x08\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x61taInCount\x18\n \x01(\x03\x12\x14\n\x0c\x64\x61taOutCount\x18\x0b \x01(\x03\x12\x16\n\x0e\x64\x65tailedStatus\x18\t \x01(\t\x12\x12\n\nparentName\x18\x0c \x01(\t\x12\x35\n\x07\x61\x63tions\x18\r \x03(\x0b\x32$.yamcs.protobuf.links.LinkActionInfo\x12&\n\x05\x65xtra\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x12\n\nparameters\x18\x0f \x03(\tJ\x04\x08\x05\x10\x06J\x04\x08\x08\x10\t\"\x8b\x01\n\x0eLinkActionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05style\x18\x03 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x04 \x01(\x08\x12\x0f\n\x07\x63hecked\x18\x05 \x01(\x08\x12-\n\x04spec\x18\x06 \x01(\x0b\x32\x1f.yamcs.protobuf.config.SpecInfo2\x8b\t\n\x08LinksApi\x12z\n\tListLinks\x12&.yamcs.protobuf.links.ListLinksRequest\x1a\'.yamcs.protobuf.links.ListLinksResponse\"\x1c\x8a\x92\x03\x18\n\x16/api/links/{instance?}\x12s\n\x07GetLink\x12$.yamcs.protobuf.links.GetLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"\"\x8a\x92\x03\x1e\n\x1c/api/links/{instance}/{link}\x12\x93\x01\n\nUpdateLink\x12%.yamcs.protobuf.links.EditLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\">\x8a\x92\x03:*\x1c/api/links/{instance}/{link}0\x01:\x01*b\x15Link \'{link}\' updated\x12\x97\x01\n\nEnableLink\x12\'.yamcs.protobuf.links.EnableLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"@\x8a\x92\x03<\x1a#/api/links/{instance}/{link}:enableb\x15Link \'{link}\' enabled\x12\x9b\x01\n\x0b\x44isableLink\x12(.yamcs.protobuf.links.DisableLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"B\x8a\x92\x03>\x1a$/api/links/{instance}/{link}:disableb\x16Link \'{link}\' disabled\x12\x95\x01\n\x11ResetLinkCounters\x12..yamcs.protobuf.links.ResetLinkCountersRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"0\x8a\x92\x03,\x1a*/api/links/{instance}/{link}:resetCounters\x12m\n\x0eSubscribeLinks\x12+.yamcs.protobuf.links.SubscribeLinksRequest\x1a\x1f.yamcs.protobuf.links.LinkEvent\"\x0b\xda\x92\x03\x07\n\x05links0\x01\x12\xb8\x01\n\tRunAction\x12&.yamcs.protobuf.links.RunActionRequest\x1a\x17.google.protobuf.Struct\"j\x8a\x92\x03\x66\x1a-/api/links/{instance}/{link}/actions/{action}:\x07messageb,Action \'{action}\' performed on link \'{link}\'B/\n\x18org.yamcs.protobuf.linksB\x11LinksServiceProtoP\x01'
+  serialized_pb=b'\n yamcs/protobuf/links/links.proto\x12\x14yamcs.protobuf.links\x1a\x1byamcs/api/annotations.proto\x1a$yamcs/protobuf/actions/actions.proto\x1a\x1cgoogle/protobuf/struct.proto\"$\n\x10ListLinksRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"B\n\x11ListLinksResponse\x12-\n\x05links\x18\x01 \x03(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfo\"0\n\x0eGetLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"3\n\x11\x45nableLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"4\n\x12\x44isableLinkRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\":\n\x18ResetLinkCountersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\"W\n\x0f\x45\x64itLinkRequest\x12\x10\n\x08instance\x18\x03 \x01(\t\x12\x0c\n\x04link\x18\x04 \x01(\t\x12\r\n\x05state\x18\x01 \x01(\t\x12\x15\n\rresetCounters\x18\x02 \x01(\x08\"l\n\x10RunActionRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04link\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12(\n\x07message\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xef\x01\n\tLinkEvent\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32$.yamcs.protobuf.links.LinkEvent.TypeB\x02\x18\x01\x12\x34\n\x08linkInfo\x18\x02 \x01(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfoB\x02\x18\x01\x12-\n\x05links\x18\x03 \x03(\x0b\x32\x1e.yamcs.protobuf.links.LinkInfo\"E\n\x04Type\x12\x0e\n\nREGISTERED\x10\x01\x12\x10\n\x0cUNREGISTERED\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\x12\x0e\n\nUPDATE_ALL\x10\x04\")\n\x15SubscribeLinksRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\xbc\x02\n\x08LinkInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x10\n\x08\x64isabled\x18\x06 \x01(\x08\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x61taInCount\x18\n \x01(\x03\x12\x14\n\x0c\x64\x61taOutCount\x18\x0b \x01(\x03\x12\x16\n\x0e\x64\x65tailedStatus\x18\t \x01(\t\x12\x12\n\nparentName\x18\x0c \x01(\t\x12\x33\n\x07\x61\x63tions\x18\r \x03(\x0b\x32\".yamcs.protobuf.actions.ActionInfo\x12&\n\x05\x65xtra\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x12\n\nparameters\x18\x0f \x03(\tJ\x04\x08\x05\x10\x06J\x04\x08\x08\x10\t2\x8b\t\n\x08LinksApi\x12z\n\tListLinks\x12&.yamcs.protobuf.links.ListLinksRequest\x1a\'.yamcs.protobuf.links.ListLinksResponse\"\x1c\x8a\x92\x03\x18\n\x16/api/links/{instance?}\x12s\n\x07GetLink\x12$.yamcs.protobuf.links.GetLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"\"\x8a\x92\x03\x1e\n\x1c/api/links/{instance}/{link}\x12\x93\x01\n\nUpdateLink\x12%.yamcs.protobuf.links.EditLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\">\x8a\x92\x03:*\x1c/api/links/{instance}/{link}0\x01:\x01*b\x15Link \'{link}\' updated\x12\x97\x01\n\nEnableLink\x12\'.yamcs.protobuf.links.EnableLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"@\x8a\x92\x03<\x1a#/api/links/{instance}/{link}:enableb\x15Link \'{link}\' enabled\x12\x9b\x01\n\x0b\x44isableLink\x12(.yamcs.protobuf.links.DisableLinkRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"B\x8a\x92\x03>\x1a$/api/links/{instance}/{link}:disableb\x16Link \'{link}\' disabled\x12\x95\x01\n\x11ResetLinkCounters\x12..yamcs.protobuf.links.ResetLinkCountersRequest\x1a\x1e.yamcs.protobuf.links.LinkInfo\"0\x8a\x92\x03,\x1a*/api/links/{instance}/{link}:resetCounters\x12m\n\x0eSubscribeLinks\x12+.yamcs.protobuf.links.SubscribeLinksRequest\x1a\x1f.yamcs.protobuf.links.LinkEvent\"\x0b\xda\x92\x03\x07\n\x05links0\x01\x12\xb8\x01\n\tRunAction\x12&.yamcs.protobuf.links.RunActionRequest\x1a\x17.google.protobuf.Struct\"j\x8a\x92\x03\x66\x1a-/api/links/{instance}/{link}/actions/{action}:\x07messageb,Action \'{action}\' performed on link \'{link}\'B/\n\x18org.yamcs.protobuf.linksB\x11LinksServiceProtoP\x01'
   ,
-  dependencies=[yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_config_dot_config__pb2.DESCRIPTOR,google_dot_protobuf_dot_struct__pb2.DESCRIPTOR,])
+  dependencies=[yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_actions_dot_actions__pb2.DESCRIPTOR,google_dot_protobuf_dot_struct__pb2.DESCRIPTOR,])
 
 
 
 _LINKEVENT_TYPE = _descriptor.EnumDescriptor(
   name='Type',
   full_name='yamcs.protobuf.links.LinkEvent.Type',
   filename=None,
@@ -48,16 +48,16 @@
     _descriptor.EnumValueDescriptor(
       name='UPDATE_ALL', index=3, number=4,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=846,
-  serialized_end=915,
+  serialized_start=848,
+  serialized_end=917,
 )
 _sym_db.RegisterEnumDescriptor(_LINKEVENT_TYPE)
 
 
 _LISTLINKSREQUEST = _descriptor.Descriptor(
   name='ListLinksRequest',
   full_name='yamcs.protobuf.links.ListLinksRequest',
@@ -80,16 +80,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=153,
-  serialized_end=189,
+  serialized_start=155,
+  serialized_end=191,
 )
 
 
 _LISTLINKSRESPONSE = _descriptor.Descriptor(
   name='ListLinksResponse',
   full_name='yamcs.protobuf.links.ListLinksResponse',
   filename=None,
@@ -111,16 +111,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=191,
-  serialized_end=257,
+  serialized_start=193,
+  serialized_end=259,
 )
 
 
 _GETLINKREQUEST = _descriptor.Descriptor(
   name='GetLinkRequest',
   full_name='yamcs.protobuf.links.GetLinkRequest',
   filename=None,
@@ -149,16 +149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=259,
-  serialized_end=307,
+  serialized_start=261,
+  serialized_end=309,
 )
 
 
 _ENABLELINKREQUEST = _descriptor.Descriptor(
   name='EnableLinkRequest',
   full_name='yamcs.protobuf.links.EnableLinkRequest',
   filename=None,
@@ -187,16 +187,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=309,
-  serialized_end=360,
+  serialized_start=311,
+  serialized_end=362,
 )
 
 
 _DISABLELINKREQUEST = _descriptor.Descriptor(
   name='DisableLinkRequest',
   full_name='yamcs.protobuf.links.DisableLinkRequest',
   filename=None,
@@ -225,16 +225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=362,
-  serialized_end=414,
+  serialized_start=364,
+  serialized_end=416,
 )
 
 
 _RESETLINKCOUNTERSREQUEST = _descriptor.Descriptor(
   name='ResetLinkCountersRequest',
   full_name='yamcs.protobuf.links.ResetLinkCountersRequest',
   filename=None,
@@ -263,16 +263,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=416,
-  serialized_end=474,
+  serialized_start=418,
+  serialized_end=476,
 )
 
 
 _EDITLINKREQUEST = _descriptor.Descriptor(
   name='EditLinkRequest',
   full_name='yamcs.protobuf.links.EditLinkRequest',
   filename=None,
@@ -315,16 +315,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=476,
-  serialized_end=563,
+  serialized_start=478,
+  serialized_end=565,
 )
 
 
 _RUNACTIONREQUEST = _descriptor.Descriptor(
   name='RunActionRequest',
   full_name='yamcs.protobuf.links.RunActionRequest',
   filename=None,
@@ -367,16 +367,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=565,
-  serialized_end=673,
+  serialized_start=567,
+  serialized_end=675,
 )
 
 
 _LINKEVENT = _descriptor.Descriptor(
   name='LinkEvent',
   full_name='yamcs.protobuf.links.LinkEvent',
   filename=None,
@@ -413,16 +413,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=676,
-  serialized_end=915,
+  serialized_start=678,
+  serialized_end=917,
 )
 
 
 _SUBSCRIBELINKSREQUEST = _descriptor.Descriptor(
   name='SubscribeLinksRequest',
   full_name='yamcs.protobuf.links.SubscribeLinksRequest',
   filename=None,
@@ -444,16 +444,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=917,
-  serialized_end=958,
+  serialized_start=919,
+  serialized_end=960,
 )
 
 
 _LINKINFO = _descriptor.Descriptor(
   name='LinkInfo',
   full_name='yamcs.protobuf.links.LinkInfo',
   filename=None,
@@ -559,105 +559,37 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=961,
+  serialized_start=963,
   serialized_end=1279,
 )
 
-
-_LINKACTIONINFO = _descriptor.Descriptor(
-  name='LinkActionInfo',
-  full_name='yamcs.protobuf.links.LinkActionInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='id', full_name='yamcs.protobuf.links.LinkActionInfo.id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='label', full_name='yamcs.protobuf.links.LinkActionInfo.label', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='style', full_name='yamcs.protobuf.links.LinkActionInfo.style', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='enabled', full_name='yamcs.protobuf.links.LinkActionInfo.enabled', index=3,
-      number=4, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='checked', full_name='yamcs.protobuf.links.LinkActionInfo.checked', index=4,
-      number=5, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='spec', full_name='yamcs.protobuf.links.LinkActionInfo.spec', index=5,
-      number=6, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1282,
-  serialized_end=1421,
-)
-
 _LISTLINKSRESPONSE.fields_by_name['links'].message_type = _LINKINFO
 _RUNACTIONREQUEST.fields_by_name['message'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
 _LINKEVENT.fields_by_name['type'].enum_type = _LINKEVENT_TYPE
 _LINKEVENT.fields_by_name['linkInfo'].message_type = _LINKINFO
 _LINKEVENT.fields_by_name['links'].message_type = _LINKINFO
 _LINKEVENT_TYPE.containing_type = _LINKEVENT
-_LINKINFO.fields_by_name['actions'].message_type = _LINKACTIONINFO
+_LINKINFO.fields_by_name['actions'].message_type = yamcs_dot_protobuf_dot_actions_dot_actions__pb2._ACTIONINFO
 _LINKINFO.fields_by_name['extra'].message_type = google_dot_protobuf_dot_struct__pb2._STRUCT
-_LINKACTIONINFO.fields_by_name['spec'].message_type = yamcs_dot_protobuf_dot_config_dot_config__pb2._SPECINFO
 DESCRIPTOR.message_types_by_name['ListLinksRequest'] = _LISTLINKSREQUEST
 DESCRIPTOR.message_types_by_name['ListLinksResponse'] = _LISTLINKSRESPONSE
 DESCRIPTOR.message_types_by_name['GetLinkRequest'] = _GETLINKREQUEST
 DESCRIPTOR.message_types_by_name['EnableLinkRequest'] = _ENABLELINKREQUEST
 DESCRIPTOR.message_types_by_name['DisableLinkRequest'] = _DISABLELINKREQUEST
 DESCRIPTOR.message_types_by_name['ResetLinkCountersRequest'] = _RESETLINKCOUNTERSREQUEST
 DESCRIPTOR.message_types_by_name['EditLinkRequest'] = _EDITLINKREQUEST
 DESCRIPTOR.message_types_by_name['RunActionRequest'] = _RUNACTIONREQUEST
 DESCRIPTOR.message_types_by_name['LinkEvent'] = _LINKEVENT
 DESCRIPTOR.message_types_by_name['SubscribeLinksRequest'] = _SUBSCRIBELINKSREQUEST
 DESCRIPTOR.message_types_by_name['LinkInfo'] = _LINKINFO
-DESCRIPTOR.message_types_by_name['LinkActionInfo'] = _LINKACTIONINFO
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 ListLinksRequest = _reflection.GeneratedProtocolMessageType('ListLinksRequest', (_message.Message,), {
   'DESCRIPTOR' : _LISTLINKSREQUEST,
   '__module__' : 'yamcs.protobuf.links.links_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.links.ListLinksRequest)
   })
@@ -729,34 +661,27 @@
 LinkInfo = _reflection.GeneratedProtocolMessageType('LinkInfo', (_message.Message,), {
   'DESCRIPTOR' : _LINKINFO,
   '__module__' : 'yamcs.protobuf.links.links_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.links.LinkInfo)
   })
 _sym_db.RegisterMessage(LinkInfo)
 
-LinkActionInfo = _reflection.GeneratedProtocolMessageType('LinkActionInfo', (_message.Message,), {
-  'DESCRIPTOR' : _LINKACTIONINFO,
-  '__module__' : 'yamcs.protobuf.links.links_pb2'
-  # @@protoc_insertion_point(class_scope:yamcs.protobuf.links.LinkActionInfo)
-  })
-_sym_db.RegisterMessage(LinkActionInfo)
-
 
 DESCRIPTOR._options = None
 _LINKEVENT.fields_by_name['type']._options = None
 _LINKEVENT.fields_by_name['linkInfo']._options = None
 
 _LINKSAPI = _descriptor.ServiceDescriptor(
   name='LinksApi',
   full_name='yamcs.protobuf.links.LinksApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1424,
-  serialized_end=2587,
+  serialized_start=1282,
+  serialized_end=2445,
   methods=[
   _descriptor.MethodDescriptor(
     name='ListLinks',
     full_name='yamcs.protobuf.links.LinksApi.ListLinks',
     index=0,
     containing_service=None,
     input_type=_LISTLINKSREQUEST,
```

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/mdb/mdb_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/mdb/mdb_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/packets/packets_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/packets/packets_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/plists/plists_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/plists/plists_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/processing/mdb_override_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/processing/mdb_override_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/processing/processing_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/processing/processing_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/pvalue/pvalue_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/pvalue/pvalue.proto',
   package='yamcs.protobuf.pvalue',
   syntax='proto2',
   serialized_options=b'\n\022org.yamcs.protobuf',
-  serialized_pb=b'\n\"yamcs/protobuf/pvalue/pvalue.proto\x12\x15yamcs.protobuf.pvalue\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb8\x04\n\x0eParameterValue\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\'\n\x08rawValue\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\'\n\x08\x65ngValue\x18\x03 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x33\n\x0f\x61\x63quisitionTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0egenerationTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x11\x61\x63quisitionStatus\x18\x06 \x01(\x0e\x32(.yamcs.protobuf.pvalue.AcquisitionStatus\x12\x1c\n\x10processingStatus\x18\x07 \x01(\x08\x42\x02\x18\x01\x12\x41\n\x10monitoringResult\x18\x08 \x01(\x0e\x32\'.yamcs.protobuf.pvalue.MonitoringResult\x12=\n\x0erangeCondition\x18\t \x01(\x0e\x32%.yamcs.protobuf.pvalue.RangeCondition\x12\x32\n\nalarmRange\x18\x19 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12\x14\n\x0c\x65xpireMillis\x18\x1a \x01(\x03\x12\x11\n\tnumericId\x18\x1b \x01(\r\"\xa2\x02\n\x0fParameterStatus\x12\x43\n\x11\x61\x63quisitionStatus\x18\x01 \x01(\x0e\x32(.yamcs.protobuf.pvalue.AcquisitionStatus\x12\x41\n\x10monitoringResult\x18\x02 \x01(\x0e\x32\'.yamcs.protobuf.pvalue.MonitoringResult\x12=\n\x0erangeCondition\x18\x03 \x01(\x0e\x32%.yamcs.protobuf.pvalue.RangeCondition\x12\x32\n\nalarmRange\x18\x04 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12\x14\n\x0c\x65xpireMillis\x18\x05 \x01(\x03\"\x98\x01\n\rParameterData\x12\x38\n\tparameter\x18\x01 \x03(\x0b\x32%.yamcs.protobuf.pvalue.ParameterValue\x12\r\n\x05group\x18\x02 \x01(\t\x12\x16\n\x0egenerationTime\x18\x03 \x01(\x03\x12\x0e\n\x06seqNum\x18\x04 \x01(\x05\x12\x16\n\x0esubscriptionId\x18\x05 \x01(\x05\"\x9f\x02\n\nTimeSeries\x12\x38\n\x06sample\x18\x01 \x03(\x0b\x32(.yamcs.protobuf.pvalue.TimeSeries.Sample\x1a\xd6\x01\n\x06Sample\x12\x16\n\ntimeString\x18\x01 \x01(\tB\x02\x18\x01\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03\x61vg\x18\x02 \x01(\x01\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\t\n\x01n\x18\x05 \x01(\x05\x12+\n\x07minTime\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07maxTime\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x91\x02\n\x06Ranges\x12\x32\n\x05range\x18\x01 \x03(\x0b\x32#.yamcs.protobuf.pvalue.Ranges.Range\x1a\xd2\x01\n\x05Range\x12)\n\x05start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\ttimeStart\x18\x01 \x01(\tB\x02\x18\x01\x12\x14\n\x08timeStop\x18\x02 \x01(\tB\x02\x18\x01\x12\r\n\x05\x63ount\x18\x04 \x01(\x05\x12(\n\tengValues\x18\x05 \x03(\x0b\x32\x15.yamcs.protobuf.Value\x12\x0e\n\x06\x63ounts\x18\x06 \x03(\x05*M\n\x11\x41\x63quisitionStatus\x12\x0c\n\x08\x41\x43QUIRED\x10\x00\x12\x10\n\x0cNOT_RECEIVED\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03*o\n\x10MonitoringResult\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\r\n\tIN_LIMITS\x10\x01\x12\t\n\x05WATCH\x10\x07\x12\x0b\n\x07WARNING\x10\n\x12\x0c\n\x08\x44ISTRESS\x10\r\x12\x0c\n\x08\x43RITICAL\x10\x10\x12\n\n\x06SEVERE\x10\x13*#\n\x0eRangeCondition\x12\x07\n\x03LOW\x10\x00\x12\x08\n\x04HIGH\x10\x01\x42\x14\n\x12org.yamcs.protobuf'
+  serialized_pb=b'\n\"yamcs/protobuf/pvalue/pvalue.proto\x12\x15yamcs.protobuf.pvalue\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb8\x04\n\x0eParameterValue\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\'\n\x08rawValue\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\'\n\x08\x65ngValue\x18\x03 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x33\n\x0f\x61\x63quisitionTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0egenerationTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x11\x61\x63quisitionStatus\x18\x06 \x01(\x0e\x32(.yamcs.protobuf.pvalue.AcquisitionStatus\x12\x1c\n\x10processingStatus\x18\x07 \x01(\x08\x42\x02\x18\x01\x12\x41\n\x10monitoringResult\x18\x08 \x01(\x0e\x32\'.yamcs.protobuf.pvalue.MonitoringResult\x12=\n\x0erangeCondition\x18\t \x01(\x0e\x32%.yamcs.protobuf.pvalue.RangeCondition\x12\x32\n\nalarmRange\x18\x19 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12\x14\n\x0c\x65xpireMillis\x18\x1a \x01(\x03\x12\x11\n\tnumericId\x18\x1b \x01(\r\"\xa2\x02\n\x0fParameterStatus\x12\x43\n\x11\x61\x63quisitionStatus\x18\x01 \x01(\x0e\x32(.yamcs.protobuf.pvalue.AcquisitionStatus\x12\x41\n\x10monitoringResult\x18\x02 \x01(\x0e\x32\'.yamcs.protobuf.pvalue.MonitoringResult\x12=\n\x0erangeCondition\x18\x03 \x01(\x0e\x32%.yamcs.protobuf.pvalue.RangeCondition\x12\x32\n\nalarmRange\x18\x04 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12\x14\n\x0c\x65xpireMillis\x18\x05 \x01(\x03\"\x98\x01\n\rParameterData\x12\x38\n\tparameter\x18\x01 \x03(\x0b\x32%.yamcs.protobuf.pvalue.ParameterValue\x12\r\n\x05group\x18\x02 \x01(\t\x12\x16\n\x0egenerationTime\x18\x03 \x01(\x03\x12\x0e\n\x06seqNum\x18\x04 \x01(\x05\x12\x16\n\x0esubscriptionId\x18\x05 \x01(\x05\"\x87\x02\n\nTimeSeries\x12\x38\n\x06sample\x18\x01 \x03(\x0b\x32(.yamcs.protobuf.pvalue.TimeSeries.Sample\x1a\xbe\x01\n\x06Sample\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03\x61vg\x18\x02 \x01(\x01\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\t\n\x01n\x18\x05 \x01(\x05\x12+\n\x07minTime\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07maxTime\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe4\x01\n\x06Ranges\x12\x32\n\x05range\x18\x01 \x03(\x0b\x32#.yamcs.protobuf.pvalue.Ranges.Range\x1a\xa5\x01\n\x05Range\x12)\n\x05start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x63ount\x18\x04 \x01(\x05\x12(\n\tengValues\x18\x05 \x03(\x0b\x32\x15.yamcs.protobuf.Value\x12\x0e\n\x06\x63ounts\x18\x06 \x03(\x05*M\n\x11\x41\x63quisitionStatus\x12\x0c\n\x08\x41\x43QUIRED\x10\x00\x12\x10\n\x0cNOT_RECEIVED\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03*o\n\x10MonitoringResult\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\r\n\tIN_LIMITS\x10\x01\x12\t\n\x05WATCH\x10\x07\x12\x0b\n\x07WARNING\x10\n\x12\x0c\n\x08\x44ISTRESS\x10\r\x12\x0c\n\x08\x43RITICAL\x10\x10\x12\n\n\x06SEVERE\x10\x13*#\n\x0eRangeCondition\x12\x07\n\x03LOW\x10\x00\x12\x08\n\x04HIGH\x10\x01\x42\x14\n\x12org.yamcs.protobuf'
   ,
   dependencies=[yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_mdb_dot_mdb__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 _ACQUISITIONSTATUS = _descriptor.EnumDescriptor(
   name='AcquisitionStatus',
   full_name='yamcs.protobuf.pvalue.AcquisitionStatus',
   filename=None,
@@ -47,16 +47,16 @@
     _descriptor.EnumValueDescriptor(
       name='EXPIRED', index=3, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1737,
-  serialized_end=1814,
+  serialized_start=1668,
+  serialized_end=1745,
 )
 _sym_db.RegisterEnumDescriptor(_ACQUISITIONSTATUS)
 
 AcquisitionStatus = enum_type_wrapper.EnumTypeWrapper(_ACQUISITIONSTATUS)
 _MONITORINGRESULT = _descriptor.EnumDescriptor(
   name='MonitoringResult',
   full_name='yamcs.protobuf.pvalue.MonitoringResult',
@@ -90,16 +90,16 @@
     _descriptor.EnumValueDescriptor(
       name='SEVERE', index=6, number=19,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1816,
-  serialized_end=1927,
+  serialized_start=1747,
+  serialized_end=1858,
 )
 _sym_db.RegisterEnumDescriptor(_MONITORINGRESULT)
 
 MonitoringResult = enum_type_wrapper.EnumTypeWrapper(_MONITORINGRESULT)
 _RANGECONDITION = _descriptor.EnumDescriptor(
   name='RangeCondition',
   full_name='yamcs.protobuf.pvalue.RangeCondition',
@@ -113,16 +113,16 @@
     _descriptor.EnumValueDescriptor(
       name='HIGH', index=1, number=1,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1929,
-  serialized_end=1964,
+  serialized_start=1860,
+  serialized_end=1895,
 )
 _sym_db.RegisterEnumDescriptor(_RANGECONDITION)
 
 RangeCondition = enum_type_wrapper.EnumTypeWrapper(_RANGECONDITION)
 ACQUIRED = 0
 NOT_RECEIVED = 1
 INVALID = 2
@@ -369,64 +369,57 @@
   name='Sample',
   full_name='yamcs.protobuf.pvalue.TimeSeries.Sample',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='timeString', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.timeString', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='time', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.time', index=1,
+      name='time', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.time', index=0,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='avg', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.avg', index=2,
+      name='avg', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.avg', index=1,
       number=2, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='min', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.min', index=3,
+      name='min', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.min', index=2,
       number=3, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='max', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.max', index=4,
+      name='max', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.max', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='n', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.n', index=5,
+      name='n', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.n', index=4,
       number=5, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='minTime', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.minTime', index=6,
+      name='minTime', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.minTime', index=5,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='maxTime', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.maxTime', index=7,
+      name='maxTime', full_name='yamcs.protobuf.pvalue.TimeSeries.Sample.maxTime', index=6,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -437,15 +430,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1245,
-  serialized_end=1459,
+  serialized_end=1435,
 )
 
 _TIMESERIES = _descriptor.Descriptor(
   name='TimeSeries',
   full_name='yamcs.protobuf.pvalue.TimeSeries',
   filename=None,
   file=DESCRIPTOR,
@@ -467,15 +460,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1172,
-  serialized_end=1459,
+  serialized_end=1435,
 )
 
 
 _RANGES_RANGE = _descriptor.Descriptor(
   name='Range',
   full_name='yamcs.protobuf.pvalue.Ranges.Range',
   filename=None,
@@ -493,43 +486,29 @@
       name='stop', full_name='yamcs.protobuf.pvalue.Ranges.Range.stop', index=1,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='timeStart', full_name='yamcs.protobuf.pvalue.Ranges.Range.timeStart', index=2,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='timeStop', full_name='yamcs.protobuf.pvalue.Ranges.Range.timeStop', index=3,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='count', full_name='yamcs.protobuf.pvalue.Ranges.Range.count', index=4,
+      name='count', full_name='yamcs.protobuf.pvalue.Ranges.Range.count', index=2,
       number=4, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='engValues', full_name='yamcs.protobuf.pvalue.Ranges.Range.engValues', index=5,
+      name='engValues', full_name='yamcs.protobuf.pvalue.Ranges.Range.engValues', index=3,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='counts', full_name='yamcs.protobuf.pvalue.Ranges.Range.counts', index=6,
+      name='counts', full_name='yamcs.protobuf.pvalue.Ranges.Range.counts', index=4,
       number=6, type=5, cpp_type=1, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -539,16 +518,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1525,
-  serialized_end=1735,
+  serialized_start=1501,
+  serialized_end=1666,
 )
 
 _RANGES = _descriptor.Descriptor(
   name='Ranges',
   full_name='yamcs.protobuf.pvalue.Ranges',
   filename=None,
   file=DESCRIPTOR,
@@ -569,16 +548,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1462,
-  serialized_end=1735,
+  serialized_start=1438,
+  serialized_end=1666,
 )
 
 _PARAMETERVALUE.fields_by_name['id'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._NAMEDOBJECTID
 _PARAMETERVALUE.fields_by_name['rawValue'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._VALUE
 _PARAMETERVALUE.fields_by_name['engValue'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._VALUE
 _PARAMETERVALUE.fields_by_name['acquisitionTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PARAMETERVALUE.fields_by_name['generationTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -661,11 +640,8 @@
   })
 _sym_db.RegisterMessage(Ranges)
 _sym_db.RegisterMessage(Ranges.Range)
 
 
 DESCRIPTOR._options = None
 _PARAMETERVALUE.fields_by_name['processingStatus']._options = None
-_TIMESERIES_SAMPLE.fields_by_name['timeString']._options = None
-_RANGES_RANGE.fields_by_name['timeStart']._options = None
-_RANGES_RANGE.fields_by_name['timeStop']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/replication/replication_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/replication/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/server/server_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/server/server_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/services/services_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/services/services_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/services/services_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/services/services_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/table/table_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/table/table_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/tco/tco_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/tco/tco_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/time/time_service_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/time/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/timeline/timeline_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/timeline/timeline_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/protobuf/yamcs_pb2.py` & `yamcs_client-1.9.6/src/yamcs/protobuf/yamcs_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/storage/client.py` & `yamcs_client-1.9.6/src/yamcs/storage/client.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/storage/model.py` & `yamcs_client-1.9.6/src/yamcs/storage/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import datetime
-from typing import IO, List, Mapping, Optional, Union
+from typing import IO, TYPE_CHECKING, List, Mapping, Optional, Union
 
 from yamcs.core.helpers import parse_server_time
 
+if TYPE_CHECKING:
+    from yamcs.storage.client import StorageClient
+
 
 class Bucket:
-    def __init__(self, proto, storage_client):
+    def __init__(self, proto, storage_client: "StorageClient"):
         self._proto = proto
         self._storage_client = storage_client
 
     @property
     def name(self) -> str:
         """Name of this bucket."""
         return self._proto.name
 
     @property
-    def created(self) -> Optional[datetime.datetime]:
+    def created(self) -> datetime.datetime:
         """
         When this bucket was created.
         """
-        if self._proto.HasField("created"):
-            return parse_server_time(self._proto.created)
-        return None
+        return parse_server_time(self._proto.created)
 
     @property
     def object_count(self) -> int:
         """Number of objects in this bucket."""
         return self._proto.numObjects
 
     @property
@@ -157,21 +158,19 @@
     def size(self) -> int:
         """
         Size in bytes of this object (excluding metadata).
         """
         return self._proto.size
 
     @property
-    def created(self) -> Optional[datetime.datetime]:
+    def created(self) -> datetime.datetime:
         """
         Return when this object was created (or re-created).
         """
-        if self._proto.HasField("created"):
-            return parse_server_time(self._proto.created)
-        return None
+        return parse_server_time(self._proto.created)
 
     def delete(self):
         """
         Remove this object.
         """
         self._storage_client.remove_object(self._bucket, self.name)
```

### Comparing `yamcs-client-1.9.5/src/yamcs/tco/client.py` & `yamcs_client-1.9.6/src/yamcs/tco/client.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/tco/model.py` & `yamcs_client-1.9.6/src/yamcs/tco/model.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/timeline/client.py` & `yamcs_client-1.9.6/src/yamcs/timeline/client.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/timeline/model.py` & `yamcs_client-1.9.6/src/yamcs/timeline/model.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.9.5/src/yamcs/tmtc/client.py` & `yamcs_client-1.9.6/src/yamcs/tmtc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,27 +389,29 @@
     """
     Local object providing access to the acknowledgment progress
     of command updates.
 
     Only commands issued from this object are monitored.
     """
 
-    def __init__(self, manager, tmtc_client):
+    def __init__(self, manager, tmtc_client: "ProcessorClient"):
         super(CommandConnection, self).__init__(manager)
         self._cmdhist_cache = {}
         self._command_cache = {}
         self._tmtc_client = tmtc_client
 
     def issue(
         self,
         command: str,
         args: Optional[Mapping[str, Any]] = None,
+        *,
         dry_run: bool = False,
         comment: Optional[str] = None,
         verification: Optional[VerificationConfig] = None,
+        stream: Optional[str] = None,
         extra: Optional[Mapping[str, Any]] = None,
         sequence_number: Optional[int] = None,
     ) -> MonitoredCommand:
         """
         Issue the given command
 
         :param command:
@@ -421,14 +423,18 @@
             If ``True`` the command is not actually issued. This can be used
             to test if the server would generate errors when preparing the
             command (for example because an argument is missing).
         :param comment:
             Comment attached to the command.
         :param verification:
             Overrides to the default verification handling of this command.
+        :param stream:
+            Override the stream on which the command should be sent out.
+
+            .. versionadded:: 1.9.6
         :param extra:
             Extra command options for interpretation by non-core extensions
             (custom preprocessor, datalinks, command listeners). Note that
             Yamcs will refuse command options that it does now know about.
             Extensions should therefore register available options.
         :param sequence_number:
             Sequence number of this command. This is used to determine unicity
@@ -439,20 +445,21 @@
             .. versionadded:: 1.9.0
 
         :return:
             An object providing access to properties of the newly issued
             command and updated according to command history updates.
         """
         issued_command = self._tmtc_client.issue_command(
-            command,
-            args,
-            dry_run,
-            comment,
-            verification,
-            extra,
+            command=command,
+            args=args,
+            dry_run=dry_run,
+            comment=comment,
+            verification=verification,
+            stream=stream,
+            extra=extra,
             sequence_number=sequence_number,
         )
         cmd = MonitoredCommand(issued_command._proto)
 
         self._command_cache[cmd.id] = cmd
 
         # It may be that we already received some cmdhist updates
@@ -684,17 +691,19 @@
         url = f"/processors/{self._instance}/{self._processor}/parameters:batchSet"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
     def issue_command(
         self,
         command: str,
         args: Optional[Mapping[str, Any]] = None,
+        *,
         dry_run: bool = False,
         comment: Optional[str] = None,
         verification: Optional[VerificationConfig] = None,
+        stream: Optional[str] = None,
         extra: Optional[Mapping[str, Any]] = None,
         sequence_number: Optional[int] = None,
     ) -> IssuedCommand:
         """
         Issue the given command
 
         :param command:
@@ -706,14 +715,18 @@
             If ``True`` the command is not actually issued. This can be used
             to test if the server would generate errors when preparing the
             command (for example because an argument is missing).
         :param comment:
             Comment attached to the command.
         :param verification:
             Overrides to the default verification handling of this command.
+        :param stream:
+            Override the stream on which the command should be sent out.
+
+            .. versionadded:: 1.9.6
         :param extra:
             Extra command options for interpretation by non-core
             extensions (custom preprocessor, datalinks, command listeners).
             Note that Yamcs will refuse command options that it does now know
             about. Extensions should therefore register available options.
         :param sequence_number:
             Sequence number of this command. This is used
@@ -733,14 +746,16 @@
         if comment:
             req.comment = comment
         if sequence_number is not None:
             req.sequenceNumber = sequence_number
         if args:
             for key in args:
                 req.args[key] = to_argument_value(args[key], force_string=True)
+        if stream:
+            req.stream = stream
 
         if verification:
             if verification._disable_all:
                 req.disableVerifiers = True
             else:
                 for verifier in verification._disabled:
                     req.verifierConfig[verifier].disable = True
@@ -816,15 +831,15 @@
         url = f"/processors/{self._instance}/{self._processor}/alarms"
         response = self.ctx.get_proto(path=url, params=params)
         message = alarms_service_pb2.ListAlarmsResponse()
         message.ParseFromString(response.content)
         alarms = getattr(message, "alarms")
         return iter([_parse_alarm(alarm) for alarm in alarms])
 
-    def set_default_calibrator(self, parameter: str, type: str, data):
+    def set_default_calibrator(self, parameter: str, type: Optional[str], data):
         """
         Apply a calibrator while processing raw values of the specified
         parameter. If there is already a default calibrator associated
         to this parameter, that calibrator gets replaced.
 
         .. note::
```

### Comparing `yamcs-client-1.9.5/src/yamcs/tmtc/model.py` & `yamcs_client-1.9.6/src/yamcs/tmtc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1066,17 +1066,15 @@
     @property
     def link(self) -> str:
         """
         Name of the Yamcs link where this packet was received from.
 
         .. versionadded:: 1.9.1
         """
-        if self._proto.HasField("link"):
-            return self._proto.link
-        return None
+        return self._proto.link
 
     @property
     def binary(self) -> bytes:
         """
         Raw binary of this packet
         """
         if self._proto.HasField("packet"):
```

### Comparing `yamcs-client-1.9.5/src/yamcs_client.egg-info/PKG-INFO` & `yamcs_client-1.9.6/src/yamcs_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.5
+Version: 1.9.6
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs-client-1.9.5/src/yamcs_client.egg-info/SOURCES.txt` & `yamcs_client-1.9.6/src/yamcs_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/yamcs/link/__init__.py
 src/yamcs/link/client.py
 src/yamcs/link/model.py
 src/yamcs/mdb/__init__.py
 src/yamcs/mdb/client.py
 src/yamcs/mdb/model.py
 src/yamcs/protobuf/yamcs_pb2.py
+src/yamcs/protobuf/actions/actions_pb2.py
 src/yamcs/protobuf/activities/activities_pb2.py
 src/yamcs/protobuf/activities/activities_service_pb2.py
 src/yamcs/protobuf/alarms/alarms_pb2.py
 src/yamcs/protobuf/alarms/alarms_service_pb2.py
 src/yamcs/protobuf/archive/archive_pb2.py
 src/yamcs/protobuf/archive/index_service_pb2.py
 src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
```

