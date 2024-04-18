# Comparing `tmp/buildgrid-0.0.91.tar.gz` & `tmp/buildgrid-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.91.tar", last modified: Thu Apr 11 15:18:19 2024, max compression
+gzip compressed data, was "buildgrid-0.0.92.tar", last modified: Thu Apr 18 10:44:10 2024, max compression
```

## Comparing `buildgrid-0.0.91.tar` & `buildgrid-0.0.92.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.055489 buildgrid-0.0.91/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-11 15:17:48.000000 buildgrid-0.0.91/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-11 15:17:48.000000 buildgrid-0.0.91/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-11 15:17:48.000000 buildgrid-0.0.91/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-11 15:17:48.000000 buildgrid-0.0.91/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6336 2024-04-11 15:18:19.055489 buildgrid-0.0.91/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-11 15:17:48.000000 buildgrid-0.0.91/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.941489 buildgrid-0.0.91/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.943489 buildgrid-0.0.91/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.946489 buildgrid-0.0.91/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.947489 buildgrid-0.0.91/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.947489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.948489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.949489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.949489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.949489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.950489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.952489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.956489 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.956489 buildgrid-0.0.91/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.956489 buildgrid-0.0.91/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.956489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.957489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.957489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.959489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.959489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.961489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.962489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.964489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.965489 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.967489 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.967489 buildgrid-0.0.91/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.972489 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.972489 buildgrid-0.0.91/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.979489 buildgrid-0.0.91/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.981489 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.981489 buildgrid-0.0.91/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.981489 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.986489 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.987489 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.993489 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.995489 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.000489 buildgrid-0.0.91/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.000489 buildgrid-0.0.91/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.001489 buildgrid-0.0.91/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9520 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.002489 buildgrid-0.0.91/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.005489 buildgrid-0.0.91/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.009489 buildgrid-0.0.91/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.010489 buildgrid-0.0.91/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.012489 buildgrid-0.0.91/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     5944 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.014489 buildgrid-0.0.91/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.015489 buildgrid-0.0.91/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8848 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.015489 buildgrid-0.0.91/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.016489 buildgrid-0.0.91/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3971 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.017489 buildgrid-0.0.91/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21869 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    17643 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.020489 buildgrid-0.0.91/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.021489 buildgrid-0.0.91/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.022489 buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11305 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.022489 buildgrid-0.0.91/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18121 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.023489 buildgrid-0.0.91/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.025489 buildgrid-0.0.91/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7936 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.025489 buildgrid-0.0.91/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.026489 buildgrid-0.0.91/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.027489 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.032489 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    77301 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.033489 buildgrid-0.0.91/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.033489 buildgrid-0.0.91/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.034489 buildgrid-0.0.91/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.035489 buildgrid-0.0.91/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-11 15:17:48.000000 buildgrid-0.0.91/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.049489 buildgrid-0.0.91/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6336 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 15:18:18.000000 buildgrid-0.0.91/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.935489 buildgrid-0.0.91/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.040489 buildgrid-0.0.91/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-11 15:17:48.000000 buildgrid-0.0.91/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.040489 buildgrid-0.0.91/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.040489 buildgrid-0.0.91/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.042489 buildgrid-0.0.91/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-11 15:17:48.000000 buildgrid-0.0.91/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4292 2024-04-11 15:17:48.000000 buildgrid-0.0.91/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2024-04-11 15:18:19.056489 buildgrid-0.0.91/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-11 15:17:48.000000 buildgrid-0.0.91/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.045489 buildgrid-0.0.91/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:18.937489 buildgrid-0.0.91/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:18:19.048489 buildgrid-0.0.91/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-11 15:17:48.000000 buildgrid-0.0.91/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.959592 buildgrid-0.0.92/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-18 10:43:42.000000 buildgrid-0.0.92/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-18 10:43:42.000000 buildgrid-0.0.92/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-18 10:43:42.000000 buildgrid-0.0.92/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-18 10:43:42.000000 buildgrid-0.0.92/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6265 2024-04-18 10:44:10.959592 buildgrid-0.0.92/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-18 10:43:42.000000 buildgrid-0.0.92/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.855591 buildgrid-0.0.92/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.856591 buildgrid-0.0.92/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.859591 buildgrid-0.0.92/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.860591 buildgrid-0.0.92/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.860591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.861591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.861591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.864591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.867591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.867591 buildgrid-0.0.92/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.870591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.871591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.873591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.873591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.875591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.877591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.879591 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.879591 buildgrid-0.0.92/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.884591 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.885591 buildgrid-0.0.92/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.891591 buildgrid-0.0.92/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.893591 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.893591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.894591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.898591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.898591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.904591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.905591 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.910591 buildgrid-0.0.92/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.910591 buildgrid-0.0.92/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.911591 buildgrid-0.0.92/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9520 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.912591 buildgrid-0.0.92/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.915591 buildgrid-0.0.92/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.917591 buildgrid-0.0.92/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.918591 buildgrid-0.0.92/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.920591 buildgrid-0.0.92/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.922591 buildgrid-0.0.92/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.923591 buildgrid-0.0.92/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.923591 buildgrid-0.0.92/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.924591 buildgrid-0.0.92/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.925591 buildgrid-0.0.92/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21869 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    11124 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.927591 buildgrid-0.0.92/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.928591 buildgrid-0.0.92/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.929592 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.930591 buildgrid-0.0.92/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18121 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.931591 buildgrid-0.0.92/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.932592 buildgrid-0.0.92/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.933591 buildgrid-0.0.92/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.934591 buildgrid-0.0.92/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.934591 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.939592 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    78610 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.939592 buildgrid-0.0.92/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.940591 buildgrid-0.0.92/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.940591 buildgrid-0.0.92/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.941592 buildgrid-0.0.92/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.954592 buildgrid-0.0.92/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6265 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      995 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.850591 buildgrid-0.0.92/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.948592 buildgrid-0.0.92/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-18 10:43:42.000000 buildgrid-0.0.92/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-18 10:44:10.960592 buildgrid-0.0.92/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-18 10:43:42.000000 buildgrid-0.0.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.950592 buildgrid-0.0.92/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.851591 buildgrid-0.0.92/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.953592 buildgrid-0.0.92/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_utils.py
```

### Comparing `buildgrid-0.0.91/BuildGrid.doap` & `buildgrid-0.0.92/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/CONTRIBUTING.rst` & `buildgrid-0.0.92/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/LICENSE` & `buildgrid-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/PKG-INFO` & `buildgrid-0.0.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.91
+Version: 0.0.92
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -12,16 +12,16 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: dnspython
 Requires-Dist: grpcio-reflection>=1.62.0
 Requires-Dist: grpcio>=1.62.0
 Requires-Dist: janus>=0.6.2
-Requires-Dist: jinja2==3.0.3
-Requires-Dist: protobuf<4.24.0
+Requires-Dist: jinja2
+Requires-Dist: protobuf
 Requires-Dist: alembic
 Requires-Dist: Click
 Requires-Dist: SQLAlchemy[mypy]<2.0,>=1.4.24
 Requires-Dist: pydantic>2.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: jsonschema>=3.0.0
 Requires-Dist: lark-parser
@@ -39,19 +39,18 @@
 Provides-Extra: database
 Requires-Dist: psycopg2-binary; extra == "database"
 Provides-Extra: redis
 Requires-Dist: fakeredis>=2.10.1; extra == "redis"
 Requires-Dist: redis>=4.5.1; extra == "redis"
 Requires-Dist: hiredis; extra == "redis"
 Provides-Extra: docs
-Requires-Dist: Sphinx<7; extra == "docs"
+Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: cryptography>=38.0.0; extra == "tests"
 Requires-Dist: flaky; extra == "tests"
 Requires-Dist: flask; extra == "tests"
 Requires-Dist: flask-cors; extra == "tests"
 Requires-Dist: moto<4.1.12; extra == "tests"
```

### Comparing `buildgrid-0.0.91/README.rst` & `buildgrid-0.0.92/README.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/__init__.py` & `buildgrid-0.0.92/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/__init__.py` & `buildgrid-0.0.92/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/cli.py` & `buildgrid-0.0.92/buildgrid/_app/cli.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.92/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.92/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.92/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.92/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.92/buildgrid/_app/settings/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.92/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_enums.py` & `buildgrid-0.0.92/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_exceptions.py` & `buildgrid-0.0.92/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_types.py` & `buildgrid-0.0.92/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/_version.py` & `buildgrid-0.0.92/buildgrid/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.91"
+__version__ = "0.0.92"
```

### Comparing `buildgrid-0.0.91/buildgrid/browser/__init__.py` & `buildgrid-0.0.92/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/browser/app.py` & `buildgrid-0.0.92/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/browser/rest_api.py` & `buildgrid-0.0.92/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/browser/utils.py` & `buildgrid-0.0.92/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.92/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.92/buildgrid/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.92/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.92/buildgrid/cleanup/janitor/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.92/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.92/buildgrid/cleanup/janitor/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.92/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/__init__.py` & `buildgrid-0.0.92/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/actioncache.py` & `buildgrid-0.0.92/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/asset.py` & `buildgrid-0.0.92/buildgrid/client/asset.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.92/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/authentication.py` & `buildgrid-0.0.92/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/capabilities.py` & `buildgrid-0.0.92/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/cas.py` & `buildgrid-0.0.92/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/channel.py` & `buildgrid-0.0.92/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/interceptors.py` & `buildgrid-0.0.92/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/logstream.py` & `buildgrid-0.0.92/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/client/retrier.py` & `buildgrid-0.0.92/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/__init__.py` & `buildgrid-0.0.92/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/action_cache_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/lru_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.92/buildgrid/server/actioncache/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.92/buildgrid/server/bots/service.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,137 +10,134 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
-ActionCacheService
-==================
+BotsService
+=================
 
-Allows clients to manually query/update the action cache.
 """
 
 import logging
-from typing import Union, cast
+from typing import cast
 
 import grpc
+from google.protobuf import empty_pb2
 
-import buildgrid.server.context as context_module
-from buildgrid._exceptions import InvalidArgumentError, NotFoundError, RetriableError, StorageFullError
-from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import DESCRIPTOR as RE_DESCRIPTOR
-from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import (
-    ActionResult,
-    GetActionResultRequest,
-    UpdateActionResultRequest,
+from buildgrid._enums import BotStatus
+from buildgrid._exceptions import InvalidArgumentError
+from buildgrid._protos.google.devtools.remoteworkers.v1test2.bots_pb2 import DESCRIPTOR as BOTS_DESCRIPTOR
+from buildgrid._protos.google.devtools.remoteworkers.v1test2.bots_pb2 import (
+    BotSession,
+    CreateBotSessionRequest,
+    PostBotEventTempRequest,
+    UpdateBotSessionRequest,
 )
-from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2_grpc import (
-    ActionCacheServicer,
-    add_ActionCacheServicer_to_server,
+from buildgrid._protos.google.devtools.remoteworkers.v1test2.bots_pb2_grpc import (
+    BotsServicer,
+    add_BotsServicer_to_server,
 )
-from buildgrid.server.actioncache.caches.action_cache_abc import ActionCacheABC
-from buildgrid.server.actioncache.instance import ActionCache
 from buildgrid.server.auth.manager import authorize_unary_unary
+from buildgrid.server.bots.instance import BotsInterface
 from buildgrid.server.metrics_names import (
-    AC_CACHE_HITS_METRIC_NAME,
-    AC_CACHE_MISSES_METRIC_NAME,
-    AC_GET_ACTION_RESULT_TIME_METRIC_NAME,
-    AC_UPDATE_ACTION_RESULT_TIME_METRIC_NAME,
+    BOTS_CREATE_BOT_SESSION_TIME_METRIC_NAME,
+    BOTS_UPDATE_BOT_SESSION_TIME_METRIC_NAME,
 )
-from buildgrid.server.metrics_utils import DurationMetric, publish_counter_metric
-from buildgrid.server.request_metadata_utils import printable_request_metadata
+from buildgrid.server.metrics_utils import DurationMetric
 from buildgrid.server.servicer import InstancedServicer
-from buildgrid.server.utils.decorators import track_request_id
+from buildgrid.server.utils.context import CancellationContext
+from buildgrid.server.utils.decorators import handle_errors_unary_unary, track_request_id
 
 LOGGER = logging.getLogger(__name__)
 
 
-class ActionCacheService(ActionCacheServicer, InstancedServicer[Union[ActionCache, ActionCacheABC]]):
-    REGISTER_METHOD = add_ActionCacheServicer_to_server
-    FULL_NAME = RE_DESCRIPTOR.services_by_name["ActionCache"].full_name
+def _instance_name_from_bot_name(name: str) -> str:
+    names = name.split("/")
+    return "/".join(names[:-1])
 
-    @authorize_unary_unary(lambda r: cast(str, r.instance_name))
-    @context_module.metadatacontext()
-    @track_request_id
-    def GetActionResult(self, request: GetActionResultRequest, context: grpc.ServicerContext) -> ActionResult:
-        LOGGER.info(
-            f"GetActionResult request from [{context.peer()}] "
-            f"([{printable_request_metadata(context.invocation_metadata())}])"
-        )
 
-        try:
-            instance = self.get_instance(request.instance_name)
-            with DurationMetric(AC_GET_ACTION_RESULT_TIME_METRIC_NAME, request.instance_name, instanced=True):
-                action_result = instance.get_action_result(request.action_digest)
-            publish_counter_metric(AC_CACHE_HITS_METRIC_NAME, 1, {"instance-name": request.instance_name})
-            return action_result
-
-        except InvalidArgumentError as e:
-            LOGGER.info(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INVALID_ARGUMENT)
-
-        except NotFoundError as e:
-            LOGGER.debug(e)
-            context.set_code(grpc.StatusCode.NOT_FOUND)
-            publish_counter_metric(AC_CACHE_MISSES_METRIC_NAME, 1, {"instance-name": request.instance_name})
-
-        except ConnectionError as e:
-            LOGGER.exception(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.UNAVAILABLE)
-
-        except RetriableError as e:
-            LOGGER.info(f"Retriable error, client should retry in: {e.retry_info.retry_delay}")
-            context.abort_with_status(e.error_status)
-
-        except Exception as e:
-            LOGGER.exception(f"Unexpected error in GetActionResult; request=[{request}]")
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INTERNAL)
+class BotsService(BotsServicer, InstancedServicer[BotsInterface]):
+    REGISTER_METHOD = add_BotsServicer_to_server
+    FULL_NAME = BOTS_DESCRIPTOR.services_by_name["Bots"].full_name
 
-        return ActionResult()
+    # --- Public API: Servicer ---
+    @authorize_unary_unary(lambda r: cast(str, r.parent))
+    @track_request_id
+    @DurationMetric(BOTS_CREATE_BOT_SESSION_TIME_METRIC_NAME)
+    @handle_errors_unary_unary(BotSession)
+    def CreateBotSession(self, request: CreateBotSessionRequest, context: grpc.ServicerContext) -> BotSession:
+        """Handles CreateBotSessionRequest messages.
+
+        Args:
+            request (CreateBotSessionRequest): The incoming RPC request.
+            context (grpc.ServicerContext): Context for the RPC call.
+        """
+        LOGGER.info(f"CreateBotSession request from [{context.peer()}]")
+
+        instance_name = request.parent
+        instance = self.get_instance(instance_name)
+        bot_session = instance.create_bot_session(
+            request.bot_session, CancellationContext(context), deadline=context.time_remaining()
+        )
+        return bot_session
 
-    @authorize_unary_unary(lambda r: cast(str, r.instance_name))
-    @context_module.metadatacontext()
+    @authorize_unary_unary(lambda r: _instance_name_from_bot_name(r.name))
     @track_request_id
-    def UpdateActionResult(self, request: UpdateActionResultRequest, context: grpc.ServicerContext) -> ActionResult:
-        LOGGER.info(
-            f"UpdateActionResult request from [{context.peer()}] "
-            f"([{printable_request_metadata(context.invocation_metadata())}])"
+    @DurationMetric(BOTS_UPDATE_BOT_SESSION_TIME_METRIC_NAME)
+    @handle_errors_unary_unary(BotSession)
+    def UpdateBotSession(self, request: UpdateBotSessionRequest, context: grpc.ServicerContext) -> BotSession:
+        """Handles UpdateBotSessionRequest messages.
+
+        Args:
+            request (UpdateBotSessionRequest): The incoming RPC request.
+            context (grpc.ServicerContext): Context for the RPC call.
+        """
+        LOGGER.debug(f"UpdateBotSession request from [{context.peer()}]")
+
+        if request.name != request.bot_session.name:
+            raise InvalidArgumentError(
+                "Name in UpdateBotSessionRequest does not match BotSession. "
+                f" UpdateBotSessionRequest.name=[{request.name}] BotSession.name=[{request.bot_session.name}]"
+            )
+
+        instance_name = _instance_name_from_bot_name(request.name)
+        instance = self.get_instance(instance_name)
+        bot_session, metadata = instance.update_bot_session(
+            request.bot_session, CancellationContext(context), deadline=context.time_remaining()
         )
 
-        try:
-            instance = self.get_instance(request.instance_name)
-            with DurationMetric(AC_UPDATE_ACTION_RESULT_TIME_METRIC_NAME, request.instance_name, instanced=True):
-                instance.update_action_result(request.action_digest, request.action_result)
-            return request.action_result
-
-        except InvalidArgumentError as e:
-            LOGGER.info(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INVALID_ARGUMENT)
-
-        except NotImplementedError as e:
-            LOGGER.info(e)
-            context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-
-        except StorageFullError as e:
-            LOGGER.exception(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.RESOURCE_EXHAUSTED)
-
-        except ConnectionError as e:
-            LOGGER.exception(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.UNAVAILABLE)
-
-        except RetriableError as e:
-            LOGGER.info(f"Retriable error, client should retry in: {e.retry_info.retry_delay}")
-            context.abort_with_status(e.error_status)
-
-        except Exception as e:
-            LOGGER.exception(f"Unexpected error in UpdateActionResult; request=[{request}]")
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INTERNAL)
+        context.set_trailing_metadata(metadata)  # type: ignore[arg-type]  # tricky covariance issue.
+
+        return bot_session
+
+    @authorize_unary_unary(lambda r: _instance_name_from_bot_name(r.name))
+    @track_request_id
+    def PostBotEventTemp(self, request: PostBotEventTempRequest, context: grpc.ServicerContext) -> empty_pb2.Empty:
+        """Handles PostBotEventTempRequest messages.
 
-        return ActionResult()
+        Args:
+            request (PostBotEventTempRequest): The incoming RPC request.
+            context (grpc.ServicerContext): Context for the RPC call.
+        """
+        LOGGER.info(f"PostBotEventTemp request from [{context.peer()}]")
+
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+
+        return empty_pb2.Empty()
+
+    def query_n_bots(self) -> int:
+        return sum(map(self.query_n_bots_for_instance, self.instances))
+
+    def query_n_bots_for_instance(self, instance_name: str) -> int:
+        if instance := self.instances.get(instance_name):
+            return instance.count_bots()
+        return 0
+
+    def query_n_bots_for_status(self, bot_status: BotStatus) -> int:
+        return sum(self.query_n_bots_for_instance_for_status(instance, bot_status) for instance in self.instances)
+
+    def query_n_bots_for_instance_for_status(self, instance_name: str, bot_status: BotStatus) -> int:
+        if instance := self.instances.get(instance_name):
+            return instance.count_bots_by_status(bot_status)
+        return 0
```

### Comparing `buildgrid-0.0.91/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.92/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/auth/config.py` & `buildgrid-0.0.92/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/auth/enums.py` & `buildgrid-0.0.92/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.92/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/auth/manager.py` & `buildgrid-0.0.92/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.92/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/bots/instance.py` & `buildgrid-0.0.92/buildgrid/server/bots/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,17 +94,18 @@
             raise InvalidArgumentError("Bot's id must be set by client.")
 
         # Create new record
         bot_session.name = self.scheduler.add_bot_entry(
             bot_session_id=bot_session.bot_id, bot_session_status=bot_session.status
         )
 
+        LOGGER.info(f"Opened BotSession name=[{bot_session.name}] for bot_id=[{bot_session.bot_id}].")
+
         self._request_leases(bot_session, context, deadline=deadline)
 
-        LOGGER.info(f"Opened BotSession name=[{bot_session.name}] for bot_id=[{bot_session.bot_id}].")
         leases = ",".join(lease.id[:8] for lease in bot_session.leases)
         LOGGER.debug(
             f"Leases assigned to newly opened BotSession name=[{bot_session.name}] "
             f"for bot_id=[{bot_session.bot_id}]: [{leases}]."
         )
 
         # Update status for bot session
```

### Comparing `buildgrid-0.0.91/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.92/buildgrid/server/bots/job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.92/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/build_events/service.py` & `buildgrid-0.0.92/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.92/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.92/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.92/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.92/buildgrid/server/capabilities/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 import logging
 from typing import Union, cast
 
 import grpc
 
-from buildgrid._exceptions import InvalidArgumentError, RetriableError
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import DESCRIPTOR as RE_DESCRIPTOR
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import (
     GetCapabilitiesRequest,
     ServerCapabilities,
 )
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2_grpc import (
     CapabilitiesServicer,
@@ -32,15 +31,15 @@
 from buildgrid.server.actioncache.instance import ActionCache
 from buildgrid.server.auth.manager import authorize_unary_unary
 from buildgrid.server.capabilities.instance import CapabilitiesInstance
 from buildgrid.server.cas.instance import ContentAddressableStorageInstance
 from buildgrid.server.execution.instance import ExecutionInstance
 from buildgrid.server.request_metadata_utils import printable_request_metadata
 from buildgrid.server.servicer import InstancedServicer
-from buildgrid.server.utils.decorators import track_request_id
+from buildgrid.server.utils.decorators import handle_errors_unary_unary, track_request_id
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CapabilitiesService(CapabilitiesServicer, InstancedServicer[CapabilitiesInstance]):
     REGISTER_METHOD = add_CapabilitiesServicer_to_server
     FULL_NAME = RE_DESCRIPTOR.services_by_name["Capabilities"].full_name
@@ -59,39 +58,22 @@
     def add_execution_instance(self, name: str, instance: ExecutionInstance) -> None:
         self.get_instance(name).add_execution_instance(instance)
 
     # --- Public API: Servicer ---
 
     @authorize_unary_unary(lambda r: cast(str, r.instance_name))
     @track_request_id
+    @handle_errors_unary_unary(ServerCapabilities)
     def GetCapabilities(self, request: GetCapabilitiesRequest, context: grpc.ServicerContext) -> ServerCapabilities:
         """Handles GetCapabilitiesRequest messages.
 
         Args:
             request (GetCapabilitiesRequest): The incoming RPC request.
             context (grpc.ServicerContext): Context for the RPC call.
         """
         LOGGER.info(
             f"GetCapabilities request from [{context.peer()}] "
             f"([{printable_request_metadata(context.invocation_metadata())}])"
         )
 
-        try:
-            instance = self.get_instance(request.instance_name)
-
-            return instance.get_capabilities()
-
-        except InvalidArgumentError as e:
-            LOGGER.info(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INVALID_ARGUMENT)
-
-        except RetriableError as e:
-            LOGGER.info(f"Retriable error, client should retry in: {e.retry_info.retry_delay}")
-            context.abort_with_status(e.error_status)
-
-        except Exception as e:
-            LOGGER.exception(f"Unexpected error in GetCapabilities; request=[{request}]")
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INTERNAL)
-
-        return ServerCapabilities()
+        instance = self.get_instance(request.instance_name)
+        return instance.get_capabilities()
```

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.92/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/instance.py` & `buildgrid-0.0.92/buildgrid/server/cas/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/replicated.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,43 +60,42 @@
         for storage in self._storages.values():
             self._stack.enter_context(storage)
 
     def stop(self) -> None:
         self._stack.close()
 
     def has_blob(self, digest: Digest) -> bool:
-        LOGGER.debug(f"Checking for blob: [{digest}]")
         has_blob: Set[int] = set(i for i in self._storages if self._storages[i].has_blob(digest))
         missing_blob = set(self._storages.keys()) - has_blob
         if len(missing_blob) < len(self._storages):
             publish_counter_metric(
                 CAS_REPLICATED_STORAGE_BLOBS_NEED_REPLICATING_COUNT_METRIC_NAME,
                 len(missing_blob),
                 {"instance_name": self._instance_name or ""},
             )
         return len(has_blob) > 0
 
     def get_blob(self, digest: Digest) -> Optional[IO[bytes]]:
-        LOGGER.debug(f"Getting blob: [{digest}]")
         has_blob: Set[int] = set(i for i in self._storages if self._storages[i].has_blob(digest))
         missing_blob = set(self._storages.keys()) - has_blob
         blob = None
         failed_writes = 0
         for idx in has_blob:
             if blob := self._storages[idx].get_blob(digest):
                 break
             LOGGER.error(f"Storage #{idx} reported {digest} exists but downloading failed")
             missing_blob.add(idx)
         if len(missing_blob) < len(self._storages):
             assert blob is not None
             for idx in missing_blob:
                 try:
                     self._storages[idx].commit_write(digest, blob)
+                    LOGGER.debug(f"Replicated {digest.hash}/{digest.size_bytes} to storage #{idx}")
                 except Exception as e:
-                    LOGGER.warning(f"Failed to replicate {digest} to storage #{idx}: {e}")
+                    LOGGER.warning(f"Failed to replicate {digest.hash}/{digest.size_bytes} to storage #{idx}: {e}")
                     failed_writes += 1
                 blob.seek(0)
 
             publish_counter_metric(
                 CAS_REPLICATED_STORAGE_ERRORED_BLOBS_COUNT_METRIC_NAME,
                 failed_writes,
                 {"instance_name": self._instance_name or ""},
@@ -105,20 +104,18 @@
                 CAS_REPLICATED_STORAGE_REPLICATED_BLOBS_COUNT_METRIC_NAME,
                 len(missing_blob) - failed_writes,
                 {"instance_name": self._instance_name or ""},
             )
         return blob
 
     def delete_blob(self, digest: Digest) -> None:
-        LOGGER.debug(f"Deleting blob: [{digest}]")
         for storage in self._storages.values():
             storage.delete_blob(digest)
 
     def commit_write(self, digest: Digest, write_session: IO[bytes]) -> None:
-        LOGGER.debug(f"Writing blob: [{digest}]")
         failed_writes = 0
         error_msgs: List[str] = []
         for idx, storage in self._storages.items():
             try:
                 storage.commit_write(digest, write_session)
             except Exception as error:
                 LOGGER.warning(f"Failed to write {digest.hash}/{digest.size_bytes} to storage #{idx}: {error}")
@@ -193,15 +190,15 @@
                     errored_blobs_for_storage += 1
 
                 # Keep track of the status code for this digest, preferring OK over errors
                 if hdigest not in digest_result or digest_result[hdigest].code != code_pb2.OK:
                     digest_result[hdigest] = result
 
             if errored_blobs_for_storage > 0:
-                LOGGER.warning(f"Failed to write {errored_blobs_for_storage} digests to storage #{idx}")
+                LOGGER.warning(f"Failed to write {errored_blobs_for_storage}/{len(results)} digests to storage #{idx}")
                 errored_blobs_total += errored_blobs_for_storage
 
         publish_counter_metric(
             CAS_REPLICATED_STORAGE_ERRORED_BLOBS_COUNT_METRIC_NAME,
             errored_blobs_total,
             {"instance_name": self._instance_name or ""},
         )
@@ -229,21 +226,22 @@
         errored_blobs_count = 0
         for idx, missing in missing_blobs.items():
             # Write any blobs that exist in other storages which are missing from this storage
             write_batch: List[Tuple[Digest, bytes]] = []
             for digest in missing:
                 if digest.hash in bulk_read_results:
                     write_batch.append((digest.to_digest(), bulk_read_results[digest.hash]))
-            update_results = self._storages[idx].bulk_update_blobs(write_batch)
-            for result in update_results:
-                if result.code != code_pb2.OK:
-                    errored_blobs_count += 1
-                else:
-                    replicated_blobs_count += 1
-            LOGGER.debug(f"Replicated {len(write_batch)} blobs to storage #{idx}")
+            if write_batch:
+                update_results = self._storages[idx].bulk_update_blobs(write_batch)
+                for result in update_results:
+                    if result.code != code_pb2.OK:
+                        errored_blobs_count += 1
+                    else:
+                        replicated_blobs_count += 1
+                LOGGER.debug(f"Replicated {len(write_batch)} blobs to storage #{idx}")
 
         publish_counter_metric(
             CAS_REPLICATED_STORAGE_REPLICATED_BLOBS_COUNT_METRIC_NAME,
             replicated_blobs_count,
             {"instance_name": self._instance_name or ""},
         )
         publish_counter_metric(
```

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/sharded.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/storage_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.92/buildgrid/server/cas/storage/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/context.py` & `buildgrid-0.0.92/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/controller.py` & `buildgrid-0.0.92/buildgrid/server/controller.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.92/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/execution/instance.py` & `buildgrid-0.0.92/buildgrid/server/execution/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/execution/service.py` & `buildgrid-0.0.92/buildgrid/server/execution/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 
 import logging
 from typing import Iterable, Iterator, Union, cast
 
 import grpc
 
-from buildgrid._exceptions import CancelledError, FailedPreconditionError, InvalidArgumentError, RetriableError
+from buildgrid._exceptions import CancelledError, RetriableError
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import DESCRIPTOR as RE_DESCRIPTOR
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import ExecuteRequest, WaitExecutionRequest
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2_grpc import (
     ExecutionServicer,
     add_ExecutionServicer_to_server,
 )
 from buildgrid._protos.google.longrunning import operations_pb2
@@ -52,15 +52,15 @@
     extract_client_identity,
     extract_request_metadata,
     printable_client_identity,
     printable_request_metadata,
 )
 from buildgrid.server.servicer import InstancedServicer
 from buildgrid.server.utils.context import CancellationContext
-from buildgrid.server.utils.decorators import track_request_id_generator
+from buildgrid.server.utils.decorators import handle_errors_unary_stream, track_request_id_generator
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _parse_instance_name(operation_name: str) -> str:
     names = operation_name.split("/")
     return "/".join(names[:-1])
@@ -75,14 +75,15 @@
     @authorize_unary_stream(lambda r: cast(str, r.instance_name))
     @track_request_id_generator
     @generator_method_duration_metric(EXECUTE_SERVICER_TIME_METRIC_NAME)
     @generator_method_exception_counter(
         EXECUTE_EXCEPTION_COUNT_METRIC_NAME,
         ignored_exceptions=execute_ignored_exceptions,
     )
+    @handle_errors_unary_stream(operations_pb2.Operation)
     def Execute(self, request: ExecuteRequest, context: grpc.ServicerContext) -> Iterator[operations_pb2.Operation]:
         """Handles ExecuteRequest messages.
 
         Args:
             request (ExecuteRequest): The incoming RPC request.
             context (grpc.ServicerContext): Context for the RPC call.
         """
@@ -104,14 +105,15 @@
     @authorize_unary_stream(lambda r: _parse_instance_name(r.name))
     @track_request_id_generator
     @generator_method_duration_metric(WAIT_EXECUTION_SERVICER_TIME_METRIC_NAME)
     @generator_method_exception_counter(
         WAIT_EXECUTION_EXCEPTION_COUNT_METRIC_NAME,
         ignored_exceptions=wait_execution_ignored_exceptions,
     )
+    @handle_errors_unary_stream(operations_pb2.Operation)
     def WaitExecution(
         self, request: WaitExecutionRequest, context: grpc.ServicerContext
     ) -> Iterator[operations_pb2.Operation]:
         """Handles WaitExecutionRequest messages.
 
         Args:
             request (WaitExecutionRequest): The incoming RPC request.
@@ -174,40 +176,12 @@
                 LOGGER.info(
                     f"Peer peer_uid=[{peer_uid}] was holding up a thread for "
                     f"`stream_operation_updates()` for instance_name=[{instance_name}], "
                     f"operation_name=[{operation_name}], but the rpc context is not "
                     "active anymore; releasing thread."
                 )
 
-        except InvalidArgumentError as e:
-            LOGGER.info(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INVALID_ARGUMENT)
-            yield operations_pb2.Operation()
-
-        except FailedPreconditionError as e:
-            LOGGER.error(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.FAILED_PRECONDITION)
-            yield operations_pb2.Operation()
-
         except CancelledError as e:
             LOGGER.info(e)
             context.set_details(str(e))
             context.set_code(grpc.StatusCode.CANCELLED)
             yield e.last_response  # type: ignore[misc]  # need a better signature
-
-        except ConnectionError as e:
-            LOGGER.info(e)
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.UNAVAILABLE)
-            yield operations_pb2.Operation()
-
-        # Attempt to catch postgres connection failures and instruct clients to retry
-        except RetriableError as e:
-            LOGGER.info(f"Retriable error, client should retry in: {e.retry_info.retry_delay}")
-            context.abort_with_status(e.error_status)
-
-        except Exception as e:
-            LOGGER.exception(f"Unexpected error in Execute: request=[{request}]")
-            context.set_details(str(e))
-            context.set_code(grpc.StatusCode.INTERNAL)
```

### Comparing `buildgrid-0.0.91/buildgrid/server/job_metrics.py` & `buildgrid-0.0.92/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/metrics_names.py` & `buildgrid-0.0.92/buildgrid/server/metrics_names.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.92/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/monitoring.py` & `buildgrid-0.0.92/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.92/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.92/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/operations/instance.py` & `buildgrid-0.0.92/buildgrid/server/operations/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.92/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1110,17 +1110,23 @@
             locate_bot_stmt = (
                 select(BotEntry).where(BotEntry.name == bot_name, self._bot_in_instance()).with_for_update()
             )
             self._close_bot_sessions(session, session.execute(locate_bot_stmt).scalars().all())
 
     def _close_bot_sessions(self, session: Session, bots: List[BotEntry]) -> None:
         for bot in bots:
+            log_tags = f" instance_name=[{self._instance_name}] request.bot_name=[{bot.name}]"
+            log_tags += f" request.bot_id=[{bot.bot_id}] request.bot_status=[{bot.bot_status}]"
+
+            LOGGER.debug(f"Closing bot session. {log_tags}")
             if bot.lease_id:
                 if job := self._get_job(bot.lease_id, session, with_for_update=True):
                     for db_lease in job.active_leases:
+                        lease_tags = log_tags + f" db.lease_id=[{job.name}] db.lease_state=[{db_lease.state}]"
+                        LOGGER.debug(f"Reassigning lease for bot session. {lease_tags}")
                         self._retry_job_lease(session, job, db_lease)
                         self._notify_job_updated(job.name, session)
             session.delete(bot)
 
     def reap_expired_sessions(self) -> bool:
         """
         Find and close expired bot sessions. Returns True if sessions were closed.
@@ -1160,28 +1166,39 @@
         with self._sql.session(exceptions_to_not_raise_on=[Exception]) as session:
             locate_bot_stmt = (
                 select(BotEntry).where(BotEntry.bot_id == bot_id, self._bot_in_instance()).with_for_update()
             )
             bots: List[BotEntry] = session.execute(locate_bot_stmt).scalars().all()
             if not bots:
                 raise InvalidArgumentError(f"Bot does not exist while validating leases. {log_tags}")
+
+            # This is a tricky case. This case happens when a new bot session is created while an older
+            # session for a bot id is waiting on leases. This can happen when a worker reboots but the
+            # connection context takes a long time to close. In this case, we DO NOT want to update anything
+            # in the database, because the work/lease has already been re-assigned to a new session.
+            # Closing anything in the database at this point would cause the newly restarted worker
+            # to get cancelled prematurely.
+            if len(bots) == 1 and bots[0].name != bot_name:
+                raise BotSessionMismatchError(
+                    "Mismatch between client supplied bot_id/bot_name and buildgrid database record. "
+                    f"db.bot_name=[{bots[0].name}] {log_tags}"
+                )
+
+            # Everything at this point is wrapped in try/catch, so we can raise BotSessionMismatchError or
+            # BotSessionClosedError and have the session be closed if preconditions from here out fail.
             try:
-                # Time for some housekeeping.
-                # If we have more than one bot name registered with a worker, or if this session doesn't
-                # match up with the expect job in the database, shut the sessions down.
+                # There should never be time when two bot sessions exist for the same bot id. We have logic to
+                # assert that old database entries for a given bot id are closed and deleted prior to making a
+                # new one. If this case happens shut everything down, so we can hopefully recover.
                 if len(bots) > 1:
                     raise BotSessionMismatchError(
                         "Bot id is registered to more than one bot session. "
                         f"names=[{', '.join(bot.name for bot in bots)}] {log_tags}"
                     )
-                if bots[0].name != bot_name:
-                    raise BotSessionMismatchError(
-                        "Mismatch between client supplied bot_id/bot_name and buildgrid database record. "
-                        f"db.bot_name=[{bots[0].name}] {log_tags}"
-                    )
+
                 bot = bots[0]
                 log_tags += f" db.lease_id=[{bot.lease_id}]"
 
                 # Validate that the lease_id matches the client and database if both are supplied.
                 if (session_lease and session_lease.id and bot.lease_id) and (session_lease.id != bot.lease_id):
                     raise BotSessionMismatchError(
                         f"Mismatch between client supplied lease_id and buildgrid database record. {log_tags}"
```

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,16 +105,15 @@
             # The subscribers can choose how they want to act (e.g. by querying the full job data).
             statement = sql_select(JobEntry.name, JobEntry.cancelled, JobEntry.stage).where(JobEntry.name.in_(names))
             next_data: Dict[str, Tuple[bool, int]] = {}
             for [name, cancelled, stage] in session.execute(statement).all():
                 next_data[name] = (cancelled, stage)
 
             for name in next_data:
-                # Don't notify on the first poll of this data.
-                if name in prev_data and prev_data[name] != next_data[name]:
+                if name not in prev_data or prev_data[name] != next_data[name]:
                     self.notify(name)
 
             prev_data = next_data
             shutdown_requested.wait(timeout=self.poll_interval)
 
     def notify(self, job_name: str) -> None:
         with self._lock:
```

### Comparing `buildgrid-0.0.91/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.92/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.92/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/redis/provider.py` & `buildgrid-0.0.92/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.92/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.92/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.92/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/server.py` & `buildgrid-0.0.92/buildgrid/server/server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/servicer.py` & `buildgrid-0.0.92/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.92/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/sql/provider.py` & `buildgrid-0.0.92/buildgrid/server/sql/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.92/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/threading.py` & `buildgrid-0.0.92/buildgrid/server/threading.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.92/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.92/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/server/utils/context.py` & `buildgrid-0.0.92/buildgrid/server/utils/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/settings.py` & `buildgrid-0.0.92/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid/utils.py` & `buildgrid-0.0.92/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.92/buildgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.91
+Version: 0.0.92
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -12,16 +12,16 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: dnspython
 Requires-Dist: grpcio-reflection>=1.62.0
 Requires-Dist: grpcio>=1.62.0
 Requires-Dist: janus>=0.6.2
-Requires-Dist: jinja2==3.0.3
-Requires-Dist: protobuf<4.24.0
+Requires-Dist: jinja2
+Requires-Dist: protobuf
 Requires-Dist: alembic
 Requires-Dist: Click
 Requires-Dist: SQLAlchemy[mypy]<2.0,>=1.4.24
 Requires-Dist: pydantic>2.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: jsonschema>=3.0.0
 Requires-Dist: lark-parser
@@ -39,19 +39,18 @@
 Provides-Extra: database
 Requires-Dist: psycopg2-binary; extra == "database"
 Provides-Extra: redis
 Requires-Dist: fakeredis>=2.10.1; extra == "redis"
 Requires-Dist: redis>=4.5.1; extra == "redis"
 Requires-Dist: hiredis; extra == "redis"
 Provides-Extra: docs
-Requires-Dist: Sphinx<7; extra == "docs"
+Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: cryptography>=38.0.0; extra == "tests"
 Requires-Dist: flaky; extra == "tests"
 Requires-Dist: flask; extra == "tests"
 Requires-Dist: flask-cors; extra == "tests"
 Requires-Dist: moto<4.1.12; extra == "tests"
```

### Comparing `buildgrid-0.0.91/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.92/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.92/buildgrid.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 boto3
 botocore
 dnspython
 grpcio-reflection>=1.62.0
 grpcio>=1.62.0
 janus>=0.6.2
-jinja2==3.0.3
-protobuf<4.24.0
+jinja2
+protobuf
 alembic
 Click
 SQLAlchemy[mypy]<2.0,>=1.4.24
 pydantic>2.0
 PyYAML>=6.0.1
 jsonschema>=3.0.0
 lark-parser
@@ -41,19 +41,18 @@
 pytest-forked
 pytest-pycodestyle
 pytest-xdist
 pip-tools
 memray
 
 [docs]
-Sphinx<7
+Sphinx
 sphinx-click
 sphinx-rtd-theme
 sphinxcontrib-apidoc
-sphinxcontrib-napoleon
 
 [mypy]
 mypy
 grpc-stubs>=1.53
 boto3-stubs
 mypy-boto3-s3
 sqlalchemy2-stubs<=0.0.2a22
```

### Comparing `buildgrid-0.0.91/data/config/all-in-one.yml` & `buildgrid-0.0.92/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/artifacts.yml` & `buildgrid-0.0.92/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/basic-with-disk.yml` & `buildgrid-0.0.92/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/bots-interface.yml` & `buildgrid-0.0.92/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/cache.yml` & `buildgrid-0.0.92/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/controller.yml` & `buildgrid-0.0.92/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/default.yml` & `buildgrid-0.0.92/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.92/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/index-sqlite.yml` & `buildgrid-0.0.92/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/monitoring-controller.yml` & `buildgrid-0.0.92/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/multi-layer-storage.yml` & `buildgrid-0.0.92/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/redis-cache.yml` & `buildgrid-0.0.92/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.92/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/storage-redis.yml` & `buildgrid-0.0.92/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/storage-s3.yml` & `buildgrid-0.0.92/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/storage.yml` & `buildgrid-0.0.92/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/with-metering.yml` & `buildgrid-0.0.92/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/data/config/with-pgbouncer.yml` & `buildgrid-0.0.92/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/docs/Makefile` & `buildgrid-0.0.92/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.92/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.92/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/docs/source/index.rst` & `buildgrid-0.0.92/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/pyproject.toml` & `buildgrid-0.0.92/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.91"
+version = "0.0.92"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "boto3",
     "botocore",
     "dnspython",
     "grpcio-reflection >= 1.62.0",
     "grpcio >= 1.62.0",
     "janus >= 0.6.2",
-    "jinja2 == 3.0.3",
-    "protobuf < 4.24.0", # https://github.com/protocolbuffers/protobuf/issues/13485 # TODO: remove this once it's fixed!
+    "jinja2",
+    "protobuf",
     "alembic",
     "Click",
     "SQLAlchemy[mypy] >= 1.4.24, < 2.0", # For _ConnectionFairy.dbapi_connection
     "pydantic > 2.0", # required by new models in metering-client
     "PyYAML >= 6.0.1", # https://github.com/yaml/pyyaml/issues/724 cython issue in 6.0.0
     "jsonschema >= 3.0.0",
     "lark-parser",
@@ -66,28 +66,28 @@
 ]
 redis = [
     "fakeredis >= 2.10.1",
     "redis >= 4.5.1",
     "hiredis",  # Faster parsing of redis response.
 ]
 docs = [
-    "Sphinx < 7",  # Sphinx 7 removes support for `setup.py build_sphinx`, which CI still requires
+    "Sphinx",
     "sphinx-click",
     "sphinx-rtd-theme",
     "sphinxcontrib-apidoc",
-    "sphinxcontrib-napoleon",
 ]
 tests = [
     "coverage",
     "cryptography >= 38.0.0",  # For compatibility with pyopenssl>=22.0.0 https://github.com/pyca/pyopenssl/issues/1143
     "flaky",  # until we pin down why the bots tests are so painful.
     "flask",
     "flask-cors",
     # 4.1.12 breaks tests using S3 with 400/403. No obvious reasons can be found from the CHANGELOG / open issues yet.
     # TODO: investigate the root cause and unpin moto
+    # NOTE: unpinning this will also require some code change, as `mock_s3` is removed in favour of `mock_aws` in modern moto
     "moto < 4.1.12",
     "psutil",
     "pycodestyle",
     "pyopenssl >= 22.0.0",  # For compatibility with cryptography>=38.0.0 https://github.com/pyca/pyopenssl/issues/1143
     "pytest",
     "pytest-aiohttp",
     "pytest-asyncio",
@@ -151,7 +151,53 @@
 multi_line_output = 3
 include_trailing_comma = true
 use_parentheses = true
 extend_skip_glob = ["buildgrid/_protos/*"]
 ensure_newline_before_comments = true
 
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
+
+[tool.mypy]
+plugins = "sqlalchemy.ext.mypy.plugin"
+python_version = "3.8"
+strict = true
+
+[[tool.mypy.overrides]]
+module = "buildgrid._app.*"
+disable_error_code = [
+    "no-untyped-def",
+    "no-untyped-call"
+]
+
+# mypy errors from 3rd party libs
+# https://github.com/python/mypy/issues/12299
+[[tool.mypy.overrides]]
+module = "referencing.*"
+follow_imports = "skip"
+
+[tool.coverage.run]
+concurrency = [
+    "multiprocessing",
+    "thread"
+]
+source = [
+    "buildgrid/*"
+]
+omit = [
+    "buildgrid/_app/*",
+    "buildgrid/_protos/*",
+    "*_pb2.py",
+    "*_pb2_grpc.py"
+]
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+
+[tool.pytest.ini_options]
+addopts = "--verbose --pycodestyle --cov=buildgrid --cov-config=pyproject.toml -n auto --no-success-flaky-report"
+python_files = "tests/*.py"
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore::PendingDeprecationWarning",
+    "ignore::sqlalchemy.exc.SAWarning"
+]
```

### Comparing `buildgrid-0.0.91/setup.py` & `buildgrid-0.0.92/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/auth/data/auth.yaml` & `buildgrid-0.0.92/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.92/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_async_lru_cache.py` & `buildgrid-0.0.92/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_execution_instance.py` & `buildgrid-0.0.92/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_job_assigner.py` & `buildgrid-0.0.92/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_metrics_utils.py` & `buildgrid-0.0.92/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_mirrored_cache.py` & `buildgrid-0.0.92/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.92/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_parser.py` & `buildgrid-0.0.92/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_request_metadata_utils.py` & `buildgrid-0.0.92/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_scheduler.py` & `buildgrid-0.0.92/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.91/tests/test_utils.py` & `buildgrid-0.0.92/tests/test_utils.py`

 * *Files identical despite different names*

