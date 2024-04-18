# Comparing `tmp/grpclib-0.4.7rc1.tar.gz` & `tmp/grpclib-0.4.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpclib-0.4.7rc1.tar", last modified: Sat Oct 28 18:23:26 2023, max compression
+gzip compressed data, was "grpclib-0.4.8rc1.tar", last modified: Thu Apr 18 15:26:16 2024, max compression
```

## Comparing `grpclib-0.4.7rc1.tar` & `grpclib-0.4.8rc1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/channelz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/channelz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/channelz/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/channelz/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/channelz/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2023-10-28 18:23:24.000000 grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16431 2023-10-28 18:23:24.000000 grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    55995 2023-10-28 18:23:24.000000 grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35799 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/encoding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/encoding/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/health/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/health/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/health/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/health/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/health/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-10-28 18:23:22.000000 grpclib-0.4.7rc1/grpclib/health/v1/health_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-10-28 18:23:22.000000 grpclib-0.4.7rc1/grpclib/health/v1/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2023-10-28 18:23:22.000000 grpclib-0.4.7rc1/grpclib/health/v1/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    25144 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/reflection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/reflection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/reflection/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/reflection/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/reflection/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib/reflection/v1alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/reflection/v1alpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2023-10-28 18:23:23.000000 grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27218 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/grpclib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/grpclib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-10-28 18:23:26.000000 grpclib-0.4.7rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-28 18:23:04.000000 grpclib-0.4.7rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.644494 grpclib-0.4.8rc1/grpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.644494 grpclib-0.4.8rc1/grpclib/channelz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/channelz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/channelz/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.644494 grpclib-0.4.8rc1/grpclib/channelz/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/channelz/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54835 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35799 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.644494 grpclib-0.4.8rc1/grpclib/encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/encoding/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/health/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/health/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/health/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/health/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/health/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/health/v1/health_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/health/v1/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/health/v1/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25144 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/reflection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/reflection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/reflection/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/reflection/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/reflection/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.648494 grpclib-0.4.8rc1/grpclib/reflection/v1alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/reflection/v1alpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-18 15:26:14.000000 grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27218 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/grpclib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:16.644494 grpclib-0.4.8rc1/grpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 15:26:16.000000 grpclib-0.4.8rc1/grpclib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 15:26:16.652494 grpclib-0.4.8rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 15:26:00.000000 grpclib-0.4.8rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grpclib-0.4.7rc1/LICENSE.txt` & `grpclib-0.4.8rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/PKG-INFO` & `grpclib-0.4.8rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.7rc1
+Version: 0.4.8rc1
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
         
         .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
           :target: https://standforukraine.com
         
         |project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
         
-        This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
+        This project is based on `hyper-h2`_ and **requires Python >= 3.8**.
         
         .. contents::
           :local:
         
         Example
         ~~~~~~~
         
@@ -170,18 +170,18 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: protobuf
```

### Comparing `grpclib-0.4.7rc1/README.rst` & `grpclib-0.4.8rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ===========================================
 
 .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
   :target: https://standforukraine.com
 
 |project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
 
-This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
+This project is based on `hyper-h2`_ and **requires Python >= 3.8**.
 
 .. contents::
   :local:
 
 Example
 ~~~~~~~
```

### Comparing `grpclib-0.4.7rc1/grpclib/_typing.py` & `grpclib-0.4.8rc1/grpclib/_typing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/channelz/service.py` & `grpclib-0.4.8rc1/grpclib/channelz/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_grpc.py` & `grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_pb2.py` & `grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpclib/channelz/v1/channelz.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -19,16 +20,16 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"grpclib/channelz/v1/channelz.proto\x12\x10grpc.channelz.v1\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfe\x01\n\x07\x43hannel\x12)\n\x03ref\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\x84\x02\n\nSubchannel\x12,\n\x03ref\x18\x01 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xbb\x01\n\x18\x43hannelConnectivityState\x12?\n\x05state\x18\x01 \x01(\x0e\x32\x30.grpc.channelz.v1.ChannelConnectivityState.State\"^\n\x05State\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04IDLE\x10\x01\x12\x0e\n\nCONNECTING\x10\x02\x12\t\n\x05READY\x10\x03\x12\x15\n\x11TRANSIENT_FAILURE\x10\x04\x12\x0c\n\x08SHUTDOWN\x10\x05\"\x8e\x02\n\x0b\x43hannelData\x12\x39\n\x05state\x18\x01 \x01(\x0b\x32*.grpc.channelz.v1.ChannelConnectivityState\x12\x0e\n\x06target\x18\x02 \x01(\t\x12-\n\x05trace\x18\x03 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x04 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x05 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x06 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xdb\x02\n\x11\x43hannelTraceEvent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12>\n\x08severity\x18\x02 \x01(\x0e\x32,.grpc.channelz.v1.ChannelTraceEvent.Severity\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0b\x63hannel_ref\x18\x04 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRefH\x00\x12\x39\n\x0esubchannel_ref\x18\x05 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRefH\x00\"E\n\x08Severity\x12\x0e\n\nCT_UNKNOWN\x10\x00\x12\x0b\n\x07\x43T_INFO\x10\x01\x12\x0e\n\nCT_WARNING\x10\x02\x12\x0c\n\x08\x43T_ERROR\x10\x03\x42\x0b\n\tchild_ref\"\x96\x01\n\x0c\x43hannelTrace\x12\x19\n\x11num_events_logged\x18\x01 \x01(\x03\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x65vents\x18\x03 \x03(\x0b\x32#.grpc.channelz.v1.ChannelTraceEvent\"R\n\nChannelRef\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"X\n\rSubchannelRef\x12\x15\n\rsubchannel_id\x18\x07 \x01(\x03\x12\x0c\n\x04name\x18\x08 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"P\n\tSocketRef\x12\x11\n\tsocket_id\x18\x03 \x01(\x03\x12\x0c\n\x04name\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"P\n\tServerRef\x12\x11\n\tserver_id\x18\x05 \x01(\x03\x12\x0c\n\x04name\x18\x06 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\x92\x01\n\x06Server\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.ServerRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.ServerData\x12\x32\n\rlisten_socket\x18\x03 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xc2\x01\n\nServerData\x12-\n\x05trace\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x02 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x03 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x04 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf6\x01\n\x06Socket\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.SocketData\x12(\n\x05local\x18\x03 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12)\n\x06remote\x18\x04 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12,\n\x08security\x18\x05 \x01(\x0b\x32\x1a.grpc.channelz.v1.Security\x12\x13\n\x0bremote_name\x18\x06 \x01(\t\"\xee\x04\n\nSocketData\x12\x17\n\x0fstreams_started\x18\x01 \x01(\x03\x12\x19\n\x11streams_succeeded\x18\x02 \x01(\x03\x12\x16\n\x0estreams_failed\x18\x03 \x01(\x03\x12\x15\n\rmessages_sent\x18\x04 \x01(\x03\x12\x19\n\x11messages_received\x18\x05 \x01(\x03\x12\x18\n\x10keep_alives_sent\x18\x06 \x01(\x03\x12G\n#last_local_stream_created_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12H\n$last_remote_stream_created_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x1blast_message_sent_timestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x1flast_message_received_timestamp\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x19local_flow_control_window\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12?\n\x1aremote_flow_control_window\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12.\n\x06option\x18\r \x03(\x0b\x32\x1e.grpc.channelz.v1.SocketOption\"\xe8\x02\n\x07\x41\x64\x64ress\x12?\n\rtcpip_address\x18\x01 \x01(\x0b\x32&.grpc.channelz.v1.Address.TcpIpAddressH\x00\x12;\n\x0buds_address\x18\x02 \x01(\x0b\x32$.grpc.channelz.v1.Address.UdsAddressH\x00\x12?\n\rother_address\x18\x03 \x01(\x0b\x32&.grpc.channelz.v1.Address.OtherAddressH\x00\x1a\x30\n\x0cTcpIpAddress\x12\x12\n\nip_address\x18\x01 \x01(\x0c\x12\x0c\n\x04port\x18\x02 \x01(\x05\x1a\x1e\n\nUdsAddress\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x1a\x41\n\x0cOtherAddress\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\t\n\x07\x61\x64\x64ress\"\xbe\x02\n\x08Security\x12-\n\x03tls\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.Security.TlsH\x00\x12\x39\n\x05other\x18\x02 \x01(\x0b\x32(.grpc.channelz.v1.Security.OtherSecurityH\x00\x1a{\n\x03Tls\x12\x17\n\rstandard_name\x18\x01 \x01(\tH\x00\x12\x14\n\nother_name\x18\x02 \x01(\tH\x00\x12\x19\n\x11local_certificate\x18\x03 \x01(\x0c\x12\x1a\n\x12remote_certificate\x18\x04 \x01(\x0c\x42\x0e\n\x0c\x63ipher_suite\x1a\x42\n\rOtherSecurity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\x07\n\x05model\"U\n\x0cSocketOption\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12(\n\nadditional\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"B\n\x13SocketOptionTimeout\x12+\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"Q\n\x12SocketOptionLinger\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xae\x05\n\x13SocketOptionTcpInfo\x12\x12\n\ntcpi_state\x18\x01 \x01(\r\x12\x15\n\rtcpi_ca_state\x18\x02 \x01(\r\x12\x18\n\x10tcpi_retransmits\x18\x03 \x01(\r\x12\x13\n\x0btcpi_probes\x18\x04 \x01(\r\x12\x14\n\x0ctcpi_backoff\x18\x05 \x01(\r\x12\x14\n\x0ctcpi_options\x18\x06 \x01(\r\x12\x17\n\x0ftcpi_snd_wscale\x18\x07 \x01(\r\x12\x17\n\x0ftcpi_rcv_wscale\x18\x08 \x01(\r\x12\x10\n\x08tcpi_rto\x18\t \x01(\r\x12\x10\n\x08tcpi_ato\x18\n \x01(\r\x12\x14\n\x0ctcpi_snd_mss\x18\x0b \x01(\r\x12\x14\n\x0ctcpi_rcv_mss\x18\x0c \x01(\r\x12\x14\n\x0ctcpi_unacked\x18\r \x01(\r\x12\x13\n\x0btcpi_sacked\x18\x0e \x01(\r\x12\x11\n\ttcpi_lost\x18\x0f \x01(\r\x12\x14\n\x0ctcpi_retrans\x18\x10 \x01(\r\x12\x14\n\x0ctcpi_fackets\x18\x11 \x01(\r\x12\x1b\n\x13tcpi_last_data_sent\x18\x12 \x01(\r\x12\x1a\n\x12tcpi_last_ack_sent\x18\x13 \x01(\r\x12\x1b\n\x13tcpi_last_data_recv\x18\x14 \x01(\r\x12\x1a\n\x12tcpi_last_ack_recv\x18\x15 \x01(\r\x12\x11\n\ttcpi_pmtu\x18\x16 \x01(\r\x12\x19\n\x11tcpi_rcv_ssthresh\x18\x17 \x01(\r\x12\x10\n\x08tcpi_rtt\x18\x18 \x01(\r\x12\x13\n\x0btcpi_rttvar\x18\x19 \x01(\r\x12\x19\n\x11tcpi_snd_ssthresh\x18\x1a \x01(\r\x12\x15\n\rtcpi_snd_cwnd\x18\x1b \x01(\r\x12\x13\n\x0btcpi_advmss\x18\x1c \x01(\r\x12\x17\n\x0ftcpi_reordering\x18\x1d \x01(\r\"F\n\x15GetTopChannelsRequest\x12\x18\n\x10start_channel_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"Q\n\x16GetTopChannelsResponse\x12*\n\x07\x63hannel\x18\x01 \x03(\x0b\x32\x19.grpc.channelz.v1.Channel\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"A\n\x11GetServersRequest\x12\x17\n\x0fstart_server_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"K\n\x12GetServersResponse\x12(\n\x06server\x18\x01 \x03(\x0b\x32\x18.grpc.channelz.v1.Server\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"%\n\x10GetServerRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\"=\n\x11GetServerResponse\x12(\n\x06server\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Server\"Z\n\x17GetServerSocketsRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\x12\x17\n\x0fstart_socket_id\x18\x02 \x01(\x03\x12\x13\n\x0bmax_results\x18\x03 \x01(\x03\"X\n\x18GetServerSocketsResponse\x12/\n\nsocket_ref\x18\x01 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"\'\n\x11GetChannelRequest\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\"@\n\x12GetChannelResponse\x12*\n\x07\x63hannel\x18\x01 \x01(\x0b\x32\x19.grpc.channelz.v1.Channel\"-\n\x14GetSubchannelRequest\x12\x15\n\rsubchannel_id\x18\x01 \x01(\x03\"I\n\x15GetSubchannelResponse\x12\x30\n\nsubchannel\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.Subchannel\"6\n\x10GetSocketRequest\x12\x11\n\tsocket_id\x18\x01 \x01(\x03\x12\x0f\n\x07summary\x18\x02 \x01(\x08\"=\n\x11GetSocketResponse\x12(\n\x06socket\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Socket2\x9a\x05\n\x08\x43hannelz\x12\x63\n\x0eGetTopChannels\x12\'.grpc.channelz.v1.GetTopChannelsRequest\x1a(.grpc.channelz.v1.GetTopChannelsResponse\x12W\n\nGetServers\x12#.grpc.channelz.v1.GetServersRequest\x1a$.grpc.channelz.v1.GetServersResponse\x12T\n\tGetServer\x12\".grpc.channelz.v1.GetServerRequest\x1a#.grpc.channelz.v1.GetServerResponse\x12i\n\x10GetServerSockets\x12).grpc.channelz.v1.GetServerSocketsRequest\x1a*.grpc.channelz.v1.GetServerSocketsResponse\x12W\n\nGetChannel\x12#.grpc.channelz.v1.GetChannelRequest\x1a$.grpc.channelz.v1.GetChannelResponse\x12`\n\rGetSubchannel\x12&.grpc.channelz.v1.GetSubchannelRequest\x1a\'.grpc.channelz.v1.GetSubchannelResponse\x12T\n\tGetSocket\x12\".grpc.channelz.v1.GetSocketRequest\x1a#.grpc.channelz.v1.GetSocketResponseBX\n\x13io.grpc.channelz.v1B\rChannelzProtoP\x01Z0google.golang.org/grpc/channelz/grpc_channelz_v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpclib.channelz.v1.channelz_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\023io.grpc.channelz.v1B\rChannelzProtoP\001Z0google.golang.org/grpc/channelz/grpc_channelz_v1'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\023io.grpc.channelz.v1B\rChannelzProtoP\001Z0google.golang.org/grpc/channelz/grpc_channelz_v1'
   _globals['_CHANNEL']._serialized_start=181
   _globals['_CHANNEL']._serialized_end=435
   _globals['_SUBCHANNEL']._serialized_start=438
   _globals['_SUBCHANNEL']._serialized_end=698
   _globals['_CHANNELCONNECTIVITYSTATE']._serialized_start=701
   _globals['_CHANNELCONNECTIVITYSTATE']._serialized_end=888
   _globals['_CHANNELCONNECTIVITYSTATE_STATE']._serialized_start=794
```

### Comparing `grpclib-0.4.7rc1/grpclib/channelz/v1/channelz_pb2.pyi` & `grpclib-0.4.8rc1/grpclib/channelz/v1/channelz_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This file defines an interface for exporting monitoring information
 out of gRPC servers.  See the full design at
 https://github.com/grpc/proposal/blob/master/A14-channelz.md
 
 The canonical version of this proto can be found at
 https://github.com/grpc/grpc-proto/blob/master/grpc/channelz/v1/channelz.proto
 """
+
 import builtins
 import collections.abc
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
@@ -24,64 +25,69 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Channel(google.protobuf.message.Message):
     """Channel is a logical grouping of channels, subchannels, and sockets."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REF_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     CHANNEL_REF_FIELD_NUMBER: builtins.int
     SUBCHANNEL_REF_FIELD_NUMBER: builtins.int
     SOCKET_REF_FIELD_NUMBER: builtins.int
     @property
     def ref(self) -> global___ChannelRef:
         """The identifier for this channel. This should be set."""
+
     @property
     def data(self) -> global___ChannelData:
         """Data specific to this channel.
         At most one of 'channel_ref+subchannel_ref' and 'socket' is set.
         """
+
     @property
     def channel_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelRef]:
         """There are no ordering guarantees on the order of channel refs.
         There may not be cycles in the ref graph.
         A channel ref may be present in more than one channel or subchannel.
         """
+
     @property
     def subchannel_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SubchannelRef]:
         """At most one of 'channel_ref+subchannel_ref' and 'socket' is set.
         There are no ordering guarantees on the order of subchannel refs.
         There may not be cycles in the ref graph.
         A sub channel ref may be present in more than one channel or subchannel.
         """
+
     @property
     def socket_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SocketRef]:
         """There are no ordering guarantees on the order of sockets."""
+
     def __init__(
         self,
         *,
         ref: global___ChannelRef | None = ...,
         data: global___ChannelData | None = ...,
         channel_ref: collections.abc.Iterable[global___ChannelRef] | None = ...,
         subchannel_ref: collections.abc.Iterable[global___SubchannelRef] | None = ...,
         socket_ref: collections.abc.Iterable[global___SocketRef] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_ref", b"channel_ref", "data", b"data", "ref", b"ref", "socket_ref", b"socket_ref", "subchannel_ref", b"subchannel_ref"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["channel_ref", b"channel_ref", "data", b"data", "ref", b"ref", "socket_ref", b"socket_ref", "subchannel_ref", b"subchannel_ref"]) -> None: ...
 
 global___Channel = Channel
 
-@typing_extensions.final
+@typing.final
 class Subchannel(google.protobuf.message.Message):
     """Subchannel is a logical grouping of channels, subchannels, and sockets.
     A subchannel is load balanced over by it's ancestor
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -89,62 +95,67 @@
     DATA_FIELD_NUMBER: builtins.int
     CHANNEL_REF_FIELD_NUMBER: builtins.int
     SUBCHANNEL_REF_FIELD_NUMBER: builtins.int
     SOCKET_REF_FIELD_NUMBER: builtins.int
     @property
     def ref(self) -> global___SubchannelRef:
         """The identifier for this channel."""
+
     @property
     def data(self) -> global___ChannelData:
         """Data specific to this channel.
         At most one of 'channel_ref+subchannel_ref' and 'socket' is set.
         """
+
     @property
     def channel_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelRef]:
         """There are no ordering guarantees on the order of channel refs.
         There may not be cycles in the ref graph.
         A channel ref may be present in more than one channel or subchannel.
         """
+
     @property
     def subchannel_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SubchannelRef]:
         """At most one of 'channel_ref+subchannel_ref' and 'socket' is set.
         There are no ordering guarantees on the order of subchannel refs.
         There may not be cycles in the ref graph.
         A sub channel ref may be present in more than one channel or subchannel.
         """
+
     @property
     def socket_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SocketRef]:
         """There are no ordering guarantees on the order of sockets."""
+
     def __init__(
         self,
         *,
         ref: global___SubchannelRef | None = ...,
         data: global___ChannelData | None = ...,
         channel_ref: collections.abc.Iterable[global___ChannelRef] | None = ...,
         subchannel_ref: collections.abc.Iterable[global___SubchannelRef] | None = ...,
         socket_ref: collections.abc.Iterable[global___SocketRef] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_ref", b"channel_ref", "data", b"data", "ref", b"ref", "socket_ref", b"socket_ref", "subchannel_ref", b"subchannel_ref"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["channel_ref", b"channel_ref", "data", b"data", "ref", b"ref", "socket_ref", b"socket_ref", "subchannel_ref", b"subchannel_ref"]) -> None: ...
 
 global___Subchannel = Subchannel
 
-@typing_extensions.final
+@typing.final
 class ChannelConnectivityState(google.protobuf.message.Message):
     """These come from the specified states in this document:
     https://github.com/grpc/grpc/blob/master/doc/connectivity-semantics-and-api.md
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _State:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _StateEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ChannelConnectivityState._State.ValueType], builtins.type):  # noqa: F821
+    class _StateEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ChannelConnectivityState._State.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         UNKNOWN: ChannelConnectivityState._State.ValueType  # 0
         IDLE: ChannelConnectivityState._State.ValueType  # 1
         CONNECTING: ChannelConnectivityState._State.ValueType  # 2
         READY: ChannelConnectivityState._State.ValueType  # 3
         TRANSIENT_FAILURE: ChannelConnectivityState._State.ValueType  # 4
         SHUTDOWN: ChannelConnectivityState._State.ValueType  # 5
@@ -160,79 +171,82 @@
     STATE_FIELD_NUMBER: builtins.int
     state: global___ChannelConnectivityState.State.ValueType
     def __init__(
         self,
         *,
         state: global___ChannelConnectivityState.State.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["state", b"state"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["state", b"state"]) -> None: ...
 
 global___ChannelConnectivityState = ChannelConnectivityState
 
-@typing_extensions.final
+@typing.final
 class ChannelData(google.protobuf.message.Message):
     """Channel data is data related to a specific Channel or Subchannel."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATE_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
     TRACE_FIELD_NUMBER: builtins.int
     CALLS_STARTED_FIELD_NUMBER: builtins.int
     CALLS_SUCCEEDED_FIELD_NUMBER: builtins.int
     CALLS_FAILED_FIELD_NUMBER: builtins.int
     LAST_CALL_STARTED_TIMESTAMP_FIELD_NUMBER: builtins.int
-    @property
-    def state(self) -> global___ChannelConnectivityState:
-        """The connectivity state of the channel or subchannel.  Implementations
-        should always set this.
-        """
     target: builtins.str
     """The target this channel originally tried to connect to.  May be absent"""
-    @property
-    def trace(self) -> global___ChannelTrace:
-        """A trace of recent events on the channel.  May be absent."""
     calls_started: builtins.int
     """The number of calls started on the channel"""
     calls_succeeded: builtins.int
     """The number of calls that have completed with an OK status"""
     calls_failed: builtins.int
     """The number of calls that have completed with a non-OK status"""
     @property
+    def state(self) -> global___ChannelConnectivityState:
+        """The connectivity state of the channel or subchannel.  Implementations
+        should always set this.
+        """
+
+    @property
+    def trace(self) -> global___ChannelTrace:
+        """A trace of recent events on the channel.  May be absent."""
+
+    @property
     def last_call_started_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a call was started on the channel."""
+
     def __init__(
         self,
         *,
         state: global___ChannelConnectivityState | None = ...,
         target: builtins.str = ...,
         trace: global___ChannelTrace | None = ...,
         calls_started: builtins.int = ...,
         calls_succeeded: builtins.int = ...,
         calls_failed: builtins.int = ...,
         last_call_started_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["last_call_started_timestamp", b"last_call_started_timestamp", "state", b"state", "trace", b"trace"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["calls_failed", b"calls_failed", "calls_started", b"calls_started", "calls_succeeded", b"calls_succeeded", "last_call_started_timestamp", b"last_call_started_timestamp", "state", b"state", "target", b"target", "trace", b"trace"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["last_call_started_timestamp", b"last_call_started_timestamp", "state", b"state", "trace", b"trace"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["calls_failed", b"calls_failed", "calls_started", b"calls_started", "calls_succeeded", b"calls_succeeded", "last_call_started_timestamp", b"last_call_started_timestamp", "state", b"state", "target", b"target", "trace", b"trace"]) -> None: ...
 
 global___ChannelData = ChannelData
 
-@typing_extensions.final
+@typing.final
 class ChannelTraceEvent(google.protobuf.message.Message):
     """A trace event is an interesting thing that happened to a channel or
     subchannel, such as creation, address resolution, subchannel creation, etc.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Severity:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _SeverityEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ChannelTraceEvent._Severity.ValueType], builtins.type):  # noqa: F821
+    class _SeverityEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ChannelTraceEvent._Severity.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         CT_UNKNOWN: ChannelTraceEvent._Severity.ValueType  # 0
         CT_INFO: ChannelTraceEvent._Severity.ValueType  # 1
         CT_WARNING: ChannelTraceEvent._Severity.ValueType  # 2
         CT_ERROR: ChannelTraceEvent._Severity.ValueType  # 3
 
     class Severity(_Severity, metaclass=_SeverityEnumTypeWrapper):
@@ -251,34 +265,35 @@
     description: builtins.str
     """High level description of the event."""
     severity: global___ChannelTraceEvent.Severity.ValueType
     """the severity of the trace event"""
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """When this event occurred."""
+
     @property
     def channel_ref(self) -> global___ChannelRef: ...
     @property
     def subchannel_ref(self) -> global___SubchannelRef: ...
     def __init__(
         self,
         *,
         description: builtins.str = ...,
         severity: global___ChannelTraceEvent.Severity.ValueType = ...,
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         channel_ref: global___ChannelRef | None = ...,
         subchannel_ref: global___SubchannelRef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["channel_ref", b"channel_ref", "child_ref", b"child_ref", "subchannel_ref", b"subchannel_ref", "timestamp", b"timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_ref", b"channel_ref", "child_ref", b"child_ref", "description", b"description", "severity", b"severity", "subchannel_ref", b"subchannel_ref", "timestamp", b"timestamp"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["child_ref", b"child_ref"]) -> typing_extensions.Literal["channel_ref", "subchannel_ref"] | None: ...
+    def HasField(self, field_name: typing.Literal["channel_ref", b"channel_ref", "child_ref", b"child_ref", "subchannel_ref", b"subchannel_ref", "timestamp", b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["channel_ref", b"channel_ref", "child_ref", b"child_ref", "description", b"description", "severity", b"severity", "subchannel_ref", b"subchannel_ref", "timestamp", b"timestamp"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["child_ref", b"child_ref"]) -> typing.Literal["channel_ref", "subchannel_ref"] | None: ...
 
 global___ChannelTraceEvent = ChannelTraceEvent
 
-@typing_extensions.final
+@typing.final
 class ChannelTrace(google.protobuf.message.Message):
     """ChannelTrace represents the recent events that have occurred on the channel."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NUM_EVENTS_LOGGED_FIELD_NUMBER: builtins.int
     CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
@@ -287,30 +302,32 @@
     """Number of events ever logged in this tracing object. This can differ from
     events.size() because events can be overwritten or garbage collected by
     implementations.
     """
     @property
     def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Time that this channel was created."""
+
     @property
     def events(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelTraceEvent]:
         """List of events that have occurred on this channel."""
+
     def __init__(
         self,
         *,
         num_events_logged: builtins.int = ...,
         creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         events: collections.abc.Iterable[global___ChannelTraceEvent] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "events", b"events", "num_events_logged", b"num_events_logged"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["creation_timestamp", b"creation_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["creation_timestamp", b"creation_timestamp", "events", b"events", "num_events_logged", b"num_events_logged"]) -> None: ...
 
 global___ChannelTrace = ChannelTrace
 
-@typing_extensions.final
+@typing.final
 class ChannelRef(google.protobuf.message.Message):
     """ChannelRef is a reference to a Channel."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHANNEL_ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -320,19 +337,19 @@
     """An optional name associated with the channel."""
     def __init__(
         self,
         *,
         channel_id: builtins.int = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_id", b"channel_id", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel_id", b"channel_id", "name", b"name"]) -> None: ...
 
 global___ChannelRef = ChannelRef
 
-@typing_extensions.final
+@typing.final
 class SubchannelRef(google.protobuf.message.Message):
     """SubchannelRef is a reference to a Subchannel."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBCHANNEL_ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -342,19 +359,19 @@
     """An optional name associated with the subchannel."""
     def __init__(
         self,
         *,
         subchannel_id: builtins.int = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "subchannel_id", b"subchannel_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "subchannel_id", b"subchannel_id"]) -> None: ...
 
 global___SubchannelRef = SubchannelRef
 
-@typing_extensions.final
+@typing.final
 class SocketRef(google.protobuf.message.Message):
     """SocketRef is a reference to a Socket."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOCKET_ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -364,19 +381,19 @@
     """An optional name associated with the socket."""
     def __init__(
         self,
         *,
         socket_id: builtins.int = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "socket_id", b"socket_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "socket_id", b"socket_id"]) -> None: ...
 
 global___SocketRef = SocketRef
 
-@typing_extensions.final
+@typing.final
 class ServerRef(google.protobuf.message.Message):
     """ServerRef is a reference to a Server."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVER_ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -386,138 +403,148 @@
     """An optional name associated with the server."""
     def __init__(
         self,
         *,
         server_id: builtins.int = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "server_id", b"server_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "server_id", b"server_id"]) -> None: ...
 
 global___ServerRef = ServerRef
 
-@typing_extensions.final
+@typing.final
 class Server(google.protobuf.message.Message):
     """Server represents a single server.  There may be multiple servers in a single
     program.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REF_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     LISTEN_SOCKET_FIELD_NUMBER: builtins.int
     @property
     def ref(self) -> global___ServerRef:
         """The identifier for a Server.  This should be set."""
+
     @property
     def data(self) -> global___ServerData:
         """The associated data of the Server."""
+
     @property
     def listen_socket(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SocketRef]:
         """The sockets that the server is listening on.  There are no ordering
         guarantees.  This may be absent.
         """
+
     def __init__(
         self,
         *,
         ref: global___ServerRef | None = ...,
         data: global___ServerData | None = ...,
         listen_socket: collections.abc.Iterable[global___SocketRef] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "listen_socket", b"listen_socket", "ref", b"ref"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "ref", b"ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data", "listen_socket", b"listen_socket", "ref", b"ref"]) -> None: ...
 
 global___Server = Server
 
-@typing_extensions.final
+@typing.final
 class ServerData(google.protobuf.message.Message):
     """ServerData is data for a specific Server."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRACE_FIELD_NUMBER: builtins.int
     CALLS_STARTED_FIELD_NUMBER: builtins.int
     CALLS_SUCCEEDED_FIELD_NUMBER: builtins.int
     CALLS_FAILED_FIELD_NUMBER: builtins.int
     LAST_CALL_STARTED_TIMESTAMP_FIELD_NUMBER: builtins.int
-    @property
-    def trace(self) -> global___ChannelTrace:
-        """A trace of recent events on the server.  May be absent."""
     calls_started: builtins.int
     """The number of incoming calls started on the server"""
     calls_succeeded: builtins.int
     """The number of incoming calls that have completed with an OK status"""
     calls_failed: builtins.int
     """The number of incoming calls that have a completed with a non-OK status"""
     @property
+    def trace(self) -> global___ChannelTrace:
+        """A trace of recent events on the server.  May be absent."""
+
+    @property
     def last_call_started_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a call was started on the server."""
+
     def __init__(
         self,
         *,
         trace: global___ChannelTrace | None = ...,
         calls_started: builtins.int = ...,
         calls_succeeded: builtins.int = ...,
         calls_failed: builtins.int = ...,
         last_call_started_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["last_call_started_timestamp", b"last_call_started_timestamp", "trace", b"trace"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["calls_failed", b"calls_failed", "calls_started", b"calls_started", "calls_succeeded", b"calls_succeeded", "last_call_started_timestamp", b"last_call_started_timestamp", "trace", b"trace"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["last_call_started_timestamp", b"last_call_started_timestamp", "trace", b"trace"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["calls_failed", b"calls_failed", "calls_started", b"calls_started", "calls_succeeded", b"calls_succeeded", "last_call_started_timestamp", b"last_call_started_timestamp", "trace", b"trace"]) -> None: ...
 
 global___ServerData = ServerData
 
-@typing_extensions.final
+@typing.final
 class Socket(google.protobuf.message.Message):
     """Information about an actual connection.  Pronounced "sock-ay"."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REF_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     LOCAL_FIELD_NUMBER: builtins.int
     REMOTE_FIELD_NUMBER: builtins.int
     SECURITY_FIELD_NUMBER: builtins.int
     REMOTE_NAME_FIELD_NUMBER: builtins.int
+    remote_name: builtins.str
+    """Optional, represents the name of the remote endpoint, if different than
+    the original target name.
+    """
     @property
     def ref(self) -> global___SocketRef:
         """The identifier for the Socket."""
+
     @property
     def data(self) -> global___SocketData:
         """Data specific to this Socket."""
+
     @property
     def local(self) -> global___Address:
         """The locally bound address."""
+
     @property
     def remote(self) -> global___Address:
         """The remote bound address.  May be absent."""
+
     @property
     def security(self) -> global___Security:
         """Security details for this socket.  May be absent if not available, or
         there is no security on the socket.
         """
-    remote_name: builtins.str
-    """Optional, represents the name of the remote endpoint, if different than
-    the original target name.
-    """
+
     def __init__(
         self,
         *,
         ref: global___SocketRef | None = ...,
         data: global___SocketData | None = ...,
         local: global___Address | None = ...,
         remote: global___Address | None = ...,
         security: global___Security | None = ...,
         remote_name: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "local", b"local", "ref", b"ref", "remote", b"remote", "security", b"security"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "local", b"local", "ref", b"ref", "remote", b"remote", "remote_name", b"remote_name", "security", b"security"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "local", b"local", "ref", b"ref", "remote", b"remote", "security", b"security"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data", "local", b"local", "ref", b"ref", "remote", b"remote", "remote_name", b"remote_name", "security", b"security"]) -> None: ...
 
 global___Socket = Socket
 
-@typing_extensions.final
+@typing.final
 class SocketData(google.protobuf.message.Message):
     """SocketData is data associated for a specific Socket.  The fields present
     are specific to the implementation, so there may be minor differences in
     the semantics.  (e.g. flow control windows)
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -556,42 +583,49 @@
     ping messages.
     """
     @property
     def last_local_stream_created_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a stream was created by this endpoint.  Usually unset for
         servers.
         """
+
     @property
     def last_remote_stream_created_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a stream was created by the remote endpoint.  Usually unset
         for clients.
         """
+
     @property
     def last_message_sent_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a message was sent by this endpoint."""
+
     @property
     def last_message_received_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The last time a message was received by this endpoint."""
+
     @property
     def local_flow_control_window(self) -> google.protobuf.wrappers_pb2.Int64Value:
         """The amount of window, granted to the local endpoint by the remote endpoint.
         This may be slightly out of date due to network latency.  This does NOT
         include stream level or TCP level flow control info.
         """
+
     @property
     def remote_flow_control_window(self) -> google.protobuf.wrappers_pb2.Int64Value:
         """The amount of window, granted to the remote endpoint by the local endpoint.
         This may be slightly out of date due to network latency.  This does NOT
         include stream level or TCP level flow control info.
         """
+
     @property
     def option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SocketOption]:
         """Socket options set on this socket.  May be absent if 'summary' is set
         on GetSocketRequest.
         """
+
     def __init__(
         self,
         *,
         streams_started: builtins.int = ...,
         streams_succeeded: builtins.int = ...,
         streams_failed: builtins.int = ...,
         messages_sent: builtins.int = ...,
@@ -601,26 +635,26 @@
         last_remote_stream_created_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_message_sent_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_message_received_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         local_flow_control_window: google.protobuf.wrappers_pb2.Int64Value | None = ...,
         remote_flow_control_window: google.protobuf.wrappers_pb2.Int64Value | None = ...,
         option: collections.abc.Iterable[global___SocketOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["last_local_stream_created_timestamp", b"last_local_stream_created_timestamp", "last_message_received_timestamp", b"last_message_received_timestamp", "last_message_sent_timestamp", b"last_message_sent_timestamp", "last_remote_stream_created_timestamp", b"last_remote_stream_created_timestamp", "local_flow_control_window", b"local_flow_control_window", "remote_flow_control_window", b"remote_flow_control_window"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["keep_alives_sent", b"keep_alives_sent", "last_local_stream_created_timestamp", b"last_local_stream_created_timestamp", "last_message_received_timestamp", b"last_message_received_timestamp", "last_message_sent_timestamp", b"last_message_sent_timestamp", "last_remote_stream_created_timestamp", b"last_remote_stream_created_timestamp", "local_flow_control_window", b"local_flow_control_window", "messages_received", b"messages_received", "messages_sent", b"messages_sent", "option", b"option", "remote_flow_control_window", b"remote_flow_control_window", "streams_failed", b"streams_failed", "streams_started", b"streams_started", "streams_succeeded", b"streams_succeeded"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["last_local_stream_created_timestamp", b"last_local_stream_created_timestamp", "last_message_received_timestamp", b"last_message_received_timestamp", "last_message_sent_timestamp", b"last_message_sent_timestamp", "last_remote_stream_created_timestamp", b"last_remote_stream_created_timestamp", "local_flow_control_window", b"local_flow_control_window", "remote_flow_control_window", b"remote_flow_control_window"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["keep_alives_sent", b"keep_alives_sent", "last_local_stream_created_timestamp", b"last_local_stream_created_timestamp", "last_message_received_timestamp", b"last_message_received_timestamp", "last_message_sent_timestamp", b"last_message_sent_timestamp", "last_remote_stream_created_timestamp", b"last_remote_stream_created_timestamp", "local_flow_control_window", b"local_flow_control_window", "messages_received", b"messages_received", "messages_sent", b"messages_sent", "option", b"option", "remote_flow_control_window", b"remote_flow_control_window", "streams_failed", b"streams_failed", "streams_started", b"streams_started", "streams_succeeded", b"streams_succeeded"]) -> None: ...
 
 global___SocketData = SocketData
 
-@typing_extensions.final
+@typing.final
 class Address(google.protobuf.message.Message):
     """Address represents the address used to create the socket."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class TcpIpAddress(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         IP_ADDRESS_FIELD_NUMBER: builtins.int
         PORT_FIELD_NUMBER: builtins.int
         ip_address: builtins.bytes
         """Either the IPv4 or IPv6 address in bytes.  Will be either 4 bytes or 16
@@ -630,52 +664,53 @@
         """0-64k, or -1 if not appropriate."""
         def __init__(
             self,
             *,
             ip_address: builtins.bytes = ...,
             port: builtins.int = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["ip_address", b"ip_address", "port", b"port"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["ip_address", b"ip_address", "port", b"port"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class UdsAddress(google.protobuf.message.Message):
         """A Unix Domain Socket address."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         FILENAME_FIELD_NUMBER: builtins.int
         filename: builtins.str
         def __init__(
             self,
             *,
             filename: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["filename", b"filename"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["filename", b"filename"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class OtherAddress(google.protobuf.message.Message):
         """An address type not included above."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         name: builtins.str
         """The human readable version of the value.  This value should be set."""
         @property
         def value(self) -> google.protobuf.any_pb2.Any:
             """The actual address message."""
+
         def __init__(
             self,
             *,
             name: builtins.str = ...,
             value: google.protobuf.any_pb2.Any | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["name", b"name", "value", b"value"]) -> None: ...
 
     TCPIP_ADDRESS_FIELD_NUMBER: builtins.int
     UDS_ADDRESS_FIELD_NUMBER: builtins.int
     OTHER_ADDRESS_FIELD_NUMBER: builtins.int
     @property
     def tcpip_address(self) -> global___Address.TcpIpAddress: ...
     @property
@@ -685,27 +720,27 @@
     def __init__(
         self,
         *,
         tcpip_address: global___Address.TcpIpAddress | None = ...,
         uds_address: global___Address.UdsAddress | None = ...,
         other_address: global___Address.OtherAddress | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["address", b"address", "other_address", b"other_address", "tcpip_address", b"tcpip_address", "uds_address", b"uds_address"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "other_address", b"other_address", "tcpip_address", b"tcpip_address", "uds_address", b"uds_address"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["address", b"address"]) -> typing_extensions.Literal["tcpip_address", "uds_address", "other_address"] | None: ...
+    def HasField(self, field_name: typing.Literal["address", b"address", "other_address", b"other_address", "tcpip_address", b"tcpip_address", "uds_address", b"uds_address"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "other_address", b"other_address", "tcpip_address", b"tcpip_address", "uds_address", b"uds_address"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["address", b"address"]) -> typing.Literal["tcpip_address", "uds_address", "other_address"] | None: ...
 
 global___Address = Address
 
-@typing_extensions.final
+@typing.final
 class Security(google.protobuf.message.Message):
     """Security represents details about how secure the socket is."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Tls(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         STANDARD_NAME_FIELD_NUMBER: builtins.int
         OTHER_NAME_FIELD_NUMBER: builtins.int
         LOCAL_CERTIFICATE_FIELD_NUMBER: builtins.int
         REMOTE_CERTIFICATE_FIELD_NUMBER: builtins.int
@@ -725,57 +760,58 @@
             self,
             *,
             standard_name: builtins.str = ...,
             other_name: builtins.str = ...,
             local_certificate: builtins.bytes = ...,
             remote_certificate: builtins.bytes = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["cipher_suite", b"cipher_suite", "other_name", b"other_name", "standard_name", b"standard_name"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["cipher_suite", b"cipher_suite", "local_certificate", b"local_certificate", "other_name", b"other_name", "remote_certificate", b"remote_certificate", "standard_name", b"standard_name"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["cipher_suite", b"cipher_suite"]) -> typing_extensions.Literal["standard_name", "other_name"] | None: ...
+        def HasField(self, field_name: typing.Literal["cipher_suite", b"cipher_suite", "other_name", b"other_name", "standard_name", b"standard_name"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["cipher_suite", b"cipher_suite", "local_certificate", b"local_certificate", "other_name", b"other_name", "remote_certificate", b"remote_certificate", "standard_name", b"standard_name"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing.Literal["cipher_suite", b"cipher_suite"]) -> typing.Literal["standard_name", "other_name"] | None: ...
 
-    @typing_extensions.final
+    @typing.final
     class OtherSecurity(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         name: builtins.str
         """The human readable version of the value."""
         @property
         def value(self) -> google.protobuf.any_pb2.Any:
             """The actual security details message."""
+
         def __init__(
             self,
             *,
             name: builtins.str = ...,
             value: google.protobuf.any_pb2.Any | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["name", b"name", "value", b"value"]) -> None: ...
 
     TLS_FIELD_NUMBER: builtins.int
     OTHER_FIELD_NUMBER: builtins.int
     @property
     def tls(self) -> global___Security.Tls: ...
     @property
     def other(self) -> global___Security.OtherSecurity: ...
     def __init__(
         self,
         *,
         tls: global___Security.Tls | None = ...,
         other: global___Security.OtherSecurity | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["model", b"model", "other", b"other", "tls", b"tls"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["model", b"model", "other", b"other", "tls", b"tls"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["model", b"model"]) -> typing_extensions.Literal["tls", "other"] | None: ...
+    def HasField(self, field_name: typing.Literal["model", b"model", "other", b"other", "tls", b"tls"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["model", b"model", "other", b"other", "tls", b"tls"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["model", b"model"]) -> typing.Literal["tls", "other"] | None: ...
 
 global___Security = Security
 
-@typing_extensions.final
+@typing.final
 class SocketOption(google.protobuf.message.Message):
     """SocketOption represents socket options for a socket.  Specifically, these
     are the options returned by getsockopt().
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -791,27 +827,28 @@
     additional will be set.
     """
     @property
     def additional(self) -> google.protobuf.any_pb2.Any:
         """Additional data associated with the socket option.  At least one of value
         or additional will be set.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         value: builtins.str = ...,
         additional: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["additional", b"additional"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional", b"additional", "name", b"name", "value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["additional", b"additional"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["additional", b"additional", "name", b"name", "value", b"value"]) -> None: ...
 
 global___SocketOption = SocketOption
 
-@typing_extensions.final
+@typing.final
 class SocketOptionTimeout(google.protobuf.message.Message):
     """For use with SocketOption's additional field.  This is primarily used for
     SO_RCVTIMEO and SO_SNDTIMEO
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -819,46 +856,47 @@
     @property
     def duration(self) -> google.protobuf.duration_pb2.Duration: ...
     def __init__(
         self,
         *,
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["duration", b"duration"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["duration", b"duration"]) -> None: ...
 
 global___SocketOptionTimeout = SocketOptionTimeout
 
-@typing_extensions.final
+@typing.final
 class SocketOptionLinger(google.protobuf.message.Message):
     """For use with SocketOption's additional field.  This is primarily used for
     SO_LINGER.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACTIVE_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     active: builtins.bool
     """active maps to `struct linger.l_onoff`"""
     @property
     def duration(self) -> google.protobuf.duration_pb2.Duration:
         """duration maps to `struct linger.l_linger`"""
+
     def __init__(
         self,
         *,
         active: builtins.bool = ...,
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["active", b"active", "duration", b"duration"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["duration", b"duration"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["active", b"active", "duration", b"duration"]) -> None: ...
 
 global___SocketOptionLinger = SocketOptionLinger
 
-@typing_extensions.final
+@typing.final
 class SocketOptionTcpInfo(google.protobuf.message.Message):
     """For use with SocketOption's additional field.  Tcp info for
     SOL_TCP and TCP_INFO.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -949,19 +987,19 @@
         tcpi_rtt: builtins.int = ...,
         tcpi_rttvar: builtins.int = ...,
         tcpi_snd_ssthresh: builtins.int = ...,
         tcpi_snd_cwnd: builtins.int = ...,
         tcpi_advmss: builtins.int = ...,
         tcpi_reordering: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tcpi_advmss", b"tcpi_advmss", "tcpi_ato", b"tcpi_ato", "tcpi_backoff", b"tcpi_backoff", "tcpi_ca_state", b"tcpi_ca_state", "tcpi_fackets", b"tcpi_fackets", "tcpi_last_ack_recv", b"tcpi_last_ack_recv", "tcpi_last_ack_sent", b"tcpi_last_ack_sent", "tcpi_last_data_recv", b"tcpi_last_data_recv", "tcpi_last_data_sent", b"tcpi_last_data_sent", "tcpi_lost", b"tcpi_lost", "tcpi_options", b"tcpi_options", "tcpi_pmtu", b"tcpi_pmtu", "tcpi_probes", b"tcpi_probes", "tcpi_rcv_mss", b"tcpi_rcv_mss", "tcpi_rcv_ssthresh", b"tcpi_rcv_ssthresh", "tcpi_rcv_wscale", b"tcpi_rcv_wscale", "tcpi_reordering", b"tcpi_reordering", "tcpi_retrans", b"tcpi_retrans", "tcpi_retransmits", b"tcpi_retransmits", "tcpi_rto", b"tcpi_rto", "tcpi_rtt", b"tcpi_rtt", "tcpi_rttvar", b"tcpi_rttvar", "tcpi_sacked", b"tcpi_sacked", "tcpi_snd_cwnd", b"tcpi_snd_cwnd", "tcpi_snd_mss", b"tcpi_snd_mss", "tcpi_snd_ssthresh", b"tcpi_snd_ssthresh", "tcpi_snd_wscale", b"tcpi_snd_wscale", "tcpi_state", b"tcpi_state", "tcpi_unacked", b"tcpi_unacked"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["tcpi_advmss", b"tcpi_advmss", "tcpi_ato", b"tcpi_ato", "tcpi_backoff", b"tcpi_backoff", "tcpi_ca_state", b"tcpi_ca_state", "tcpi_fackets", b"tcpi_fackets", "tcpi_last_ack_recv", b"tcpi_last_ack_recv", "tcpi_last_ack_sent", b"tcpi_last_ack_sent", "tcpi_last_data_recv", b"tcpi_last_data_recv", "tcpi_last_data_sent", b"tcpi_last_data_sent", "tcpi_lost", b"tcpi_lost", "tcpi_options", b"tcpi_options", "tcpi_pmtu", b"tcpi_pmtu", "tcpi_probes", b"tcpi_probes", "tcpi_rcv_mss", b"tcpi_rcv_mss", "tcpi_rcv_ssthresh", b"tcpi_rcv_ssthresh", "tcpi_rcv_wscale", b"tcpi_rcv_wscale", "tcpi_reordering", b"tcpi_reordering", "tcpi_retrans", b"tcpi_retrans", "tcpi_retransmits", b"tcpi_retransmits", "tcpi_rto", b"tcpi_rto", "tcpi_rtt", b"tcpi_rtt", "tcpi_rttvar", b"tcpi_rttvar", "tcpi_sacked", b"tcpi_sacked", "tcpi_snd_cwnd", b"tcpi_snd_cwnd", "tcpi_snd_mss", b"tcpi_snd_mss", "tcpi_snd_ssthresh", b"tcpi_snd_ssthresh", "tcpi_snd_wscale", b"tcpi_snd_wscale", "tcpi_state", b"tcpi_state", "tcpi_unacked", b"tcpi_unacked"]) -> None: ...
 
 global___SocketOptionTcpInfo = SocketOptionTcpInfo
 
-@typing_extensions.final
+@typing.final
 class GetTopChannelsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     START_CHANNEL_ID_FIELD_NUMBER: builtins.int
     MAX_RESULTS_FIELD_NUMBER: builtins.int
     start_channel_id: builtins.int
     """start_channel_id indicates that only channels at or above this id should be
@@ -977,46 +1015,47 @@
     """
     def __init__(
         self,
         *,
         start_channel_id: builtins.int = ...,
         max_results: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_results", b"max_results", "start_channel_id", b"start_channel_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_results", b"max_results", "start_channel_id", b"start_channel_id"]) -> None: ...
 
 global___GetTopChannelsRequest = GetTopChannelsRequest
 
-@typing_extensions.final
+@typing.final
 class GetTopChannelsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHANNEL_FIELD_NUMBER: builtins.int
     END_FIELD_NUMBER: builtins.int
+    end: builtins.bool
+    """If set, indicates that the list of channels is the final list.  Requesting
+    more channels can only return more if they are created after this RPC
+    completes.
+    """
     @property
     def channel(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Channel]:
         """list of channels that the connection detail service knows about.  Sorted in
         ascending channel_id order.
         Must contain at least 1 result, otherwise 'end' must be true.
         """
-    end: builtins.bool
-    """If set, indicates that the list of channels is the final list.  Requesting
-    more channels can only return more if they are created after this RPC
-    completes.
-    """
+
     def __init__(
         self,
         *,
         channel: collections.abc.Iterable[global___Channel] | None = ...,
         end: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel", "end", b"end"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel", b"channel", "end", b"end"]) -> None: ...
 
 global___GetTopChannelsResponse = GetTopChannelsResponse
 
-@typing_extensions.final
+@typing.final
 class GetServersRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     START_SERVER_ID_FIELD_NUMBER: builtins.int
     MAX_RESULTS_FIELD_NUMBER: builtins.int
     start_server_id: builtins.int
     """start_server_id indicates that only servers at or above this id should be
@@ -1032,82 +1071,84 @@
     """
     def __init__(
         self,
         *,
         start_server_id: builtins.int = ...,
         max_results: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_results", b"max_results", "start_server_id", b"start_server_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_results", b"max_results", "start_server_id", b"start_server_id"]) -> None: ...
 
 global___GetServersRequest = GetServersRequest
 
-@typing_extensions.final
+@typing.final
 class GetServersResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVER_FIELD_NUMBER: builtins.int
     END_FIELD_NUMBER: builtins.int
+    end: builtins.bool
+    """If set, indicates that the list of servers is the final list.  Requesting
+    more servers will only return more if they are created after this RPC
+    completes.
+    """
     @property
     def server(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Server]:
         """list of servers that the connection detail service knows about.  Sorted in
         ascending server_id order.
         Must contain at least 1 result, otherwise 'end' must be true.
         """
-    end: builtins.bool
-    """If set, indicates that the list of servers is the final list.  Requesting
-    more servers will only return more if they are created after this RPC
-    completes.
-    """
+
     def __init__(
         self,
         *,
         server: collections.abc.Iterable[global___Server] | None = ...,
         end: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "server", b"server"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end", b"end", "server", b"server"]) -> None: ...
 
 global___GetServersResponse = GetServersResponse
 
-@typing_extensions.final
+@typing.final
 class GetServerRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVER_ID_FIELD_NUMBER: builtins.int
     server_id: builtins.int
     """server_id is the identifier of the specific server to get."""
     def __init__(
         self,
         *,
         server_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["server_id", b"server_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["server_id", b"server_id"]) -> None: ...
 
 global___GetServerRequest = GetServerRequest
 
-@typing_extensions.final
+@typing.final
 class GetServerResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVER_FIELD_NUMBER: builtins.int
     @property
     def server(self) -> global___Server:
         """The Server that corresponds to the requested server_id.  This field
         should be set.
         """
+
     def __init__(
         self,
         *,
         server: global___Server | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["server", b"server"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["server", b"server"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["server", b"server"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["server", b"server"]) -> None: ...
 
 global___GetServerResponse = GetServerResponse
 
-@typing_extensions.final
+@typing.final
 class GetServerSocketsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVER_ID_FIELD_NUMBER: builtins.int
     START_SOCKET_ID_FIELD_NUMBER: builtins.int
     MAX_RESULTS_FIELD_NUMBER: builtins.int
     server_id: builtins.int
@@ -1126,118 +1167,121 @@
     def __init__(
         self,
         *,
         server_id: builtins.int = ...,
         start_socket_id: builtins.int = ...,
         max_results: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_results", b"max_results", "server_id", b"server_id", "start_socket_id", b"start_socket_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_results", b"max_results", "server_id", b"server_id", "start_socket_id", b"start_socket_id"]) -> None: ...
 
 global___GetServerSocketsRequest = GetServerSocketsRequest
 
-@typing_extensions.final
+@typing.final
 class GetServerSocketsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOCKET_REF_FIELD_NUMBER: builtins.int
     END_FIELD_NUMBER: builtins.int
+    end: builtins.bool
+    """If set, indicates that the list of sockets is the final list.  Requesting
+    more sockets will only return more if they are created after this RPC
+    completes.
+    """
     @property
     def socket_ref(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SocketRef]:
         """list of socket refs that the connection detail service knows about.  Sorted in
         ascending socket_id order.
         Must contain at least 1 result, otherwise 'end' must be true.
         """
-    end: builtins.bool
-    """If set, indicates that the list of sockets is the final list.  Requesting
-    more sockets will only return more if they are created after this RPC
-    completes.
-    """
+
     def __init__(
         self,
         *,
         socket_ref: collections.abc.Iterable[global___SocketRef] | None = ...,
         end: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "socket_ref", b"socket_ref"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end", b"end", "socket_ref", b"socket_ref"]) -> None: ...
 
 global___GetServerSocketsResponse = GetServerSocketsResponse
 
-@typing_extensions.final
+@typing.final
 class GetChannelRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHANNEL_ID_FIELD_NUMBER: builtins.int
     channel_id: builtins.int
     """channel_id is the identifier of the specific channel to get."""
     def __init__(
         self,
         *,
         channel_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_id", b"channel_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel_id", b"channel_id"]) -> None: ...
 
 global___GetChannelRequest = GetChannelRequest
 
-@typing_extensions.final
+@typing.final
 class GetChannelResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHANNEL_FIELD_NUMBER: builtins.int
     @property
     def channel(self) -> global___Channel:
         """The Channel that corresponds to the requested channel_id.  This field
         should be set.
         """
+
     def __init__(
         self,
         *,
         channel: global___Channel | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["channel", b"channel"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["channel", b"channel"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["channel", b"channel"]) -> None: ...
 
 global___GetChannelResponse = GetChannelResponse
 
-@typing_extensions.final
+@typing.final
 class GetSubchannelRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBCHANNEL_ID_FIELD_NUMBER: builtins.int
     subchannel_id: builtins.int
     """subchannel_id is the identifier of the specific subchannel to get."""
     def __init__(
         self,
         *,
         subchannel_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["subchannel_id", b"subchannel_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["subchannel_id", b"subchannel_id"]) -> None: ...
 
 global___GetSubchannelRequest = GetSubchannelRequest
 
-@typing_extensions.final
+@typing.final
 class GetSubchannelResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBCHANNEL_FIELD_NUMBER: builtins.int
     @property
     def subchannel(self) -> global___Subchannel:
         """The Subchannel that corresponds to the requested subchannel_id.  This
         field should be set.
         """
+
     def __init__(
         self,
         *,
         subchannel: global___Subchannel | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["subchannel", b"subchannel"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["subchannel", b"subchannel"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["subchannel", b"subchannel"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["subchannel", b"subchannel"]) -> None: ...
 
 global___GetSubchannelResponse = GetSubchannelResponse
 
-@typing_extensions.final
+@typing.final
 class GetSocketRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOCKET_ID_FIELD_NUMBER: builtins.int
     SUMMARY_FIELD_NUMBER: builtins.int
     socket_id: builtins.int
     """socket_id is the identifier of the specific socket to get."""
@@ -1248,30 +1292,31 @@
     """
     def __init__(
         self,
         *,
         socket_id: builtins.int = ...,
         summary: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["socket_id", b"socket_id", "summary", b"summary"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["socket_id", b"socket_id", "summary", b"summary"]) -> None: ...
 
 global___GetSocketRequest = GetSocketRequest
 
-@typing_extensions.final
+@typing.final
 class GetSocketResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOCKET_FIELD_NUMBER: builtins.int
     @property
     def socket(self) -> global___Socket:
         """The Socket that corresponds to the requested socket_id.  This field
         should be set.
         """
+
     def __init__(
         self,
         *,
         socket: global___Socket | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["socket", b"socket"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["socket", b"socket"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["socket", b"socket"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["socket", b"socket"]) -> None: ...
 
 global___GetSocketResponse = GetSocketResponse
```

### Comparing `grpclib-0.4.7rc1/grpclib/client.py` & `grpclib-0.4.8rc1/grpclib/client.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/config.py` & `grpclib-0.4.8rc1/grpclib/config.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/const.py` & `grpclib-0.4.8rc1/grpclib/const.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/encoding/base.py` & `grpclib-0.4.8rc1/grpclib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/encoding/proto.py` & `grpclib-0.4.8rc1/grpclib/encoding/proto.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/events.py` & `grpclib-0.4.8rc1/grpclib/events.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/exceptions.py` & `grpclib-0.4.8rc1/grpclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/health/check.py` & `grpclib-0.4.8rc1/grpclib/health/check.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/health/service.py` & `grpclib-0.4.8rc1/grpclib/health/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/health/v1/health_grpc.py` & `grpclib-0.4.8rc1/grpclib/health/v1/health_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/health/v1/health_pb2.py` & `grpclib-0.4.8rc1/grpclib/health/v1/health_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpclib/health/v1/health.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +16,16 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1egrpclib/health/v1/health.proto\x12\x0egrpc.health.v1\"%\n\x12HealthCheckRequest\x12\x0f\n\x07service\x18\x01 \x01(\t\"\xa9\x01\n\x13HealthCheckResponse\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.grpc.health.v1.HealthCheckResponse.ServingStatus\"O\n\rServingStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x0f\n\x0bNOT_SERVING\x10\x02\x12\x13\n\x0fSERVICE_UNKNOWN\x10\x03\x32\xae\x01\n\x06Health\x12P\n\x05\x43heck\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse\x12R\n\x05Watch\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse0\x01\x42\x61\n\x11io.grpc.health.v1B\x0bHealthProtoP\x01Z,google.golang.org/grpc/health/grpc_health_v1\xaa\x02\x0eGrpc.Health.V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpclib.health.v1.health_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021io.grpc.health.v1B\013HealthProtoP\001Z,google.golang.org/grpc/health/grpc_health_v1\252\002\016Grpc.Health.V1'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\021io.grpc.health.v1B\013HealthProtoP\001Z,google.golang.org/grpc/health/grpc_health_v1\252\002\016Grpc.Health.V1'
   _globals['_HEALTHCHECKREQUEST']._serialized_start=50
   _globals['_HEALTHCHECKREQUEST']._serialized_end=87
   _globals['_HEALTHCHECKRESPONSE']._serialized_start=90
   _globals['_HEALTHCHECKRESPONSE']._serialized_end=259
   _globals['_HEALTHCHECKRESPONSE_SERVINGSTATUS']._serialized_start=180
   _globals['_HEALTHCHECKRESPONSE_SERVINGSTATUS']._serialized_end=259
   _globals['_HEALTH']._serialized_start=262
```

### Comparing `grpclib-0.4.7rc1/grpclib/health/v1/health_pb2.pyi` & `grpclib-0.4.8rc1/grpclib/health/v1/health_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 The canonical version of this proto can be found at
 https://github.com/grpc/grpc-proto/blob/master/grpc/health/v1/health.proto
 """
+
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class HealthCheckRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_FIELD_NUMBER: builtins.int
     service: builtins.str
     def __init__(
         self,
         *,
         service: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["service", b"service"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["service", b"service"]) -> None: ...
 
 global___HealthCheckRequest = HealthCheckRequest
 
-@typing_extensions.final
+@typing.final
 class HealthCheckResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ServingStatus:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _ServingStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[HealthCheckResponse._ServingStatus.ValueType], builtins.type):  # noqa: F821
+    class _ServingStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[HealthCheckResponse._ServingStatus.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         UNKNOWN: HealthCheckResponse._ServingStatus.ValueType  # 0
         SERVING: HealthCheckResponse._ServingStatus.ValueType  # 1
         NOT_SERVING: HealthCheckResponse._ServingStatus.ValueType  # 2
         SERVICE_UNKNOWN: HealthCheckResponse._ServingStatus.ValueType  # 3
         """Used only by the Watch method."""
 
@@ -59,10 +60,10 @@
     STATUS_FIELD_NUMBER: builtins.int
     status: global___HealthCheckResponse.ServingStatus.ValueType
     def __init__(
         self,
         *,
         status: global___HealthCheckResponse.ServingStatus.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["status", b"status"]) -> None: ...
 
 global___HealthCheckResponse = HealthCheckResponse
```

### Comparing `grpclib-0.4.7rc1/grpclib/metadata.py` & `grpclib-0.4.8rc1/grpclib/metadata.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/plugin/main.py` & `grpclib-0.4.8rc1/grpclib/plugin/main.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/protocol.py` & `grpclib-0.4.8rc1/grpclib/protocol.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/_deprecated.py` & `grpclib-0.4.8rc1/grpclib/reflection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/service.py` & `grpclib-0.4.8rc1/grpclib/reflection/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_grpc.py` & `grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_pb2.py` & `grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpclib/reflection/v1/reflection.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +16,16 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&grpclib/reflection/v1/reflection.proto\x12\x12grpc.reflection.v1\"\x85\x02\n\x17ServerReflectionRequest\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1a\n\x10\x66ile_by_filename\x18\x03 \x01(\tH\x00\x12 \n\x16\x66ile_containing_symbol\x18\x04 \x01(\tH\x00\x12I\n\x19\x66ile_containing_extension\x18\x05 \x01(\x0b\x32$.grpc.reflection.v1.ExtensionRequestH\x00\x12\'\n\x1d\x61ll_extension_numbers_of_type\x18\x06 \x01(\tH\x00\x12\x17\n\rlist_services\x18\x07 \x01(\tH\x00\x42\x11\n\x0fmessage_request\"E\n\x10\x45xtensionRequest\x12\x17\n\x0f\x63ontaining_type\x18\x01 \x01(\t\x12\x18\n\x10\x65xtension_number\x18\x02 \x01(\x05\"\xb8\x03\n\x18ServerReflectionResponse\x12\x12\n\nvalid_host\x18\x01 \x01(\t\x12\x45\n\x10original_request\x18\x02 \x01(\x0b\x32+.grpc.reflection.v1.ServerReflectionRequest\x12N\n\x18\x66ile_descriptor_response\x18\x04 \x01(\x0b\x32*.grpc.reflection.v1.FileDescriptorResponseH\x00\x12U\n\x1e\x61ll_extension_numbers_response\x18\x05 \x01(\x0b\x32+.grpc.reflection.v1.ExtensionNumberResponseH\x00\x12I\n\x16list_services_response\x18\x06 \x01(\x0b\x32\'.grpc.reflection.v1.ListServiceResponseH\x00\x12;\n\x0e\x65rror_response\x18\x07 \x01(\x0b\x32!.grpc.reflection.v1.ErrorResponseH\x00\x42\x12\n\x10message_response\"7\n\x16\x46ileDescriptorResponse\x12\x1d\n\x15\x66ile_descriptor_proto\x18\x01 \x03(\x0c\"K\n\x17\x45xtensionNumberResponse\x12\x16\n\x0e\x62\x61se_type_name\x18\x01 \x01(\t\x12\x18\n\x10\x65xtension_number\x18\x02 \x03(\x05\"K\n\x13ListServiceResponse\x12\x34\n\x07service\x18\x01 \x03(\x0b\x32#.grpc.reflection.v1.ServiceResponse\"\x1f\n\x0fServiceResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\":\n\rErrorResponse\x12\x12\n\nerror_code\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t2\x89\x01\n\x10ServerReflection\x12u\n\x14ServerReflectionInfo\x12+.grpc.reflection.v1.ServerReflectionRequest\x1a,.grpc.reflection.v1.ServerReflectionResponse(\x01\x30\x01\x42\x66\n\x15io.grpc.reflection.v1B\x15ServerReflectionProtoP\x01Z4google.golang.org/grpc/reflection/grpc_reflection_v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpclib.reflection.v1.reflection_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\025io.grpc.reflection.v1B\025ServerReflectionProtoP\001Z4google.golang.org/grpc/reflection/grpc_reflection_v1'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\025io.grpc.reflection.v1B\025ServerReflectionProtoP\001Z4google.golang.org/grpc/reflection/grpc_reflection_v1'
   _globals['_SERVERREFLECTIONREQUEST']._serialized_start=63
   _globals['_SERVERREFLECTIONREQUEST']._serialized_end=324
   _globals['_EXTENSIONREQUEST']._serialized_start=326
   _globals['_EXTENSIONREQUEST']._serialized_end=395
   _globals['_SERVERREFLECTIONRESPONSE']._serialized_start=398
   _globals['_SERVERREFLECTIONRESPONSE']._serialized_end=838
   _globals['_FILEDESCRIPTORRESPONSE']._serialized_start=840
```

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1/reflection_pb2.pyi` & `grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Service exported by server reflection.  A more complete description of how
-server reflection works can be found at
-https://github.com/grpc/grpc/blob/master/doc/server-reflection.md
-
-The canonical version of this proto can be found at
+Warning: this entire file is deprecated. Use this instead:
 https://github.com/grpc/grpc-proto/blob/master/grpc/reflection/v1/reflection.proto
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ServerReflectionRequest(google.protobuf.message.Message):
     """The message sent by the client when calling ServerReflectionInfo method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HOST_FIELD_NUMBER: builtins.int
     FILE_BY_FILENAME_FIELD_NUMBER: builtins.int
@@ -38,50 +30,51 @@
     file_by_filename: builtins.str
     """Find a proto file by the file name."""
     file_containing_symbol: builtins.str
     """Find the proto file that declares the given fully-qualified symbol name.
     This field should be a fully-qualified symbol name
     (e.g. <package>.<service>[.<method>] or <package>.<type>).
     """
-    @property
-    def file_containing_extension(self) -> global___ExtensionRequest:
-        """Find the proto file which defines an extension extending the given
-        message type with the given field number.
-        """
     all_extension_numbers_of_type: builtins.str
-    """Finds the tag numbers used by all known extensions of the given message
-    type, and appends them to ExtensionNumberResponse in an undefined order.
+    """Finds the tag numbers used by all known extensions of extendee_type, and
+    appends them to ExtensionNumberResponse in an undefined order.
     Its corresponding method is best-effort: it's not guaranteed that the
     reflection service will implement this method, and it's not guaranteed
     that this method will provide all extensions. Returns
     StatusCode::UNIMPLEMENTED if it's not implemented.
     This field should be a fully-qualified type name. The format is
     <package>.<type>
     """
     list_services: builtins.str
     """List the full names of registered services. The content will not be
     checked.
     """
+    @property
+    def file_containing_extension(self) -> global___ExtensionRequest:
+        """Find the proto file which defines an extension extending the given
+        message type with the given field number.
+        """
+
     def __init__(
         self,
         *,
         host: builtins.str = ...,
         file_by_filename: builtins.str = ...,
         file_containing_symbol: builtins.str = ...,
         file_containing_extension: global___ExtensionRequest | None = ...,
         all_extension_numbers_of_type: builtins.str = ...,
         list_services: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "list_services", b"list_services", "message_request", b"message_request"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "host", b"host", "list_services", b"list_services", "message_request", b"message_request"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["message_request", b"message_request"]) -> typing_extensions.Literal["file_by_filename", "file_containing_symbol", "file_containing_extension", "all_extension_numbers_of_type", "list_services"] | None: ...
+    def HasField(self, field_name: typing.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "list_services", b"list_services", "message_request", b"message_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "host", b"host", "list_services", b"list_services", "message_request", b"message_request"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["message_request", b"message_request"]) -> typing.Literal["file_by_filename", "file_containing_symbol", "file_containing_extension", "all_extension_numbers_of_type", "list_services"] | None: ...
 
 global___ServerReflectionRequest = ServerReflectionRequest
 
-@typing_extensions.final
+@typing.final
 class ExtensionRequest(google.protobuf.message.Message):
     """The type name and extension number sent by the client when requesting
     file_containing_extension.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -92,19 +85,19 @@
     extension_number: builtins.int
     def __init__(
         self,
         *,
         containing_type: builtins.str = ...,
         extension_number: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["containing_type", b"containing_type", "extension_number", b"extension_number"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["containing_type", b"containing_type", "extension_number", b"extension_number"]) -> None: ...
 
 global___ExtensionRequest = ExtensionRequest
 
-@typing_extensions.final
+@typing.final
 class ServerReflectionResponse(google.protobuf.message.Message):
     """The message sent by the server to answer ServerReflectionInfo method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALID_HOST_FIELD_NUMBER: builtins.int
     ORIGINAL_REQUEST_FIELD_NUMBER: builtins.int
@@ -114,46 +107,50 @@
     ERROR_RESPONSE_FIELD_NUMBER: builtins.int
     valid_host: builtins.str
     @property
     def original_request(self) -> global___ServerReflectionRequest: ...
     @property
     def file_descriptor_response(self) -> global___FileDescriptorResponse:
         """This message is used to answer file_by_filename, file_containing_symbol,
-        file_containing_extension requests with transitive dependencies.
-        As the repeated label is not allowed in oneof fields, we use a
+        file_containing_extension requests with transitive dependencies. As
+        the repeated label is not allowed in oneof fields, we use a
         FileDescriptorResponse message to encapsulate the repeated fields.
         The reflection service is allowed to avoid sending FileDescriptorProtos
         that were previously sent in response to earlier requests in the stream.
         """
+
     @property
     def all_extension_numbers_response(self) -> global___ExtensionNumberResponse:
-        """This message is used to answer all_extension_numbers_of_type requests."""
+        """This message is used to answer all_extension_numbers_of_type requst."""
+
     @property
     def list_services_response(self) -> global___ListServiceResponse:
-        """This message is used to answer list_services requests."""
+        """This message is used to answer list_services request."""
+
     @property
     def error_response(self) -> global___ErrorResponse:
         """This message is used when an error occurs."""
+
     def __init__(
         self,
         *,
         valid_host: builtins.str = ...,
         original_request: global___ServerReflectionRequest | None = ...,
         file_descriptor_response: global___FileDescriptorResponse | None = ...,
         all_extension_numbers_response: global___ExtensionNumberResponse | None = ...,
         list_services_response: global___ListServiceResponse | None = ...,
         error_response: global___ErrorResponse | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request", "valid_host", b"valid_host"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["message_response", b"message_response"]) -> typing_extensions.Literal["file_descriptor_response", "all_extension_numbers_response", "list_services_response", "error_response"] | None: ...
+    def HasField(self, field_name: typing.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request", "valid_host", b"valid_host"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["message_response", b"message_response"]) -> typing.Literal["file_descriptor_response", "all_extension_numbers_response", "list_services_response", "error_response"] | None: ...
 
 global___ServerReflectionResponse = ServerReflectionResponse
 
-@typing_extensions.final
+@typing.final
 class FileDescriptorResponse(google.protobuf.message.Message):
     """Serialized FileDescriptorProto messages sent by the server answering
     a file_by_filename, file_containing_symbol, or file_containing_extension
     request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -161,24 +158,25 @@
     FILE_DESCRIPTOR_PROTO_FIELD_NUMBER: builtins.int
     @property
     def file_descriptor_proto(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]:
         """Serialized FileDescriptorProto messages. We avoid taking a dependency on
         descriptor.proto, which uses proto2 only features, by making them opaque
         bytes instead.
         """
+
     def __init__(
         self,
         *,
         file_descriptor_proto: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_descriptor_proto", b"file_descriptor_proto"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_descriptor_proto", b"file_descriptor_proto"]) -> None: ...
 
 global___FileDescriptorResponse = FileDescriptorResponse
 
-@typing_extensions.final
+@typing.final
 class ExtensionNumberResponse(google.protobuf.message.Message):
     """A list of extension numbers sent by the server answering
     all_extension_numbers_of_type request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -192,40 +190,41 @@
     def extension_number(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         base_type_name: builtins.str = ...,
         extension_number: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_type_name", b"base_type_name", "extension_number", b"extension_number"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["base_type_name", b"base_type_name", "extension_number", b"extension_number"]) -> None: ...
 
 global___ExtensionNumberResponse = ExtensionNumberResponse
 
-@typing_extensions.final
+@typing.final
 class ListServiceResponse(google.protobuf.message.Message):
     """A list of ServiceResponse sent by the server answering list_services request."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_FIELD_NUMBER: builtins.int
     @property
     def service(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceResponse]:
         """The information of each service may be expanded in the future, so we use
         ServiceResponse message to encapsulate it.
         """
+
     def __init__(
         self,
         *,
         service: collections.abc.Iterable[global___ServiceResponse] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["service", b"service"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["service", b"service"]) -> None: ...
 
 global___ListServiceResponse = ListServiceResponse
 
-@typing_extensions.final
+@typing.final
 class ServiceResponse(google.protobuf.message.Message):
     """The information of a single service used by ListServiceResponse to answer
     list_services request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -235,19 +234,19 @@
     is <package>.<service>
     """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name"]) -> None: ...
 
 global___ServiceResponse = ServiceResponse
 
-@typing_extensions.final
+@typing.final
 class ErrorResponse(google.protobuf.message.Message):
     """The error code and error message sent by the server when an error occurs."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_CODE_FIELD_NUMBER: builtins.int
     ERROR_MESSAGE_FIELD_NUMBER: builtins.int
@@ -256,10 +255,10 @@
     error_message: builtins.str
     def __init__(
         self,
         *,
         error_code: builtins.int = ...,
         error_message: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "error_message", b"error_message"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "error_message", b"error_message"]) -> None: ...
 
 global___ErrorResponse = ErrorResponse
```

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_grpc.py` & `grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_pb2.py` & `grpclib-0.4.8rc1/grpclib/reflection/v1alpha/reflection_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpclib/reflection/v1alpha/reflection.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +16,16 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+grpclib/reflection/v1alpha/reflection.proto\x12\x17grpc.reflection.v1alpha\"\x8a\x02\n\x17ServerReflectionRequest\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1a\n\x10\x66ile_by_filename\x18\x03 \x01(\tH\x00\x12 \n\x16\x66ile_containing_symbol\x18\x04 \x01(\tH\x00\x12N\n\x19\x66ile_containing_extension\x18\x05 \x01(\x0b\x32).grpc.reflection.v1alpha.ExtensionRequestH\x00\x12\'\n\x1d\x61ll_extension_numbers_of_type\x18\x06 \x01(\tH\x00\x12\x17\n\rlist_services\x18\x07 \x01(\tH\x00\x42\x11\n\x0fmessage_request\"E\n\x10\x45xtensionRequest\x12\x17\n\x0f\x63ontaining_type\x18\x01 \x01(\t\x12\x18\n\x10\x65xtension_number\x18\x02 \x01(\x05\"\xd1\x03\n\x18ServerReflectionResponse\x12\x12\n\nvalid_host\x18\x01 \x01(\t\x12J\n\x10original_request\x18\x02 \x01(\x0b\x32\x30.grpc.reflection.v1alpha.ServerReflectionRequest\x12S\n\x18\x66ile_descriptor_response\x18\x04 \x01(\x0b\x32/.grpc.reflection.v1alpha.FileDescriptorResponseH\x00\x12Z\n\x1e\x61ll_extension_numbers_response\x18\x05 \x01(\x0b\x32\x30.grpc.reflection.v1alpha.ExtensionNumberResponseH\x00\x12N\n\x16list_services_response\x18\x06 \x01(\x0b\x32,.grpc.reflection.v1alpha.ListServiceResponseH\x00\x12@\n\x0e\x65rror_response\x18\x07 \x01(\x0b\x32&.grpc.reflection.v1alpha.ErrorResponseH\x00\x42\x12\n\x10message_response\"7\n\x16\x46ileDescriptorResponse\x12\x1d\n\x15\x66ile_descriptor_proto\x18\x01 \x03(\x0c\"K\n\x17\x45xtensionNumberResponse\x12\x16\n\x0e\x62\x61se_type_name\x18\x01 \x01(\t\x12\x18\n\x10\x65xtension_number\x18\x02 \x03(\x05\"P\n\x13ListServiceResponse\x12\x39\n\x07service\x18\x01 \x03(\x0b\x32(.grpc.reflection.v1alpha.ServiceResponse\"\x1f\n\x0fServiceResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\":\n\rErrorResponse\x12\x12\n\nerror_code\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t2\x93\x01\n\x10ServerReflection\x12\x7f\n\x14ServerReflectionInfo\x12\x30.grpc.reflection.v1alpha.ServerReflectionRequest\x1a\x31.grpc.reflection.v1alpha.ServerReflectionResponse(\x01\x30\x01\x42\x38\n\x1aio.grpc.reflection.v1alphaB\x15ServerReflectionProtoP\x01\xb8\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpclib.reflection.v1alpha.reflection_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\032io.grpc.reflection.v1alphaB\025ServerReflectionProtoP\001\270\001\001'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\032io.grpc.reflection.v1alphaB\025ServerReflectionProtoP\001\270\001\001'
   _globals['_SERVERREFLECTIONREQUEST']._serialized_start=73
   _globals['_SERVERREFLECTIONREQUEST']._serialized_end=339
   _globals['_EXTENSIONREQUEST']._serialized_start=341
   _globals['_EXTENSIONREQUEST']._serialized_end=410
   _globals['_SERVERREFLECTIONRESPONSE']._serialized_start=413
   _globals['_SERVERREFLECTIONRESPONSE']._serialized_end=878
   _globals['_FILEDESCRIPTORRESPONSE']._serialized_start=880
```

### Comparing `grpclib-0.4.7rc1/grpclib/reflection/v1alpha/reflection_pb2.pyi` & `grpclib-0.4.8rc1/grpclib/reflection/v1/reflection_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Warning: this entire file is deprecated. Use this instead:
+Service exported by server reflection.  A more complete description of how
+server reflection works can be found at
+https://github.com/grpc/grpc/blob/master/doc/server-reflection.md
+
+The canonical version of this proto can be found at
 https://github.com/grpc/grpc-proto/blob/master/grpc/reflection/v1/reflection.proto
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ServerReflectionRequest(google.protobuf.message.Message):
     """The message sent by the client when calling ServerReflectionInfo method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HOST_FIELD_NUMBER: builtins.int
     FILE_BY_FILENAME_FIELD_NUMBER: builtins.int
@@ -34,50 +34,51 @@
     file_by_filename: builtins.str
     """Find a proto file by the file name."""
     file_containing_symbol: builtins.str
     """Find the proto file that declares the given fully-qualified symbol name.
     This field should be a fully-qualified symbol name
     (e.g. <package>.<service>[.<method>] or <package>.<type>).
     """
-    @property
-    def file_containing_extension(self) -> global___ExtensionRequest:
-        """Find the proto file which defines an extension extending the given
-        message type with the given field number.
-        """
     all_extension_numbers_of_type: builtins.str
-    """Finds the tag numbers used by all known extensions of extendee_type, and
-    appends them to ExtensionNumberResponse in an undefined order.
+    """Finds the tag numbers used by all known extensions of the given message
+    type, and appends them to ExtensionNumberResponse in an undefined order.
     Its corresponding method is best-effort: it's not guaranteed that the
     reflection service will implement this method, and it's not guaranteed
     that this method will provide all extensions. Returns
     StatusCode::UNIMPLEMENTED if it's not implemented.
     This field should be a fully-qualified type name. The format is
     <package>.<type>
     """
     list_services: builtins.str
     """List the full names of registered services. The content will not be
     checked.
     """
+    @property
+    def file_containing_extension(self) -> global___ExtensionRequest:
+        """Find the proto file which defines an extension extending the given
+        message type with the given field number.
+        """
+
     def __init__(
         self,
         *,
         host: builtins.str = ...,
         file_by_filename: builtins.str = ...,
         file_containing_symbol: builtins.str = ...,
         file_containing_extension: global___ExtensionRequest | None = ...,
         all_extension_numbers_of_type: builtins.str = ...,
         list_services: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "list_services", b"list_services", "message_request", b"message_request"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "host", b"host", "list_services", b"list_services", "message_request", b"message_request"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["message_request", b"message_request"]) -> typing_extensions.Literal["file_by_filename", "file_containing_symbol", "file_containing_extension", "all_extension_numbers_of_type", "list_services"] | None: ...
+    def HasField(self, field_name: typing.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "list_services", b"list_services", "message_request", b"message_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_extension_numbers_of_type", b"all_extension_numbers_of_type", "file_by_filename", b"file_by_filename", "file_containing_extension", b"file_containing_extension", "file_containing_symbol", b"file_containing_symbol", "host", b"host", "list_services", b"list_services", "message_request", b"message_request"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["message_request", b"message_request"]) -> typing.Literal["file_by_filename", "file_containing_symbol", "file_containing_extension", "all_extension_numbers_of_type", "list_services"] | None: ...
 
 global___ServerReflectionRequest = ServerReflectionRequest
 
-@typing_extensions.final
+@typing.final
 class ExtensionRequest(google.protobuf.message.Message):
     """The type name and extension number sent by the client when requesting
     file_containing_extension.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -88,19 +89,19 @@
     extension_number: builtins.int
     def __init__(
         self,
         *,
         containing_type: builtins.str = ...,
         extension_number: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["containing_type", b"containing_type", "extension_number", b"extension_number"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["containing_type", b"containing_type", "extension_number", b"extension_number"]) -> None: ...
 
 global___ExtensionRequest = ExtensionRequest
 
-@typing_extensions.final
+@typing.final
 class ServerReflectionResponse(google.protobuf.message.Message):
     """The message sent by the server to answer ServerReflectionInfo method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALID_HOST_FIELD_NUMBER: builtins.int
     ORIGINAL_REQUEST_FIELD_NUMBER: builtins.int
@@ -110,46 +111,50 @@
     ERROR_RESPONSE_FIELD_NUMBER: builtins.int
     valid_host: builtins.str
     @property
     def original_request(self) -> global___ServerReflectionRequest: ...
     @property
     def file_descriptor_response(self) -> global___FileDescriptorResponse:
         """This message is used to answer file_by_filename, file_containing_symbol,
-        file_containing_extension requests with transitive dependencies. As
-        the repeated label is not allowed in oneof fields, we use a
+        file_containing_extension requests with transitive dependencies.
+        As the repeated label is not allowed in oneof fields, we use a
         FileDescriptorResponse message to encapsulate the repeated fields.
         The reflection service is allowed to avoid sending FileDescriptorProtos
         that were previously sent in response to earlier requests in the stream.
         """
+
     @property
     def all_extension_numbers_response(self) -> global___ExtensionNumberResponse:
-        """This message is used to answer all_extension_numbers_of_type requst."""
+        """This message is used to answer all_extension_numbers_of_type requests."""
+
     @property
     def list_services_response(self) -> global___ListServiceResponse:
-        """This message is used to answer list_services request."""
+        """This message is used to answer list_services requests."""
+
     @property
     def error_response(self) -> global___ErrorResponse:
         """This message is used when an error occurs."""
+
     def __init__(
         self,
         *,
         valid_host: builtins.str = ...,
         original_request: global___ServerReflectionRequest | None = ...,
         file_descriptor_response: global___FileDescriptorResponse | None = ...,
         all_extension_numbers_response: global___ExtensionNumberResponse | None = ...,
         list_services_response: global___ListServiceResponse | None = ...,
         error_response: global___ErrorResponse | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request", "valid_host", b"valid_host"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["message_response", b"message_response"]) -> typing_extensions.Literal["file_descriptor_response", "all_extension_numbers_response", "list_services_response", "error_response"] | None: ...
+    def HasField(self, field_name: typing.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_extension_numbers_response", b"all_extension_numbers_response", "error_response", b"error_response", "file_descriptor_response", b"file_descriptor_response", "list_services_response", b"list_services_response", "message_response", b"message_response", "original_request", b"original_request", "valid_host", b"valid_host"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["message_response", b"message_response"]) -> typing.Literal["file_descriptor_response", "all_extension_numbers_response", "list_services_response", "error_response"] | None: ...
 
 global___ServerReflectionResponse = ServerReflectionResponse
 
-@typing_extensions.final
+@typing.final
 class FileDescriptorResponse(google.protobuf.message.Message):
     """Serialized FileDescriptorProto messages sent by the server answering
     a file_by_filename, file_containing_symbol, or file_containing_extension
     request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -157,24 +162,25 @@
     FILE_DESCRIPTOR_PROTO_FIELD_NUMBER: builtins.int
     @property
     def file_descriptor_proto(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]:
         """Serialized FileDescriptorProto messages. We avoid taking a dependency on
         descriptor.proto, which uses proto2 only features, by making them opaque
         bytes instead.
         """
+
     def __init__(
         self,
         *,
         file_descriptor_proto: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_descriptor_proto", b"file_descriptor_proto"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_descriptor_proto", b"file_descriptor_proto"]) -> None: ...
 
 global___FileDescriptorResponse = FileDescriptorResponse
 
-@typing_extensions.final
+@typing.final
 class ExtensionNumberResponse(google.protobuf.message.Message):
     """A list of extension numbers sent by the server answering
     all_extension_numbers_of_type request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -188,40 +194,41 @@
     def extension_number(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         base_type_name: builtins.str = ...,
         extension_number: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_type_name", b"base_type_name", "extension_number", b"extension_number"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["base_type_name", b"base_type_name", "extension_number", b"extension_number"]) -> None: ...
 
 global___ExtensionNumberResponse = ExtensionNumberResponse
 
-@typing_extensions.final
+@typing.final
 class ListServiceResponse(google.protobuf.message.Message):
     """A list of ServiceResponse sent by the server answering list_services request."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_FIELD_NUMBER: builtins.int
     @property
     def service(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceResponse]:
         """The information of each service may be expanded in the future, so we use
         ServiceResponse message to encapsulate it.
         """
+
     def __init__(
         self,
         *,
         service: collections.abc.Iterable[global___ServiceResponse] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["service", b"service"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["service", b"service"]) -> None: ...
 
 global___ListServiceResponse = ListServiceResponse
 
-@typing_extensions.final
+@typing.final
 class ServiceResponse(google.protobuf.message.Message):
     """The information of a single service used by ListServiceResponse to answer
     list_services request.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -231,19 +238,19 @@
     is <package>.<service>
     """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name"]) -> None: ...
 
 global___ServiceResponse = ServiceResponse
 
-@typing_extensions.final
+@typing.final
 class ErrorResponse(google.protobuf.message.Message):
     """The error code and error message sent by the server when an error occurs."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_CODE_FIELD_NUMBER: builtins.int
     ERROR_MESSAGE_FIELD_NUMBER: builtins.int
@@ -252,10 +259,10 @@
     error_message: builtins.str
     def __init__(
         self,
         *,
         error_code: builtins.int = ...,
         error_message: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "error_message", b"error_message"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "error_message", b"error_message"]) -> None: ...
 
 global___ErrorResponse = ErrorResponse
```

### Comparing `grpclib-0.4.7rc1/grpclib/server.py` & `grpclib-0.4.8rc1/grpclib/server.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/stream.py` & `grpclib-0.4.8rc1/grpclib/stream.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/testing.py` & `grpclib-0.4.8rc1/grpclib/testing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/grpclib/utils.py` & `grpclib-0.4.8rc1/grpclib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import signal
 import asyncio
 import warnings
 
 from types import TracebackType
 from typing import TYPE_CHECKING, Optional, Set, Type, ContextManager, List
-from typing import Iterator, Collection, Callable, Any
+from typing import Iterator, Collection, Callable, Any, cast
 from functools import wraps
 from contextlib import contextmanager
 
 
 if sys.version_info > (3, 7):
     _current_task = asyncio.current_task
 else:
@@ -139,22 +139,22 @@
 
 
 def _second_stage(sig_num: 'signal.Signals') -> None:
     raise SystemExit(128 + sig_num)
 
 
 def _exit_handler(
-    sig_num: 'signal.Signals',
+    sig_num: int,
     servers: Collection['IClosable'],
     flag: List[bool],
 ) -> None:
     if flag:
-        _second_stage(sig_num)
+        _second_stage(cast('signal.Signals', sig_num))
     else:
-        _first_stage(sig_num, servers)
+        _first_stage(cast('signal.Signals', sig_num), servers)
         flag.append(True)
 
 
 @contextmanager
 def graceful_exit(
     servers: Collection['IClosable'],
     *,
```

### Comparing `grpclib-0.4.7rc1/grpclib.egg-info/PKG-INFO` & `grpclib-0.4.8rc1/grpclib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.7rc1
+Version: 0.4.8rc1
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
         
         .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
           :target: https://standforukraine.com
         
         |project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
         
-        This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
+        This project is based on `hyper-h2`_ and **requires Python >= 3.8**.
         
         .. contents::
           :local:
         
         Example
         ~~~~~~~
         
@@ -170,18 +170,18 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: protobuf
```

### Comparing `grpclib-0.4.7rc1/grpclib.egg-info/SOURCES.txt` & `grpclib-0.4.8rc1/grpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.7rc1/setup.cfg` & `grpclib-0.4.8rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 url = https://github.com/vmagamedov/grpclib
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Internet :: WWW/HTTP :: HTTP Servers
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	h2<5,>=3.1.0
 	multidict
 
 [options.extras_require]
 protobuf = 
 	protobuf>=3.20.0
```

