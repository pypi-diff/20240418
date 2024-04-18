# Comparing `tmp/fedn-0.9.0b1.tar.gz` & `tmp/fedn-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedn-0.9.0b1.tar", last modified: Mon Apr 15 08:31:46 2024, max compression
+gzip compressed data, was "fedn-0.9.0b2.tar", last modified: Mon Apr 15 12:06:13 2024, max compression
```

## Comparing `fedn-0.9.0b1.tar` & `fedn-0.9.0b2.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 08:31:46.397624 fedn-0.9.0b1/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-01-29 16:01:38.000000 fedn-0.9.0b1/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       80 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/main.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     8980 2024-04-15 08:28:35.000000 fedn-0.9.0b1/cli/run_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/cli/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/tests/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2024-01-29 16:01:38.000000 fedn-0.9.0b1/cli/tests/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3140 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3499 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3421 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/common/net/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2338 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24093 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    38027 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5115 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    20111 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/api/v1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/client_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10343 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/combiner_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18235 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/model_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13598 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/package_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9335 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/round_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9284 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/session_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12614 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/status_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13391 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/api/v1/validation_routes.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32914 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5827 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5967 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      633 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5323 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregator.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6744 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4353 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5905 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/aggregators/fedopt.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    26190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4694 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10314 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7239 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14861 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14347 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11363 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3564 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      591 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1343 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      421 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1153 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1634 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3220 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3897 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3943 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    30398 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/network/storage/statestore/stores/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/client_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/combiner_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/model_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/package_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/round_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/session_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/status_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/network/storage/statestore/stores/validation_store.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-01-29 16:01:38.000000 fedn-0.9.0b1/fedn/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9331 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/dispatcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4067 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/environment.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/flowercompat/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/flowercompat/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4767 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/flowercompat/client_app_adapter.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1132 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.397624 fedn-0.9.0b1/fedn/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:02.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3377 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4640 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/helpers/plugins/numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15799 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6033 2024-04-15 08:28:35.000000 fedn-0.9.0b1/fedn/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:31:46.393624 fedn-0.9.0b1/fedn.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3841 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       35 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/entry_points.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-01-29 16:02:31.000000 fedn-0.9.0b1/fedn.egg-info/not-zip-safe
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      235 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2024-04-15 08:31:46.000000 fedn-0.9.0b1/fedn.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-04-15 08:31:46.397624 fedn-0.9.0b1/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1294 2024-04-15 08:31:26.000000 fedn-0.9.0b1/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 12:06:13.729063 fedn-0.9.0b2/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-01-29 16:01:38.000000 fedn-0.9.0b2/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/cli/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       80 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/main.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     8980 2024-04-15 08:28:35.000000 fedn-0.9.0b2/cli/run_cmd.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/cli/tests/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/tests/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/tests/tests.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/certificate/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/certificate/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3140 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/certificate/certificate.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/certificate/certificatemanager.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3499 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/config.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/exceptions.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3421 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/log_config.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/net/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/net/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/api/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/api/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2338 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/auth.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    24093 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/client.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    38027 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/interface.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5115 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/network.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    19873 2024-04-15 12:05:57.000000 fedn-0.9.0b2/fedn/network/api/server.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/api/tests.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/api/v1/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    11190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/client_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10343 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/combiner_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    18235 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/model_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13598 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/package_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9335 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/round_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9284 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/session_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/shared.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    12614 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/status_routes.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13391 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/validation_routes.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/clients/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    33231 2024-04-15 09:34:49.000000 fedn-0.9.0b2/fedn/network/clients/client.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5827 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/clients/connect.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5967 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/clients/package.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      633 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/state.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/test_client.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/combiner/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/combiner/aggregators/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5323 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregator.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6744 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregatorbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4353 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/fedavg.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5905 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/fedopt.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    26190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/combiner.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/combiner_tests.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4694 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/connect.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10314 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/interfaces.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     7239 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/modelservice.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14861 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/roundhandler.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/config.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/controller/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/controller/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14347 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/controller/control.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    11363 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/controller/controlbase.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/grpc/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/grpc/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3564 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/auth.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/fedn_pb2.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/fedn_pb2_grpc.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/server.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/loadbalancer/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      591 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/firstavailable.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1343 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/leastpacked.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      421 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/loadbalancerbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1153 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/state.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/__init__.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/models/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/memorymodelstorage.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1634 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/modelstorage.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3220 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/models/tempmodelstorage.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/s3/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/s3/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/s3/base.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3897 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/s3/miniorepository.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3943 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/s3/repository.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/statestore/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/statestore/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    30398 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/mongostatestore.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/statestore/statestorebase.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/statestore/stores/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/client_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/combiner_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/model_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/package_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/round_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/session_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/shared.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/status_store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/store.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/validation_store.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/utils/checksum.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     9331 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/dispatcher.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4067 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/environment.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/flowercompat/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/flowercompat/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4767 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/flowercompat/client_app_adapter.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/helpers/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/helperbase.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1132 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/helpers.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/helpers/plugins/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3377 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/androidhelper.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4640 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/numpyhelper.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    15799 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/plots.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6033 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/process.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3841 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       35 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/entry_points.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-01-29 16:02:31.000000 fedn-0.9.0b2/fedn.egg-info/not-zip-safe
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      233 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/top_level.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-04-15 12:06:13.729063 fedn-0.9.0b2/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-04-15 12:06:06.000000 fedn-0.9.0b2/setup.py
```

### Comparing `fedn-0.9.0b1/PKG-INFO` & `fedn-0.9.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Scaleout Federated Learning
 Home-page: https://www.scaleoutsystems.com
 Author: Scaleout Systems AB
 Author-email: contact@scaleoutsystems.com
 License: Apache 2.0
 Keywords: Federated learning
 Platform: UNKNOWN
```

### Comparing `fedn-0.9.0b1/cli/run_cmd.py` & `fedn-0.9.0b2/cli/run_cmd.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/cli/tests/tests.py` & `fedn-0.9.0b2/cli/tests/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/common/certificate/certificate.py` & `fedn-0.9.0b2/fedn/common/certificate/certificate.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/common/certificate/certificatemanager.py` & `fedn-0.9.0b2/fedn/common/certificate/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/common/config.py` & `fedn-0.9.0b2/fedn/common/config.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/common/log_config.py` & `fedn-0.9.0b2/fedn/common/log_config.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/auth.py` & `fedn-0.9.0b2/fedn/network/api/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/client.py` & `fedn-0.9.0b2/fedn/network/api/client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/interface.py` & `fedn-0.9.0b2/fedn/network/api/interface.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/network.py` & `fedn-0.9.0b2/fedn/network/api/network.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/server.py` & `fedn-0.9.0b2/fedn/network/api/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-from flasgger import Swagger
 from flask import Flask, jsonify, request
 
 from fedn.common.config import (get_controller_config, get_modelstorage_config,
                                 get_network_config, get_statestore_config)
 from fedn.network.api.auth import jwt_auth_required
 from fedn.network.api.interface import API
 from fedn.network.api.v1 import _routes
@@ -24,25 +23,14 @@
 for bp in _routes:
     app.register_blueprint(bp)
     if custom_url_prefix:
         app.register_blueprint(bp,
                                name=f"{bp.name}_custom",
                                url_prefix=f"{custom_url_prefix}{bp.url_prefix}")
 
-template = {
-    "swagger": "2.0",
-    "info": {
-        "title": "FEDn API",
-        "description": "API for the FEDn network.",
-        "version": "0.0.1"
-    }
-}
-
-swagger = Swagger(app, template=template)
-
 
 @app.route('/health', methods=["GET"])
 def health_check():
     return 'OK', 200
 
 
 if custom_url_prefix:
```

### Comparing `fedn-0.9.0b1/fedn/network/api/tests.py` & `fedn-0.9.0b2/fedn/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/__init__.py` & `fedn-0.9.0b2/fedn/network/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/client_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/client_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/combiner_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/combiner_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/model_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/model_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/package_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/package_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/round_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/round_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/session_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/session_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/shared.py` & `fedn-0.9.0b2/fedn/network/api/v1/shared.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/status_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/status_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/api/v1/validation_routes.py` & `fedn-0.9.0b2/fedn/network/api/v1/validation_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/clients/client.py` & `fedn-0.9.0b2/fedn/network/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,22 +94,22 @@
 
         self.inbox = queue.Queue()
 
         # Attach to the FEDn network (get combiner)
         combiner_config = self.assign()
         self.connect(combiner_config)
 
-        self._initialize_dispatcher(config)
+        self._initialize_dispatcher(self.config)
 
         self._initialize_helper(combiner_config)
         if not self.helper:
             logger.warning("Failed to retrieve helper class settings: {}".format(
                 combiner_config))
 
-        self._subscribe_to_combiner(config)
+        self._subscribe_to_combiner(self.config)
 
         self.state = ClientState.idle
 
     def assign(self):
         """Contacts the controller and asks for combiner assignment.
 
         :return: A configuration dictionary containing connection information for combiner.
@@ -691,20 +691,14 @@
                     self.state = ClientState.idle
                     self.inbox.task_done()
             except queue.Empty:
                 pass
             except grpc.RpcError as e:
                 logger.critical(f"GRPC process_request: An error occurred during process request: {e}")
 
-    def _handle_combiner_failure(self):
-        """ Register failed combiner connection."""
-        self._missed_heartbeat += 1
-        if self._missed_heartbeat > self.config['reconnect_after_missed_heartbeat']:
-            self.disconnect()
-
     def _send_heartbeat(self, update_frequency=2.0):
         """Send a heartbeat to the combiner.
 
         :param update_frequency: The frequency of the heartbeat in seconds.
         :type update_frequency: float
         :return: None if the client is detached.
         :rtype: None
@@ -714,22 +708,26 @@
                 name=self.name, role=fedn.WORKER))
             try:
                 self.connectorStub.SendHeartbeat(heartbeat, metadata=self.metadata)
                 self._missed_heartbeat = 0
             except grpc.RpcError as e:
                 status_code = e.code()
                 if status_code == grpc.StatusCode.UNAVAILABLE:
-                    logger.warning("GRPC hearbeat: server unavailable during send heartbeat. Retrying.")
+                    self._missed_heartbeat += 1
+                    logger.error("GRPC hearbeat: combiner unavailable, retrying (attempt {}/{}).".format(self._missed_heartbeat,
+                                                                                                         self.config['reconnect_after_missed_heartbeat']))
+                    if self._missed_heartbeat > self.config['reconnect_after_missed_heartbeat']:
+                        self.disconnect()
                 if status_code == grpc.StatusCode.UNAUTHENTICATED:
                     details = e.details()
                     if details == 'Token expired':
-                        logger.warning("GRPC hearbeat: Token expired. Reconnecting.")
-                        self.detach()
+                        logger.error("GRPC hearbeat: Token expired. Disconnecting.")
+                        self.disconnect()
+                        sys.exit("Unauthorized. Token expired. Please obtain a new token.")
                 logger.debug(e)
-                self._handle_combiner_failure()
 
             time.sleep(update_frequency)
             if not self._connected:
                 logger.info("SendStatus: Client disconnected.")
                 return
 
     def send_status(self, msg, log_level=fedn.Status.INFO, type=None, request=None, sesssion_id: str = None):
@@ -785,15 +783,17 @@
                 time.sleep(1)
                 if cnt == 0:
                     logger.info("Client is active, waiting for model update requests.")
                     cnt = 1
                 if self.state != old_state:
                     logger.info("Client in {} state.".format(ClientStateToString(self.state)))
                 if not self._connected:
-                    logger.info("Detached from combiner.")
-                    # TODO: Implement a check/condition to ulitmately close down if too many reattachment attepts have failed. s
-                    self.attach()
+                    logger.warning("Client lost connection to combiner. Attempting to reconnect to FEDn network.")
+                    combiner_config = self.assign()
+                    self.connect(combiner_config)
                     self._subscribe_to_combiner(self.config)
+                    cnt = 0
                 if self.error_state:
-                    return
+                    logger.error("Client in error state. Terminiating.")
+                    sys.exit("Client in error state. Terminiating.")
         except KeyboardInterrupt:
             logger.info("Shutting down.")
```

### Comparing `fedn-0.9.0b1/fedn/network/clients/connect.py` & `fedn-0.9.0b2/fedn/network/clients/connect.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/clients/package.py` & `fedn-0.9.0b2/fedn/network/clients/package.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/clients/state.py` & `fedn-0.9.0b2/fedn/network/clients/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/clients/test_client.py` & `fedn-0.9.0b2/fedn/network/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregator.py` & `fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/aggregators/aggregatorbase.py` & `fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregatorbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/aggregators/fedavg.py` & `fedn-0.9.0b2/fedn/network/combiner/aggregators/fedavg.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/aggregators/fedopt.py` & `fedn-0.9.0b2/fedn/network/combiner/aggregators/fedopt.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/combiner.py` & `fedn-0.9.0b2/fedn/network/combiner/combiner.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/connect.py` & `fedn-0.9.0b2/fedn/network/combiner/connect.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/interfaces.py` & `fedn-0.9.0b2/fedn/network/combiner/interfaces.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/modelservice.py` & `fedn-0.9.0b2/fedn/network/combiner/modelservice.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/combiner/roundhandler.py` & `fedn-0.9.0b2/fedn/network/combiner/roundhandler.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/controller/control.py` & `fedn-0.9.0b2/fedn/network/controller/control.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/controller/controlbase.py` & `fedn-0.9.0b2/fedn/network/controller/controlbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/grpc/auth.py` & `fedn-0.9.0b2/fedn/network/grpc/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/grpc/fedn_pb2.py` & `fedn-0.9.0b2/fedn/network/grpc/fedn_pb2.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/grpc/fedn_pb2_grpc.py` & `fedn-0.9.0b2/fedn/network/grpc/fedn_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/grpc/server.py` & `fedn-0.9.0b2/fedn/network/grpc/server.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/loadbalancer/firstavailable.py` & `fedn-0.9.0b2/fedn/network/loadbalancer/firstavailable.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/loadbalancer/leastpacked.py` & `fedn-0.9.0b2/fedn/network/loadbalancer/leastpacked.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/state.py` & `fedn-0.9.0b2/fedn/network/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/models/memorymodelstorage.py` & `fedn-0.9.0b2/fedn/network/storage/models/memorymodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/models/modelstorage.py` & `fedn-0.9.0b2/fedn/network/storage/models/modelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/models/tempmodelstorage.py` & `fedn-0.9.0b2/fedn/network/storage/models/tempmodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/s3/base.py` & `fedn-0.9.0b2/fedn/network/storage/s3/base.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/s3/miniorepository.py` & `fedn-0.9.0b2/fedn/network/storage/s3/miniorepository.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/s3/repository.py` & `fedn-0.9.0b2/fedn/network/storage/s3/repository.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/mongostatestore.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/mongostatestore.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/statestorebase.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/statestorebase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/client_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/client_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/combiner_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/combiner_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/model_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/model_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/package_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/package_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/round_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/round_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/session_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/session_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/status_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/status_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/network/storage/statestore/stores/validation_store.py` & `fedn-0.9.0b2/fedn/network/storage/statestore/stores/validation_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/dispatcher.py` & `fedn-0.9.0b2/fedn/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/environment.py` & `fedn-0.9.0b2/fedn/utils/environment.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/flowercompat/client_app_adapter.py` & `fedn-0.9.0b2/fedn/utils/flowercompat/client_app_adapter.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/helpers/helperbase.py` & `fedn-0.9.0b2/fedn/utils/helpers/helperbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/helpers/helpers.py` & `fedn-0.9.0b2/fedn/utils/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/helpers/plugins/androidhelper.py` & `fedn-0.9.0b2/fedn/utils/helpers/plugins/androidhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/helpers/plugins/numpyhelper.py` & `fedn-0.9.0b2/fedn/utils/helpers/plugins/numpyhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/plots.py` & `fedn-0.9.0b2/fedn/utils/plots.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn/utils/process.py` & `fedn-0.9.0b2/fedn/utils/process.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/fedn.egg-info/PKG-INFO` & `fedn-0.9.0b2/fedn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Scaleout Federated Learning
 Home-page: https://www.scaleoutsystems.com
 Author: Scaleout Systems AB
 Author-email: contact@scaleoutsystems.com
 License: Apache 2.0
 Keywords: Federated learning
 Platform: UNKNOWN
```

### Comparing `fedn-0.9.0b1/fedn.egg-info/SOURCES.txt` & `fedn-0.9.0b2/fedn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b1/setup.py` & `fedn-0.9.0b2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='fedn',
-    version='0.9.0b1',
+    version='0.9.0b2',
     description="""Scaleout Federated Learning""",
     author='Scaleout Systems AB',
     author_email='contact@scaleoutsystems.com',
     url='https://www.scaleoutsystems.com',
     py_modules=['fedn'],
     python_requires='>=3.8,<3.12',
     install_requires=[
@@ -14,21 +14,21 @@
         "urllib3>=1.26.4",
         "minio",
         "grpcio~=1.60.0",
         "grpcio-tools~=1.60.0",
         "numpy>=1.21.6",
         "protobuf~=4.25.2",
         "pymongo",
-        "Flask",
+        "Flask==3.0.3",
         "pyjwt",
         "pyopenssl",
         "psutil",
-        "click==8.0.1",
+        "click==8.1.7",
         "grpcio-health-checking~=1.60.0",
-        "flasgger==0.9.5",
+        "pyyaml",
         "plotly",
         "virtualenv",
     ],
     extras_require={
         'flower': ["flwr==1.8.0"]
     },
     license='Apache 2.0',
```

