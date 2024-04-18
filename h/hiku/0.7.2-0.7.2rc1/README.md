# Comparing `tmp/hiku-0.7.2.tar.gz` & `tmp/hiku-0.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiku-0.7.2.tar", last modified: Thu Apr 18 10:23:13 2024, max compression
+gzip compressed data, was "hiku-0.7.2rc1.tar", last modified: Mon Mar 25 09:32:55 2024, max compression
```

## Comparing `hiku-0.7.2.tar` & `hiku-0.7.2rc1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1480 2024-04-18 10:23:01.886566 hiku-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     3482 2024-04-18 10:23:01.886566 hiku-0.7.2/README.rst
--rw-r--r--   0        0        0       22 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/builder.py
--rw-r--r--   0        0        0     6714 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/cache.py
--rw-r--r--   0        0        0      974 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/compat.py
--rw-r--r--   0        0        0     3582 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/context.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/denormalize/__init__.py
--rw-r--r--   0        0        0     5095 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/denormalize/base.py
--rw-r--r--   0        0        0     1919 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/denormalize/graphql.py
--rw-r--r--   0        0        0     8908 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/directives/__init__.py
--rw-r--r--   0        0        0     9855 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/edn.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/endpoint/__init__.py
--rw-r--r--   0        0        0    12011 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/endpoint/graphql.py
--rw-r--r--   0        0        0    32703 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/engine.py
--rw-r--r--   0        0        0     2864 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/enum.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/asyncio.py
--rw-r--r--   0        0        0      826 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/base.py
--rw-r--r--   0        0        0     4717 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/queue.py
--rw-r--r--   0        0        0      796 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/sync.py
--rw-r--r--   0        0        0      878 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/executors/threads.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/export/__init__.py
--rw-r--r--   0        0        0     2462 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/export/graphql.py
--rw-r--r--   0        0        0      917 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/export/protobuf.py
--rw-r--r--   0        0        0     1134 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/export/simple.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/__init__.py
--rw-r--r--   0        0        0     6192 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/checker.py
--rw-r--r--   0        0        0     5497 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/compiler.py
--rw-r--r--   0        0        0     6221 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/core.py
--rw-r--r--   0        0        0     3048 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/nodes.py
--rw-r--r--   0        0        0     4329 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/expr/refs.py
--rw-r--r--   0        0        0       70 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/__init__.py
--rw-r--r--   0        0        0     8691 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/base_extension.py
--rw-r--r--   0        0        0      298 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/base_validator.py
--rw-r--r--   0        0        0      477 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/context.py
--rw-r--r--   0        0        0     1666 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/prometheus.py
--rw-r--r--   0        0        0     2071 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/query_depth_validator.py
--rw-r--r--   0        0        0     1088 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/query_parse_cache.py
--rw-r--r--   0        0        0      993 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/query_transform_cache.py
--rw-r--r--   0        0        0      800 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/query_validation_cache.py
--rw-r--r--   0        0        0     2038 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/extensions/sentry.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/__init__.py
--rw-r--r--   0        0        0      513 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/denormalize.py
--rw-r--r--   0        0        0    10024 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/directive.py
--rw-r--r--   0        0        0    12095 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/endpoint.py
--rw-r--r--   0        0        0      926 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/engine.py
--rw-r--r--   0        0        0     6379 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/graph.py
--rw-r--r--   0        0        0     1597 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/introspection.py
--rw-r--r--   0        0        0      835 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/scalars.py
--rw-r--r--   0        0        0    18794 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/sdl.py
--rw-r--r--   0        0        0      777 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/utils.py
--rw-r--r--   0        0        0      330 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/validate.py
--rw-r--r--   0        0        0       31 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/federation/version.py
--rw-r--r--   0        0        0    31217 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/graph.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/introspection/__init__.py
--rw-r--r--   0        0        0    33040 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/introspection/graphql.py
--rw-r--r--   0        0        0     1467 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/introspection/types.py
--rw-r--r--   0        0        0      825 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/operation.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/protobuf/__init__.py
--rw-r--r--   0        0        0      380 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/protobuf/query.proto
--rw-r--r--   0        0        0     9766 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/protobuf/query_pb2.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/py.typed
--rw-r--r--   0        0        0    11445 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/query.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/readers/__init__.py
--rw-r--r--   0        0        0    18134 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/readers/graphql.py
--rw-r--r--   0        0        0     2238 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/readers/protobuf.py
--rw-r--r--   0        0        0     2846 2024-04-18 10:23:01.890566 hiku-0.7.2/hiku/readers/simple.py
--rw-r--r--   0        0        0     7980 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/result.py
--rw-r--r--   0        0        0     2491 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/scalar.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/sources/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/sources/aiopg.py
--rw-r--r--   0        0        0     5591 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/sources/graph.py
--rw-r--r--   0        0        0     6517 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/sources/sqlalchemy.py
--rw-r--r--   0        0        0     1647 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/sources/sqlalchemy_async.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/telemetry/__init__.py
--rw-r--r--   0        0        0     6897 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/telemetry/prometheus.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/typedef/__init__.py
--rw-r--r--   0        0        0     4405 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/typedef/kinko.py
--rw-r--r--   0        0        0      270 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/typedef/types.py
--rw-r--r--   0        0        0    11351 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/types.py
--rw-r--r--   0        0        0      805 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/__init__.py
--rw-r--r--   0        0        0      365 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/cached_property.py
--rw-r--r--   0        0        0      245 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/const.py
--rw-r--r--   0        0        0     1069 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/immutable.py
--rw-r--r--   0        0        0      706 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/serialize.py
--rw-r--r--   0        0        0     2294 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/utils/typing.py
--rw-r--r--   0        0        0        0 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/validate/__init__.py
--rw-r--r--   0        0        0      177 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/validate/errors.py
--rw-r--r--   0        0        0    12898 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/validate/graph.py
--rw-r--r--   0        0        0    17459 2024-04-18 10:23:01.894566 hiku-0.7.2/hiku/validate/query.py
--rw-r--r--   0        0        0     5368 2024-04-18 10:23:13.002563 hiku-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 hiku-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1480 2024-03-25 09:32:44.436763 hiku-0.7.2rc1/LICENSE.txt
+-rw-r--r--   0        0        0     3482 2024-03-25 09:32:44.436763 hiku-0.7.2rc1/README.rst
+-rw-r--r--   0        0        0       25 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/__init__.py
+-rw-r--r--   0        0        0     2315 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/builder.py
+-rw-r--r--   0        0        0     6714 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/cache.py
+-rw-r--r--   0        0        0      974 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/compat.py
+-rw-r--r--   0        0        0     3582 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/context.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/denormalize/__init__.py
+-rw-r--r--   0        0        0     5095 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/denormalize/base.py
+-rw-r--r--   0        0        0     1919 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/denormalize/graphql.py
+-rw-r--r--   0        0        0     8908 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/directives/__init__.py
+-rw-r--r--   0        0        0     9855 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/edn.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/endpoint/__init__.py
+-rw-r--r--   0        0        0    12011 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/endpoint/graphql.py
+-rw-r--r--   0        0        0    32703 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/engine.py
+-rw-r--r--   0        0        0     2864 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/enum.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/__init__.py
+-rw-r--r--   0        0        0     1505 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/asyncio.py
+-rw-r--r--   0        0        0      826 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/base.py
+-rw-r--r--   0        0        0     4717 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/queue.py
+-rw-r--r--   0        0        0      796 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/sync.py
+-rw-r--r--   0        0        0      878 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/executors/threads.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/export/__init__.py
+-rw-r--r--   0        0        0     2462 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/export/graphql.py
+-rw-r--r--   0        0        0      917 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/export/protobuf.py
+-rw-r--r--   0        0        0     1134 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/export/simple.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/__init__.py
+-rw-r--r--   0        0        0     6192 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/checker.py
+-rw-r--r--   0        0        0     5497 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/compiler.py
+-rw-r--r--   0        0        0     6221 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/core.py
+-rw-r--r--   0        0        0     3048 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/nodes.py
+-rw-r--r--   0        0        0     4329 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/expr/refs.py
+-rw-r--r--   0        0        0       70 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/__init__.py
+-rw-r--r--   0        0        0     8691 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/base_extension.py
+-rw-r--r--   0        0        0      298 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/base_validator.py
+-rw-r--r--   0        0        0      477 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/context.py
+-rw-r--r--   0        0        0     1666 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/prometheus.py
+-rw-r--r--   0        0        0     2071 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/query_depth_validator.py
+-rw-r--r--   0        0        0     1088 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/query_parse_cache.py
+-rw-r--r--   0        0        0      993 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/query_transform_cache.py
+-rw-r--r--   0        0        0      800 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/query_validation_cache.py
+-rw-r--r--   0        0        0     2038 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/extensions/sentry.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/federation/__init__.py
+-rw-r--r--   0        0        0      513 2024-03-25 09:32:44.440763 hiku-0.7.2rc1/hiku/federation/denormalize.py
+-rw-r--r--   0        0        0    10024 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/directive.py
+-rw-r--r--   0        0        0    12095 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/endpoint.py
+-rw-r--r--   0        0        0      926 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/engine.py
+-rw-r--r--   0        0        0     6379 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/graph.py
+-rw-r--r--   0        0        0     1597 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/introspection.py
+-rw-r--r--   0        0        0      835 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/scalars.py
+-rw-r--r--   0        0        0    18695 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/sdl.py
+-rw-r--r--   0        0        0      777 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/utils.py
+-rw-r--r--   0        0        0      330 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/validate.py
+-rw-r--r--   0        0        0       31 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/federation/version.py
+-rw-r--r--   0        0        0    31217 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/graph.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/introspection/__init__.py
+-rw-r--r--   0        0        0    33040 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/introspection/graphql.py
+-rw-r--r--   0        0        0     1467 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/introspection/types.py
+-rw-r--r--   0        0        0      825 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/operation.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/protobuf/__init__.py
+-rw-r--r--   0        0        0      380 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/protobuf/query.proto
+-rw-r--r--   0        0        0     9766 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/protobuf/query_pb2.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/py.typed
+-rw-r--r--   0        0        0    11445 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/query.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/readers/__init__.py
+-rw-r--r--   0        0        0    18134 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/readers/graphql.py
+-rw-r--r--   0        0        0     2238 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/readers/protobuf.py
+-rw-r--r--   0        0        0     2846 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/readers/simple.py
+-rw-r--r--   0        0        0     7980 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/result.py
+-rw-r--r--   0        0        0     2491 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/scalar.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/sources/__init__.py
+-rw-r--r--   0        0        0     2019 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/sources/aiopg.py
+-rw-r--r--   0        0        0     5591 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/sources/graph.py
+-rw-r--r--   0        0        0     6517 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/sources/sqlalchemy.py
+-rw-r--r--   0        0        0     1647 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/sources/sqlalchemy_async.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/telemetry/__init__.py
+-rw-r--r--   0        0        0     6897 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/telemetry/prometheus.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/typedef/__init__.py
+-rw-r--r--   0        0        0     4405 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/typedef/kinko.py
+-rw-r--r--   0        0        0      270 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/typedef/types.py
+-rw-r--r--   0        0        0    11351 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/types.py
+-rw-r--r--   0        0        0      805 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/__init__.py
+-rw-r--r--   0        0        0      365 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/cached_property.py
+-rw-r--r--   0        0        0      245 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/const.py
+-rw-r--r--   0        0        0     1069 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/immutable.py
+-rw-r--r--   0        0        0      706 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/serialize.py
+-rw-r--r--   0        0        0     2294 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/utils/typing.py
+-rw-r--r--   0        0        0        0 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/validate/__init__.py
+-rw-r--r--   0        0        0      177 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/validate/errors.py
+-rw-r--r--   0        0        0    12898 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/validate/graph.py
+-rw-r--r--   0        0        0    17459 2024-03-25 09:32:44.444763 hiku-0.7.2rc1/hiku/validate/query.py
+-rw-r--r--   0        0        0     5929 2024-03-25 09:32:55.168775 hiku-0.7.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 hiku-0.7.2rc1/PKG-INFO
```

### Comparing `hiku-0.7.2/LICENSE.txt` & `hiku-0.7.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/README.rst` & `hiku-0.7.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/builder.py` & `hiku-0.7.2rc1/hiku/builder.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/cache.py` & `hiku-0.7.2rc1/hiku/cache.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/compat.py` & `hiku-0.7.2rc1/hiku/compat.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/context.py` & `hiku-0.7.2rc1/hiku/context.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/denormalize/base.py` & `hiku-0.7.2rc1/hiku/denormalize/base.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/denormalize/graphql.py` & `hiku-0.7.2rc1/hiku/denormalize/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/directives/__init__.py` & `hiku-0.7.2rc1/hiku/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/edn.py` & `hiku-0.7.2rc1/hiku/edn.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/endpoint/graphql.py` & `hiku-0.7.2rc1/hiku/endpoint/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/engine.py` & `hiku-0.7.2rc1/hiku/engine.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/enum.py` & `hiku-0.7.2rc1/hiku/enum.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/executors/asyncio.py` & `hiku-0.7.2rc1/hiku/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/executors/base.py` & `hiku-0.7.2rc1/hiku/executors/base.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/executors/queue.py` & `hiku-0.7.2rc1/hiku/executors/queue.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/executors/sync.py` & `hiku-0.7.2rc1/hiku/executors/sync.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/executors/threads.py` & `hiku-0.7.2rc1/hiku/executors/threads.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/export/graphql.py` & `hiku-0.7.2rc1/hiku/export/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/export/protobuf.py` & `hiku-0.7.2rc1/hiku/export/protobuf.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/export/simple.py` & `hiku-0.7.2rc1/hiku/export/simple.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/expr/checker.py` & `hiku-0.7.2rc1/hiku/expr/checker.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/expr/compiler.py` & `hiku-0.7.2rc1/hiku/expr/compiler.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/expr/core.py` & `hiku-0.7.2rc1/hiku/expr/core.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/expr/nodes.py` & `hiku-0.7.2rc1/hiku/expr/nodes.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/expr/refs.py` & `hiku-0.7.2rc1/hiku/expr/refs.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/base_extension.py` & `hiku-0.7.2rc1/hiku/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/prometheus.py` & `hiku-0.7.2rc1/hiku/extensions/prometheus.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/query_depth_validator.py` & `hiku-0.7.2rc1/hiku/extensions/query_depth_validator.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/query_parse_cache.py` & `hiku-0.7.2rc1/hiku/extensions/query_parse_cache.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/query_transform_cache.py` & `hiku-0.7.2rc1/hiku/extensions/query_transform_cache.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/query_validation_cache.py` & `hiku-0.7.2rc1/hiku/extensions/query_validation_cache.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/extensions/sentry.py` & `hiku-0.7.2rc1/hiku/extensions/sentry.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/denormalize.py` & `hiku-0.7.2rc1/hiku/federation/denormalize.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/directive.py` & `hiku-0.7.2rc1/hiku/federation/directive.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/endpoint.py` & `hiku-0.7.2rc1/hiku/federation/endpoint.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/engine.py` & `hiku-0.7.2rc1/hiku/federation/engine.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/graph.py` & `hiku-0.7.2rc1/hiku/federation/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/introspection.py` & `hiku-0.7.2rc1/hiku/federation/introspection.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/scalars.py` & `hiku-0.7.2rc1/hiku/federation/scalars.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/federation/sdl.py` & `hiku-0.7.2rc1/hiku/federation/sdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     Option,
     Graph,
     Union,
 )
 from hiku.scalar import ScalarMeta
 from hiku.types import (
     EnumRefMeta,
-    UnionRefMeta,
     IDMeta,
     IntegerMeta,
     MappingMeta,
     String,
     TypeRefMeta,
     StringMeta,
     SequenceMeta,
@@ -98,16 +97,14 @@
             return _encode(val.__type__), True
         elif isinstance(val, TypeRefMeta):
             if input_type:
                 return f"IO{val.__type_name__}"
             return val.__type_name__
         elif isinstance(val, EnumRefMeta):
             return val.__type_name__
-        elif isinstance(val, UnionRefMeta):
-            return val.__type_name__
         elif isinstance(val, ScalarMeta):
             return val.__type_name__
         elif isinstance(val, IntegerMeta):
             return "Int"
         elif isinstance(val, StringMeta):
             return "String"
         elif isinstance(val, IDMeta):
```

### Comparing `hiku-0.7.2/hiku/federation/utils.py` & `hiku-0.7.2rc1/hiku/federation/utils.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/graph.py` & `hiku-0.7.2rc1/hiku/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/introspection/graphql.py` & `hiku-0.7.2rc1/hiku/introspection/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/introspection/types.py` & `hiku-0.7.2rc1/hiku/introspection/types.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/operation.py` & `hiku-0.7.2rc1/hiku/operation.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/protobuf/query_pb2.py` & `hiku-0.7.2rc1/hiku/protobuf/query_pb2.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/query.py` & `hiku-0.7.2rc1/hiku/query.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/readers/graphql.py` & `hiku-0.7.2rc1/hiku/readers/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/readers/protobuf.py` & `hiku-0.7.2rc1/hiku/readers/protobuf.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/readers/simple.py` & `hiku-0.7.2rc1/hiku/readers/simple.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/result.py` & `hiku-0.7.2rc1/hiku/result.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/scalar.py` & `hiku-0.7.2rc1/hiku/scalar.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/sources/aiopg.py` & `hiku-0.7.2rc1/hiku/sources/aiopg.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/sources/graph.py` & `hiku-0.7.2rc1/hiku/sources/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/sources/sqlalchemy.py` & `hiku-0.7.2rc1/hiku/sources/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/sources/sqlalchemy_async.py` & `hiku-0.7.2rc1/hiku/sources/sqlalchemy_async.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/telemetry/prometheus.py` & `hiku-0.7.2rc1/hiku/telemetry/prometheus.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/typedef/kinko.py` & `hiku-0.7.2rc1/hiku/typedef/kinko.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/types.py` & `hiku-0.7.2rc1/hiku/types.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/utils/__init__.py` & `hiku-0.7.2rc1/hiku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/utils/immutable.py` & `hiku-0.7.2rc1/hiku/utils/immutable.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/utils/serialize.py` & `hiku-0.7.2rc1/hiku/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/utils/typing.py` & `hiku-0.7.2rc1/hiku/utils/typing.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/validate/graph.py` & `hiku-0.7.2rc1/hiku/validate/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/hiku/validate/query.py` & `hiku-0.7.2rc1/hiku/validate/query.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.2/pyproject.toml` & `hiku-0.7.2rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.7.2"
+version = "0.7.2rc1"
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [project.license]
 text = "BSD-3-Clause"
@@ -113,14 +113,21 @@
 composite = [
     "fmt",
     "test",
     "mypy",
     "flake",
 ]
 
+[tool.pdm.scripts.release]
+shell = "set -e\nUSAGE=\"Usage: VERSION=<> MESSAGE=<> pdm run release\"\n\nif [ -z \"${VERSION}\" ]; then\n    echo $USAGE\n    echo \"VERSION is not set\"\n    exit 1\nfi\nif [ -z \"${MESSAGE}\" ]; then\n    echo $USAGE\n    echo \"MESSAGE is not set\"\n    exit 1\nfi\necho \"__version__ = \\\"${VERSION}\\\"\" > hiku/__init__.py\ngit add hiku/__init__.py\ngit commit -m \"Release ${VERSION}\"\ngit tag -a v${VERSION} -m \"${MESSAGE}\"\ngit push origin master --tags\n"
+
+[tool.pdm.scripts.release.env]
+VERSION = ""
+MESSAGE = ""
+
 [tool.pytest.ini_options]
 addopts = "--tb=native --benchmark-disable"
 testpaths = [
     "tests",
     "tests_pg",
 ]
 filterwarnings = [
```

### Comparing `hiku-0.7.2/PKG-INFO` & `hiku-0.7.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiku
-Version: 0.7.2
+Version: 0.7.2rc1
 Summary: Library to implement Graph APIs
 Author-Email: Vladimir Magamedov <vladimir@magamedov.com>, Maksym Kindritskyi <kindritskiy.m@gmail.com>
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

